# AnatomIQ Camera Language

| Field | Value |
| --- | --- |
| Document ID | AQ-DSN-007 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before motion blocking, prototype testing, and camera-system review |
| Related documents | [Lesson Experience Flow](../04-UX/LESSON_EXPERIENCE_FLOW.md), [Navigation Model](../04-UX/NAVIGATION_MODEL.md), [Interaction Model](../04-UX/INTERACTION_MODEL.md), [Motion System](MOTION_SYSTEM.md) |

## Purpose

This document defines how the camera should behave in AnatomIQ. Camera language must help the learner orient, inspect, and follow the lesson without losing context.

## Scope

### In scope

- Camera framing rules.
- Transition behavior between lesson stages.
- Focus, zoom, and return-to-context behavior.
- Camera rules for learner control and recovery.

### Out of scope

- Implementation details for a specific 3D library.
- Low-level animation curve parameters.
- Advanced free-camera sandbox behavior not needed for the MVP.

## Camera principles

- The camera must tell the learner where they are.
- Movement must have a teaching purpose.
- Camera changes should be smooth enough to orient the learner, not to show off.
- The learner must always have a path back to broader context.

## Camera roles

| Role | Purpose |
| --- | --- |
| Orientation | Establish where the body/system/lesson is located |
| Focus | Bring the learner close to the active structure or process |
| Follow | Track a key route or event when useful for understanding |
| Return | Restore broader context without losing progress |
| Inspect | Support detail review of a structure or annotation |

## Camera rules

- Avoid sudden movement unless it is necessary for a controlled transition.
- Do not make the learner guess what the camera is trying to show.
- Pair camera changes with labels, explanation, or state cues.
- Respect reduced-motion or step-based paths when motion is not essential.
- Return-to-context behavior must be predictable and easy to locate.

## Camera acceptance criteria

- [ ] Camera movement supports orientation and teaching.
- [ ] The learner can return to a broader context after focusing on detail.
- [ ] Camera changes are clear and do not break lesson state.
- [ ] AI Context is current.

## Open questions

- [ ] How much camera motion is needed before the lesson becomes disorienting?
- [ ] Should all major camera moves be tied to scroll or can some be triggered by explicit controls?
- [ ] What should the default reset framing be for the whole-body context?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial camera language draft for the design bible. |

## Review checklist

- [ ] Camera roles and rules are explicit.
- [ ] Orientation, focus, and return are covered.
- [ ] The camera supports learner control and recovery.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define how camera movement should support teaching and learner orientation in AnatomIQ. |
| Constraints | Preserve context, support reduced motion, and pair motion with clear educational cues. |
| Inputs | Lesson Experience Flow, Navigation Model, Interaction Model, Motion System. |
| Outputs | Camera roles, movement rules, or framing guidance. |
| Do not assume | Free-form camera movement improves comprehension. |
| Validation | Confirm the learner can orient, inspect, and return without losing the lesson context. |