# AnatomIQ Content and Lesson Requirements

| Field | Value |
| --- | --- |
| Document ID | AQ-PRD-007 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-27 |
| Last updated | 2026-07-27 |
| Review cadence | Before cardiovascular content production and every medical-content change |
| Related documents | [Product Requirements Document](PRODUCT_REQUIREMENTS_DOCUMENT.md), [MVP Scope](MVP_SCOPE.md), [Educational Philosophy](../01-Vision/EDUCATIONAL_PHILOSOPHY.md), [Success Criteria](../01-Vision/SUCCESS_CRITERIA.md) |

## Purpose

This document defines the content contract for the cardiovascular MVP. It explains what a lesson specification must contain, which circulation concepts are in scope, and how medical accuracy, simplification, annotations, and formative assessment are governed.

It does not replace the future detailed cardiovascular medical specification; it establishes what that specification must deliver.

## Required lesson package

Every AnatomIQ lesson package must contain:

| Element | Requirement |
| --- | --- |
| Audience and level | Intended learner level, vocabulary assumptions, prerequisites, and excluded depth. |
| Objectives | Observable learner outcomes mapped to questions and lesson stages. |
| Medical model | Approved structures, relationships, route, timing scope, and source references. |
| Scene plan | Ordered scenes, each with visual focus, explanation, interaction, and expected takeaway. |
| Annotation register | Structure name, function, display context, optional depth, source, and review status. |
| Assessment register | Question, objective mapping, correct reasoning, misconception addressed, feedback, and review link. |
| Simplification register | Omission or teaching convention, reason, learner-facing wording, and reviewer approval. |
| Accessibility content | Text equivalents, captions/transcripts if needed, non-colour cues, and reduced-motion sequence wording. |
| Review record | Content owner, source check, medical review status, educational review status, and revision history. |

## Cardiovascular MVP learning outcomes

| ID | Outcome | Minimum evidence |
| --- | --- | --- |
| LO-CV-01 | Locate heart and lungs in the lesson’s body context. | Contextual selection, explanation, or identification task. |
| LO-CV-02 | Trace deoxygenated blood from body to lungs through the right side of the heart. | Ordering or explanation task. |
| LO-CV-03 | Trace oxygenated blood from lungs to body through the left side of the heart. | Ordering or explanation task. |
| LO-CV-04 | Distinguish the broad roles of arteries, veins, and capillaries in the taught model. | Contextual matching or explanation task. |
| LO-CV-05 | Explain why pulmonary and systemic circulation form a connected loop. | Cause-and-effect response in learner-appropriate language. |

## Required route model

The lesson must teach this high-level route, subject to qualified content review:

```text
Body → venae cavae → right atrium → right ventricle → pulmonary artery → lungs
Lungs → pulmonary veins → left atrium → left ventricle → aorta → body
```

The visual and verbal model must make these points clear:

- arteries and veins are defined by direction relative to the heart, not by oxygenation colour;
- blood travels from the right side of the heart to the lungs and returns to the left side;
- blood then travels from the left side of the heart to the body and returns to the right side;
- capillaries are the broad exchange interface in the taught model;
- the MVP uses a simplified major-route model and does not show every branch, pressure change, or anatomical variation.

Exact wording, anatomical detail, valve inclusion, and source citations require the detailed cardiovascular specification and qualified review.

## Scene requirements

| Scene type | Required learner takeaway | Required content elements |
| --- | --- | --- |
| Entry | “I know what I will learn and this is educational content.” | Title, objective, scope, control orientation. |
| Whole-body orientation | “I know where heart and lungs are.” | System context, spatial explanation, accessible equivalent. |
| Right-heart return | “Blood returning from the body enters the right side.” | Direction cues, major structures, concise explanation. |
| Pulmonary route | “Blood travels from the heart to the lungs.” | Pulmonary artery, lung context, non-colour state cues. |
| Lung exchange overview | “The lungs change the blood’s oxygenation state in this simplified model.” | Clear limitation wording and broad function. |
| Left-heart return | “Blood returns from the lungs to the left side.” | Pulmonary veins, chambers, route continuity. |
| Systemic route | “Blood leaves the left side for the body.” | Aorta/systemic context and direction. |
| Body return and summary | “The route is a connected loop.” | Recap, comparison, review path. |

## Annotation requirements

Required primary annotations are provisional pending the medical specification:

- heart;
- right atrium;
- right ventricle;
- left atrium;
- left ventricle;
- lungs;
- pulmonary artery;
- pulmonary veins;
- aorta;
- venae cavae;
- arteries, veins, and capillaries as category concepts.

Each annotation must include a learner-level name, concise function in the current route, a source/review reference, and a non-hover access path. Additional clinical detail must be optional and clearly scoped.

## Assessment requirements

- Every assessment item maps to one or more `LO-CV` outcomes.
- The item tests a taught relationship, not an unintroduced detail.
- Correct feedback states the relevant reasoning.
- Incorrect feedback addresses a likely misconception and links to a scene or annotation for review.
- The assessment is formative; do not use language that implies certification or diagnosis.
- Questions must remain accessible through keyboard and reduced-motion paths.

## Simplification rules

| Rule | Requirement |
| --- | --- |
| Disclose material simplifications | State when branches, scale, timing, pressure, microscopic detail, or variation are intentionally omitted. |
| Never invert causality | A simplified model cannot teach a direction or function that is false. |
| Separate fact from teaching convention | Do not imply that an illustrative colour, route thickness, or camera position is literal anatomy. |
| Keep caveats proportional | Explain meaningful limitations without overwhelming the learner’s first pass. |
| Review changes | A changed visual model or simplification requires source and reviewer re-check. |

## Content review workflow

1. Lesson author drafts the package with source placeholders and objectives.
2. Educational reviewer verifies clarity, cognitive load, objective alignment, and assessment quality.
3. Qualified medical reviewer verifies the model, labels, claims, route, and simplifications.
4. Design and accessibility reviewers verify that visual and alternative representations communicate the same core concept.
5. The owner resolves feedback, updates the review record, and approves the package for implementation.

## Open questions

- [ ] Which sources and qualified reviewer will approve the cardiovascular route and learner-facing wording?
- [ ] Should the MVP name specific valves, and if so, what objective requires them?
- [ ] How much capillary exchange detail is needed to explain oxygenation without expanding beyond MVP scope?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-27 | AnatomIQ Project Team | Initial MVP content and lesson requirements. |

## Review checklist

- [x] Required lesson package and cardiovascular outcomes are defined.
- [x] High-level route model, scene requirements, annotations, assessment, and simplification rules are defined.
- [x] Review workflow and unresolved content decisions are explicit.
- [x] AI Context is complete.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Author or evaluate cardiovascular MVP content that teaches the approved high-level circulation model accurately, progressively, and accessibly. |
| Constraints | Do not invent medical sources, detailed anatomy, clinical advice, or unapproved valve/pathology content. Map every scene and question to an outcome; disclose material simplifications. |
| Inputs | This document, Educational Philosophy, approved medical sources/review, the master PRD, and future cardiovascular specification. |
| Outputs | A scene plan, annotation register, assessment register, simplification note, or review record. |
| Do not assume | That a visual convention is medically literal or that a detail not in the route model is in scope. |
| Validation | Verify source/review status, objective mapping, accessibility equivalent, simplification disclosure, and formative-feedback quality. |
