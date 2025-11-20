# ADR-001 – Architecture Scope and Guardrails

- Status: Accepted
- Date: 2025-11-20
- Owner: Peter Kruth

## Context

The platform has grown organically around a single codebase and database.
Multiple teams touch the same components and data models, which slows down
changes and increases the risk of regressions.

We need a clear scope for "core booking" and guardrails for integrations.

## Decision

We define the "Booking Core" as a separate architectural unit that:

- owns booking lifecycle and state,
- exposes APIs for search, booking, change and cancellation,
- does not directly integrate with frontends or external partners.

Integrations:
- Channels (web, app, agencies) must consume the Booking Core via well-defined APIs.
- Partner integrations are handled by dedicated integration services.

## Consequences

- Positive:
  - Clear ownership for booking logic and data.
  - Easier to reason about changes and test impact.
  - Better alignment with future event-driven patterns.

- Negative:
  - Initial effort to refactor existing code and APIs.
  - Temporary complexity while old and new patterns coexist.

- Follow-ups:
  - Define service boundaries and bounded contexts.
  - Align team structure with architectural responsibilities.

