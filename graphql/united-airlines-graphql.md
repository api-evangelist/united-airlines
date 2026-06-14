# United Airlines GraphQL Schema

## Overview

This GraphQL schema provides a conceptual representation of the United Airlines flight and travel API domain, covering the NDC (New Distribution Capability) API, Flight Status API, and MileagePlus loyalty program. The schema is derived from United Airlines public developer documentation at https://united.business/NDC-corporate and the IATA developer portal at https://api.developer.iata.org/united-airlines-united-airlines-default/api/flight-status2.

## Schema Source

- **Provider:** United Airlines
- **API:** United Airlines NDC API and Flight Status API
- **Base URL:** https://api.united.com/v1
- **Documentation:** https://united.business/NDC-corporate
- **Schema Type:** Conceptual GraphQL (derived from REST/NDC API surface)

## Domain Coverage

The schema covers the following functional areas:

### Flight Operations
Flight search, schedules, real-time status, delays, cancellations, diversions, gate information, boarding groups, and interconnecting/codeshare flights via Star Alliance partners.

### Booking and Reservation
PNR (Passenger Name Record) management, itinerary building, ticket issuance, seat maps and selection, fare rules, continuous pricing, dynamic bundles, and ancillary product attachment.

### Check-In and Boarding
Online check-in, boarding pass generation, bag check, baggage allowance, excess baggage, and special assistance requests.

### Fares and Pricing
Fare class hierarchy (Basic Economy through Polaris Business), cabin types, fare rules, refund policies, change fees, exchange fees, and voucher management.

### Aircraft and Seats
Aircraft type, seat maps, seat availability, seat preferences, seat upgrade eligibility, and in-flight amenity data (Wi-Fi, entertainment, meal service).

### Loyalty — MileagePlus
Member profiles, status tiers (Silver, Gold, Platinum, 1K, Global Services), Premier Qualifying Points/Flights/Segments, award redemption, and upgrade instruments.

### Airport and Infrastructure
Airport details, terminal assignments, lounge access, and inter-terminal connectivity.

### Passenger Profiles
Traveler identity, known traveler numbers, TSA PreCheck/CLEAR enrollment, pet policy, wheelchair and special assistance needs.

## Types Summary

The schema defines 65 named types organized as:

| Category | Types |
|---|---|
| Flight Operations | Flight, FlightNumber, FlightSchedule, FlightStatus, FlightLeg, FlightSegment, DepartureInfo, ArrivalInfo, Gate, GateChange, BoardingGroup, Delay, Cancellation, Diversion |
| Aircraft | Aircraft, AircraftType, Seat, SeatMap, SeatAvailability, SeatPreference, SeatUpgrade |
| Booking | Booking, Reservation, PNR, Itinerary, Ticket, BoardingPass, Checkin |
| Baggage | BagCheck, BaggageAllowance, BaggageTag, ExcessBaggage |
| Fares | Fare, FareClass, Cabin, BasicEconomy, FareRules, Refund, Voucher, CancelPenalty, Change, ExchangeFee |
| Passenger | Passenger, PassengerProfile |
| Loyalty | FrequentFlyer, MileagePlus, MileagePlusStatus, Points, Award, PQP, PQF, PQS, Upgrade, GlobalServices |
| Airport | Airport, Terminal, InterconnectingFlight, Codeshare, StarAlliance |
| Amenities | LoungeAccess, WiFi, InFlightEntertainment, MealService, PetPolicy, Wheelchair, SpecialAssistance |
| Auth | APIKey, Token |

## Usage Notes

United Airlines distributes its NDC API through agency and corporate partnerships rather than a self-serve developer hub. Access to the NDC API requires onboarding through United's NDC agency program (ndcagency@united.com). Flight status data is also available via the IATA API marketplace. This GraphQL schema is a conceptual translation of the REST/NDC API surface and is intended for schema modeling, tooling integration, and API design reference purposes.
