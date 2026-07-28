# AnatomIQ Task Backlog

| Field | Value |
| --- | --- |
| Document ID | AQ-RDM-003 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before sprint planning and before task assignment changes |
| Related documents | [Implementation Plan](IMPLEMENTATION_PLAN.md), [Sprint Plan](SPRINT_PLAN.md), [Task System](../08-AI/TASK_SYSTEM.md), [Definition of Done](../08-AI/DEFINITION_OF_DONE.md) |

## Purpose

This document defines the backlog structure for AnatomIQ implementation tasks. It provides a durable list of work items that can be planned into sprints and traced back to the approved documentation.

## Scope

### In scope

- Milestone-aligned backlog grouping.
- Task prioritization and dependency awareness.
- Backlog hygiene and update rules.

### Out of scope

- Tool-specific ticket synchronization.
- Capacity estimates.
- Detailed engineering task breakdown beyond milestone planning.

## Backlog principles

- Every backlog item should map to a governing document.
- Backlog items should be small enough to be reviewable.
- Items should preserve the implementation order defined in the roadmap.
- Items should not mix unrelated concerns unless the dependency is explicit.

## Backlog groups

| Group | Examples |
| --- | --- |
| Foundation | App scaffold, shared structure, build setup |
| Engines | Lesson engine, Human Body Engine, camera, scroll, interaction, annotations |
| Content | Cardiovascular data, scene flow, annotations, assessments |
| Quality | Accessibility, performance, testing, recovery |
| Release | Deployment, validation, demo preparation |

## Backlog rules

- Prioritize reusable system work before lesson-specific work.
- Keep validation tasks visible and explicit.
- Mark dependency blockers clearly.
- Remove or revise backlog items when the documentation changes.

## Acceptance criteria

- [ ] The backlog is grouped by implementation concern and milestone.
- [ ] Items are dependency-aware and traceable.
- [ ] The backlog can support sprint planning.
- [ ] AI Context is current.

## Open questions

- [ ] Which backlog items should be created first once implementation begins?
- [ ] How should blocked items be represented in the backlog view?
- [ ] Should the backlog contain only work items or also validation tasks and review tasks?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial task backlog draft for the roadmap. |

## Review checklist

- [ ] Backlog groups and rules are explicit.
- [ ] Traceability to documents is clear.
- [ ] The backlog supports sprint planning and dependency handling.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the implementation backlog structure for AnatomIQ. |
| Constraints | Keep backlog items traceable, reviewable, and aligned to the implementation order. |
| Inputs | Implementation Plan, Sprint Plan, Task System, Definition of Done. |
| Outputs | Backlog groupings, item rules, or dependency guidance. |
| Do not assume | A backlog item is ready without traceability and dependency clarity. |
| Validation | Confirm the backlog can support sprint planning and milestone execution. |