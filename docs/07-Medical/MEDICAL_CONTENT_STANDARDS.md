# AnatomIQ Medical Content Standards

| Field | Value |
| --- | --- |
| Document ID | AQ-MED-001 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before cardiovascular content production and before any medical-content change |
| Related documents | [Content and Lesson Requirements](../03-PRD/CONTENT_AND_LESSON_REQUIREMENTS.md), [MVP Scope](../03-PRD/MVP_SCOPE.md), [Design Accessibility](../05-Design/DESIGN_ACCESSIBILITY.md), [System Architecture](../06-Engineering/SYSTEM_ARCHITECTURE.md) |

## Purpose

This document defines the standards for medical and educational content in AnatomIQ. It establishes how anatomy, physiology, simplification, sourcing, and review must be handled so the cardiovascular MVP remains scientifically responsible and reusable.

## Scope

### In scope

- Content structure and review expectations.
- Medical sourcing and review requirements.
- Simplification and limitation rules.
- Scope control for the cardiovascular lesson package.

### Out of scope

- Diagnosis, treatment, or patient-specific advice.
- Detailed source evaluation of every future organ system in this document.
- Engineering implementation details.

## Medical content principles

- Medical content must be accurate, traceable, and proportional to the lesson objective.
- Simplification is allowed only when it does not reverse the underlying concept.
- The lesson must remain educational and not drift into clinical advice.
- Medical claims and visual choices must be reviewable by a qualified reviewer.

## Required medical content structure

Every medical lesson package should define:

- learning objectives;
- anatomy scope;
- physiology scope;
- scene storyboard;
- annotation register;
- assessment register;
- simplifications and limitations;
- source and review record.

## Review rules

- Do not present unreviewed medical content as final.
- Keep learner-facing wording clear and age-appropriate.
- Distinguish normal anatomy from simplified teaching conventions.
- Record medical review status before implementation or public release.

## Acceptance criteria

- [ ] Medical content is traceable and reviewable.
- [ ] Simplifications and limits are explicitly controlled.
- [ ] The content standard supports the cardiovascular lesson package.
- [ ] AI Context is current.

## Open questions

- [ ] Who is the qualified medical reviewer for the first cardiovascular package?
- [ ] What source format will be used to track versioned references?
- [ ] What is the minimum medical review record required before implementation starts?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial medical content standards draft for the medical bible. |

## Review checklist

- [ ] Scope, traceability, and simplification rules are explicit.
- [ ] Review expectations are stated.
- [ ] The standard aligns with the PRD and scope documents.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the medical content rules for AnatomIQ so cardiovascular lesson content remains scientifically responsible. |
| Constraints | Do not invent clinical advice, unsupported facts, or unreviewed anatomy claims. |
| Inputs | Content and Lesson Requirements, MVP Scope, Design Accessibility, System Architecture. |
| Outputs | Medical content standards, review rules, or simplification requirements. |
| Do not assume | Medical content can be finalized without review and source tracking. |
| Validation | Confirm that every future medical lesson package can be reviewed, traced, and simplified responsibly. |