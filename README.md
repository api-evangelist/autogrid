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
- OpenADR
- IEEE 2030.5
- Smart Grid
- Conformance

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
- **Data standard:** OpenADR 2.0a + 2.0b (VTN/server) and IEEE 2030.5-2018 / CSIP (server) — **certified, with published evidence** (see below). Not found: CTA-2045, IEC CIM 61968/61970, OCPP, OCPI, Green Button/ESPI.
- **Consumer data API:** no. Nothing lets a third party obtain an individual customer's usage or billing data from AutoGrid.
- **Open market data:** no. AutoGrid publishes no grid, market, or system data anonymously.
- **Access gate:** none-published for AutoGrid itself; the successor product is reached only through a Uplight partner/customer login.

## Certified Protocol Surface

AutoGrid published no API description of its own, but its contract exists as **protocol conformance**, and the certifying bodies still publish it:

| Standard | Role | Product | Evidence |
|---|---|---|---|
| OpenADR 2.0a | VTN (server) | AutoGrid DROMS (firmware 1.7, cloud) | [OpenADR registry](https://products.openadr.org/product/autogrid-systems-inc-autogrid-droms/) · DoC signed 2012-11-08 |
| OpenADR 2.0b | VTN (server) | OpenDR Server 2.0 | [OpenADR registry](https://products.openadr.org/product/autogrid-systems-inc-opendr-server-2-0-2/) · PICS v1.0.1 · DoC signed 2013-08-14 |
| IEEE 2030.5-2018 / CSIP | Server | AutoGrid Flex ("Flex 2030.5 server") | [SunSpec certificate CS-000074](https://sunspec.org/wp-content/uploads/2009/03/AutoGrid_Cert_CS-000074.pdf) · Intertek, tested 2023-12-12, awarded 2024-01-22 |

The OpenADR 2.0b PICS declares both A and B profiles, SimpleHTTP-Pull, SimpleHTTP-Push and XMPP-Push transports, the EiEvent / EiOpt / EiReport / EiRegisterParty / OadrPoll services, SHA2 security (TLS 1.2, x.509 SHA2, RSA + ECC), and B-schema validation of all fifteen VTN-generated payloads. The IEEE 2030.5 PICS workbook records 64 passing test cases and 2 not-applicable across aggregator operation, DER identification and group management, the full inverter-control set, events, alarms, meter reading, subscriptions and maintenance. Both surfaces authenticate with **mutual TLS x.509 client certificates** — no API key, no OAuth.

Captured in [`conformance/`](conformance/), with the certificate, PICS and Declaration-of-Conformity PDFs mirrored under [`conformance/documents/`](conformance/documents/).

## Common Properties

- [Protocol conformance profile](conformance/autogrid-conformance.yml)
- [IEEE 2030.5 / CSIP PICS + lab test results](conformance/autogrid-ieee-2030-5-csip-pics.yml)
- [OpenADR 2.0a / 2.0b PICS + Declarations of Conformity](conformance/autogrid-openadr-pics.yml)
- [Lifecycle (acquisition timeline, retirement)](lifecycle/autogrid-lifecycle.yml)
- [Packages — none published](packages/autogrid-packages.yml)
- [Well-known probes — nothing published](well-known/autogrid-well-known.yml)
- [Domain security probe](security/autogrid-domain-security.yml)
- [llms.txt](llms/autogrid-llms.txt)
- [Website](https://auto-grid.com/)
- [Parent Company](https://uplight.com/)
- [GitHub Organization](https://github.com/auto-grid)
- [About](https://uplight.com/resources/derms/)
- [Press Release](https://uplight.com/press/uplight-to-acquire-autogrid/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
