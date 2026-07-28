# AnatomIQ Prompt Library

| Field | Value |
| --- | --- |
| Document ID | AQ-AI-005 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before prompt use, prompt updates, and new milestone execution |
| Related documents | [Project Context](PROJECT_CONTEXT.md), [AI Rules](AI_RULES.md), [Task System](TASK_SYSTEM.md), [Review Checklist](REVIEW_CHECKLIST.md) |

## Purpose

This document defines the prompt patterns used for AnatomIQ. The prompt library helps AI collaborators work with the right context, constraints, and expected outputs.

## Scope

### In scope

- Prompt templates and prompt structure.
- Prompt inputs and expected outputs.
- Prompt selection guidance.
- Prompt review expectations.

### Out of scope

- Model-specific tuning.
- Runtime prompt orchestration.
- External prompt analytics.

## Prompt principles

- Prompts should be narrow enough to produce reviewable output.
- Prompts must reference the relevant source documents.
- Prompts should state the expected validation.
- Prompts should not ask AI to invent missing scope or approval.

## Prompt types

| Type | Purpose |
| --- | --- |
| Document drafting | Create or expand a specification from approved context |
| Implementation task | Produce code or structured changes for a single task |
| Review task | Evaluate work against the governing documents |
| Debugging task | Diagnose behavior using logs, errors, or state evidence |

## Prompt template fields

| Field | Purpose |
| --- | --- |
| context | Relevant project and document background |
| objective | What the AI should accomplish |
| constraints | Non-negotiable limits |
| inputs | Source documents or artifacts |
| output | Expected artifact or result |
| validation | How to check the result |

## Prompt rules

- Always include the governing document references.
- State whether the task is drafting, implementing, reviewing, or debugging.
- Keep the prompt focused on one coherent outcome.
- Ask for assumptions to be stated explicitly when needed.

## Acceptance criteria

- [ ] The prompt library provides reusable prompt structure.
- [ ] Prompt types match common AI-assisted workflow needs.
- [ ] The prompts align with the task system and review process.
- [ ] AI Context is current.

## Open questions

- [ ] Which prompts should be standardized first for the MVP workflow?
- [ ] Should prompts include milestone-specific examples or remain abstract?
- [ ] How much prompt reuse is desirable before the project is partially implemented?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial prompt library draft for the AI bible. |

## Review checklist

- [ ] Prompt types and fields are explicit.
- [ ] The library aligns with the task system and AI rules.
- [ ] Validation is part of every prompt pattern.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the reusable prompt patterns for AI-assisted work in AnatomIQ. |
| Constraints | Prompts must reference governing documents and avoid inventing missing context. |
| Inputs | Project Context, AI Rules, Task System, Review Checklist. |
| Outputs | Prompt templates, prompt types, or selection guidance. |
| Do not assume | AI can safely infer task scope without explicit documentation references. |
| Validation | Confirm the prompt library produces narrow, reviewable outputs. |