# AutoGrid (autogrid)

AutoGrid Systems is a United States grid-technology company founded in 2011 by Amit Narayan in Redwood City, California, that built AI and machine-learning software for distributed energy resource management (DERMS), virtual power plants, and automated demand response under the AutoGrid Flex platform, selling to investor-owned utilities, retailers, and aggregators rather than to end consumers. It sits on the grid-tech / DERMS layer of the energy value chain — a buyer and orchestrator of utility and device data, not a data custodian — so no Green Button, Consumer Data Right, or smart-meter data-sharing obligation attaches to it. Schneider Electric took control of AutoGrid and then sold it to Uplight in a deal announced 14 December 2023 and closed in early 2024; auto-grid.com now serves only a 270-byte meta-refresh to uplight.com (on an expired TLS certificate as of 27 July 2026) and every developer, docs, api, and data subdomain fails to resolve. Its API posture is therefore honestly none-published — no public developer portal, no OpenAPI, no consumer usage API, and no open market data. The successor surface at docs.uplight.com is real but fully login-gated, redirecting anonymous visitors to a ReadMe dashboard login, and api.uplight.com answers HTTP 401 with "Invalid or no token provided" — partner and customer access only.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/autogrid/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/autogrid/refs/heads/main/apis.yml)

## Tags

- Energy
- United States
- Utilities
- Electricity
- Grid
- DERMS
- Distributed Energy Resources
- Virtual Power Plant
- Demand Response
- Acquired

## Timestamps

- **Created:** 2026-07-27
- **Modified:** 2026-07-27

## APIs

No public, documented APIs were found for AutoGrid.

The company's primary domain, `auto-grid.com`, resolves (35.208.127.125) but serves a single 270-byte HTML meta-refresh to `https://uplight.com` on **every** path — `/`, `/developers`, `/api`, `/docs`, `/robots.txt`, `/openapi.json`, `/.well-known/openid-configuration`, and `/favicon.ico` all return the identical document. Its Let's Encrypt certificate (CN=auto-grid.com) **expired on 24 July 2026**, so plain HTTPS requests fail certificate verification. No `api.`, `developer.`, `developers.`, `data.`, `portal.`, `app.`, `flex.`, or `partner.` subdomain resolves in DNS; `docs.auto-grid.com` points at `ghs.google.com` and returns a Google 404.

AutoGrid's GitHub organization, [github.com/auto-grid](https://github.com/auto-grid), holds three public repositories — all forks of unrelated third-party projects (`external-storage`, `nifi`, `null`). No API contract, SDK, or specification is published there.

The product now lives inside Uplight. `docs.uplight.com` is a live ReadMe hub, but every content path (`/developer/docs`, `/developer/reference`, `/developer/page/contact-support`) redirects anonymous visitors to `dash.readme.com/to/uplight` for login, and `api.uplight.com` returns `401 {"errors":[{"message":"Invalid or no token provided"}]}`. Access is partner/customer only.

## Mandate and Data Posture

- **Mandate regime:** none. AutoGrid is a software vendor and DER orchestrator, not a utility, retailer, or metering data custodian. Green Button / NAESB ESPI obligations attach to data custodians; the Australian Consumer Data Right and Ontario's Green Button regulation do not reach a US DERMS vendor.
- **Mandate status:** not-applicable. No obligation was found, and none is claimed by the company.
- **Data standard:** no first-party standard reference found. Third-party commentary associates DERMS aggregators of this class with OpenADR, IEEE 2030.5, and CTA-2045, but no AutoGrid or Uplight documentation confirming conformance was reachable — the AutoGrid site is retired and the Uplight docs are gated.
- **Consumer data API:** no. Nothing lets a third party obtain an individual customer's usage or billing data from AutoGrid.
- **Open market data:** no. AutoGrid publishes no grid, market, or system data anonymously.
- **Access gate:** none-published for AutoGrid itself; the successor product is reached only through a Uplight partner/customer login.

## Common Properties

- [Website](https://auto-grid.com/)
- [Parent Company](https://uplight.com/)
- [GitHub Organization](https://github.com/auto-grid)
- [About](https://uplight.com/resources/derms/)
- [Press Release](https://uplight.com/press/uplight-to-acquire-autogrid/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
