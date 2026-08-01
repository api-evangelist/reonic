---
name: Consume and verify Reonic webhooks
description: Receive Reonic webhook deliveries, verify the HMAC signature, dedupe, and fetch current resource state.
api: openapi/reonic-openapi-original.json
operations:
  - "GET /residentialProjects/{projectId}"
  - "GET /commercialProjects/{projectId}"
  - "GET /contacts/{contactId}"
---

# Consume and verify Reonic webhooks

Reonic sends a signed HTTPS `POST` to your configured URL whenever a selected event occurs (17 event types — see `asyncapi/reonic-webhooks.yml`). Payloads are thin: they carry ids, not resource snapshots.

## Endpoint requirements
- Public `https://` URL (private/internal addresses are rejected), no redirects, responds within 5 seconds.
- Acknowledge with any `2xx` first, then process asynchronously.

## Steps
1. Read headers: `X-Reonic-Event` (type), `X-Reonic-Event-Id` (idempotency key), `X-Reonic-Timestamp`, `X-Reonic-Signature`, `X-Reonic-Client-Id`.
2. **Verify the signature:** compute `HMAC-SHA256(secret, "${timestamp}.${rawBody}")` over the raw body and compare (constant-time) to the hex in `X-Reonic-Signature` (`sha256=<hex>`). The signing secret starts with `whsec_`.
3. **Reject replays:** drop deliveries whose `X-Reonic-Timestamp` is more than 5 minutes old.
4. **Dedupe:** store `X-Reonic-Event-Id` and ignore duplicates — order is not guaranteed and events may be redelivered.
5. **Fetch state:** using the ids in `data`, call the matching read endpoint — e.g. a `project_created` event's `projectId` via `GET /residentialProjects/{projectId}` or `GET /commercialProjects/{projectId}` depending on `projectType`; `contact_created` via `GET /contacts/{contactId}`.

## Rules
- Use the raw request body exactly as received (before JSON parsing) for signature checks.
- Retries: ~1m, 5m, 30m, 2h, 5h, 12h, 1d, 2d. After exhaustion Reonic disables the subscription and emails your workspace contact.
- The body `version` (currently 1) only bumps on breaking envelope changes; ignore unknown event types and fields.
