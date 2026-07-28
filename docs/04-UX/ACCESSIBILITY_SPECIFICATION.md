# AnatomIQ Accessibility Specification

| Field | Value |
| --- | --- |
| Document ID | AQ-UX-004 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before wireframes, implementation, and accessibility testing |
| Related documents | [Information Architecture](INFORMATION_ARCHITECTURE.md), [Navigation Model](NAVIGATION_MODEL.md), [Interaction Model](INTERACTION_MODEL.md), [Functional Requirements](../03-PRD/FUNCTIONAL_REQUIREMENTS.md), [Non-Functional Requirements](../03-PRD/NON_FUNCTIONAL_REQUIREMENTS.md) |

## Purpose

This document defines the accessibility expectations for the AnatomIQ cardiovascular MVP. It ensures the lesson remains usable when a learner relies on keyboard input, reduced motion, screen-reader support, stronger contrast, or non-colour cues.

## Scope

### In scope

- Keyboard behavior and focus order.
- Reduced-motion and step-based alternatives.
- Text alternatives for essential visuals.
- Colour-independent communication of meaning.
- Captions, transcripts, and accessible feedback.
- Error recovery that remains usable across input methods.

### Out of scope

- Final legal conformance claims for a specific accessibility standard.
- Device- or browser-specific implementation details.
- Full internationalization and localization behavior.
- Accessibility of future systems not yet in the MVP lesson package.

## Accessibility principles

- Essential learning must not depend on a single input mode.
- Meaning must be available without colour alone.
- Motion must be optional or reducible when it is not required for the objective.
- Important information must remain readable and reachable before it disappears or changes.
- Recovery paths must be as accessible as the primary path.

## Keyboard behavior

- All essential lesson controls must be reachable by keyboard.
- Focus order must match the visual reading order.
- The focused element must be clearly visible at all times.
- Enter and Space must activate the intended control.
- Escape should close recoverable overlays when appropriate.
- No essential control may require pointer hover.

## Reduced-motion behavior

- The lesson must provide a reduced-motion or step-based path for the cardiovascular story.
- Camera motion, pulsing effects, and flow animation should be pausable or substitutable.
- The reduced-motion path must still teach the same route, concepts, and review points.
- Time-based transitions should become clearer, not more confusing, in reduced-motion mode.

## Colour-independent meaning

The lesson must not use colour as the only signal for:

- direction of flow;
- oxygenation state;
- selected structure;
- correct or incorrect feedback;
- locked or unavailable content.

Alternative cues may include:

- labels;
- arrows;
- position;
- pattern;
- text;
- icon shape;
- emphasis or contrast.

## Text alternatives

- Essential anatomy and process explanations must be readable in text form.
- Text alternatives must explain what the learner is meant to understand, not merely describe the image.
- If narration or essential audio is introduced later, captions or transcripts are required.
- Visual-only labels do not satisfy the accessibility requirement for core content.

## Contrast and readability

- Text and controls must be legible against their background.
- Focus states must remain visible in all supported lesson views.
- Important labels should not rely on small type or thin overlays.
- When a lesson view is visually dense, the interface must provide a clearer fallback or summary.

## Accessible feedback and errors

- Wrong-answer feedback must explain the misconception in simple language.
- Error messages must identify the problem and offer a safe next step.
- If a scene cannot load, the learner should still have a route to retry, review, or exit safely.
- The accessible path must remain available when the primary 3D experience fails.

## Interaction equivalence

| Default path | Accessible expectation |
| --- | --- |
| Scroll-driven progression | Step-based or equivalent narrative progression |
| Hover previews | Focusable or explicit open actions |
| Animated blood flow | Textual and structural explanation of direction and sequence |
| Camera movement | Stable orientation and reviewable content |
| Colour state cues | Labels, direction cues, and text feedback |

## Accessibility acceptance criteria

- [ ] Every essential lesson action is keyboard operable.
- [ ] The focus order is visible and logical.
- [ ] Reduced-motion users can complete the cardiovascular learning objectives.
- [ ] Colour is not the only way meaning is communicated.
- [ ] Essential text alternatives are available for all Must learning content.
- [ ] Error and recovery paths remain accessible.

## Open questions

- [ ] What target conformance level should the project adopt for public release?
- [ ] Should captions and transcripts be prepared during MVP creation or deferred until audio is added?
- [ ] What assistive technology combinations should be included in the first test pass?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial accessibility specification draft for the cardiovascular MVP. |

## Review checklist

- [ ] Keyboard, focus, motion, colour, text, and error behavior are defined.
- [ ] Accessible and default paths are equivalent in learning outcome.
- [ ] The specification aligns with functional and non-functional requirements.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define accessibility requirements for the cardiovascular MVP so the lesson remains usable through alternative input and perception paths. |
| Constraints | Do not rely on colour alone, hover alone, or continuous motion for essential learning. |
| Inputs | Information Architecture, Navigation Model, Interaction Model, Functional Requirements, Non-Functional Requirements. |
| Outputs | Accessibility rules, fallback behavior, focus behavior, or validation tasks. |
| Do not assume | The learner can use a mouse, tolerate motion, or interpret the visual scene without text support. |
| Validation | Verify the essential lesson journey through keyboard and reduced-motion paths with clear text alternatives. |