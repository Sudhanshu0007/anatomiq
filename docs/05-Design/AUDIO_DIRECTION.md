# AnatomIQ Audio Direction

| Field | Value |
| --- | --- |
| Document ID | AQ-DSN-007 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before audio production, prototype testing, and accessibility review |
| Related documents | [Brand Identity](BRAND_IDENTITY.md), [Motion and Animation](MOTION_AND_ANIMATION.md), [UX Copy and Feedback](../04-UX/UX_COPY_AND_FEEDBACK.md), [Accessibility Specification](../04-UX/ACCESSIBILITY_SPECIFICATION.md) |

## Purpose

This document defines the audio direction for AnatomIQ. Audio should support atmosphere, orientation, and feedback when it genuinely helps the lesson.

## Scope

### In scope

- Ambient and feedback audio direction.
- Narration and instructional audio considerations.
- Sound cues for interactions.
- Accessibility expectations for captioning and transcripts when needed.

### Out of scope

- Full sound design implementation.
- Audio engine configuration.
- Music licensing or production specifics.

## Audio principles

- Audio must support comprehension rather than distract from it.
- Important lesson meaning must not depend on sound alone.
- Audio should be calm, restrained, and purposeful.
- Any essential audio must have a documented accessible alternative.

## Audio roles

| Role | Purpose |
| --- | --- |
| Ambient bed | Support atmosphere without overpowering explanation |
| Event cue | Mark transitions or important interactions |
| Feedback cue | Reinforce correct, incorrect, or recovery states |
| Narration | Explain a stage when text alone is not sufficient |
| Silence | Preserve focus when no sound is needed |

## Audio rules

- Use audio sparingly and only when it adds value.
- Keep sound cues distinct but not startling.
- Narration should be clear and concise if introduced.
- Captions or transcripts must be available if audio becomes essential.
- Do not use audio as the only signal for a required action or state.

## Audio acceptance criteria

- [ ] Audio supports lesson focus and feedback.
- [ ] The experience still works when audio is unavailable or muted.
- [ ] Essential audio has an accessible equivalent.
- [ ] AI Context is current.

## Open questions

- [ ] Should the MVP use any narration at all, or stay fully text-led?
- [ ] What kinds of sound cues are useful without creating distraction?
- [ ] Should ambient audio differ between orientation, flow, quiz, and summary states?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial audio direction draft for the design bible. |

## Review checklist

- [ ] Audio roles and rules are explicit.
- [ ] Accessibility requirements are covered.
- [ ] Audio remains optional or supportable by text equivalents.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define how audio should support the educational experience in AnatomIQ. |
| Constraints | Do not depend on audio alone for essential meaning; keep sound purposeful and accessible. |
| Inputs | Brand Identity, Motion and Animation, UX Copy and Feedback, Accessibility Specification. |
| Outputs | Audio roles, rules, or accessibility expectations. |
| Do not assume | Sound is always available or desirable for every learner. |
| Validation | Confirm the lesson remains understandable with audio muted or absent. |