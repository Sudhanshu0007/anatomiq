# ADR 002 - Scroll Narrative

| Field | Value |
| --- | --- |
| Document ID | AQ-ADR-002 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before lesson implementation and before interaction engine work |
| Related documents | [Lesson Experience Flow](../04-UX/LESSON_EXPERIENCE_FLOW.md), [Interaction Model](../04-UX/INTERACTION_MODEL.md), [Scroll Engine](../06-Engineering/SCROLL_ENGINE.md), [Product Philosophy](../01-Vision/PRODUCT_PHILOSOPHY.md) |

## Context

The project vision and UX specification both favor a guided, scroll-driven educational story for the cardiovascular MVP. The interaction should move the learner through the route without trapping them in motion.

## Decision

Use scroll as the primary narrative progression mechanism for the guided lesson, with discrete stage boundaries and alternate controls for pause, replay, and reduced-motion access.

## Rationale

- Scroll supports a cinematic lesson flow that still feels learner-controlled.
- The narrative can move through the cardiovascular route in a clear sequence.
- The interaction model and accessibility specification require alternatives and safe recovery.
- Discrete boundaries prevent accidental over-scrolling from breaking the lesson.

## Consequences

- The Scroll Engine must convert scroll input into valid lesson transitions.
- Reduced-motion and step-based alternatives remain required.
- The lesson must never depend on precise scrolling to remain understandable.
- The narrative sequence must be authored with clear stage boundaries.

## Alternatives considered

- Page-by-page navigation: rejected because it would weaken the continuous learning story.
- Freeform scrolling without stage boundaries: rejected because it would make the lesson harder to control and review.
- Video-only storytelling: rejected because the product requires learner agency and reviewable interaction.

## Acceptance criteria

- [ ] The scroll narrative decision is explicit and aligned to the UX documents.
- [ ] The consequence of needing discrete boundaries is documented.
- [ ] Accessibility and review controls remain required.
- [ ] AI Context is current.

## Open questions

- [ ] How should scroll thresholds be tuned for the first prototype?
- [ ] Which stages should be tied to explicit learner actions versus passive scroll progression?
- [ ] How should reverse scroll behave during review or return-to-context actions?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial scroll narrative ADR draft. |

## Review checklist

- [ ] The decision, rationale, and consequences are explicit.
- [ ] The choice aligns with the UX specification and accessibility requirements.
- [ ] Alternatives were considered.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Record the decision to use scroll as the primary lesson narrative mechanism. |
| Constraints | Preserve learner control, stage boundaries, and accessibility alternatives. |
| Inputs | Lesson Experience Flow, Interaction Model, Scroll Engine, Product Philosophy. |
| Outputs | Scroll narrative decision and implementation consequences. |
| Do not assume | Scroll alone is sufficient without discrete stage control and fallback paths. |
| Validation | Confirm the lesson can be advanced, reviewed, and reduced-motion access remains available. |