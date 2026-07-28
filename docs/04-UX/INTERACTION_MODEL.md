# AnatomIQ Interaction Model

| Field | Value |
| --- | --- |
| Document ID | AQ-UX-003 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before wireframes, implementation, and interaction testing |
| Related documents | [Information Architecture](INFORMATION_ARCHITECTURE.md), [Navigation Model](NAVIGATION_MODEL.md), [Functional Requirements](../03-PRD/FUNCTIONAL_REQUIREMENTS.md), [User Journeys](../03-PRD/USER_JOURNEYS.md), [Content and Lesson Requirements](../03-PRD/CONTENT_AND_LESSON_REQUIREMENTS.md) |

## Purpose

This document defines how learners interact with the AnatomIQ cardiovascular MVP. It specifies the supported input patterns, what each interaction is allowed to do, and which behaviors are reserved for the reusable lesson engine.

## Scope

### In scope

- Scroll-driven lesson progression.
- Click, hover, and keyboard interaction rules.
- Pause, replay, annotation access, and feedback behavior.
- Drag and rotate behavior for supported views.
- Interaction feedback and state preservation.

### Out of scope

- Final visual styling and component layout.
- Technical implementation details for a specific framework or library.
- AI tutor interactions and natural-language commands.
- Advanced simulation controls that are not required for the MVP learning outcomes.

## Interaction principles

- Every interaction must support a learning objective or a recovery need.
- Scroll should move the learner through a clear story, not trap them in motion.
- Optional detail should never block the primary lesson flow.
- Interaction feedback must be immediate, understandable, and reversible where practical.
- The same concept must remain accessible through pointer, keyboard, and reduced-motion paths.

## Supported inputs

| Input | Primary use | Required behavior |
| --- | --- | --- |
| Scroll | Advance the guided story | Moves to the next approved lesson step or stage boundary. |
| Click or tap | Start, focus, open, or confirm | Activates controls, annotations, and review actions. |
| Hover | Preview or highlight | Never required for essential content. |
| Keyboard | Core navigation and accessibility | Reaches all essential controls and content without a pointer. |
| Drag | Rotate or inspect the body/context view | Preserves lesson state while the learner reorients. |
| Pause control | Stop active motion | Freezes story motion without losing the current step. |
| Replay control | Repeat the current step or scene | Restores a valid starting point for the current stage. |

## Interaction rules

### Scroll

- Scroll is the default narrative driver in the cardiovascular lesson.
- Each major scroll boundary should represent a meaningful lesson transition, not a decorative camera shift.
- The learner must not need perfect scroll precision to continue.
- Rapid scroll should not skip the lesson into an invalid state.

### Click and tap

- Click and tap open lesson controls, system cards, annotations, and review links.
- Important actions must have a visible affordance and clear label.
- Clicking a structure should focus the relevant content without destroying the current lesson state.

### Hover

- Hover may highlight structures, labels, or optional context.
- Hover must never be the only route to the required annotation content.
- Hover previews should not auto-advance the story.

### Keyboard

- Keyboard interaction must reach start, pause, replay, help, annotations, review, summary, and exit.
- Focus order must follow the visual and reading order.
- Enter and Space should activate buttons or open selected content.
- Escape should close non-destructive overlays when appropriate.

### Drag and rotate

- Drag and rotate are allowed for spatial understanding when the lesson stage supports them.
- Rotation must not detach the learner from the active narrative stage.
- A reset orientation control must be available if rotation disorients the learner.

### Pause, replay, and reset

- Pause must suspend motion, camera travel, and synchronized effects together.
- Replay must return the current stage to a valid beginning state.
- Reset must clearly explain whether progress, focus, or preferences will change.

## Annotation behavior

Annotations are secondary educational layers. They must:

- open without destroying lesson progress;
- show a concise title and a clear close action;
- expose the structure name, function, and relevance to the current route;
- preserve the learner’s place in the lesson;
- remain accessible without hover-only input.

## Feedback behavior

- Correct feedback should confirm the reasoning, not just the answer.
- Incorrect feedback should explain the likely misconception and point to the relevant review stage.
- Feedback panels must be treated as recoverable overlays, not dead ends.
- The learner should be able to return to the question, review the route, or continue the lesson.

## State preservation

The interaction model must preserve these states across supported interactions:

| State | Meaning | Must persist across |
| --- | --- | --- |
| Current lesson step | The learner’s current point in the cardiovascular route | Scroll, hover, annotation open/close, and pause |
| Current system context | The learner’s selected body system | Review, replay, and body-context return |
| Annotation context | The structure or explanation opened by the learner | Pause, replay, and non-destructive navigation |
| Feedback context | Question, response, and review link | Review and return to practice |
| Accessibility preference | Reduced motion or equivalent session preference | The lesson session unless clearly reset |

## Interaction acceptance criteria

- [ ] Scroll progression can be completed without accidental state loss.
- [ ] Hover-only behavior is never required for a Must learning outcome.
- [ ] Keyboard users can access every essential action and annotation.
- [ ] Drag and rotate do not break the lesson sequence.
- [ ] Pause and replay preserve a coherent lesson state.
- [ ] Feedback can be reviewed and returned from without losing context.

## Open questions

- [ ] Which interactions should be allowed only in the guided lesson and not in summary or help views?
- [ ] Should drag/rotate be enabled by default or only after explicit learner action?
- [ ] What is the minimum interaction set for a reduced-motion learner who still wants to inspect structures?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial interaction model draft for the cardiovascular MVP. |

## Review checklist

- [ ] Supported inputs and their roles are explicit.
- [ ] Scroll, click, hover, keyboard, drag, and replay rules are clear.
- [ ] Interaction state preservation is documented.
- [ ] The model matches the core journey and accessibility requirements.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define how the learner may interact with the cardiovascular MVP without breaking the educational story. |
| Constraints | Do not require hover for essential content; preserve state; keep interactions tied to learning value. |
| Inputs | Information Architecture, Navigation Model, Functional Requirements, User Journeys, Content and Lesson Requirements. |
| Outputs | Interaction rules, component behavior, state behavior, or test cases. |
| Do not assume | A specific frontend library, animation stack, or hover-capable device is always available. |
| Validation | Confirm each supported input can complete the intended action without losing lesson context. |