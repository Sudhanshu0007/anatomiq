# AnatomIQ Cardiovascular Annotation Register

| Field | Value |
| --- | --- |
| Document ID | AQ-MED-008 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation and before medical review |
| Related documents | [Scene-by-Scene Specification](05_SCENE_BY_SCENE_SPECIFICATION.md), [Learning Objectives](01_LEARNING_OBJECTIVES.md), [Content and Lesson Requirements](../../03-PRD/CONTENT_AND_LESSON_REQUIREMENTS.md) |

## Purpose

This document lists the cardiovascular annotations required by the lesson. It defines the names, functions, and review expectations for the structure labels used in the MVP.

## Required annotations

| Structure | Function in lesson | Display context |
| --- | --- | --- |
| heart | Main pumping organ of the circulation loop | Orientation and flow scenes |
| right atrium | Receives returning blood from the body | Right-heart return scene |
| right ventricle | Sends blood toward the lungs | Right-heart and pulmonary scenes |
| left atrium | Receives blood returning from the lungs | Left-heart return scene |
| left ventricle | Sends blood into the systemic route | Left-heart and systemic scenes |
| lungs | Site of gas exchange in the simplified model | Pulmonary and exchange scenes |
| pulmonary artery | Carries blood from heart to lungs in the taught route | Pulmonary route scene |
| pulmonary veins | Carries blood from lungs to heart in the taught route | Left-heart return scene |
| aorta | Main systemic outflow vessel in the taught route | Systemic route scene |
| venae cavae | Major body-return vessels in the taught route | Right-heart return scene |
| arteries, veins, capillaries | Broad vessel categories used for comparison and reasoning | Multiple scenes as needed |

## Annotation rules

- Every required annotation must include a concise function statement.
- Every annotation must be accessible without hover-only input.
- Optional depth should not obscure the main label and function.
- Annotation wording must remain consistent across scenes and assessments.

## Required annotation fields

| Field | Purpose |
| --- | --- |
| id | Stable annotation identifier |
| structure | Anatomical object being labeled |
| name | Learner-facing label |
| function | Short relevance statement |
| context | Scene or route context |
| depth | Optional extended explanation |
| accessibilityText | Non-visual equivalent |
| reviewStatus | Medical review state |

## Acceptance criteria

- [ ] The required annotations match the approved route and objectives.
- [ ] Each annotation has a function statement and non-hover access path.
- [ ] Optional depth is clearly separated from required content.
- [ ] AI Context is current.

## Open questions

- [ ] Which annotations should have optional depth in the MVP and which should remain concise only?
- [ ] Should vessel categories appear as standalone annotations or only inside broader route explanations?
- [ ] What is the minimum annotation set that still supports the assessment items?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial cardiovascular annotation register. |

## Review checklist

- [ ] Required structures are listed.
- [ ] Function, context, and accessibility fields are explicit.
- [ ] Annotation scope aligns with the lesson objectives.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the cardiovascular annotation set and its lesson roles. |
| Constraints | Do not require hover-only access; keep labels and functions aligned to the approved route. |
| Inputs | Scene-by-Scene Specification, Learning Objectives, Content and Lesson Requirements. |
| Outputs | Annotation register and required fields. |
| Do not assume | Optional depth is automatically necessary for every structure. |
| Validation | Confirm each required annotation supports the lesson route and objectives. |