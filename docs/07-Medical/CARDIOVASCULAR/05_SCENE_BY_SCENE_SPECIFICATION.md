# AnatomIQ Cardiovascular Scene-by-Scene Specification

| Field | Value |
| --- | --- |
| Document ID | AQ-MED-007 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation and before medical review |
| Related documents | [Circulation Storyboard](04_CIRCULATION_STORYBOARD.md), [Annotation Register](06_ANNOTATION_REGISTER.md), [Assessment Register](07_ASSESSMENT_REGISTER.md), [Simplifications and Limitations](08_SIMPLIFICATIONS_AND_LIMITATIONS.md) |

## Purpose

This document specifies the cardiovascular lesson scenes one by one. It turns the storyboard into implementation-ready scene requirements that stay aligned to the MVP objectives and route.

## Scene specification rules

- Each scene must have one primary learner takeaway.
- Each scene must define what must be visible, explainable, and reviewable.
- Each scene must identify any simplification or limitation that the learner needs to know.
- Each scene must be compatible with annotations and assessments.

## Scene list

| Scene | Learner takeaway | Required focus |
| --- | --- | --- |
| Entry | I know what I will learn. | Title, objective, scope, educational framing |
| Whole-body orientation | I know where heart and lungs are. | Body context, heart, lungs, active system |
| Right-heart return | Blood returning from the body enters the right side. | Body return, right atrium, right ventricle |
| Pulmonary route | Blood travels from the heart to the lungs. | Pulmonary artery, lungs, flow direction |
| Lung exchange overview | The lungs change the blood’s oxygenation state in a simplified model. | Simplification note, exchange concept |
| Left-heart return | Blood returns from the lungs to the left side. | Pulmonary veins, left atrium, left ventricle |
| Systemic route | Blood leaves the left side for the body. | Aorta, body distribution, loop completion |
| Knowledge check | I can explain the route. | Objective-aligned assessment, feedback, review |
| Summary | The route is a connected loop. | Recap, replay, exit or revisit |

## Required scene fields

| Field | Purpose |
| --- | --- |
| id | Stable scene identifier |
| title | Learner-facing scene name |
| takeaway | The primary learner takeaway |
| focus | Required anatomical or physiological focus |
| visibleElements | Structures and cues that must be present |
| explanation | Concise learner-facing explanation |
| interaction | Supported learner actions |
| reviewLink | Where the learner can return after feedback |
| simplificationNote | Any required limitation or teaching convention |

## Acceptance criteria

- [ ] Every scene maps to a clear learner takeaway.
- [ ] Required visible elements are defined.
- [ ] Each scene can support annotation and assessment hooks.
- [ ] AI Context is current.

## Open questions

- [ ] How much camera movement is specified per scene versus left to the engine?
- [ ] Should the lesson be split into more or fewer scene steps for first-time learners?
- [ ] Which scene should carry the strongest explanation of the simplified model?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial scene-by-scene cardiovascular specification. |

## Review checklist

- [ ] Every scene has a learner takeaway and required focus.
- [ ] Required fields are clear and implementation-ready.
- [ ] The scene list matches the storyboard and objectives.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the scene-by-scene cardiovascular lesson specification for implementation and medical review. |
| Constraints | Keep each scene tied to the approved route, learning objective, and simplification rules. |
| Inputs | Storyboard, Learning Objectives, Anatomy Scope, Physiology Scope, Simplifications and Limitations. |
| Outputs | Scene definitions, required fields, or implementation-ready content structure. |
| Do not assume | A scene can be added without a clear learner takeaway or review linkage. |
| Validation | Confirm each scene is ready for implementation and medical review. |