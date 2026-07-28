# AnatomIQ Motion and Animation

| Field | Value |
| --- | --- |
| Document ID | AQ-DSN-005 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before animation production, prototype testing, and motion review |
| Related documents | [Lesson Experience Flow](../04-UX/LESSON_EXPERIENCE_FLOW.md), [Interaction Model](../04-UX/INTERACTION_MODEL.md), [Accessibility Specification](../04-UX/ACCESSIBILITY_SPECIFICATION.md), [Camera Language](CAMERA_LANGUAGE.md) |

## Purpose

This document defines the motion direction for AnatomIQ. Motion should improve attention, orientation, and comprehension while preserving control and accessibility.

## Scope

### In scope

- Scene motion and transition behavior.
- Flow animation and emphasis motion.
- Reduced-motion considerations.
- Motion rules for overlays and feedback.

### Out of scope

- Low-level animation engine setup.
- Full motion curves and timing values.
- Decorative motion unrelated to the lesson objective.

## Motion principles

- Motion must teach, orient, or clarify.
- Motion should never be decorative by default.
- The learner must be able to pause or reduce motion when needed.
- Motion must not obscure labels, controls, or important structures.

## Motion categories

| Category | Purpose |
| --- | --- |
| Narrative motion | Move the learner through the lesson story |
| Emphasis motion | Highlight a structure or event |
| Transition motion | Move between states or screens |
| Feedback motion | Confirm correct actions or show recoverable errors |
| Reduced-motion substitute | Preserve meaning without continuous movement |

## Motion rules

- Use motion to show change over time where that change is central to the concept.
- Keep motion pace understandable for a learner trying to follow anatomy.
- Avoid stacking multiple strong motions at once.
- Provide a stable fallback for learners who cannot or do not want continuous motion.
- Motion should never replace explanation.

## Motion acceptance criteria

- [ ] Motion supports the educational story.
- [ ] Motion can be paused or reduced for accessibility.
- [ ] Motion does not obscure core information.
- [ ] AI Context is current.

## Open questions

- [ ] Which motions are essential and which are only helpful embellishments?
- [ ] How much motion should be reserved for the cardiovascular MVP before the lesson becomes too busy?
- [ ] Should motion timing be standardized across all lesson stages or vary by concept type?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial motion and animation draft for the design bible. |

## Review checklist

- [ ] Motion categories and rules are explicit.
- [ ] Accessibility and reduced-motion needs are included.
- [ ] Motion is tied to educational purpose.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define how motion should be used across AnatomIQ lessons and interfaces. |
| Constraints | Motion must serve comprehension, remain pausable or reducible, and never obscure essential content. |
| Inputs | Lesson Experience Flow, Interaction Model, Accessibility Specification, Camera Language. |
| Outputs | Motion rules, categories, or accessibility substitutions. |
| Do not assume | More motion means better learning. |
| Validation | Verify the lesson remains understandable with motion reduced or paused. |