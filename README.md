# TIER (tier-mobility)

TIER Mobility was a Berlin-headquartered shared electric micromobility operator founded in 2018 by Lawrence Leuschner, Julian Blessin, and Matthias Laug, providing e-scooter, e-bike, and e-moped sharing across European and Middle Eastern cities. In March 2024, TIER merged with Amsterdam-based Dott to form the combined European micromobility champion that now trades under the Dott brand on ridedott.com, operating in 400+ cities across roughly 22 countries including Germany, France, the United Kingdom, Italy, Spain, the Netherlands, Belgium, Sweden, Norway, Finland, Denmark, Austria, Switzerland, Poland, Greece, Hungary, Israel, Saudi Arabia, Qatar, and the UAE. All public real-time data — fleet positions, battery levels, vehicle types, pricing plans, stations, and geofencing zones — is published via GBFS 2.3 (General Bikeshare Feed Specification) endpoints at https://gbfs.api.ridedott.com/public/v2/{system_id}/, with one `system_id` per city. There is no consumer authentication or paid API tier; feeds are open data consumed by city regulators, MaaS aggregators, and trip-planning apps.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- Mobility
- Micromobility
- Shared Mobility
- E-Scooter
- E-Bike
- Transportation
- Smart Cities
- MaaS
- GBFS
- Open Data
- Europe
- Real-Time

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### TIER / Dott GBFS API

GBFS 2.3 public feeds covering every Dott (formerly TIER) city. Per-city endpoints return real-time vehicle positions and battery state (free_bike_status), vehicle types, pricing plans, station information and status, and geofencing zones. Unauthenticated, free, and aligned with the MobilityData GBFS standard.

- **Human URL:** [https://gbfs.api.ridedott.com/public/v2/berlin/gbfs.json](https://gbfs.api.ridedott.com/public/v2/berlin/gbfs.json)

#### Tags

- GBFS
- Micromobility
- Real-Time
- Open Data

#### Properties

- [G B F S](https://gbfs.api.ridedott.com/public/v2/berlin/gbfs.json)
- [OpenAPI](openapi/tier-mobility-gbfs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tier-mobility-gbfs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tier-mobility-gbfs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tier-mobility-vehicle-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tier-mobility-pricing-plan-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/tier-mobility-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/tier-mobility-rules.yml)
- [Vocabulary](vocabulary/tier-mobility-vocabulary.yml)
- [Plans](plans/tier-mobility-plans-pricing.yml)
- [Rate Limits](rate-limits/tier-mobility-rate-limits.yml)
- [Fin Ops](finops/tier-mobility-finops.yml)
- [Example](examples/tier-mobility-gbfs-discovery-example.json)
- [Example](examples/tier-mobility-free-bike-status-example.json)
- [Example](examples/tier-mobility-vehicle-types-example.json)
- [Example](examples/tier-mobility-pricing-plans-example.json)
- [Standard](https://github.com/MobilityData/gbfs)

## Common Properties

- [Website](https://ridedott.com/)
- [Company](https://ridedott.com/about)
- [Newsroom](https://ridedott.com/press)
- [Careers](https://ridedott.com/careers)
- [Privacy Policy](https://ridedott.com/privacy)
- [Terms of Service](https://ridedott.com/terms)
- [Support](https://help.ridedott.com/)
- [i O S App](https://apps.apple.com/app/id1440301673)
- [Android App](https://play.google.com/store/apps/details?id=com.ridedott.rider)
- [LinkedIn](https://www.linkedin.com/company/ridedott)
- [Twitter](https://twitter.com/ridedott)
- [Standard](https://github.com/MobilityData/gbfs)
- [G B F S](https://gbfs.api.ridedott.com/public/v2/gbfs_versions.json)
- [Systems Registry](https://github.com/MobilityData/gbfs/blob/master/systems.csv)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
**URL:** https://apievangelist.com
