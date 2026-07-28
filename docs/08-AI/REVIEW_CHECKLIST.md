# AnatomIQ AI Review Checklist

| Field | Value |
| --- | --- |
| Document ID | AQ-AI-006 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before merge, before approval, and after AI-assisted output is produced |
| Related documents | [AI Rules](AI_RULES.md), [Coding Standards](CODING_STANDARDS.md), [Definition of Done](DEFINITION_OF_DONE.md), [Testing Strategy](../06-Engineering/TESTING_STRATEGY.md) |

## Purpose

This document defines the checklist used to review AI-assisted work in AnatomIQ. It ensures outputs are checked against documentation, scope, and validation expectations before approval.

## Scope

### In scope

- Review checks for documents, code, prompts, and tasks.
- Verification of scope, accuracy, and validation.
- Consistency and traceability checks.

### Out of scope

- Human performance review.
- External audit procedures.
- Tool-specific review automation.

## Review checklist

- [ ] The output matches the governing document(s).
- [ ] The scope has not drifted.
- [ ] Claims, labels, and terminology are accurate.
- [ ] No invented sources, approvals, or test results appear.
- [ ] Accessibility and recovery requirements are preserved where relevant.
- [ ] Validation is stated and supported.
- [ ] Open questions are explicitly identified.
- [ ] The output is consistent with the project’s canonical terminology.

## Review rules

- Missing context should be surfaced, not guessed.
- If review fails, the output should be revised before merge or approval.
- Review should be tied to the relevant milestone and document family.

## Acceptance criteria

- [ ] The checklist covers scope, accuracy, traceability, and validation.
- [ ] The checklist can be used for documents and implementation work.
- [ ] The checklist aligns with the AI rules and definition of done.
- [ ] AI Context is current.

## Open questions

- [ ] Should the review checklist be expanded for medical versus engineering work later?
- [ ] Which checks should be mandatory versus recommended for a first pass?
- [ ] Should the checklist become a reusable template for AI task outputs?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial AI review checklist draft. |

## Review checklist

- [ ] The checklist is actionable and complete.
- [ ] The items align with the project documentation rules.
- [ ] The checklist supports AI-assisted review before approval.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the checklist used to review AI-assisted work before approval. |
| Constraints | Check the output against governing documentation, traceability, and validation. |
| Inputs | AI Rules, Coding Standards, Definition of Done, Testing Strategy. |
| Outputs | Review checklist items and review rules. |
| Do not assume | An AI-generated output is acceptable without explicit review checks. |
| Validation | Confirm the checklist identifies scope drift, invented claims, and missing validation. |