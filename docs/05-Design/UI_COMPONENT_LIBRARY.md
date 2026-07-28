# AnatomIQ UI Component Library

| Field | Value |
| --- | --- |
| Document ID | AQ-DSN-004 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before component design, implementation, and design-system review |
| Related documents | [Information Architecture](../04-UX/INFORMATION_ARCHITECTURE.md), [Navigation Model](../04-UX/NAVIGATION_MODEL.md), [Lesson Experience Flow](../04-UX/LESSON_EXPERIENCE_FLOW.md), [UX Copy and Feedback](../04-UX/UX_COPY_AND_FEEDBACK.md) |

## Purpose

This document defines the reusable UI components for AnatomIQ. The component set must support lesson navigation, explanation, review, and accessibility without becoming tied to one specific lesson.

## Scope

### In scope

- Lesson shell components.
- Navigation and control components.
- Annotation and feedback components.
- Helper, help, and summary components.

### Out of scope

- Final visual styling and token values.
- Specific implementation framework details.
- Body-system-specific lesson content.

## Component principles

- Components must be reusable across body systems where practical.
- Controls must have clear states and labels.
- Educational content containers must support long and short copy.
- Overlays must preserve context and be easy to dismiss.

## Core component families

| Family | Examples | Purpose |
| --- | --- | --- |
| Lesson shell | header, stage indicator, progress, footer controls | Provide stable structure across the lesson |
| Navigation | start, continue, back, replay, reset, exit | Move through the experience predictably |
| Annotation | label chip, callout, detail panel | Explain structures in context |
| Feedback | quiz answer state, explanation panel, retry action | Support formative practice |
| Help and recovery | help overlay, accessibility help, error state | Support learner control and recovery |
| Summary | recap card, replay card, next-step card | Close the lesson loop and offer next actions |

## Component rules

- Lesson shell controls must stay in predictable places.
- Annotation components must support open, close, and return focus behavior.
- Feedback components must support both correct and incorrect states.
- The same control language should be used across the product.
- Components must not depend on hover to expose required information.

## State rules

Every core component should account for states such as:

- default;
- hover;
- focused;
- active;
- disabled;
- loading;
- error;
- completed.

## Accessibility rules

- All essential controls must be keyboard reachable.
- Focus states must be visible.
- Disabled states must be understandable.
- Components must not hide necessary text behind motion or pointer-only behavior.

## Component acceptance criteria

- [ ] The component set covers the lesson shell, controls, annotation, feedback, and summary needs.
- [ ] The same components can be reused across future systems.
- [ ] States and accessibility behavior are defined.
- [ ] AI Context is current.

## Open questions

- [ ] Should the lesson shell use a fixed top bar, a persistent rail, or a hybrid layout?
- [ ] Which components should be built as shared primitives versus lesson-specific composites?
- [ ] How much of the component system should be documented before implementation starts?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial UI component draft for the design bible. |

## Review checklist

- [ ] Core component families are identified.
- [ ] Reuse and accessibility requirements are clear.
- [ ] State behavior is documented.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the reusable UI component families needed for AnatomIQ lessons and controls. |
| Constraints | Keep components reusable, accessible, and consistent across the lesson engine. |
| Inputs | Information Architecture, Navigation Model, Lesson Experience Flow, UX Copy and Feedback. |
| Outputs | Component families, state rules, or design-system requirements. |
| Do not assume | A component can be reused without preserving state and accessibility behavior. |
| Validation | Confirm the components support the lesson shell, annotations, feedback, and recovery paths. |