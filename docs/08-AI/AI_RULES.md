# AnatomIQ AI Rules

| Field | Value |
| --- | --- |
| Document ID | AQ-AI-002 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before AI-assisted implementation, prompt updates, and milestone changes |
| Related documents | [Project Context](PROJECT_CONTEXT.md), [Coding Standards](CODING_STANDARDS.md), [Task System](TASK_SYSTEM.md), [Review Checklist](REVIEW_CHECKLIST.md) |

## Purpose

This document defines the non-negotiable rules for AI-assisted work on AnatomIQ. It prevents AI collaborators from inventing requirements, claiming unverified results, or drifting outside approved scope.

## Scope

### In scope

- AI collaboration boundaries.
- Output quality and verification rules.
- Content, code, and documentation behavior.
- Claim and assumption rules.

### Out of scope

- Model vendor selection.
- Prompt-engine implementation details.
- Runtime safety systems outside the documentation workflow.

## AI rules

- Always follow the approved documentation before proposing changes.
- Do not invent sources, tests, approvals, or capabilities.
- Do not alter medical scope without matching document updates.
- Treat all AI-generated work as draft until reviewed by a responsible human.
- Prefer small, reviewable changes over broad speculative rewrites.

## Verification rules

| Rule | Requirement |
| --- | --- |
| Source verification | Medical and factual claims must be traceable to approved documents or sources |
| Scope control | Changes must stay within the current milestone and related documents |
| Safety | Do not introduce privacy, accessibility, or clinical risks without explicit review |
| Honesty | Do not state that testing, approval, or completion happened unless it did |
| Consistency | Use canonical terms and document IDs exactly as written |

## Response rules

- Prefer direct answers tied to the current documentation.
- If information is missing, identify the gap rather than filling it with assumptions.
- When a decision is needed, state the tradeoff and relevant document references.
- When multiple options exist, prefer the one that preserves reuse, clarity, and reviewability.

## Acceptance criteria

- [ ] The rules prevent invented scope and unsupported claims.
- [ ] The rules align with the project constitution and documentation standards.
- [ ] The rules are clear enough for AI-assisted implementation and review.
- [ ] AI Context is current.

## Open questions

- [ ] Should AI-generated content be tagged in review notes or only tracked in task history?
- [ ] What additional rules are needed once implementation starts in earnest?
- [ ] Should the AI rules be duplicated in future system-specific prompts or kept centralized here?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial AI rules draft for the AI bible. |

## Review checklist

- [ ] AI boundaries and verification rules are explicit.
- [ ] The rules align with documented scope and governance.
- [ ] The document is suitable for AI-assisted work.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the non-negotiable rules AI collaborators must follow in AnatomIQ. |
| Constraints | Do not invent claims, scope, review status, or test results. |
| Inputs | Project Context, Coding Standards, Task System, Review Checklist. |
| Outputs | AI collaboration rules, verification constraints, or response guidelines. |
| Do not assume | AI output is accepted without human review and documentation alignment. |
| Validation | Confirm the rules prevent scope drift and unverified claims. |