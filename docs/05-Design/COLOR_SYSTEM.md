# AnatomIQ Color System

| Field | Value |
| --- | --- |
| Document ID | AQ-DSN-003 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before visual mockups, asset production, and accessibility review |
| Related documents | [Brand Identity](BRAND_IDENTITY.md), [Design Accessibility](DESIGN_ACCESSIBILITY.md), [UX Copy and Feedback](../04-UX/UX_COPY_AND_FEEDBACK.md), [Project Constitution](../00-Constitution/PROJECT_CONSTITUTION.md) |

## Purpose

This document defines how colour is used in AnatomIQ. The colour system must support educational clarity, anatomical distinction, and accessibility rather than serve as decoration.

## Scope

### In scope

- Core colour roles and usage rules.
- Educational states and emphasis usage.
- Contrast and readability considerations.
- Colour restrictions for accessible meaning.

### Out of scope

- Final hex values for every UI token.
- Full brand asset production.
- Detailed theming implementation.

## Color principles

- Color must support understanding, not replace it.
- Meaning must remain available without color alone.
- Important states should be distinct and consistent.
- Color should not compete with anatomy labels or explanations.

## Color roles

| Role | Intended use |
| --- | --- |
| Background | Provide a stable, low-distraction field for the lesson. |
| Surface | Support panels, overlays, and content containers. |
| Primary accent | Highlight key actions or focal structures. |
| Secondary accent | Support navigation and less prominent emphasis. |
| Educational state color | Represent lesson-specific states where colour is only one signal among several. |
| Warning or error | Indicate recovery or incorrect states with clear textual support. |

## Use rules

- The active structure or route may be highlighted, but labels and direction cues must remain clear without the highlight.
- Color should be restrained enough to keep the scientific scene legible.
- Red and blue may appear in the circulation lesson, but they must not be the only interpretation cue for arterial or venous meaning.
- Contrast must remain strong enough for reading text over surfaces and overlays.
- Unavailable or locked content must not rely on faint colour differences alone.

## Accessibility rules

- Color cannot be the only cue for direction, selection, correctness, or state.
- The design must remain understandable in grayscale or low-colour conditions.
- Contrast must support readability for text, controls, labels, and focus states.
- If a state uses colour for emphasis, it must also use text, shape, pattern, position, or label changes.

## Color acceptance criteria

- [ ] Color supports comprehension rather than decoration.
- [ ] Required meaning is preserved without color alone.
- [ ] Educational states remain visible and distinguishable.
- [ ] AI Context is current.

## Open questions

- [ ] Should the palette lean more monochrome with anatomical accents or use more visible system-specific colour coding?
- [ ] How much colour variation is useful before the body scene becomes visually noisy?
- [ ] What are the final accessibility contrast thresholds to adopt for the public release?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial color system draft for the design bible. |

## Review checklist

- [ ] Color roles and restrictions are explicit.
- [ ] Accessibility rules are stated.
- [ ] Color is tied to meaning and not decoration.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define how color should be used across AnatomIQ interfaces, lessons, and states. |
| Constraints | Do not rely on color as the only signal for meaning; preserve readability and contrast. |
| Inputs | Brand Identity, Design Accessibility, Project Constitution, UX Copy and Feedback. |
| Outputs | Color roles, palette rules, state usage, or accessibility decisions. |
| Do not assume | The learner can infer the lesson state from colour alone. |
| Validation | Confirm the design works in grayscale and remains readable for core learning tasks. |