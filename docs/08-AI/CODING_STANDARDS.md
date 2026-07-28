# AnatomIQ Coding Standards

| Field | Value |
| --- | --- |
| Document ID | AQ-AI-003 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation, code review, and major refactors |
| Related documents | [System Architecture](../06-Engineering/SYSTEM_ARCHITECTURE.md), [Lesson Engine](../06-Engineering/LESSON_ENGINE.md), [State Management](../06-Engineering/STATE_MANAGEMENT.md), [Testing Strategy](../06-Engineering/TESTING_STRATEGY.md) |

## Purpose

This document defines the coding standards for AnatomIQ so AI-generated and human-authored code stays readable, reviewable, and aligned with the documented architecture.

## Scope

### In scope

- Code readability and structure.
- Naming and reuse expectations.
- Architecture alignment.
- Review and testing expectations.

### Out of scope

- Language-specific formatter settings.
- Package manager choice.
- Repository tooling setup details.

## Coding principles

- Code must reflect the approved architecture.
- Shared behavior should be reusable and not duplicated across lessons.
- Naming should match the documentation and canonical terminology.
- Code should be easy for another contributor or AI collaborator to review.

## Standards

| Area | Standard |
| --- | --- |
| Naming | Use stable, descriptive names that match the documentation |
| Modularity | Keep engines, systems, and content separation clear |
| State | Make state transitions explicit and testable |
| Accessibility | Preserve keyboard, reduced-motion, and readable text paths |
| Comments | Use comments only when the code is not self-explanatory |

## Code review expectations

- New code must map to a requirement, task, or architectural boundary.
- AI-generated code must be reviewed for correctness and scope.
- Code should not introduce hardcoded lesson data where content-driven configuration is expected.
- Tests should be added or updated when behavior changes.

## Acceptance criteria

- [ ] The standards reinforce architecture and reuse.
- [ ] Naming and structure are compatible with the documentation set.
- [ ] The standards support reviewable, testable code.
- [ ] AI Context is current.

## Open questions

- [ ] Which code style decisions should be fixed now versus deferred to the implementation milestone?
- [ ] How strict should the project be about refactoring before the MVP is validated?
- [ ] Should code examples be added once the first application scaffold exists?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial coding standards draft for the AI bible. |

## Review checklist

- [ ] Coding standards align with architecture and accessibility requirements.
- [ ] Naming and modularity expectations are explicit.
- [ ] Review and testing expectations are clear.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define code quality standards for AnatomIQ so implementation stays aligned with the documentation set. |
| Constraints | Preserve modularity, reuse, accessibility, and traceability to requirements. |
| Inputs | System Architecture, Lesson Engine, State Management, Testing Strategy. |
| Outputs | Coding standards, review expectations, or structure guidance. |
| Do not assume | Code quality can be evaluated without reference to architecture and requirements. |
| Validation | Confirm the standards help reviewers connect code back to the documented system. |