# TIER (tier-mobility)

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
