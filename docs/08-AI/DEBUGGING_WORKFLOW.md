# AnatomIQ Debugging Workflow

| Field | Value |
| --- | --- |
| Document ID | AQ-AI-007 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation troubleshooting and after failing tests or runtime errors |
| Related documents | [Testing Strategy](../06-Engineering/TESTING_STRATEGY.md), [State Management](../06-Engineering/STATE_MANAGEMENT.md), [Task System](TASK_SYSTEM.md), [Review Checklist](REVIEW_CHECKLIST.md) |

## Purpose

This document defines the debugging workflow for AI-assisted work in AnatomIQ. It gives a structured approach for reproducing, isolating, and fixing issues without widening scope unnecessarily.

## Scope

### In scope

- Debugging steps and investigation order.
- Reproduction and evidence gathering.
- Fix, validate, and retest cycle.
- Escalation when the issue is not yet understood.

### Out of scope

- Tool-specific IDE configuration.
- Language-runtime troubleshooting guides.
- Production incident response procedures.

## Debugging principles

- Reproduce the problem before changing the solution.
- Change one thing at a time when possible.
- Use evidence from tests, logs, or state rather than guesswork.
- Re-validate after each fix.

## Workflow

1. Identify the failing behavior or test.
2. Reproduce the issue with the smallest useful scope.
3. Inspect the governing documents and the nearest implementation surface.
4. Form a local hypothesis and a cheap check that can disconfirm it.
5. Apply the smallest plausible fix.
6. Re-run the relevant validation.
7. Expand only if the hypothesis was falsified or the problem remains unresolved.

## Debugging rules

- Do not widen the search before the first focused check.
- Do not claim the issue is fixed without fresh validation.
- Do not patch unrelated areas while diagnosing a local defect.
- If an issue persists, record what was tried and what evidence changed.

## Acceptance criteria

- [ ] The workflow starts from evidence and reproduction.
- [ ] The workflow emphasizes small, verifiable changes.
- [ ] The workflow requires re-validation after a fix.
- [ ] AI Context is current.

## Open questions

- [ ] Which debugging outputs should be preserved in task history?
- [ ] How should repeated failures be escalated in the task system?
- [ ] Should a debugging prompt template be added to the prompt library later?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial debugging workflow draft for the AI bible. |

## Review checklist

- [ ] Debugging is evidence-led and reproducible.
- [ ] The workflow supports small fixes and fresh validation.
- [ ] Escalation and scope control are clear.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the debugging workflow for AI-assisted work in AnatomIQ. |
| Constraints | Start from evidence, fix the smallest plausible issue, and re-validate before claiming success. |
| Inputs | Testing Strategy, State Management, Task System, Review Checklist. |
| Outputs | Debugging steps, investigation order, or validation expectations. |
| Do not assume | A fix is correct without fresh validation evidence. |
| Validation | Confirm the workflow supports reproducible diagnosis and re-checking after changes. |