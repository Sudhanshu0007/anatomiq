# AnatomIQ Human Body Engine

| Field | Value |
| --- | --- |
| Document ID | AQ-ENG-002 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation, major content expansion, and engine review |
| Related documents | [System Architecture](SYSTEM_ARCHITECTURE.md), [Data Model](DATA_MODEL.md), [3D Art Direction](../05-Design/3D_ART_DIRECTION.md), [Lesson Experience Flow](../04-UX/LESSON_EXPERIENCE_FLOW.md) |

## Purpose

This document defines the reusable Human Body Engine. The engine is the shared anatomical presentation layer that allows lessons to reveal structures, relationships, and flow in a consistent way across body systems.

## Scope

### In scope

- Anatomical scene presentation.
- Structure registration and discovery.
- System-level context and focus management.
- Reusable support for future lesson content.

### Out of scope

- Final 3D library selection.
- Medical source approval workflow.
- Scene-specific visual design details.

## Engine responsibilities

- Load and present anatomical systems and structures.
- Expose structure focus, selection, and contextual reveal behavior.
- Support transparent layering, highlighting, and spatial orientation.
- Provide stable interfaces for lesson content and annotations.

## Engine principles

- The engine must not contain cardiovascular-only logic.
- Structure data must be distinct from scene presentation logic.
- The engine must support whole-body, regional, and focused views.
- The engine must preserve clarity when optional detail is hidden.

## Engine inputs and outputs

| Input | Output |
| --- | --- |
| System definition | Renderable body context |
| Structure registry | Visible and focusable anatomical entities |
| Lesson step instructions | Target focus, camera framing, and highlights |
| Accessibility settings | Reduced-motion or simplified presentation |
| Recovery state | Reset, retry, or alternate presentation behavior |

## Engine boundaries

- The Human Body Engine owns anatomical presentation, not lesson sequencing.
- The Lesson Engine decides which stage to show and when.
- The Data Model provides the content, labels, and route definitions.
- The Camera System can focus the engine, but does not replace the lesson logic.

## Engine acceptance criteria

- [ ] The engine can represent the cardiovascular lesson and support future systems.
- [ ] The engine separates anatomical presentation from lesson orchestration.
- [ ] The engine supports focus, context, and reduced-motion behavior.
- [ ] AI Context is current.

## Open questions

- [ ] What is the minimum anatomical scene contract every lesson must provide to the engine?
- [ ] Which presentation behaviors belong in the engine versus the lesson layer?
- [ ] How will the engine handle shared versus system-specific structures?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial Human Body Engine draft for the engineering bible. |

## Review checklist

- [ ] Engine purpose and boundaries are explicit.
- [ ] Reuse across systems is clear.
- [ ] The engine stays separate from lesson orchestration.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the reusable anatomical presentation engine that supports every AnatomIQ lesson. |
| Constraints | Do not embed cardiovascular-only logic; keep presentation reusable and data-driven. |
| Inputs | System Architecture, Data Model, 3D Art Direction, Lesson Experience Flow. |
| Outputs | Engine responsibilities, boundaries, or interface expectations. |
| Do not assume | A lesson-specific scene can substitute for a reusable body engine. |
| Validation | Confirm the engine can present at least one cardiovascular lesson and remain reusable for future systems. |