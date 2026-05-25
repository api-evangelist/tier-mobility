# TIER (tier-mobility)

TIER Mobility was a Berlin-headquartered shared electric micromobility operator (e-scooters, e-bikes, e-mopeds) founded in 2018. In March 2024 TIER merged with Amsterdam-based Dott to form the combined European micromobility champion, now trading under the **Dott** brand on `ridedott.com` and operating in 400+ cities across roughly 22 countries in Europe, the Middle East, and the Gulf.

All public real-time data is published via **GBFS 2.3** at `https://gbfs.api.ridedott.com/public/v2/{system_id}/`, one `system_id` per city. Feeds are open, unauthenticated, and aligned with the MobilityData GBFS standard.

**URL:** [Visit APIs.yml](https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Mobility, Micromobility, Shared Mobility, E-Scooter, E-Bike, Transportation, Smart Cities, MaaS, GBFS, Open Data, Europe, Real-Time

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### TIER / Dott GBFS API

GBFS 2.3 public feeds covering every Dott (formerly TIER) city. Per-city endpoints return real-time vehicle positions and battery state (`free_bike_status`), vehicle types, pricing plans, station information and status, and geofencing zones.

**Discovery URL (Berlin example):** [https://gbfs.api.ridedott.com/public/v2/berlin/gbfs.json](https://gbfs.api.ridedott.com/public/v2/berlin/gbfs.json)

- [OpenAPI](openapi/tier-mobility-gbfs-openapi.yml)
- [JSON Schema — Vehicle](json-schema/tier-mobility-vehicle-schema.json)
- [JSON Schema — Pricing Plan](json-schema/tier-mobility-pricing-plan-schema.json)
- [JSON-LD context](json-ld/tier-mobility-context.jsonld)
- [Naftiko Capability — GBFS](capabilities/tier-mobility-gbfs.yaml)
- [Spectral rules](rules/tier-mobility-rules.yml)
- [Vocabulary](vocabulary/tier-mobility-vocabulary.yml)
- [Plans / Pricing](plans/tier-mobility-plans-pricing.yml)
- [Rate Limits](rate-limits/tier-mobility-rate-limits.yml)
- [FinOps](finops/tier-mobility-finops.yml)

## Endpoints (per `system_id`)

| Feed | Path |
|---|---|
| GBFS Versions | `/gbfs_versions.json` |
| Discovery | `/{system_id}/gbfs.json` |
| System Information | `/{system_id}/system_information.json` |
| System Pricing Plans | `/{system_id}/system_pricing_plans.json` |
| Vehicle Types | `/{system_id}/vehicle_types.json` |
| Free Vehicle Status | `/{system_id}/free_bike_status.json` |
| Station Information | `/{system_id}/station_information.json` |
| Station Status | `/{system_id}/station_status.json` |
| Geofencing Zones | `/{system_id}/geofencing_zones.json` |

## Coverage

Approximately 340+ active GBFS systems across 22 countries: **AE, AT, BE, CH, DE, DK, ES, FI, FR, GB, GR, HU, IL, IT, NL, NO, PL, QA, SA, SE, SK** and others. Authoritative list maintained in [MobilityData/gbfs `systems.csv`](https://github.com/MobilityData/gbfs/blob/master/systems.csv) — filter by operator `Dott`.

## Examples

- [GBFS Discovery](examples/tier-mobility-gbfs-discovery-example.json)
- [Free Bike Status](examples/tier-mobility-free-bike-status-example.json)
- [Vehicle Types](examples/tier-mobility-vehicle-types-example.json)
- [Pricing Plans](examples/tier-mobility-pricing-plans-example.json)

## Common Properties

- [Website — ridedott.com](https://ridedott.com/)
- [Support](https://help.ridedott.com/)
- [iOS App](https://apps.apple.com/app/id1440301673)
- [Android App](https://play.google.com/store/apps/details?id=com.ridedott.rider)
- [LinkedIn](https://www.linkedin.com/company/ridedott)
- [GBFS Specification](https://github.com/MobilityData/gbfs)
- [MobilityData GBFS Systems Registry](https://github.com/MobilityData/gbfs/blob/master/systems.csv)

## Merger Note

TIER Mobility (founded Berlin, 2018) merged with Dott (founded Amsterdam, 2018) in March 2024. The legacy `tier.app` domain now redirects to `ridedott.com`; the combined company has no public GitHub organization at `github.com/tier-mobility`. All technical surfaces are unified under `gbfs.api.ridedott.com`.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
