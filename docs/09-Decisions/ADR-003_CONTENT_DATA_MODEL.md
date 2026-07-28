# ADR 003 - Content Data Model

| Field | Value |
| --- | --- |
| Document ID | AQ-ADR-003 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before content implementation and before schema changes |
| Related documents | [Data Model](../06-Engineering/DATA_MODEL.md), [Medical Content Standards](../07-Medical/MEDICAL_CONTENT_STANDARDS.md), [Content and Lesson Requirements](../03-PRD/CONTENT_AND_LESSON_REQUIREMENTS.md) |

## Context

The MVP needs cardiovascular lesson content to be reusable, reviewable, and separate from shared engine behavior. The content model must support later body systems with minimal rewrite.

## Decision

Represent lesson content as structured data for systems, lessons, stages, annotations, assessments, and simplifications, with review metadata attached to the content records.

## Rationale

- The architecture requires shared behavior and content to remain separate.
- Medical review and simplification notes need to travel with the content.
- New systems should be added mostly by authoring content rather than rewriting code.
- A structured model makes AI-assisted work more consistent and reviewable.

## Consequences

- The content package must define stable fields and identifiers.
- The authoring workflow needs validation for required metadata.
- The implementation layer should consume structured data rather than hardcoded lesson logic.
- Future content updates should be possible without engine rewrites.

## Alternatives considered

- Hardcoded content inside components: rejected because it would break reuse and reviewability.
- Unstructured prose only: rejected because it would make implementation and validation difficult.
- Database-only decision without content schema: rejected because the lesson package needs a documented contract before implementation.

## Acceptance criteria

- [ ] The content model supports lessons, stages, annotations, and assessments.
- [ ] Review and simplification metadata are represented.
- [ ] The model is reusable across future body systems.
- [ ] AI Context is current.

## Open questions

- [ ] Which data format will be easiest for content authors and AI collaborators to maintain?
- [ ] How strict should schema validation be during authoring?
- [ ] Should medical review metadata be visible in the runtime model or only in the source documents?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial content data model ADR draft. |

## Review checklist

- [ ] The content model decision is explicit.
- [ ] Rationale and consequences are documented.
- [ ] The choice aligns with architecture and medical standards.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Record the decision to represent AnatomIQ content as structured, reviewable data. |
| Constraints | Preserve reuse, reviewability, and explicit medical metadata. |
| Inputs | Data Model, Medical Content Standards, Content and Lesson Requirements. |
| Outputs | Content model decision and implementation consequences. |
| Do not assume | Content can be safely hardcoded without losing reuse and reviewability. |
| Validation | Confirm the model supports the cardiovascular MVP and future body systems. |