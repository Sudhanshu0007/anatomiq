# AnatomIQ UX Copy and Feedback

| Field | Value |
| --- | --- |
| Document ID | AQ-UX-007 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before wireframes, content production, and feedback implementation |
| Related documents | [Information Architecture](INFORMATION_ARCHITECTURE.md), [Navigation Model](NAVIGATION_MODEL.md), [Interaction Model](INTERACTION_MODEL.md), [Lesson Experience Flow](LESSON_EXPERIENCE_FLOW.md), [Content and Lesson Requirements](../03-PRD/CONTENT_AND_LESSON_REQUIREMENTS.md) |

## Purpose

This document defines the tone, phrasing, and feedback style for AnatomIQ. It ensures instructions, labels, tooltips, quiz prompts, and error messages stay clear, educational, and consistent.

## Scope

### In scope

- Entry and lesson instructions.
- Labels, button text, and system names.
- Tooltips and annotation copy.
- Quiz prompts and feedback.
- Error, limitation, and scope-disclaimer copy.

### Out of scope

- Final legal wording for future product terms or policies.
- Marketing copy for launch pages.
- Long-form medical education content that belongs in lesson or medical documents.

## Copy principles

- Keep language direct and learner-friendly.
- Explain what the learner can do next.
- Use the same term for the same concept throughout the repository.
- Avoid hype, joke copy, or language that overpromises learning outcomes.
- State simplifications and limitations plainly when they matter to understanding.

## Tone

The tone should be:

- calm;
- precise;
- educational;
- encouraging without being informal;
- confident without claiming clinical authority.

The tone should not be:

- overly playful;
- vague;
- sales-like;
- clinical to the point of being cold;
- dramatic about risks or outcomes.

## Copy rules by content type

### Entry and lesson instructions

- Tell the learner what the lesson is and what it will teach.
- Keep the first read short enough to support immediate orientation.
- Mention educational scope and no-account access when relevant.

### Labels and annotations

- Use the canonical structure name.
- Pair the name with a short function or relevance statement.
- Avoid burying the main takeaway in a paragraph of detail.

### Tooltips and helper text

- Tooltips should explain the purpose of a control or structure.
- Helper text should reduce confusion, not repeat the entire lesson.
- Keep terminology consistent with the lesson and content documents.

### Quiz prompts

- Ask about a taught relationship, not an unintroduced detail.
- Keep the prompt concise and unambiguous.
- Use feedback to reinforce reasoning, not just correctness.

### Feedback copy

- Correct feedback should explain why the answer is right.
- Incorrect feedback should identify the misconception and point to review.
- Feedback should preserve dignity and encourage another attempt.

### Error and limitation copy

- Say what failed in plain language.
- Offer a safe next step: retry, review, simplified alternative, or exit.
- If the lesson is simplified, say so without weakening the core meaning.

## Canonical phrasing guidance

Use these patterns where possible:

| Situation | Preferred phrasing |
| --- | --- |
| Lesson start | “Start lesson” or “Continue lesson” |
| Return to body | “Return to body context” |
| Review route | “Review this step” |
| Wrong answer | “That answer needs one more step of reasoning.” |
| Simplification notice | “This lesson uses a simplified model for clarity.” |
| Recovery | “Retry,” “Use simplified view,” or “Exit safely” |

## Disallowed copy patterns

- “Easy,” “just,” or similar language that hides complexity.
- “Watch and learn” when the experience requires interaction.
- Clinical claims that imply diagnosis or treatment.
- Empty labels such as “Click here.”
- Wording that makes hidden content sound available when it is not.

## Feedback patterns

| Feedback type | Requirement |
| --- | --- |
| Correct | Confirm the concept and reinforce why it works. |
| Incorrect | Identify the likely mistake and point to the right review location. |
| Help prompt | Explain the control or next action in a sentence or two. |
| Error message | State the problem, the impact, and the recovery path. |
| Scope disclaimer | Clarify educational boundaries without sounding defensive. |

## Copy examples

### Good examples

- “Return to body context”
- “This lesson uses a simplified circulation model for clarity.”
- “Review the pulmonary route”
- “That answer is close, but the flow direction needs one more step.”

### Bad examples

- “Awesome!”
- “Click this magic button”
- “You’re wrong”
- “Medical-grade results guaranteed”

## UX copy acceptance criteria

- [ ] Instructional copy is short, direct, and consistent.
- [ ] Labels and feedback use canonical terminology.
- [ ] Quiz and error copy support learning rather than judgment.
- [ ] Scope and simplification wording is explicit where needed.
- [ ] AI Context is current.

## Open questions

- [ ] Should tone vary slightly between entry, lesson, and quiz states, or remain uniform throughout?
- [ ] What level of simplification wording is enough for the first prototype without overloading the learner?
- [ ] Should pronunciation guidance be part of this milestone or deferred to the medical/content layer?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial UX copy and feedback draft for the cardiovascular MVP. |

## Review checklist

- [ ] Tone and phrasing rules are explicit.
- [ ] Labels, feedback, and disclaimers follow the same language model.
- [ ] Good and bad examples make the standard clear.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Create consistent learner-facing copy and feedback rules for the cardiovascular MVP. |
| Constraints | Use plain language, preserve educational scope, and avoid hidden or misleading claims. |
| Inputs | Information Architecture, Navigation Model, Interaction Model, Lesson Experience Flow, Content and Lesson Requirements. |
| Outputs | UI copy, feedback copy, label text, tooltip text, or review rules. |
| Do not assume | The learner already knows the anatomy terms or the project scope. |
| Validation | Check that every instruction, error, and feedback message is clear, consistent, and educational. |