# AnatomIQ Task System

| Field | Value |
| --- | --- |
| Document ID | AQ-AI-004 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before AI task generation and before milestone execution |
| Related documents | [Project Context](PROJECT_CONTEXT.md), [Prompt Library](PROMPT_LIBRARY.md), [Definition of Done](DEFINITION_OF_DONE.md), [Review Checklist](REVIEW_CHECKLIST.md) |

## Purpose

This document defines how tasks should be structured for AI-assisted work on AnatomIQ. The task system turns large milestones into small, reviewable work items.

## Scope

### In scope

- Task decomposition rules.
- Task metadata and ordering.
- Milestone-to-task mapping.
- Task review and completion tracking.

### Out of scope

- Project management software configuration.
- Automated ticket synchronization.
- Team assignment policies outside the documentation set.

## Task system principles

- Tasks should be small enough to finish and review in one pass when practical.
- Each task should map to a clear output and a governing document.
- Tasks should preserve the current milestone structure.
- Tasks should not mix unrelated areas of work unless the dependency is explicit.

## Task fields

| Field | Purpose |
| --- | --- |
| id | Stable task identifier |
| title | Short action-oriented task name |
| milestone | The milestone the task belongs to |
| document | Governing document or documents |
| input | Required context before starting |
| output | Expected artifact or change |
| validation | How to verify the task is complete |
| status | not-started, in-progress, blocked, completed |

## Task rules

- Task titles should be concise and specific.
- Tasks should not assume hidden context.
- Validation should be explicit and tied to the output.
- Dependencies should be documented before work begins.

## Acceptance criteria

- [ ] The task system supports small, reviewable AI work items.
- [ ] Task fields are explicit and reusable.
- [ ] The system maps cleanly to milestones and documents.
- [ ] AI Context is current.

## Open questions

- [ ] What is the optimal task size for AI-assisted execution in this repository?
- [ ] Should blocked tasks reference a dependency document ID or milestone only?
- [ ] How should task history be preserved once implementation begins?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial task system draft for the AI bible. |

## Review checklist

- [ ] Task fields and rules are explicit.
- [ ] The system supports small, reviewable work items.
- [ ] Validation is tied to task outputs.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define how AI-assisted work tasks should be broken down and tracked in AnatomIQ. |
| Constraints | Keep tasks small, explicit, and tied to a governing document and validation step. |
| Inputs | Project Context, Prompt Library, Review Checklist, Definition of Done. |
| Outputs | Task structure, metadata rules, or milestone mapping. |
| Do not assume | A task is actionable without validation and dependency context. |
| Validation | Confirm each task can be completed, reviewed, and traced back to its source document. |