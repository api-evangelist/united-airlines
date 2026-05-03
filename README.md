# United Airlines (united-airlines)

United Airlines is a major American airline headquartered in Chicago, Illinois, operating one of the world's largest route networks with hubs in Chicago, Denver, Houston, Los Angeles, New York, San Francisco, and Washington, D.C. United provides NDC (New Distribution Capability) APIs for flight shopping, booking, and servicing, enabling travel agencies and corporate booking tools to access continuous pricing, dynamic bundles, and full servicing capabilities.

**URL:** [View APIs.json](https://raw.githubusercontent.com/api-evangelist/united-airlines/refs/heads/main/apis.yml)

## Scope

- **Type:** Company
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Airlines
- Travel
- Flight Booking
- NDC
- Loyalty
- Fortune 100

## Timestamps

- **Created:** 2026-03-21
- **Modified:** 2026-05-03

## APIs

### United Airlines NDC API

United Airlines NDC API enables travel agencies, online booking tools, and corporate travel platforms to search, book, and service United flights. Features include continuous pricing, dynamic bundled fares (30+ combinations), ancillary products, hold bookings, exchanges, refunds, cancellations, schedule change alerts, and ARC/BSP reporting.

- **Human URL:** [https://united.business/NDC-corporate](https://united.business/NDC-corporate)
- **Base URL:** https://api.united.com/v1

#### Properties

| Type | URL |
|---|---|
| Documentation | [https://united.business/NDC-corporate](https://united.business/NDC-corporate) |
| NDC Capabilities | [https://united.business/NDC-capabilities](https://united.business/NDC-capabilities) |
| OpenAPI | [united-airlines-ndc-openapi.yml](openapi/united-airlines-ndc-openapi.yml) |

### United Airlines Flight Status API

Real-time flight status API providing estimated and actual departure/arrival times, gate information, and delay tracking for United-operated flights via the IATA Developer Portal.

- **Human URL:** [https://api.developer.iata.org/united-airlines-united-airlines-default/api/flight-status2](https://api.developer.iata.org/united-airlines-united-airlines-default/api/flight-status2)

## Common Properties

| Type | URL |
|---|---|
| Website | [https://www.united.com](https://www.united.com) |
| Developer Portal | [https://united.business/NDC-corporate](https://united.business/NDC-corporate) |
| MileagePlus | [https://www.united.com/en/us/fly/mileageplus.html](https://www.united.com/en/us/fly/mileageplus.html) |
| LinkedIn | [https://www.linkedin.com/company/united-airlines](https://www.linkedin.com/company/united-airlines) |
| X | [https://twitter.com/united](https://twitter.com/united) |

## Artifacts

### OpenAPI Specifications

- [openapi/united-airlines-ndc-openapi.yml](openapi/united-airlines-ndc-openapi.yml) — NDC API covering shopping, booking, servicing, and flight status (11 operations)

### Spectral Rules

- [rules/united-airlines-rules.yml](rules/united-airlines-rules.yml) — Spectral ruleset enforcing United Airlines API conventions

### Naftiko Capabilities

- [capabilities/flight-booking.yaml](capabilities/flight-booking.yaml) — Unified flight booking and travel management workflow (10 MCP tools)
- [capabilities/shared/united-airlines-ndc.yaml](capabilities/shared/united-airlines-ndc.yaml) — Shared per-API NDC definition

### JSON Schema

- [json-schema/united-airlines-booking-schema.json](json-schema/united-airlines-booking-schema.json) — Booking/PNR schema
- [json-schema/united-airlines-flight-status-schema.json](json-schema/united-airlines-flight-status-schema.json) — Flight status schema

### JSON Structure

- [json-structure/united-airlines-booking-structure.json](json-structure/united-airlines-booking-structure.json) — Booking data structure

### JSON-LD Context

- [json-ld/united-airlines-context.jsonld](json-ld/united-airlines-context.jsonld) — Linked data context mapping to schema.org

### Examples

- [examples/united-airlines-searchFlightOffers-example.json](examples/united-airlines-searchFlightOffers-example.json)
- [examples/united-airlines-createBooking-example.json](examples/united-airlines-createBooking-example.json)
- [examples/united-airlines-getFlightStatus-example.json](examples/united-airlines-getFlightStatus-example.json)

### Vocabulary

- [vocabulary/united-airlines-vocabulary.yml](vocabulary/united-airlines-vocabulary.yml) — Domain vocabulary (NDC, PNR, MileagePlus, fare types, etc.)

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com
