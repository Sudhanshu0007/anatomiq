# ADR 001 - Tech Stack

| Field | Value |
| --- | --- |
| Document ID | AQ-ADR-001 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation and before the first application scaffold |
| Related documents | [System Architecture](../06-Engineering/SYSTEM_ARCHITECTURE.md), [Design Vision](../05-Design/DESIGN_VISION.md), [Implementation Plan](../10-Roadmap/IMPLEMENTATION_PLAN.md) |

## Context

AnatomIQ needs a stack that can support a reusable lesson engine, 3D anatomical presentation, data-driven content, accessibility, and future body-system expansion.

## Decision

Use a modern web stack centered on React, TypeScript, and a 3D rendering approach that can support reusable lesson composition and data-driven scene control.

## Rationale

- The project already assumes a web-based experience.
- React and TypeScript support maintainable UI and shared application logic.
- The architecture needs a stack that can support lesson orchestration, scroll-driven navigation, and reusable 3D presentation.
- The stack should be familiar enough to support AI-assisted implementation and review.

## Consequences

- The codebase should organize UI, engine, and content boundaries clearly.
- The team should document engine interfaces and data flow carefully.
- The chosen stack should prioritize maintainability and reuse over novelty.

## Alternatives considered

- A non-React frontend stack: rejected because the documentation and implementation plan already center on reusable UI and shared lesson orchestration.
- A fully custom rendering stack: rejected because it would increase implementation risk without improving the documented MVP goals.

## Acceptance criteria

- [ ] The tech stack decision is clear and aligned with the architecture.
- [ ] The rationale supports reusability and AI-assisted development.
- [ ] The consequences are understood and documented.
- [ ] AI Context is current.

## Open questions

- [ ] Which supporting libraries should be selected later for 3D, animation, and state management?
- [ ] What is the minimal stack needed for the first scaffold versus the full MVP?
- [ ] Should the implementation plan include a separate ADR for the rendering library choice?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial tech stack ADR draft. |

## Review checklist

- [ ] Context, decision, rationale, and consequences are explicit.
- [ ] The decision aligns with the architecture and implementation plan.
- [ ] Alternatives were considered.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Record the technology stack direction for the AnatomIQ MVP. |
| Constraints | Preserve reuse, maintainability, and AI-assisted implementation compatibility. |
| Inputs | System Architecture, Design Vision, Implementation Plan. |
| Outputs | Stack decision and rationale. |
| Do not assume | A stack choice is final without documenting consequences and alternatives. |
| Validation | Confirm the decision supports the reusable lesson engine and MVP delivery. |