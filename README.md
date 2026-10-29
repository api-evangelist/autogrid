# AutoGrid

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

AutoGrid Systems is a United States grid-technology company founded in 2011 by Amit Narayan in Redwood City, California, that built AI and machine-learning software for distributed energy resource management (DERMS), virtual power plants, and automated demand response under the AutoGrid Flex platform, selling to investor-owned utilities, retailers, and aggregators rather than to end consumers. It sits on the grid-tech / DERMS layer of the energy value chain - a buyer and orchestrator of utility and device data, not a data custodian - so no Green Button, Consumer Data Right, or smart-meter data-sharing obligation attaches to it. Schneider Electric took control of AutoGrid and then sold it to Uplight in a deal announced 14 December 2023 and closed in early 2024; auto-grid.com now serves only a 270-byte meta-refresh to uplight.com (on an expired TLS certificate as of 27 July 2026) and every developer, docs, api, and data subdomain fails to resolve. Its API posture is therefore honestly none-published - no public developer portal, no OpenAPI, no SDK, no consumer usage API, and no open market data. Its machine-readable contract is instead expressed as protocol conformance, and that is real and still published by the certifying bodies. AutoGrid is a certified OpenADR 2.0a and 2.0b VTN (server) - AutoGrid DROMS and OpenDR Server 2.0, Simple HTTP + XMPP, pull and push - and holds SunSpec Alliance certificate CS-000074 for AutoGrid Flex as an IEEE 2030.5-2018 / CSIP server, tested by Intertek on 12 December 2023 and awarded 22 January 2024. Both surfaces authenticate with mutual TLS x.509 client certificates and were reachable only under commercial contract. The successor surface at docs.uplight.com is real but fully login-gated, redirecting anonymous visitors to a ReadMe dashboard login, and api.uplight.com answers HTTP 401 with "Invalid or no token provided" - partner and customer access only.

**Areas:** Energy · United States · Utilities · Electricity · Grid · DERMS · Distributed Energy Resources · Virtual Power Plant · Demand Response · Acquired · OpenADR · IEEE 2030.5

## AutoGrid on APIs.io

Everything profiled for AutoGrid is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/autogrid/](https://apis.io/providers/autogrid/)** — or go straight to one of the APIs or properties below.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (2)

Model Context Protocol servers that expose the API to agents.

- [Moved to /providers/autogrid/](https://apis.io/servers/autogrid/autogrid/)
- [Moved to /providers/autogrid/](https://apis.io/servers/autogrid/autogrid-2/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Autogrid Domain Security](https://apis.io/security/autogrid/autogrid-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://auto-grid.com/)
- [Compliance](https://sunspec.org/contributing-members/autogrid-2/)
- [GitHub](https://github.com/auto-grid)

## API Evangelist rating

**Kin Score 9.6** — minimal · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 55.0 |
| Contract quality | 0.0 |
| Contract governance | 18.2 |
| Operational transparency | 2.6 |
| Developer ergonomics | 0.0 |
| Access clarity | 7.9 |

**Agent readiness 2.2** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | platform (partial credit) |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 13.1** — Energy & Utilities

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/autogrid/](https://apis.io/providers/autogrid/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for AutoGrid: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/autogrid/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
