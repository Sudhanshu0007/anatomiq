# AnatomIQ Lighting and Materials

| Field | Value |
| --- | --- |
| Document ID | AQ-DSN-006 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before asset production, camera blocking, and lighting review |
| Related documents | [3D Art Direction](3D_ART_DIRECTION.md), [Brand Identity](BRAND_IDENTITY.md), [Camera Language](CAMERA_LANGUAGE.md), [Motion and Animation](MOTION_AND_ANIMATION.md) |

## Purpose

This document defines the lighting and materials direction for AnatomIQ. Lighting and material choices must support visibility, focus, and atmosphere without obscuring anatomy or interface elements.

## Scope

### In scope

- Scene lighting tone.
- Focal lighting and contrast.
- Body context and structure visibility.
- Material treatment for readability and separation.

### Out of scope

- Real-time rendering implementation details.
- Specific shader or engine configuration.
- Advanced cinematic color grading beyond the product need.

## Lighting principles

- Lighting should guide the eye to the current lesson focus.
- Important structures and labels must remain readable.
- Atmospheric lighting should never make the lesson harder to understand.
- The scene should feel controlled, not theatrical for its own sake.

## Lighting roles

| Role | Purpose |
| --- | --- |
| Ambient | Keep the body context visible and stable |
| Key light | Emphasize the current anatomy focus |
| Accent light | Separate important structures from surrounding tissue or context |
| Background light | Support depth without competing with the lesson |
| Recovery lighting | Ensure overlays and fallback screens remain readable |

## Material principles

- Materials should help distinguish anatomical layers and routes.
- Surfaces should avoid excessive shine that obscures detail.
- Transparency or translucency should be used only when it improves understanding.
- Materials must remain legible in the intended lighting setup.

## Lighting and material rules

- Use contrast to clarify the current teaching point.
- Avoid lighting that creates visual confusion in dense anatomical areas.
- Ensure labels and overlays retain readability across lighting states.
- Use changes in light and material only when they reinforce the lesson.

## Acceptance criteria

- [ ] The current learning focus remains readable.
- [ ] Lighting and materials support structure separation and attention.
- [ ] The scene does not become too dark, washed out, or distracting.
- [ ] AI Context is current.

## Open questions

- [ ] Should the lighting be more documentary-like or more cinematic?
- [ ] What lighting contrast is needed to support labels and transparency layers?
- [ ] How should lighting adapt when the learner opens overlays or feedback panels?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial lighting and materials draft for the design bible. |

## Review checklist

- [ ] Lighting roles and rules are explicit.
- [ ] Material treatment supports readability and separation.
- [ ] The scene can remain usable with overlays and annotations.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define how lighting and materials should support anatomical clarity and atmosphere in AnatomIQ. |
| Constraints | Preserve visibility, contrast, and learner focus; do not let lighting or materials obscure the lesson. |
| Inputs | 3D Art Direction, Brand Identity, Camera Language, Motion and Animation. |
| Outputs | Lighting roles, material rules, or scene readability guidance. |
| Do not assume | Atmospheric lighting or glossy materials are acceptable if they reduce comprehension. |
| Validation | Verify that structures, labels, and overlays remain readable in all intended lesson states. |