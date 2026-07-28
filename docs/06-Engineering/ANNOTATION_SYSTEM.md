# AnatomIQ Annotation System

| Field | Value |
| --- | --- |
| Document ID | AQ-ENG-007 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation, content updates, and accessibility review |
| Related documents | [Content and Lesson Requirements](../03-PRD/CONTENT_AND_LESSON_REQUIREMENTS.md), [Interaction Model](../04-UX/INTERACTION_MODEL.md), [UX Copy and Feedback](../04-UX/UX_COPY_AND_FEEDBACK.md), [Lesson Engine](LESSON_ENGINE.md) |

## Purpose

This document defines the Annotation System. The system displays structure names, functions, relevance, and optional detail without interrupting the lesson flow.

## Scope

### In scope

- Annotation data and rendering behavior.
- Open and close behavior.
- Required and optional detail levels.
- Accessibility and focus behavior.

### Out of scope

- Full medical authoring workflow.
- Final visual design tokens.
- Search or glossary tooling not needed for the MVP.

## System responsibilities

- Present structure names and concise explanations in context.
- Keep annotations tied to the active lesson stage or selected structure.
- Provide a clear path to open, close, and revisit annotations.
- Preserve context and focus behavior during overlays.

## Annotation types

| Type | Purpose |
| --- | --- |
| Required annotation | Structure or concept needed to complete the lesson objective |
| Optional annotation | Additional context that supports curiosity or depth |
| Review annotation | A linked explanation used after practice or feedback |
| Simplification note | Clear statement about what the lesson omits or simplifies |

## Annotation data fields

| Field | Purpose |
| --- | --- |
| title | The structure or concept name |
| function | Concise relevance statement for the current lesson |
| context | When and where the annotation appears |
| depth | Optional extended explanation |
| review link | Where the learner can return after feedback |
| accessibility text | Text equivalent for non-visual access |

## Annotation rules

- Required annotations must never depend on hover only.
- The system should default to concise context and allow optional depth.
- Annotations should not obscure the primary lesson story.
- The system must preserve the learner’s place in the lesson.

## Acceptance criteria

- [ ] Required annotations expose name and function clearly.
- [ ] Optional depth is available without losing context.
- [ ] Keyboard and accessibility support is complete.
- [ ] AI Context is current.

## Open questions

- [ ] What is the exact boundary between required annotation and optional depth for the MVP?
- [ ] Should review annotations be separate objects or references back to the same annotation record?
- [ ] How should annotations behave when multiple structures are selected in quick succession?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial Annotation System draft for the engineering bible. |

## Review checklist

- [ ] Annotation types and data fields are explicit.
- [ ] Required and optional content behavior is clear.
- [ ] Focus and context preservation are included.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the annotation system that presents structure context without interrupting lesson flow. |
| Constraints | Required annotations must be accessible without hover-only input and must preserve lesson context. |
| Inputs | Content and Lesson Requirements, Interaction Model, UX Copy and Feedback, Lesson Engine. |
| Outputs | Annotation data structure, behavior rules, or accessibility requirements. |
| Do not assume | An annotation can be purely visual or context-free. |
| Validation | Confirm annotations can be opened, read, and closed without losing the lesson state. |