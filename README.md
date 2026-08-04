# eZee Technosys (ezee)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

eZee Technosys is a hospitality technology company offering eZee Absolute (cloud hotel PMS), eZee Centrix (channel manager), eZee Reservation (booking engine), and eZee Optimus (restaurant POS). Its YCS Connectivity Portal exposes a partner-gated HTTP API for PMS connectivity, channel manager, booking engine, and POS integrations so third-party systems can sync reservations, room inventory, rates, restrictions, and guest data. eZee is now part of Yanolja Cloud (Yanolja Cloud Solution).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/ezee/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/ezee/refs/heads/main/apis.yml)

## Tags

- Hospitality
- Hotel
- PMS
- Channel Manager
- Reservations

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### eZee Reservations & Bookings API

Push and pull reservations through the YCS Connectivity Portal - create bookings, receive new / modified / cancelled booking notifications, and retrieve booking and transaction details for a property. Requests are JSON POST to pms_connectivity.php and authenticated with HotelCode plus AuthCode.

- **Human URL:** [https://api.ezeetechnosys.com/tag/pms-connectivity/](https://api.ezeetechnosys.com/tag/pms-connectivity/)
- **Base URL:** `https://live.ipms247.com/pmsinterface/`

#### Tags

- Reservations
- Bookings
- PMS

#### Properties

- [Documentation](https://api.ezeetechnosys.com/tag/pms-connectivity/)
- [OpenAPI](openapi/ezee-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezee.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezee.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### eZee Room Inventory & Rates API

Manage room inventory, linear and non-linear rates, and stay restrictions (stop-sell, close-on-arrival, close-on-departure, min / max nights). JSON updates POST to pms_connectivity.php; inventory and rate reads are XML POST to getdataAPI.php.

- **Human URL:** [https://api.ezeetechnosys.com/tag/pms-connectivity/](https://api.ezeetechnosys.com/tag/pms-connectivity/)
- **Base URL:** `https://live.ipms247.com/pmsinterface/`

#### Tags

- Inventory
- Rates
- Availability

#### Properties

- [Documentation](https://api.ezeetechnosys.com/tag/pms-connectivity/)
- [OpenAPI](openapi/ezee-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezee.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezee.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### eZee Guests & Configuration API

Retrieve property configuration masters - room types, rate types, rate plans, and source details - alongside guest information carried on bookings. Configuration reads are JSON POST to pms_connectivity.php scoped to a HotelCode.

- **Human URL:** [https://api.ezeetechnosys.com/tag/pms-connectivity/](https://api.ezeetechnosys.com/tag/pms-connectivity/)
- **Base URL:** `https://live.ipms247.com/pmsinterface/`

#### Tags

- Guests
- Profiles
- Configuration

#### Properties

- [Documentation](https://api.ezeetechnosys.com/tag/pms-connectivity/)
- [OpenAPI](openapi/ezee-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezee.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezee.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### eZee Centrix Channel Manager API

An XML interface that lets a third-party PMS connect to the eZee Centrix (Yanolja Cloud Solution) channel manager to two-way sync rates, availability, and reservations across connected OTAs and distribution channels. Provisioned per property through the Connectivity Portal.

- **Human URL:** [https://api.ezeetechnosys.com/](https://api.ezeetechnosys.com/)
- **Base URL:** `https://live.ipms247.com/`

#### Tags

- Channel Manager
- Distribution
- OTA

#### Properties

- [Documentation](https://api.ezeetechnosys.com/)
- [OpenAPI](openapi/ezee-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ezee.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ezee.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/ezee-technosys-pvt-ltd-/)
- [Website](https://www.ezeetechnosys.com)
- [Documentation](https://api.ezeetechnosys.com/)
- [Plans](plans/ezee-plans-pricing.yml)
- [Rate Limits](rate-limits/ezee-rate-limits.yml)
- [Fin Ops](finops/ezee-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
