# AnatomIQ Camera System

| Field | Value |
| --- | --- |
| Document ID | AQ-ENG-004 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation, motion review, and prototype testing |
| Related documents | [Camera Language](../05-Design/CAMERA_LANGUAGE.md), [Motion and Animation](../05-Design/MOTION_AND_ANIMATION.md), [Accessibility Specification](../04-UX/ACCESSIBILITY_SPECIFICATION.md), [Lesson Engine](LESSON_ENGINE.md) |

## Purpose

This document defines the Camera System. The camera must support orientation, focus, inspection, and return-to-context behavior in the AnatomIQ lesson experience.

## Scope

### In scope

- Camera framing and transitions.
- Focus and inspection behavior.
- Return-to-context behavior.
- Reduced-motion and recovery handling.

### Out of scope

- Specific engine API implementation.
- Lens or shader detail beyond the lesson need.
- Free-roam exploratory camera sandbox behavior.

## Camera responsibilities

- Frame the active anatomy or lesson stage.
- Move the learner through key lesson transitions.
- Support focus-on-structure and return-to-body-context actions.
- Respect reduced-motion and accessibility settings.

## Camera modes

| Mode | Purpose |
| --- | --- |
| Context | Show the body or system at a comprehensible scale |
| Focus | Bring attention to the current structure or event |
| Follow | Track flow or motion when it helps understanding |
| Inspect | Allow closer look at a selected structure |
| Return | Restore the broader orientation after inspection |

## Camera rules

- Camera changes must be clearly linked to the lesson step.
- The learner must never lose orientation without a way back.
- Sudden movement should be avoided unless it is necessary and explained.
- Reduced-motion settings should reduce or replace camera travel where possible.

## Camera interface expectations

- Provide explicit hooks for lesson stages to request framing.
- Allow the camera to return to a canonical body context.
- Support consistent behavior when annotations or overlays are opened.
- Preserve context during replay and review.

## Acceptance criteria

- [ ] The camera supports the lesson’s orientation and focus needs.
- [ ] The learner can return to body context after inspection.
- [ ] Camera behavior stays aligned with accessibility settings.
- [ ] AI Context is current.

## Open questions

- [ ] How many camera presets are needed for the MVP lesson flow?
- [ ] Should camera transitions be authored as part of lesson data or defined in the engine runtime?
- [ ] What is the minimal reset framing that works across body systems?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial Camera System draft for the engineering bible. |

## Review checklist

- [ ] Camera modes and responsibilities are explicit.
- [ ] Orientation, focus, and return behavior are defined.
- [ ] Reduced-motion expectations are included.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the camera system that supports lesson orientation, inspection, and recovery. |
| Constraints | Keep the learner oriented, support reduced motion, and align camera changes with lesson intent. |
| Inputs | Camera Language, Motion and Animation, Lesson Engine, Accessibility Specification. |
| Outputs | Camera modes, responsibilities, or interface expectations. |
| Do not assume | Camera motion can be arbitrary or detached from the lesson stage. |
| Validation | Confirm the learner can always return to a useful contextual framing. |