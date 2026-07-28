# AnatomIQ Scroll Engine

| Field | Value |
| --- | --- |
| Document ID | AQ-ENG-005 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation, prototype testing, and interaction review |
| Related documents | [Interaction Model](../04-UX/INTERACTION_MODEL.md), [Lesson Experience Flow](../04-UX/LESSON_EXPERIENCE_FLOW.md), [Lesson Engine](LESSON_ENGINE.md), [Accessibility Specification](../04-UX/ACCESSIBILITY_SPECIFICATION.md) |

## Purpose

This document defines the Scroll Engine. The engine converts scroll input into lesson progression while preserving state, orientation, and accessibility.

## Scope

### In scope

- Scroll-driven lesson progression.
- Step boundaries and scroll thresholds.
- Scroll safety and recovery.
- Reduced-motion and alternate progression behavior.

### Out of scope

- Physics-based scrolling simulation.
- Browser-default scrolling behavior without lesson control.
- Non-lesson page scrolling conventions.

## Scroll responsibilities

- Convert scroll movement into approved lesson transitions.
- Avoid skipping or duplicating lesson stages.
- Preserve the current story state during rapid or repeated input.
- Support step-based alternatives when continuous scroll is not appropriate.

## Scroll rules

- Scroll should move the learner forward through the story only when the lesson engine allows it.
- Thresholds should be forgiving enough that the learner does not need precision.
- Large accidental scrolls must not corrupt the lesson state.
- The engine must support recovery to the nearest valid state.

## Interaction modes

| Mode | Purpose |
| --- | --- |
| Narrative step | Advance between major lesson stages |
| Controlled replay | Return to a previous stage within safe bounds |
| Reduced-motion step | Replace continuous scrolling with discrete progression |
| Recovery scroll | Restore a valid lesson position after error or interruption |

## Acceptance criteria

- [ ] Scroll progression is predictable and recoverable.
- [ ] Rapid or repeated scroll input does not break the lesson state.
- [ ] Reduced-motion step progression is supported.
- [ ] AI Context is current.

## Open questions

- [ ] What scroll threshold strategy best balances ease of use and stage accuracy?
- [ ] Should scroll be the primary progression input for all stages or only the guided story?
- [ ] How should the engine behave when a user scrolls in the opposite direction during an active stage?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial Scroll Engine draft for the engineering bible. |

## Review checklist

- [ ] Scroll responsibilities and modes are explicit.
- [ ] State safety and reduced-motion behavior are included.
- [ ] The engine aligns with the lesson flow and accessibility rules.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the scroll engine that advances the lesson without losing state or accessibility support. |
| Constraints | Keep progression safe, forgiving, and recoverable; do not let scroll bypass lesson intent. |
| Inputs | Interaction Model, Lesson Experience Flow, Lesson Engine, Accessibility Specification. |
| Outputs | Scroll rules, thresholds, or recovery behavior. |
| Do not assume | Browser scrolling alone is sufficient for guided lessons. |
| Validation | Confirm scroll actions move through valid lesson states only. |