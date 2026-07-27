# AnatomIQ Cardiovascular MVP Scope

| Field | Value |
| --- | --- |
| Document ID | AQ-PRD-004 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-27 |
| Last updated | 2026-07-27 |
| Review cadence | Before implementation begins and whenever scope changes |
| Related documents | [Product Requirements Document](PRODUCT_REQUIREMENTS_DOCUMENT.md), [User Personas](USER_PERSONAS.md), [User Journeys](USER_JOURNEYS.md), [Success Criteria](../01-Vision/SUCCESS_CRITERIA.md) |

## Purpose

This document locks the first buildable AnatomIQ scope. It identifies the smallest responsible product that can validate the core learning hypothesis and reusable lesson model without attempting to build an entire human-body atlas.

## MVP definition

The MVP is one complete, learner-controlled cardiovascular circulation lesson. It begins with body-level orientation, follows the major pulmonary and systemic circulation route, provides contextual explanations and formative practice, and supports essential accessible alternatives.

The MVP proves the **lesson engine**, not the entire content library. It must be good enough for representative learner testing and a clearly scoped public demonstration; it is not a complete medical atlas.

## In scope

### Lesson content

- Whole-body or thoracic orientation that locates the heart and lungs.
- A high-level circulation story: body → right atrium → right ventricle → pulmonary artery → lungs → pulmonary veins → left atrium → left ventricle → aorta → body.
- The broad distinction between pulmonary and systemic circulation.
- The broad concept of oxygenation change in the lungs.
- Primary structure annotations needed to support the lesson objectives.
- Explicit simplification statements where the visual model omits relevant detail.

### Core learning experience

- Lesson title, objective, learner-level indication, and educational scope statement.
- Scroll- or step-driven story progression with a visible current-step indicator.
- Pause, replay current step, restart lesson, and revisit completed major steps.
- Contextual annotations with a name and concise functional explanation.
- Formative knowledge checks aligned to `LO-CV-01` through `LO-CV-05`.
- Feedback that explains reasoning and links to the relevant review point.
- Summary with replay and exit options.

### Essential quality and access

- Keyboard operation for core controls and knowledge checks.
- Reduced-motion or step-based presentation of the essential route.
- Flow/state cues beyond colour alone.
- Readable text alternatives for essential visual meaning.
- Recoverable handling for critical asset/view failures.
- A documented reference environment, support policy, and content-review path before public release.

### Reusable platform proof

- Data or configuration that separates lesson steps, annotations, and assessment from shared behaviors where practical.
- A documented boundary between reusable lesson capabilities and cardiovascular-specific content.
- At least one internal exercise or design review demonstrating how a second system lesson would use the shared model.

## Explicitly out of scope

| Area | Deferred MVP item | Reason |
| --- | --- | --- |
| Body systems | Full nervous, respiratory, digestive, endocrine, urinary, immune, and reproductive lessons | Validate one complete lesson model first. |
| Cardiovascular detail | Complete vessel tree, full valve mechanics, pressure curves, ECG, microcirculation detail, every anatomical variation | Exceeds the core learning objective. |
| Pathology | Heart attack, stroke, valve disease, hypertension, congenital conditions, patient cases | Requires additional medical review and a validated normal-model foundation. |
| AI | Tutor chat, natural-language lesson navigation, personalized explanations | Requires separate safety, quality, and privacy specification. |
| Accounts | Sign-in, profiles, saved learning history, classroom rosters | Adds privacy and product complexity without proving core learning value. |
| Monetization | Payments, subscriptions, ads, or licensing flows | Not needed for MVP validation. |
| Social features | Sharing, comments, leaderboards, streaks, competitive scoring | Not aligned with the initial learning goal. |
| Immersive modes | VR/AR, unrestricted free exploration, photorealistic surgery views | High complexity and accessibility risk. |
| Localization | Multiple languages and full regional curriculum mapping | Plan after validating core content and terminology. |

## Scope slices

| Slice | Outcome | Minimum evidence before moving on |
| --- | --- | --- |
| S0 — Documentation and content model | Approved route, objectives, simplifications, review plan, and journey requirements | Requirements and lesson story are coherent and reviewable. |
| S1 — Static orientation prototype | Learner can locate heart/lungs and identify system focus | Basic orientation task succeeds with representative feedback. |
| S2 — Guided route prototype | Learner can follow the route with step progression and clear cues | Learner can trace the broad route; major confusion is documented. |
| S3 — Control and annotation prototype | Pause, replay, navigation, and core annotations work | Learners can inspect and revisit without state loss. |
| S4 — Practice and accessibility path | Knowledge checks, feedback, keyboard flow, and reduced-motion path work | Essential task completion is demonstrated through default and alternative paths. |
| S5 — Release candidate | Quality gates, content review, validation, and recovery behavior are complete | MVP release gates in `AQ-VIS-004` are satisfied. |

## Scope-change rules

A proposed addition is allowed only when it does one of the following:

1. resolves a blocker to a Must requirement or release gate;
2. materially improves an existing MVP learning objective;
3. is necessary for scientific accuracy, accessibility, privacy, reliability, or recovery; or
4. reduces implementation risk without changing learner-facing scope.

All other additions are deferred to the backlog unless the owner updates this document and the master PRD with a reason, trade-off, and impact on validation timing.

## Definition of MVP complete

The MVP is complete only when:

- [ ] Every Must requirement in the master PRD has evidence of completion.
- [ ] The five cardiovascular learner outcomes have been taught and assessed at the approved level.
- [ ] Essential default and accessibility journeys pass their acceptance criteria.
- [ ] Required medical-content review and simplification disclosure are complete.
- [ ] The product meets its documented support and performance policy.
- [ ] Critical failure recovery has been tested.
- [ ] Reusable lesson boundaries are documented.
- [ ] Validation findings, unresolved risks, and approved exceptions are recorded.

## Open questions

- [ ] Which selected valves, if any, are essential to the MVP learning objective beyond the chamber-to-chamber route?
- [ ] Should the body endpoint be represented by one example organ or a broad systemic-body view?
- [ ] What is the smallest viable non-3D fallback that still teaches the route accurately?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-27 | AnatomIQ Project Team | Initial cardiovascular MVP scope and release slices. |

## Review checklist

- [x] In-scope lesson, interaction, quality, and reusability outcomes are explicit.
- [x] Deferred work is explicitly listed to prevent scope creep.
- [x] Build slices and scope-change rules are defined.
- [x] MVP completion criteria map to the master PRD and Success Criteria.
- [x] AI Context is complete.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Keep implementation focused on one complete cardiovascular learning journey that validates the reusable AnatomIQ lesson model. |
| Constraints | Do not implement deferred systems, pathology, AI, accounts, social features, monetization, or immersive modes as MVP work. Add work only under the scope-change rules. |
| Inputs | This scope document, the master PRD, User Journeys, Success Criteria, and future approved technical/content specifications. |
| Outputs | A scoped task, prototype slice, implementation plan, or release-readiness report mapped to S0–S5 and a Must requirement. |
| Do not assume | That an impressive visual, a broader anatomy model, or a new feature helps validate the MVP. |
| Validation | Confirm the work is in scope, improves a listed outcome or gate, and does not add an unapproved dependency or learner-facing commitment. |
