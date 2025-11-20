# C4 – System Context

## Primary System

**Travel Booking Platform** – core system that handles search, booking,
payment orchestration and post-booking changes.

## Primary Actors

- **Customer** – searches and books trips via web or mobile.
- **Partner System** – provides hotel, flight or rental-car inventory.
- **Operations Team** – manages bookings, overrides and support cases.

## Relationships

- Customer → Booking Platform: search, book, manage bookings.
- Booking Platform → Partner Systems: availability, pricing, booking API calls.
- Booking Platform → Payment Provider: payment authorization and capture.
- Operations → Booking Platform: manual changes, refunds, corrections.

