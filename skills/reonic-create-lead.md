---
name: Create a lead and residential project in Reonic
description: Capture a new customer as a contact and open a residential (household) solar/heat-pump project for them.
api: openapi/reonic-openapi-original.json
operations:
  - "POST /contacts/create"
  - "POST /residentialProjects/create"
  - "GET /leadSources"
  - "GET /residentialProjects/{projectId}"
---

# Create a lead and residential project in Reonic

Use the Reonic REST API v3 to turn an inbound lead into a contact and a household project.

## Auth
- Send your key in the `X-Authorization` header (value starts with `rnc_v3_`).
- You need a **read-and-write** key; a read-only key returns `403` on any `POST`.
- Base URL: `https://api.reonic.de/rest/v3/`

## Steps
1. (Optional) `GET /leadSources` to resolve the `leadSourceId` for the channel this lead came from.
2. `POST /contacts/create` with the person's name, contact details, and address. Keep the returned contact `id`.
3. `POST /residentialProjects/create` referencing the contact, plus `leadSourceId` and any `tagIds`.
4. `GET /residentialProjects/{projectId}` to confirm the project and read back its Kanban column / deal state.

## Rules
- **Rate limits:** writes hit the `uncached` bucket (30/min). Watch `X-RateLimit-Remaining`; on `429`, wait `Retry-After` seconds.
- **Validation:** a `400` returns `{ "message": ... }` plus an `errors` object with per-field detail — fix the named fields and retry.
- **No request idempotency:** there is no idempotency key on writes, so guard against double-submits on your side before calling `create`.
- Payloads are thin; resolve related ids (`leadSourceId`, `tagIds`, `keyAccountManagerId`) via their own `GET` endpoints.
