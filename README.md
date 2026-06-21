# eZee Technosys (ezee)

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
