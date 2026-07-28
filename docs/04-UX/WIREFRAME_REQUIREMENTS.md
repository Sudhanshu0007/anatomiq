# AnatomIQ Wireframe Requirements

| Field | Value |
| --- | --- |
| Document ID | AQ-UX-006 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before visual mockups, prototype production, and layout review |
| Related documents | [Information Architecture](INFORMATION_ARCHITECTURE.md), [Navigation Model](NAVIGATION_MODEL.md), [Interaction Model](INTERACTION_MODEL.md), [Lesson Experience Flow](LESSON_EXPERIENCE_FLOW.md), [Accessibility Specification](ACCESSIBILITY_SPECIFICATION.md) |

## Purpose

This document specifies what each wireframe for the cardiovascular MVP must contain before visual design begins. It defines the required screen contents, overlays, and layout concerns that the wireframes must solve.

## Scope

### In scope

- Entry, lesson entry, orientation, flow, quiz, feedback, summary, and help wireframes.
- Shared lesson shell requirements.
- Overlay and panel requirements.
- Layout constraints for accessibility and learner control.

### Out of scope

- Visual style, branding, colour palette, and typography choices.
- Technical implementation details.
- Final content wording beyond what the layout must reserve space for.

## Wireframe rules

- Every wireframe must show the learner’s current location in the lesson.
- Every important action must have a visible place in the layout.
- The layout must reserve room for labels, feedback, and accessible alternatives.
- Optional content must not crowd out the main route explanation.
- Wireframes must show how the learner gets back if they open details or feedback.

## Required screens

### Entry screen

Must contain:

- lesson title;
- brief product description;
- educational scope statement;
- primary start action;
- help or accessibility entry;
- visible note that no account is required.

### Lesson entry screen

Must contain:

- lesson name;
- learner level;
- learning objective;
- scope and limitation statement;
- control summary;
- reduced-motion entry or indicator;
- continue/start action.

### Orientation screen

Must contain:

- whole-body or thoracic body context;
- highlighted heart and lungs;
- active system label;
- current step indicator;
- continue and return actions.

### Guided flow screen

Must contain:

- main visual stage;
- current route label;
- direction cues;
- primary explanation area;
- annotation access;
- pause and replay controls;
- step navigation or equivalent review controls.

### Knowledge check screen

Must contain:

- question prompt;
- answer controls;
- submit action;
- feedback space;
- review link or stage return;
- clear state for right or wrong response.

### Summary screen

Must contain:

- route recap;
- key takeaways;
- replay and review options;
- system explorer or exit action;
- scope reminder that the lesson is formative.

### Help and accessibility overlay

Must contain:

- title;
- close action;
- control guide;
- accessibility note;
- recovery/help path;
- enough space for concise explanatory text.

## Layout requirements by region

| Region | Requirement |
| --- | --- |
| Top region | Lesson title, status, and current stage should be easy to find. |
| Main region | The active lesson visual should remain dominant. |
| Supporting region | Annotations, explanation, or help should be readable without covering the main story. |
| Control region | Pause, replay, navigation, and exit should be consistently located. |
| Feedback region | Quiz and recovery messages need enough space to explain reasoning clearly. |

## Layout constraints

- Wireframes must allow for long educational copy without breaking the layout.
- Wireframes must account for focus states and keyboard navigation.
- The layout should support an accessible alternative view without rethinking the entire structure.
- Controls should remain usable on smaller displays and shared classroom screens.

## Wireframe checklist

For each screen or overlay, wireframes must answer:

1. What is the learner looking at?
2. What can the learner do next?
3. Where is the learner in the route?
4. How does the learner get back or recover?
5. Where does the accessible alternative appear?

## Wireframe acceptance criteria

- [ ] Every required screen is represented.
- [ ] Each layout includes the required content regions.
- [ ] Control placement is consistent across the lesson shell.
- [ ] Overlays have a clear open and close path.
- [ ] The layout can support accessibility and recovery needs.

## Open questions

- [ ] Should lesson controls live in a persistent sidebar or in a floating control strip?
- [ ] How much of the annotation content should be visible by default in the main wireframe?
- [ ] Should help be a separate wireframe or a shared overlay pattern?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial wireframe requirements draft for the cardiovascular MVP. |

## Review checklist

- [ ] Screen inventory and layout regions are defined.
- [ ] Control and overlay requirements are clear.
- [ ] Accessibility and recovery space is reserved.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the minimum content each wireframe must contain before visual mockups are created. |
| Constraints | Do not remove required controls, recovery routes, or accessibility space from the layout. |
| Inputs | Information Architecture, Navigation Model, Interaction Model, Lesson Experience Flow, Accessibility Specification. |
| Outputs | Wireframe content requirements, screen inventory, or layout constraints. |
| Do not assume | A wireframe can omit controls because they will be added later in design. |
| Validation | Ensure each required screen can support the lesson flow, review, and recovery behaviors. |