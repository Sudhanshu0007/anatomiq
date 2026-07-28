# AnatomIQ Navigation Model

| Field | Value |
| --- | --- |
| Document ID | AQ-UX-002 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-27 |
| Last updated | 2026-07-27 |
| Review cadence | Before wireframes, implementation, and usability testing |
| Related documents | [Information Architecture](INFORMATION_ARCHITECTURE.md), [User Journeys](../03-PRD/USER_JOURNEYS.md), [Functional Requirements](../03-PRD/FUNCTIONAL_REQUIREMENTS.md) |

## Purpose

This document defines how learners move through AnatomIQ without losing orientation or control. It covers global movement, lesson-stage movement, overlay behavior, exits, and recovery.

## Navigation principles

- Always show where the learner is: system, lesson, and major route stage.
- Make forward progression clear, but never trap the learner in an animation or scroll sequence.
- Preserve current context when opening optional details or reviewing feedback.
- Use predictable labels and locations for pause, replay, help, and exit.
- Support pointer, keyboard, touch, and reduced-motion paths for essential movement.
- Do not use authentication, profiles, or saved-history pages as navigation prerequisites.

## Global navigation

| From | To | Trigger | Required behavior |
| --- | --- | --- | --- |
| Entry | System explorer | Explore body systems | Shows currently available and planned systems honestly. |
| Entry/system explorer | Lesson entry | Select Cardiovascular | Opens lesson entry with objective and scope. |
| Lesson entry | Orientation | Start lesson | Begins from known initial state. |
| Any lesson stage | Help/preferences | Help control | Opens non-destructive overlay; current lesson remains recoverable. |
| Any lesson stage | System explorer or entry | Exit lesson | Requests confirmation only if meaningful active progress would be lost; otherwise exits directly. |
| Summary | System explorer | Explore systems | Returns to system context without requiring an account. |

## Lesson-stage navigation

| Control | Purpose | Rule |
| --- | --- | --- |
| Continue / next | Advance the guided story | Advances only to the next approved story stage. |
| Previous completed stage | Review already taught content | Must not imply an unseen future stage is complete. |
| Stage navigator | Directly revisit completed major stages | Current stage is visibly indicated; locked future stages are not presented as available. |
| Pause / resume | Control time-based content | Must preserve the active stage state. |
| Replay stage | Repeat current stage | Restores stage start in a valid state. |
| Restart lesson | Return to first lesson stage | Explain reset impact if user settings or progress are affected. |
| Return to body context | Re-orient spatially | Must not silently reset route progress. |
| Review from feedback | Open the relevant stage | Must provide a return route to the question/feedback context. |

## Overlay and focus behavior

Annotations, help, simplification notes, and feedback panels are overlays or secondary views. They must:

- have a clear title and close action;
- preserve the underlying stage state;
- receive focus when opened and return focus to the triggering control when closed;
- avoid obscuring the active control permanently;
- be usable without hover or precise pointer movement;
- not advance the story automatically while the learner reads essential information.

## Exit and restart behavior

| Action | Expected result |
| --- | --- |
| Exit before meaningful progress | Return directly to entry/system explorer. |
| Exit after meaningful progress | Offer a concise choice: continue lesson, restart, or exit. Do not require sign-in to preserve progress. |
| Browser refresh | Use documented session behavior; do not imply progress has been saved unless it has. |
| Restart lesson | Return to lesson entry or orientation and reset story state; retain accessibility preference for the current session where practical. |
| Critical error | Offer retry, simplified alternative if available, safe exit, and plain-language explanation. |

## Keyboard navigation expectations

- Tab or equivalent moves through actionable controls in a logical visual/reading order.
- Enter/Space or equivalent activates buttons and opens annotations.
- Escape closes non-destructive overlays where appropriate.
- Keyboard navigation never depends on simulated pointer hover.
- Exact shortcuts may be defined later; no shortcut is required for core completion.

## Navigation acceptance criteria

- [ ] Learners can identify current system and lesson stage at every point.
- [ ] Learners can pause, replay, review, access help, and exit from every guided stage.
- [ ] Opening/closing details does not lose the active story context.
- [ ] Direct review preserves a logical relationship to the full route.
- [ ] Keyboard-only movement completes the essential lesson journey.
- [ ] No navigation route requires an account or payment.

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-27 | AnatomIQ Project Team | Initial global and lesson navigation model. |

## Review checklist

- [x] Global, stage, overlay, exit, recovery, and keyboard behavior are defined.
- [x] Navigation preserves learner agency and no-auth access.
- [x] Acceptance criteria map to core user journeys.
- [x] AI Context is complete.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Create predictable navigation that lets learners progress, pause, review, recover, and exit without losing orientation. |
| Constraints | Keep current system/stage visible; preserve state across overlays; support keyboard; never require authentication for movement or review. |
| Inputs | This document, Information Architecture, User Journeys, and Functional Requirements. |
| Outputs | Navigation controls, routing behavior, focus behavior, state transitions, or test cases. |
| Do not assume | Direct navigation grants access to future stages or that browser refresh has saved progress. |
| Validation | Complete each listed navigation action using pointer and keyboard, including overlay, review, restart, and error paths. |
