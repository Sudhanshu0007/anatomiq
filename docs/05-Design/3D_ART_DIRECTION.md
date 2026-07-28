# AnatomIQ 3D Art Direction

| Field | Value |
| --- | --- |
| Document ID | AQ-DSN-005 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before asset production, model sourcing, and art-direction review |
| Related documents | [Project Vision](../01-Vision/PROJECT_VISION.md), [Product Philosophy](../01-Vision/PRODUCT_PHILOSOPHY.md), [Content and Lesson Requirements](../03-PRD/CONTENT_AND_LESSON_REQUIREMENTS.md), [Lesson Experience Flow](../04-UX/LESSON_EXPERIENCE_FLOW.md) |

## Purpose

This document defines how the 3D anatomical scene should look and feel. The art direction must help learners understand body structure and flow without overwhelming them with visual noise.

## Scope

### In scope

- Anatomical scene presentation.
- Model realism and abstraction balance.
- Highlighting and focus behavior for structures.
- Visual treatment for systems, organs, and routes.

### Out of scope

- Final asset production pipelines.
- File-format and compression implementation.
- Detailed medical asset sourcing policy.

## Art direction principles

- The scene must feel educational and carefully composed.
- The visual model should be clear enough to teach, not so detailed that it loses readability.
- Important structures should be easy to locate and compare.
- The presentation should allow the learner to focus on one teaching point at a time.

## Scene treatment

- Use a controlled anatomical environment rather than a busy clinical collage.
- Keep the learner’s attention on the current route or structure.
- Use transparency, layering, and selective focus to reveal relationships.
- Avoid photorealism if it reduces comprehension or performance.

## Model treatment

| Aspect | Direction |
| --- | --- |
| Body context | Use a readable whole-body or regional frame when needed for orientation |
| Organs and vessels | Present the relevant structure clearly and consistently |
| Flow routes | Make direction and sequence understandable at a glance |
| Optional detail | Reveal progressively when it supports the lesson objective |
| Unsupported detail | Hide or simplify when it adds noise without learning value |

## Visual emphasis rules

- The current teaching target should be visually dominant.
- Secondary structures may remain visible but should not compete for attention.
- Highlights should be intentional and minimal.
- The scene should remain readable even when annotations are open.

## 3D art acceptance criteria

- [ ] The art direction supports a calm educational experience.
- [ ] The scene makes the target anatomy easy to understand.
- [ ] The presentation can support future body systems without redesign.
- [ ] AI Context is current.

## Open questions

- [ ] Should the body context be semi-transparent by default or only during certain stages?
- [ ] How much structural simplification is acceptable before the scene stops feeling anatomically trustworthy?
- [ ] Should organ focus be cinematic or more diagrammatic for the MVP?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial 3D art direction draft for the design bible. |

## Review checklist

- [ ] Scene treatment and model treatment are defined.
- [ ] The direction supports clarity, not spectacle.
- [ ] The art direction can scale to future systems.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define how anatomical 3D scenes should be presented in AnatomIQ. |
| Constraints | Preserve educational clarity, focus, and trust over visual overload or photorealistic novelty. |
| Inputs | Project Vision, Product Philosophy, Content and Lesson Requirements, Lesson Experience Flow. |
| Outputs | Art direction rules, scene treatment guidance, or focus principles. |
| Do not assume | More realism automatically improves understanding. |
| Validation | Confirm the art direction helps the learner identify structures and follow the route. |