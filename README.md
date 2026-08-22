# Searoutes (searoutes)

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

Searoutes is a maritime routing and carbon-emissions API platform for logistics, freight forwarding, and supply-chain teams. Its REST APIs compute point-to-point, port-to-point, and port-to-port sea routes with distances and durations (including SECA, High Risk Area, and ice-area avoidance), geocode ports, airports, and places, calculate multimodal CO2e emissions (sea, road, rail, air, inland waterway) using a GLEC-accredited methodology, track vessels via AIS (positions, ETAs, traces, arrivals), look up carriers and services, and return historical, real-time, and forecasted weather along routes. All APIs are served from `https://api.searoutes.com` and authenticated with an `x-api-key` header.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/apis.yml)

## Tags

- Maritime
- Sea Routing
- Ocean Freight
- CO2 Emissions
- Carbon Accounting
- Vessel Tracking
- AIS
- Geocoding
- Logistics
- Supply Chain

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## Authentication

All requests go to base URL `https://api.searoutes.com` and must include an `x-api-key` header. A free trial key (valid 7 days, up to 100 calls) is issued on signup; paid access is sold as annual per-product subscription bundles.

## APIs

### Searoutes Ocean Routing API

Compute point-to-point, port-to-point, and port-to-port sea routes between up to twenty coordinates or UN/LOCODEs, returning route geometry, distance in meters, duration in milliseconds, and crossed areas. Supports SECA, High Risk Area, and ice-area avoidance, area blocking, vessel draft and speed inputs, and departure-time-aware planning.

- **Human URL:** [https://developer.searoutes.com/reference/getsearoute](https://developer.searoutes.com/reference/getsearoute)
- **Base URL:** `https://api.searoutes.com`

#### Tags

- Sea Routing
- Ocean Freight
- Distances
- Voyage Planning

#### Properties

- [Documentation](https://developer.searoutes.com/reference/introduction)
- [API Reference](https://developer.searoutes.com/reference/getsearoute)
- [OpenAPI](openapi/searoutes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/searoutes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/searoutes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Searoutes Geocoding API

Resolve ports, airports, terminals, routing areas, postal codes, and arbitrary places by name, UN/LOCODE, or IATA code, find the nearest location or closest sea point to a coordinate, and search all location types in a single call.

- **Human URL:** [https://developer.searoutes.com/reference/introduction](https://developer.searoutes.com/reference/introduction)
- **Base URL:** `https://api.searoutes.com`

#### Tags

- Geocoding
- Ports
- Airports
- Locations

#### Properties

- [Documentation](https://developer.searoutes.com/reference/introduction)
- [OpenAPI](openapi/searoutes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/searoutes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/searoutes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Searoutes CO2 Emissions API

Calculate CO2e emissions for multimodal shipments and individual legs across sea (vessel and trade-lane), road, rail, air, and inland-waterway transport using an ISO 14083 / GLEC-accredited methodology, plus milk-run, carrier-plan, proforma, and ocean-schedule execution emission breakdowns.

- **Human URL:** [https://developer.searoutes.com/reference/introduction](https://developer.searoutes.com/reference/introduction)
- **Base URL:** `https://api.searoutes.com`

#### Tags

- CO2 Emissions
- Carbon Accounting
- GLEC
- Multimodal

#### Properties

- [Documentation](https://developer.searoutes.com/reference/introduction)
- [OpenAPI](openapi/searoutes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/searoutes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/searoutes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Searoutes Vessel Tracking API

Retrieve the latest position of a vessel by IMO or MMSI, look up vessels by name, predict ETAs from AIS, list scheduled port arrivals, and access historical position time series and processed trajectory traces.

- **Human URL:** [https://developer.searoutes.com/reference/introduction](https://developer.searoutes.com/reference/introduction)
- **Base URL:** `https://api.searoutes.com`

#### Tags

- Vessel Tracking
- AIS
- ETA
- Positions

#### Properties

- [Documentation](https://developer.searoutes.com/reference/introduction)
- [OpenAPI](openapi/searoutes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/searoutes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/searoutes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Searoutes Search & Carriers API

Find ocean carriers by name or SCAC code, retrieve carrier details, and search liner services by name with optional carrier filtering to return the vessels and ports on each service.

- **Human URL:** [https://developer.searoutes.com/reference/introduction](https://developer.searoutes.com/reference/introduction)
- **Base URL:** `https://api.searoutes.com`

#### Tags

- Carriers
- Services
- SCAC
- Search

#### Properties

- [Documentation](https://developer.searoutes.com/reference/introduction)
- [OpenAPI](openapi/searoutes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/searoutes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/searoutes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Searoutes Weather API

Query historical (2013-present), real-time, and forecasted weather at a location, retrieve bulk forecasts up to fourteen days out, and obtain weather conditions along a specific route track.

- **Human URL:** [https://developer.searoutes.com/reference/introduction](https://developer.searoutes.com/reference/introduction)
- **Base URL:** `https://api.searoutes.com`

#### Tags

- Weather
- Forecast
- Historical
- Routes

#### Properties

- [Documentation](https://developer.searoutes.com/reference/introduction)
- [OpenAPI](openapi/searoutes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/searoutes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/searoutes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/searoutes)
- [LinkedIn](https://www.linkedin.com/company/searoutes)
- [Website](https://searoutes.com)
- [Documentation](https://developer.searoutes.com/reference/introduction)
- [Plans](plans/searoutes-plans-pricing.yml)
- [Rate Limits](rate-limits/searoutes-rate-limits.yml)
- [Fin Ops](finops/searoutes-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
