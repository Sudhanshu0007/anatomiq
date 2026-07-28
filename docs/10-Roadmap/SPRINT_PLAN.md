# AnatomIQ Sprint Plan

| Field | Value |
| --- | --- |
| Document ID | AQ-RDM-002 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before sprint execution and before milestone planning changes |
| Related documents | [Implementation Plan](IMPLEMENTATION_PLAN.md), [Task Backlog](TASK_BACKLOG.md), [Task System](../08-AI/TASK_SYSTEM.md), [Testing Strategy](../06-Engineering/TESTING_STRATEGY.md) |

## Purpose

This document defines the sprint structure for AnatomIQ implementation work. It organizes the roadmap into reviewable, dependency-aware build periods.

## Scope

### In scope

- Sprint sequencing for the MVP.
- High-level sprint goals and exit criteria.
- Dependency ordering for milestone work.

### Out of scope

- Daily execution tracking.
- Team assignment or capacity planning.
- Tool-specific scrum ceremony details.

## Sprint structure

| Sprint | Focus | Exit criteria |
| --- | --- | --- |
| Sprint 1 | App scaffold and shared structure | Repository has a runnable shell and basic documentation alignment |
| Sprint 2 | Core engine foundations | Lesson engine, Human Body Engine, and shared state boundaries are in place |
| Sprint 3 | Interaction and navigation systems | Scroll, camera, input, and annotation behavior are wired together |
| Sprint 4 | Cardiovascular content integration | The lesson can express the approved cardiovascular route and content model |
| Sprint 5 | Accessibility and recovery hardening | Reduced-motion, keyboard flow, and error recovery are validated |
| Sprint 6 | Performance and release preparation | Validation passes support a public MVP demo |

## Sprint principles

- Each sprint should deliver a coherent slice of progress.
- Shared systems should be built before content-heavy features.
- Each sprint should end with a reviewable artifact or behavior.
- Validation should be included in the sprint objective, not left for later.

## Sprint planning rules

- Do not pull in tasks that depend on unapproved documentation.
- Keep the most reusable work early in the sequence.
- Assign tasks so that each sprint can be reviewed independently.
- Include testing and documentation updates in each sprint where relevant.

## Acceptance criteria

- [ ] The sprint sequence follows the implementation plan.
- [ ] Exit criteria are clear and reviewable.
- [ ] Validation is part of each sprint definition.
- [ ] AI Context is current.

## Open questions

- [ ] How long should each sprint be for the first implementation cycle?
- [ ] Which sprint should carry the first end-to-end playable lesson slice?
- [ ] How should recovery and accessibility tasks be split across sprints?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial sprint plan draft for the roadmap. |

## Review checklist

- [ ] Sprint focus and exit criteria are explicit.
- [ ] The sequence aligns with the implementation plan.
- [ ] Validation is included in the sprint structure.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the sprint structure that will guide AnatomIQ implementation work. |
| Constraints | Keep sprints dependency-aware, reviewable, and tied to validation. |
| Inputs | Implementation Plan, Task System, Testing Strategy. |
| Outputs | Sprint sequence, focus areas, and exit criteria. |
| Do not assume | A sprint can be defined without a clear exit criterion or validation target. |
| Validation | Confirm the sprint plan can be used to sequence work toward the MVP. |