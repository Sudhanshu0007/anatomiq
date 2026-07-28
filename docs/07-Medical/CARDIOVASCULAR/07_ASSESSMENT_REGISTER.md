# AnatomIQ Cardiovascular Assessment Register

| Field | Value |
| --- | --- |
| Document ID | AQ-MED-009 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation and before medical review |
| Related documents | [Learning Objectives](01_LEARNING_OBJECTIVES.md), [Scene-by-Scene Specification](05_SCENE_BY_SCENE_SPECIFICATION.md), [Content and Lesson Requirements](../../03-PRD/CONTENT_AND_LESSON_REQUIREMENTS.md) |

## Purpose

This document defines the formative assessment items for the cardiovascular lesson. It ensures questions map to the approved learning objectives and support review rather than certification.

## Assessment principles

- Questions must test taught content.
- Feedback must explain reasoning, not just correctness.
- Learners must be able to return to the relevant review point.
- The tone must remain formative and educational.

## Assessment items

| Item | Objective mapping | Required feedback behavior |
| --- | --- | --- |
| A-01 | LO-CV-01 | Confirm the learner can locate the heart and lungs in context. |
| A-02 | LO-CV-02 | Explain the body -> right heart -> lungs sequence and correct likely ordering mistakes. |
| A-03 | LO-CV-03 | Explain the lungs -> left heart -> body sequence and correct likely ordering mistakes. |
| A-04 | LO-CV-04 | Distinguish arteries, veins, and capillaries by role or route position. |
| A-05 | LO-CV-05 | Explain why the two circuits form one connected loop. |

## Assessment fields

| Field | Purpose |
| --- | --- |
| id | Stable assessment identifier |
| prompt | Learner-facing question |
| objectiveMapping | Linked learning objective(s) |
| answerModel | Accepted correct response pattern |
| misconception | Likely wrong understanding |
| feedback | Learner-facing explanation |
| reviewLink | Path back into the lesson |
| accessibilityText | Non-visual equivalent |

## Assessment rules

- Assessments should stay within the MVP route and scope.
- Feedback should guide the learner back to the scene or annotation.
- The assessment register must not imply certification or competence beyond the lesson.

## Acceptance criteria

- [ ] Every assessment maps to one or more objectives.
- [ ] Feedback explains reasoning and supports review.
- [ ] The assessment set matches the approved MVP scope.
- [ ] AI Context is current.

## Open questions

- [ ] Should questions be multiple choice, ordering, or mixed formats in the first release?
- [ ] Which assessment items need the clearest scene review links?
- [ ] Should the set include one question per objective or multiple per critical objective?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial cardiovascular assessment register. |

## Review checklist

- [ ] Assessment items map to the learning objectives.
- [ ] Feedback and review behavior are explicit.
- [ ] The formative scope is clear.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the formative cardiovascular assessment set. |
| Constraints | Keep questions inside the MVP scope and avoid certification language. |
| Inputs | Learning Objectives, Scene-by-Scene Specification, Content and Lesson Requirements. |
| Outputs | Assessment items, feedback requirements, or review links. |
| Do not assume | A good answer alone proves learning if feedback and review are missing. |
| Validation | Confirm each item maps to an objective and supports review. |