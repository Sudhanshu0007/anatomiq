# AnatomIQ Cardiovascular Sources and Medical Review

| Field | Value |
| --- | --- |
| Document ID | AQ-MED-011 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before content approval and before implementation |
| Related documents | [Medical Content Standards](../MEDICAL_CONTENT_STANDARDS.md), [Overview](00_OVERVIEW.md), [Simplifications and Limitations](08_SIMPLIFICATIONS_AND_LIMITATIONS.md), [Content and Lesson Requirements](../../03-PRD/CONTENT_AND_LESSON_REQUIREMENTS.md) |

## Purpose

This document records the source and review requirements for the cardiovascular lesson. It is the place where the medical review process and source traceability for the MVP are maintained.

## Source rules

- Every medical claim must be traceable to an approved source or approved teaching convention.
- Source records should include the source title, version or access date, and why the source is relevant.
- Medical content should not rely on unverified memory or unsupported assumptions.

## Review rules

- A qualified reviewer must confirm the lesson’s anatomy, physiology, route, and simplifications.
- Review status should be recorded for content, labels, storyboard, and assessment items.
- Any change that alters meaning or scope requires re-review.

## Review record fields

| Field | Purpose |
| --- | --- |
| item | Scene, annotation, assessment, or simplification being reviewed |
| source | Reference backing the claim or teaching convention |
| reviewer | Qualified reviewer or reviewer role |
| reviewStatus | Pending, approved, or needs changes |
| notes | Important limitations or follow-up actions |

## Source placeholders

At this stage, the package should store the authoritative source list in this document or a linked reference table once approved. No source should be treated as final until the review record is complete.

## Acceptance criteria

- [ ] The package has a clear source-traceability plan.
- [ ] Review fields are defined for each medical content item.
- [ ] The process supports approval before implementation.
- [ ] AI Context is current.

## Open questions

- [ ] Which source set will be used as the initial cardiovascular reference base?
- [ ] What reviewer role is qualified to approve the first version of the lesson package?
- [ ] Should source version tracking live here or in a separate bibliographic index?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial sources and medical review register. |

## Review checklist

- [ ] Source traceability rules are explicit.
- [ ] Review record fields are defined.
- [ ] The process supports approval before implementation.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define how the cardiovascular lesson should be sourced and medically reviewed. |
| Constraints | Do not invent sources or claim approval before the review record exists. |
| Inputs | Medical Content Standards, Overview, Simplifications and Limitations, Content and Lesson Requirements. |
| Outputs | Source traceability rules and review record structure. |
| Do not assume | A medical claim is valid without source and reviewer support. |
| Validation | Confirm every medical claim can be traced and reviewed before implementation. |