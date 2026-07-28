# AnatomIQ State Management

| Field | Value |
| --- | --- |
| Document ID | AQ-ENG-008 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before implementation, state refactors, and test strategy review |
| Related documents | [Lesson Engine](LESSON_ENGINE.md), [Interaction Engine](INTERACTION_ENGINE.md), [Annotation System](ANNOTATION_SYSTEM.md), [Functional Requirements](../03-PRD/FUNCTIONAL_REQUIREMENTS.md) |

## Purpose

This document defines the state model for AnatomIQ. State management must preserve lesson progress, interaction context, accessibility preferences, and recovery behavior.

## Scope

### In scope

- Lesson and stage state.
- Annotation and feedback state.
- Accessibility preference state.
- Recovery and resume behavior.

### Out of scope

- Network synchronization or account-backed persistence.
- Analytics event pipelines.
- External data caching policies.

## State principles

- State must be explicit and recoverable.
- State transitions should be predictable and testable.
- The learner should never be left uncertain about where they are.
- State should support both default and reduced-motion paths.

## Core state elements

| State | Meaning |
| --- | --- |
| activeLesson | Selected lesson and content set |
| currentStage | Current point in the route or lesson loop |
| playbackState | Playing, paused, replaying, or stepping |
| annotationState | Open annotations and their focus targets |
| quizState | Question, response, and review context |
| accessibilityState | Reduced motion, text alternatives, or related preferences |
| recoveryState | Fallback, retry, or safe-exit context |

## State rules

- Preserve state across pause, review, and overlay actions.
- Prevent invalid combinations of stage and playback state.
- Keep accessibility preferences active for the session unless explicitly reset.
- State changes must have clear triggers and clear results.

## Persistence expectations

| State category | Persistence expectation |
| --- | --- |
| Lesson progress | Preserved during the active session and recoverable transitions |
| Accessibility preferences | Preserved for the lesson session unless the learner resets them |
| Annotation context | Preserved while the learner inspects or returns |
| Quiz context | Preserved while reviewing feedback and retrying |
| Recovery context | Preserved until the learner retries, exits, or restores |

## Acceptance criteria

- [ ] The state model covers all core lesson behaviors.
- [ ] Invalid state combinations are prevented or resolved.
- [ ] Recovery and accessibility state are explicit.
- [ ] AI Context is current.

## Open questions

- [ ] Which states should be serializable for a future non-account session restore?
- [ ] How much state should live in the lesson engine versus shared state management?
- [ ] What is the minimal state representation needed for the cardiovascular MVP?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial State Management draft for the engineering bible. |

## Review checklist

- [ ] Core state elements are listed.
- [ ] Persistence and recovery expectations are explicit.
- [ ] State rules support lesson integrity and accessibility.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define how lesson and interaction state should be preserved and coordinated in AnatomIQ. |
| Constraints | State must remain explicit, recoverable, and compatible with accessibility and lesson flow rules. |
| Inputs | Lesson Engine, Interaction Engine, Annotation System, Functional Requirements. |
| Outputs | State model, persistence expectations, or transition rules. |
| Do not assume | Browser history or implicit component state is enough for lesson recovery. |
| Validation | Confirm state remains coherent across pause, replay, review, and error paths. |