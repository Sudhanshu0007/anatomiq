# AnatomIQ Implementation Plan

| Field | Value |
| --- | --- |
| Document ID | AQ-RDM-001 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation begins, before sprint planning, and before release candidate review |
| Related documents | [System Architecture](../06-Engineering/SYSTEM_ARCHITECTURE.md), [Lesson Engine](../06-Engineering/LESSON_ENGINE.md), [Task System](../08-AI/TASK_SYSTEM.md), [Definition of Done](../08-AI/DEFINITION_OF_DONE.md) |

## Purpose

This document defines the implementation plan for AnatomIQ. It turns the approved documentation into a practical sequence for building the MVP, starting with the app scaffold and ending with a validated cardiovascular lesson.

## Scope

### In scope

- MVP implementation sequence.
- Dependency order for engineering work.
- Milestone-to-delivery mapping.
- Readiness conditions for starting build work.

### Out of scope

- Detailed sprint execution metrics.
- Team staffing assignments.
- Release management and infrastructure specifics.

## Implementation sequence

1. Set up the app scaffold and repository structure.
2. Build the shared lesson shell and Human Body Engine foundation.
3. Implement the lesson engine, camera, scroll, and interaction systems.
4. Wire the data model, annotation system, and state management.
5. Add the cardiovascular lesson content and scene flow.
6. Validate accessibility, performance, and recovery paths.
7. Prepare the release candidate and public MVP demo.

## Implementation principles

- Build shared systems before lesson-specific details.
- Keep content data-driven wherever practical.
- Validate one complete lesson path before expanding to new systems.
- Treat accessibility, performance, and recovery as core delivery requirements.

## Dependencies

| Area | Depends on |
| --- | --- |
| App scaffold | Roadmap, architecture, and AI task system |
| Lesson engine | System architecture, data model, and state management |
| Cardiovascular content | Medical package and UX flow docs |
| Validation | Testing strategy and performance strategy |

## Acceptance criteria

- [ ] The implementation order is explicit and dependency-aware.
- [ ] The plan starts with reusable systems, not one-off lesson code.
- [ ] The plan maps cleanly to the documented milestones.
- [ ] AI Context is current.

## Open questions

- [ ] What is the exact order of build slices for the first app scaffold?
- [ ] Which pieces of the lesson shell are needed before the first playable prototype?
- [ ] How much of the implementation should be blocked until medical review is approved?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial implementation plan draft for the roadmap. |

## Review checklist

- [ ] The implementation sequence is clear and practical.
- [ ] Dependencies are explicit.
- [ ] The plan aligns with architecture, UX, and medical documents.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Turn the approved documentation into an implementation sequence for the AnatomIQ MVP. |
| Constraints | Start with reusable systems, keep content data-driven, and do not bypass accessibility or medical review gates. |
| Inputs | System Architecture, Lesson Engine, Task System, Definition of Done, Medical Package. |
| Outputs | Implementation sequence, dependency mapping, or delivery readiness criteria. |
| Do not assume | The project should begin with one-off lesson code before the shared engine is ready. |
| Validation | Confirm the plan can be executed in the stated order and supports the MVP objective. |