# Reonic

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Reonic is a German climate-tech company (founded 2021, Augsburg) building an AI-powered operating system for renewable-energy installers. Its platform covers the full workflow for selling and installing photovoltaic systems, heat pumps, EV chargers, and battery storage — CRM and lead management, 3D roof planning and shading simulation, instant pricing, proposal generation with digital signature, project and installation tracking, and documentation. The Reonic REST API v3 exposes 111 endpoints across 33 resource areas (contacts, residential and commercial projects, tasks, files, components, planning templates, time tracking, wiki, photogrammetry, and more), authenticated with rnc_v3_ API keys, plus a 17-event signed webhook surface.

**Areas:** Company · Climate Energy · Solar · Renewable Energy · Photovoltaics · Heat Pumps · Installer Software · Software-as-a-Service · CRM · Project Management

## Reonic on APIs.io

Everything profiled for Reonic is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/reonic/](https://apis.io/providers/reonic/)** — or go straight to one of the APIs or properties below.

### APIs (30)

- [Reonic Activities API](https://apis.io/apis/reonic/reonic-activities-api/) — Timeline of events on a project — automatic activity records and manually logged calls and meetings.
- [Reonic Appointments API](https://apis.io/apis/reonic/reonic-appointments-api/) — Appointments on Reonic-hosted calendars only. External calendars (Google, Microsoft) cannot be read or written through the API.
- [Reonic Calendar Categories API](https://apis.io/apis/reonic/reonic-calendar-categories-api/) — Groupings used to organize [**Calendars**](#tag/calendars).
- [Reonic Calendars API](https://apis.io/apis/reonic/reonic-calendars-api/) — Reonic-hosted calendars only. External calendar integrations (Google, Microsoft) are visible inside the Reonic Portal but are not exposed through the public…
- [Reonic Checklist Templates API](https://apis.io/apis/reonic/reonic-checklist-templates-api/) — Reusable checklists. Apply one to a residential project to populate its [**Checklists**](#tag/checklists). > [!warning] > **Beta:** These endpoints are in…
- [Reonic Checklists API](https://apis.io/apis/reonic/reonic-checklists-api/) — The active checklist for a residential project. > [!warning] > **Beta:** These endpoints are in beta and may change as the service evolves. Please report…
- [Reonic Commercial Projects API](https://apis.io/apis/reonic/reonic-commercial-projects-api/) — Commercial customer projects across the request, offer, and installation lifecycle stages. > [!warning] > **Beta:** These endpoints are in beta and may…
- [Reonic Components API](https://apis.io/apis/reonic/reonic-components-api/) — Catalog of solar, storage, EV charger, and heat-pump products available to your workspace.
- [Reonic Contacts API](https://apis.io/apis/reonic/reonic-contacts-api/) — External people you interact with, such as customers or leads. Not to be confused with [**Users**](#tag/users), which represent members of your workspace.
- [Reonic File Folders API](https://apis.io/apis/reonic/reonic-file-folders-api/) — Folders that organize [**Files**](#tag/files) within a project or contact. > [!note] > Personal and template folders are not exposed via the API.
- [Reonic Files API](https://apis.io/apis/reonic/reonic-files-api/) — Files attached to a project or contact. File responses include a download URL valid for 24 hours; refetch the file to obtain a fresh URL after it expires.
- [Reonic Kanban Boards API](https://apis.io/apis/reonic/reonic-kanban-boards-api/) — Kanban boards used to group project columns within a lifecycle stage such as request, offer, or installation.
- [Reonic Kanban Columns API](https://apis.io/apis/reonic/reonic-kanban-columns-api/) — Kanban columns projects move through on a [**Kanban Boards**](#tag/kanban-boards).
- [Reonic Lead Sources API](https://apis.io/apis/reonic/reonic-lead-sources-api/) — Channels that brought a customer/contact to your workspace, such as referrals, ad campaigns, or partner integrations. Used to attribute projects to their…
- [Reonic Links API](https://apis.io/apis/reonic/reonic-links-api/) — Resolve a resource into a URL where it can be viewed in the Reonic web app.
- [Reonic Notes API](https://apis.io/apis/reonic/reonic-notes-api/) — Free-text notes attached to a project or contact.
- [Reonic Offer Templates API](https://apis.io/apis/reonic/reonic-offer-templates-api/) — Pre-configured combinations of planning packages used to quickly populate package categories when creating an offer. > [!warning] > **Beta:** These…
- [Reonic Photogrammetry API](https://apis.io/apis/reonic/reonic-photogrammetry-api/) — 3D reconstruction jobs built from uploaded site imagery. > [!warning] > **Beta:** These endpoints are in beta and may change as the service evolves. Please…
- [Reonic Planning Packages API](https://apis.io/apis/reonic/reonic-planning-packages-api/) — Standard offer packages for PV, storage, heat pumps, and EV chargers, built from common [**Components**](#tag/components) and service combinations.
- [Reonic Planning Templates API](https://apis.io/apis/reonic/reonic-planning-templates-api/) — Small groups of [**Components**](#tag/components) that can be added to targeted planning sections when a project type or requirement calls for extra components.
- [Reonic Residential Projects API](https://apis.io/apis/reonic/reonic-residential-projects-api/) — Residential customer projects across the request, offer, and installation lifecycle stages.
- [Reonic Signature Requests API](https://apis.io/apis/reonic/reonic-signature-requests-api/) — Requests sent to a customer to sign a residential project's offer. Each carries the offer PDF for every variant the customer can choose between, available…
- [Reonic Tags API](https://apis.io/apis/reonic/reonic-tags-api/) — Reusable labels for categorizing and filtering projects, contacts, and other entities.
- [Reonic Tasks API](https://apis.io/apis/reonic/reonic-tasks-api/) — To-do items attached to a project or contact, with due dates, assignees, and completion state. > [!warning] > **Beta:** These endpoints are in beta and may…
- [Reonic Teams API](https://apis.io/apis/reonic/reonic-teams-api/) — Groups of users. Teams can be assigned to projects and nested under one another.
- [Reonic Time Tracking API](https://apis.io/apis/reonic/reonic-time-tracking-api/) — Time entries logged against projects. > [!warning] > **Beta:** These endpoints are in beta and may change as the service evolves. Please report issues or…
- [Reonic Upload API](https://apis.io/apis/reonic/reonic-upload-api/) — Two-step uploads for endpoints that accept user-provided file content. Call `POST /uploads/create` to obtain an `uploadUrl` and an `uploadId`. `PUT` the raw…
- [Reonic Users API](https://apis.io/apis/reonic/reonic-users-api/) — Members of your workspace, such as employees. Not to be confused with [**Contacts**](#tag/contacts), which represent external people like customers or leads.
- [Reonic Wiki API](https://apis.io/apis/reonic/reonic-wiki-api/) — Your company's shared knowledge base — pages and folders. > [!warning] > **Beta:** These endpoints are in beta and may change as the service evolves. Please…
- [Reonic Webhooks API](https://apis.io/apis/reonic/reonic-webhooks-api/) — Webhooks notify your systems the moment something happens in Reonic. For example when a project is created or an offer is signed. Instead of repeatedly…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (2)

Event-driven and webhook contracts.

- [Reonic Webhooks](https://apis.io/asyncapis/reonic/reonic-webhooks/)
- [Reonic Webhooks](https://apis.io/asyncapis/reonic/reonic-webhooks-asyncapi/)

#### Event channels (17)

Individual events and webhooks the provider emits.

- [commercialProject_created](https://apis.io/channels/reonic/commercialproject-created/)
- [commercialProject_dealStateChanged](https://apis.io/channels/reonic/commercialproject-dealstatechanged/)
- [commercialProject_kanbanColumnChanged](https://apis.io/channels/reonic/commercialproject-kanbancolumnchanged/)
- [contact_created](https://apis.io/channels/reonic/contact-created/)
- [project_archived](https://apis.io/channels/reonic/project-archived/)
- [project_created](https://apis.io/channels/reonic/project-created/)
- [project_dealStateChanged](https://apis.io/channels/reonic/project-dealstatechanged/)
- [project_kanbanColumnChanged](https://apis.io/channels/reonic/project-kanbancolumnchanged/)
- [projectChecklist_pdfGenerated](https://apis.io/channels/reonic/projectchecklist-pdfgenerated/)
- [projectChecklist_segmentCompletionChanged](https://apis.io/channels/reonic/projectchecklist-segmentcompletionchanged/)
- [residentialOffer_signatureRequested](https://apis.io/channels/reonic/residentialoffer-signaturerequested/)
- [residentialOffer_signatureWithdrawn](https://apis.io/channels/reonic/residentialoffer-signaturewithdrawn/)
- [residentialOffer_signed](https://apis.io/channels/reonic/residentialoffer-signed/)
- [residentialProject_created](https://apis.io/channels/reonic/residentialproject-created/)
- [residentialProject_dealStateChanged](https://apis.io/channels/reonic/residentialproject-dealstatechanged/)
- [residentialProject_kanbanColumnChanged](https://apis.io/channels/reonic/residentialproject-kanbancolumnchanged/)
- [test](https://apis.io/channels/reonic/test/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [reonic](https://apis.io/servers/reonic/reonic/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Reonic Agentic Access](https://apis.io/agentic-access/reonic/reonic-agentic-access/)

#### Collections (29)

Postman and Open Collection request collections.

- [Reonic REST Api v3 Activities API](https://apis.io/collections/reonic/open-reonic-activities-api/)
- [Reonic REST Api v3 Activities Appointments API](https://apis.io/collections/reonic/open-reonic-appointments-api/)
- [Reonic REST Api v3 Activities Calendar Categories API](https://apis.io/collections/reonic/open-reonic-calendar-categories-api/)
- [Reonic REST Api v3 Activities Calendars API](https://apis.io/collections/reonic/open-reonic-calendars-api/)
- [Reonic REST Api v3 Activities Checklist Templates API](https://apis.io/collections/reonic/open-reonic-checklist-templates-api/)
- [Reonic REST Api v3 Activities Checklists API](https://apis.io/collections/reonic/open-reonic-checklists-api/)
- [Reonic REST Api v3 Activities Commercial Projects API](https://apis.io/collections/reonic/open-reonic-commercial-projects-api/)
- [Reonic REST Api v3 Activities Components API](https://apis.io/collections/reonic/open-reonic-components-api/)
- [Reonic REST Api v3 Activities Contacts API](https://apis.io/collections/reonic/open-reonic-contacts-api/)
- [Reonic REST Api v3 Activities File Folders API](https://apis.io/collections/reonic/open-reonic-file-folders-api/)
- [Reonic REST Api v3 Activities Files API](https://apis.io/collections/reonic/open-reonic-files-api/)
- [Reonic REST Api v3 Activities Kanban Boards API](https://apis.io/collections/reonic/open-reonic-kanban-boards-api/)
- [Reonic REST Api v3 Activities Kanban Columns API](https://apis.io/collections/reonic/open-reonic-kanban-columns-api/)
- [Reonic REST Api v3 Activities Lead Sources API](https://apis.io/collections/reonic/open-reonic-lead-sources-api/)
- [Reonic REST Api v3 Activities Links API](https://apis.io/collections/reonic/open-reonic-links-api/)
- [Reonic REST Api v3 Activities Notes API](https://apis.io/collections/reonic/open-reonic-notes-api/)
- [Reonic REST Api v3 Activities Offer Templates API](https://apis.io/collections/reonic/open-reonic-offer-templates-api/)
- [Reonic REST Api v3 Activities Photogrammetry API](https://apis.io/collections/reonic/open-reonic-photogrammetry-api/)
- [Reonic REST Api v3 Activities Planning Packages API](https://apis.io/collections/reonic/open-reonic-planning-packages-api/)
- [Reonic REST Api v3 Activities Planning Templates API](https://apis.io/collections/reonic/open-reonic-planning-templates-api/)
- [Reonic REST Api v3 Activities Residential Projects API](https://apis.io/collections/reonic/open-reonic-residential-projects-api/)
- [Reonic REST Api v3 Activities Signature Requests API](https://apis.io/collections/reonic/open-reonic-signature-requests-api/)
- [Reonic REST Api v3 Activities Tags API](https://apis.io/collections/reonic/open-reonic-tags-api/)
- [Reonic REST Api v3 Activities Tasks API](https://apis.io/collections/reonic/open-reonic-tasks-api/)
- [Reonic REST Api v3 Activities Teams API](https://apis.io/collections/reonic/open-reonic-teams-api/)
- …and 4 more published on APIs.io

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Reonic V3 Overlay](https://apis.io/overlays/reonic/reonic-v3-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Reonic Authentication](https://apis.io/security/reonic/reonic-authentication/)
- [Reonic Domain Security](https://apis.io/security/reonic/reonic-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://reonic.de)
- [Documentation](https://docs.reonic.de/docs/category/integrationen/)
- [API reference](https://api.reonic.de/rest/v3/docs)
- [Sign up](https://portal.reonic.de)
- [Blog](https://reonic.com/de-de/blog/)
- [Terms of service](https://reonic.com/de-de/legal/terms/)
- [Privacy policy](https://reonic.com/de-de/legal/dataprotection/)
- [GitHub](https://github.com/reonic)

## API Evangelist rating

**Kin Score 39.8** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 55.7 |
| Contract governance | 4.5 |
| Operational transparency | 34.2 |
| Developer ergonomics | 44.6 |
| Access clarity | 23.7 |

**Agent readiness 30.0** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 17.2** — Energy & Utilities

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/reonic/](https://apis.io/providers/reonic/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Reonic: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/reonic/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
