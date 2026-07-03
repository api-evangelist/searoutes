# Searoutes (searoutes)

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
