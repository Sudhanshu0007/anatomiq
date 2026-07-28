# AnatomIQ Design Accessibility

| Field | Value |
| --- | --- |
| Document ID | AQ-DSN-008 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before visual mockups, motion review, and accessibility validation |
| Related documents | [Accessibility Specification](../04-UX/ACCESSIBILITY_SPECIFICATION.md), [Color System](COLOR_SYSTEM.md), [Typography](TYPOGRAPHY.md), [Motion and Animation](MOTION_AND_ANIMATION.md), [Audio Direction](AUDIO_DIRECTION.md) |

## Purpose

This document defines the design-level accessibility rules for AnatomIQ. It translates accessibility intent into visual and interaction design expectations.

## Scope

### In scope

- Visual accessibility rules for design work.
- Contrast, focus, and readability requirements.
- Motion and non-colour support expectations.
- Design decisions that affect accessible learning.

### Out of scope

- Final technical accessibility audit results.
- Assistive-technology testing logs.
- Legal conformance claims for a particular standard.

## Accessibility principles

- Accessibility must be designed in from the beginning.
- Essential meaning must not depend on colour, hover, motion, or sound alone.
- Focus and hierarchy should remain visible in every lesson state.
- Accessible alternatives must be considered part of the primary design, not a fallback afterthought.

## Design accessibility rules

- Use color and shape together when indicating state or meaning.
- Keep text and control sizes readable in the intended layouts.
- Ensure overlays do not trap essential content behind them.
- Design motion to be pausable or reducible.
- Reserve space for concise instructional and recovery text.
- Make focus states obvious and consistent across components.

## Accessible design checks

| Check | Design expectation |
| --- | --- |
| Color independence | Meaning remains clear without colour alone |
| Text readability | Labels and explanations remain legible |
| Motion reduction | Core learning can continue without forced motion |
| Keyboard focus | Interactive elements can be tracked visually |
| Overlay clarity | Help and feedback do not hide the lesson permanently |
| Audio independence | The lesson remains understandable when sound is muted |

## Acceptance criteria

- [ ] Accessibility rules influence the design system, not just implementation.
- [ ] Critical learning meaning remains accessible across supported modes.
- [ ] The design bible can guide later engineering and validation work.
- [ ] AI Context is current.

## Open questions

- [ ] What design-level accessibility baseline should be fixed before the engineering bible starts?
- [ ] Should accessible alternatives be fully specified in design or only at the UX layer?
- [ ] Which accessibility concerns need the most visual guidance in the MVP?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial design accessibility draft for the design bible. |

## Review checklist

- [ ] Design accessibility rules are explicit.
- [ ] The design supports readable, navigable, and non-colour-dependent learning.
- [ ] The document aligns with the UX accessibility specification.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Translate accessibility goals into design-level rules for AnatomIQ. |
| Constraints | Do not depend on colour, hover, motion, or audio alone for essential meaning. |
| Inputs | Accessibility Specification, Color System, Typography, Motion and Animation, Audio Direction. |
| Outputs | Design accessibility rules, layout checks, or visual guidance. |
| Do not assume | Accessibility can be added later without design consequences. |
| Validation | Confirm the design system supports readable, navigable, and recoverable lesson states. |