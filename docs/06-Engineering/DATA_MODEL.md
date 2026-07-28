# AnatomIQ Data Model

| Field | Value |
| --- | --- |
| Document ID | AQ-ENG-009 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation, content authoring, and schema changes |
| Related documents | [System Architecture](SYSTEM_ARCHITECTURE.md), [Human Body Engine](HUMAN_BODY_ENGINE.md), [Annotation System](ANNOTATION_SYSTEM.md), [Content and Lesson Requirements](../03-PRD/CONTENT_AND_LESSON_REQUIREMENTS.md) |

## Purpose

This document defines the data model for AnatomIQ. The model must represent systems, structures, lessons, annotations, assessments, and media in a reusable, data-driven format.

## Scope

### In scope

- Lesson and stage entities.
- Anatomical system and structure entities.
- Annotation and quiz entities.
- Simplification and review metadata.

### Out of scope

- Database vendor selection.
- Migration tooling details.
- Full API schema implementation.

## Model principles

- Content must be represented as data wherever practical.
- Lesson data should be reusable across future body systems.
- Required fields should be explicit and validated.
- Medical and accessibility metadata should travel with the content.

## Core entities

| Entity | Purpose |
| --- | --- |
| System | A body system such as cardiovascular or nervous |
| Structure | A named anatomical entity such as heart or aorta |
| Lesson | A complete learning journey for a system |
| Stage | A discrete step in the lesson flow |
| Annotation | Contextual explanation attached to a structure or stage |
| Assessment | A formative question and feedback pair |
| Simplification | A statement about what the model omits or simplifies |
| Media asset | Model, texture, audio, or related resource |

## Required fields

| Entity | Required fields |
| --- | --- |
| Lesson | id, title, level, objective, scope, stages, accessibility notes |
| Stage | id, title, focus, explanation, transitions, annotations, review links |
| Structure | id, name, role, system, visibility rules, annotation references |
| Annotation | id, title, function, context, depth, accessibility text |
| Assessment | id, prompt, answer model, feedback, review link, outcome mapping |
| Simplification | id, statement, rationale, reviewer status, affected stage |

## Data rules

- The lesson data must not be hardcoded into the presentation layer.
- Structure and lesson identifiers must remain stable.
- Review and simplification metadata must be available to the relevant systems.
- The model must support content updates without rewriting the engine.

## Acceptance criteria

- [ ] The model covers the lesson, anatomy, annotation, and assessment needs.
- [ ] The data is reusable across future systems.
- [ ] Required review and simplification metadata are represented.
- [ ] AI Context is current.

## Open questions

- [ ] Which data format is best for authoring versus runtime consumption?
- [ ] How strict should schema validation be during authoring?
- [ ] Which fields should be mandatory for every future system lesson?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial Data Model draft for the engineering bible. |

## Review checklist

- [ ] Core entities and required fields are defined.
- [ ] Reusability and metadata needs are explicit.
- [ ] The model supports content updates without engine rewrites.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the reusable data model for lessons, structures, annotations, and assessments. |
| Constraints | Keep content data-driven and reusable; do not hardcode the cardiovascular lesson into the UI layer. |
| Inputs | System Architecture, Human Body Engine, Annotation System, Content and Lesson Requirements. |
| Outputs | Data entities, required fields, or validation expectations. |
| Do not assume | A future lesson can be added safely without explicit schema support. |
| Validation | Confirm the data model can represent the cardiovascular MVP and remain reusable later. |