# AnatomIQ Non-Functional Requirements

| Field | Value |
| --- | --- |
| Document ID | AQ-PRD-006 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-27 |
| Last updated | 2026-07-27 |
| Review cadence | Before architecture approval, release candidate review, and any support-policy change |
| Related documents | [Product Requirements Document](PRODUCT_REQUIREMENTS_DOCUMENT.md), [Functional Requirements](FUNCTIONAL_REQUIREMENTS.md), [User Journeys](USER_JOURNEYS.md), [Success Criteria](../01-Vision/SUCCESS_CRITERIA.md) |

## Purpose

This document specifies the quality attributes required for AnatomIQ’s cardiovascular MVP. These requirements protect the learning experience when conditions are imperfect: differing input methods, motion preferences, devices, networks, failures, and content-review needs.

Numeric budgets are intentionally `TBD` until the reference device, browser support policy, asset approach, and prototype measurements are selected. They must be set before public release.

## Quality requirements

| ID | Quality attribute | Requirement | Release evidence |
| --- | --- | --- | --- |
| NFR-01 | Accessibility | Essential learning objectives and controls must be available by keyboard and through documented alternatives to motion, colour-only cues, hover-only behavior, and purely visual explanation. | Keyboard, reduced-motion, colour-independence, and text-alternative tests pass for core journeys. |
| NFR-02 | Performance | The primary lesson must remain responsive and visually stable on the documented reference environment. | Measured loading and interaction results meet approved budgets. |
| NFR-03 | Reliability | Core learning actions must not create crashes, silent state loss, invalid route order, or unrecoverable dead ends. | Critical-path test suite and manual journey tests pass. |
| NFR-04 | Recoverability | Failure messages must be understandable and provide a safe recovery or exit path. | Asset/rendering/network failure simulations pass Journey 5 criteria. |
| NFR-05 | Scientific integrity | Medical claims, labels, visual flows, and simplifications must be traceable and reviewed at the required level. | Source register, review record, and simplification notes are complete. |
| NFR-06 | Privacy | The MVP must not require unnecessary personal data, health information, or identity to complete the core lesson. | Data inventory confirms no unnecessary collection; any analytics are approved and documented. |
| NFR-07 | Security | Public-facing content, dependencies, and configuration must follow a basic secure-development review before release. | Dependency, configuration, and input-handling review is recorded. |
| NFR-08 | Maintainability | Lesson content must be separated from shared behavior at the documented level; changes must be reviewable and testable. | Architecture review demonstrates shared configuration and avoids unexplained duplication. |
| NFR-09 | Compatibility | Supported browser/device classes and fallback behavior must be explicitly documented. | Support matrix and test evidence are published before release. |
| NFR-10 | Observability | Any measurement must answer a defined validation question and respect the privacy boundary. | Approved event plan or a recorded decision to operate without analytics. |

## Accessibility baseline

The MVP’s accessibility standard is outcome equivalence: an alternative does not need to copy the visual presentation, but it must allow the learner to reach the same essential objective.

- Keyboard focus must be visible, logical, and operable for every core action.
- Motion must be pausable and an essential reduced-motion or step-based path must exist.
- Colour cannot be the only expression of flow direction, selection, oxygenation state, or correctness.
- Required annotations cannot depend only on hover.
- Essential visual relationships require concise, purposeful text description.
- Captions or transcripts are required if narration or essential audio is introduced.
- Exact conformance target and testing procedure will be defined in the UX/Accessibility specification before release.

## Performance and support-policy decisions

Before implementation exits prototype stage, the team must approve:

- [ ] Reference device class and minimum supported browser versions.
- [ ] Initial network condition assumptions and loading fallback.
- [ ] Initial loading-time, interaction-latency, memory, and animation-stability budgets.
- [ ] 3D capability detection and non-capable-device fallback behavior.
- [ ] Asset compression, progressive loading, and quality-reduction strategy.

Until these are approved, no performance claim may be made.

## Reliability and recovery expectations

| Situation | Required outcome |
| --- | --- |
| Rapid scroll or repeated step controls | State remains valid and the learner can identify the current stage. |
| Pause/resume during animation | All synchronized educational media resumes from a coherent point. |
| Annotation open during replay or navigation | Behavior is predictable; content closes or persists with clear context. |
| Partial asset failure | Product avoids misleading incomplete representation and offers retry, fallback, return, or exit. |
| Browser/device cannot render the primary scene | Learner receives a plain-language alternative path or an honest support message with safe exit. |
| Page refresh or session interruption | Expected reset/persistence behavior is documented; no silent claim of saved progress. |

## Privacy and measurement rules

- Do not collect personal health information for a foundational anatomy lesson.
- Do not require login to learn the core cardiovascular story.
- Do not use hidden tracking, dark patterns, or engagement metrics as a substitute for learning evaluation.
- If analytics are introduced, define each event’s purpose, data fields, retention, consent/lawful basis as applicable, and disable/fallback behavior.
- Feedback collection must clearly state whether responses are stored and how they will be used.

## Content quality controls

- Every medical claim has a source or is explicitly labelled as a planned teaching simplification pending review.
- Every visual route segment has a medical-content owner/reviewer path.
- Source version and access date are recorded for changeable sources.
- Known limitations are communicated in learner-appropriate language.
- Content changes affecting accuracy trigger medical review before public release.

## Maintainability and documentation controls

- Requirements, lesson content, design, architecture, and tests must cross-reference their governing document IDs.
- The repository must not contain unexplained hardcoded content that is intended to be reusable lesson data.
- A feature is not complete if its acceptance criteria and relevant documentation are stale.
- AI-generated code or content is reviewed against requirements and must not claim unperformed tests or nonexistent sources.

## Open questions

- [ ] What exact accessibility standard and automated/manual testing tools will the project adopt?
- [ ] What supported devices and browsers best match the primary validation group?
- [ ] What basic security review is proportionate for a static MVP versus a future data-collecting platform?
- [ ] Which performance metrics most strongly affect this lesson’s comprehension?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-27 | AnatomIQ Project Team | Initial MVP non-functional requirements. |

## Review checklist

- [x] Accessibility, performance, reliability, recovery, integrity, privacy, security, maintainability, compatibility, and observability are addressed.
- [x] Unknown numeric budgets are explicitly deferred rather than invented.
- [x] Release evidence and pending policy decisions are identified.
- [x] AI Context is complete.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Ensure every MVP implementation supports a reliable, accessible, medically responsible, privacy-respecting learning experience. |
| Constraints | Do not invent performance claims, support coverage, accessibility compliance, source review, security results, or analytics approval. |
| Inputs | This document, Functional Requirements, User Journeys, support policy, test results, and future UX/engineering/medical specifications. |
| Outputs | A quality plan, implementation constraint, test, risk, or release-evidence report mapped to an NFR-ID. |
| Do not assume | That default browser behavior, a 3D library, visual polish, or a passing happy path satisfies these requirements. |
| Validation | Produce the stated release evidence for the applicable NFR and record any gap or approved exception. |
