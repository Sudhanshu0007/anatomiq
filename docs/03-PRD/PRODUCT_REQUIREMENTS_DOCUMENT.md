# AnatomIQ Product Requirements Document

| Field | Value |
| --- | --- |
| Document ID | AQ-PRD-001 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-27 |
| Last updated | 2026-07-27 |
| Review cadence | At each PRD chapter approval, before MVP build approval, and before public release |
| Related documents | [Project Vision](../01-Vision/PROJECT_VISION.md), [Mission](../01-Vision/MISSION.md), [Product Philosophy](../01-Vision/PRODUCT_PHILOSOPHY.md), [Educational Philosophy](../01-Vision/EDUCATIONAL_PHILOSOPHY.md), [Success Criteria](../01-Vision/SUCCESS_CRITERIA.md), [Project Constitution](../00-Constitution/PROJECT_CONSTITUTION.md) |

## Purpose

This Product Requirements Document (PRD) defines what the AnatomIQ cardiovascular MVP must achieve for learners and what conditions must be met before it can be considered ready for public demonstration.

It translates the project’s vision and principles into product requirements without prescribing the final technical implementation. Detailed design, engineering, medical-content, and validation documents will refine this PRD; they must not silently change its approved scope.

## Scope

### In scope

- The problem the cardiovascular MVP addresses.
- Primary learner and educator use cases.
- MVP experience, requirements, constraints, and acceptance criteria.
- Product-level non-functional requirements and risks.
- The planned PRD chapter structure and decision boundaries.

### Out of scope

- Implementing every human body system in the first release.
- Personalized medical advice, diagnostic features, treatment guidance, or clinical decision support.
- A complete clinical simulator, curriculum replacement, or accredited examination platform.
- Final technology choices, database schema, 3D asset specifications, visual design tokens, or API contracts.

## Product summary

AnatomIQ is an interactive anatomy and physiology learning platform. Its first MVP is a learner-controlled cardiovascular lesson that uses a whole-body context, a guided heart-and-circulation journey, annotations, replayable interactions, and formative knowledge checks to help learners understand how blood moves between the body, heart, lungs, and body again.

The MVP is both a learning experience and a platform proof: it must demonstrate a reusable way to define lessons, control a visual sequence, show structures in context, expose explanations, and assess understanding.

## Problem statement

Learners often encounter anatomy and physiology through static diagrams, label lists, fragmented videos, and separate explanations of structure and function. These materials can make it difficult to understand three connected ideas at once:

1. where a structure is located;
2. how it connects to other structures; and
3. what changes over time as a physiological process unfolds.

For circulation specifically, learners may memorize chamber names and vessel names yet still struggle to trace blood flow, distinguish pulmonary from systemic circulation, or explain why the route changes oxygenation state.

The MVP addresses this learning gap with a focused, medically responsible visual story. It does not claim that a 3D experience alone solves anatomy education; it provides a complementary way to build and test a mental model.

## Product hypothesis

If learners can follow a paced, interactive visualization of circulation while receiving context-specific explanations and low-stakes practice, then they will be better able to trace the major route and explain its purpose than after reviewing disconnected labels alone.

This is a hypothesis to validate with appropriate learner research. It is not a guaranteed outcome or a marketing claim.

## Goals

### Primary goals

1. Help a learner form an accurate, high-level mental model of pulmonary and systemic circulation.
2. Give learners control to pause, replay, inspect, and revisit the circulation story.
3. Demonstrate a reusable lesson model that can later support additional body systems.
4. Establish a medically responsible, accessible, and documentation-driven product foundation.

### Secondary goals

- Give educators a clear visual aid for introducing or revising circulation.
- Create an interaction model that feels focused and memorable without distracting from learning.
- Produce an MVP-quality portfolio demonstration of product thinking, 3D interaction, and educational design.

## Non-goals

The MVP will not:

- model every heart structure, vessel branch, cell type, pressure change, disease, or physiological exception;
- simulate patient-specific conditions or provide health advice;
- require account creation, social features, payments, gamified streaks, or a full learning-management system;
- optimize for every browser, device, or assistive technology before a support policy is defined;
- build all eight planned body systems before validating the cardiovascular lesson;
- rely on photorealism as proof of educational value.

## Primary users

### Primary learner: foundational anatomy student

| Attribute | Description |
| --- | --- |
| Typical context | Secondary-school biology, pre-medical preparation, or early health-science study. |
| Need | Understand a circulation sequence that is difficult to infer from static diagrams. |
| Motivation | Prepare for a lesson, examination, revision session, or personal understanding. |
| Constraint | May have limited prior anatomy vocabulary, time, hardware capability, or 3D experience. |
| Success | Can explain the major route, locate the primary structures, and revisit confusing steps confidently. |

### Secondary user: educator

| Attribute | Description |
| --- | --- |
| Typical context | Classroom, tutoring, group study, or lecture support. |
| Need | Make circulation visible while retaining control over pace and explanation. |
| Motivation | Use a shared visual model to supplement—not replace—teaching material. |
| Constraint | Needs predictable controls, trustworthy scope, and a lesson that does not require lengthy setup. |
| Success | Can orient learners, pause at a meaningful step, explain the model, and direct follow-up discussion. |

## User needs

| Need ID | User need | Product response |
| --- | --- | --- |
| UN-01 | “Show me where the heart and lungs sit in the body.” | Begin with whole-body or thoracic context and a clear system orientation. |
| UN-02 | “Show me the order blood follows.” | Present a guided, directional circulation sequence with clear step boundaries. |
| UN-03 | “Let me stop and look again.” | Provide pause, replay, reset, and predictable step navigation. |
| UN-04 | “Tell me what I am looking at and why it matters.” | Use contextual annotations and concise explanations tied to the visible structure or event. |
| UN-05 | “Help me know whether I understand it.” | Provide objective-aligned formative questions and explanatory feedback. |
| UN-06 | “Do not make me depend on motion, colour, or a mouse to learn.” | Provide accessible controls, non-colour cues, and reduced-motion alternatives. |
| UN-07 | “Do not mislead me into thinking this is medical advice.” | State educational scope and relevant simplifications clearly. |

## MVP experience overview

The MVP experience has six learner-facing phases.

```mermaid
flowchart LR
  A[Entry and orientation] --> B[Whole-body system context]
  B --> C[Guided circulation story]
  C --> D[Contextual exploration]
  D --> E[Knowledge check]
  E --> F[Summary and replay]
```

### Phase 1 — Entry and orientation

The learner understands that they are entering an educational cardiovascular experience, sees the main learning objective, and can start with an appropriate level of context.

### Phase 2 — Whole-body system context

The learner sees a simplified human-body view that locates the heart, lungs, and the broad circulatory system. The system establishes a spatial frame before focusing on detail.

### Phase 3 — Guided circulation story

The learner follows the major route of blood through the right side of the heart, lungs, left side of the heart, systemic circulation, and return pathway. The experience makes direction, oxygenation state, and primary structure roles understandable at the MVP’s chosen level.

### Phase 4 — Contextual exploration

At appropriate points, the learner can inspect selected structures, read or hear concise annotations, and revisit a scene. Exploration supplements the primary story; it must not make the main route harder to follow.

### Phase 5 — Knowledge check

The learner completes low-stakes, lesson-aligned questions. Feedback identifies the correct reasoning and offers a route back to the relevant step.

### Phase 6 — Summary and replay

The learner receives a concise recap of the route and can replay the journey or revisit a specific section. Completion is not framed as medical competence or formal assessment.

## MVP functional requirements

The terms **must**, **should**, and **may** follow the definitions in the Documentation Standards Manual.

### FR-01: Lesson entry and orientation

| Requirement | Priority | Acceptance criteria |
| --- | --- | --- |
| The product must identify the lesson title, target learner level, and primary learning objective before the main journey begins. | Must | A learner can state the lesson topic and expected takeaway from the entry view. |
| The product must state that the experience is educational and not medical advice. | Must | The scope statement is visible or accessible before or during entry. |
| The product should provide a brief explanation of primary controls. | Should | A first-time learner can discover pause, replay, and navigation without outside instruction. |

### FR-02: Whole-body orientation

| Requirement | Priority | Acceptance criteria |
| --- | --- | --- |
| The product must show the heart and lungs in a comprehensible body context before the learner enters the focused circulation sequence. | Must | The learner can identify the broad location of the heart and lungs. |
| The product must make the active system clear. | Must | System title and visual focus remain unambiguous. |
| The product should allow a learner to return to a broader contextual view. | Should | The return action preserves or clearly communicates lesson progress. |

### FR-03: Guided circulation sequence

| Requirement | Priority | Acceptance criteria |
| --- | --- | --- |
| The lesson must represent the major route of deoxygenated blood from the body to the lungs through the right side of the heart. | Must | The learner can identify the order of major route segments taught by the lesson. |
| The lesson must represent the major route of oxygenated blood from the lungs through the left side of the heart to the body. | Must | The learner can identify the order and direction of the systemic route taught by the lesson. |
| The lesson must distinguish pulmonary and systemic circulation at the intended learner level. | Must | A learner can explain the broad purpose of each circuit after completion. |
| The lesson must communicate flow direction with more than colour alone. | Must | Direction remains understandable in grayscale or reduced-colour viewing. |
| The lesson must disclose meaningful anatomical or physiological simplifications. | Must | A learner can access a concise limitation or simplification statement where relevant. |
| The lesson should introduce terminology progressively rather than displaying all labels at once. | Should | The primary sequence remains readable at every step. |

### FR-04: Playback and lesson navigation

| Requirement | Priority | Acceptance criteria |
| --- | --- | --- |
| Learners must be able to pause a time-based sequence. | Must | Pause freezes visual movement, camera motion, and synchronized narration or effects without resetting the current step. |
| Learners must be able to replay the current sequence or restart the lesson. | Must | Replay and reset restore a predictable state without errors. |
| Learners must be able to identify their current lesson step and progress. | Must | Current position is visually and programmatically available. |
| Learners should be able to revisit completed major steps directly. | Should | Direct revisit does not corrupt state or create misleading route order. |
| The product must handle rapid scrolling or repeated controls safely. | Must | The experience remains stable, coherent, and recoverable. |

### FR-05: Annotations and contextual explanation

| Requirement | Priority | Acceptance criteria |
| --- | --- | --- |
| The lesson must identify the primary structures required for its learning objectives. | Must | Required annotations display correct names and are associated with the right visible structure. |
| Each required annotation must provide a concise function or relevance statement. | Must | Labels are not presented as names alone. |
| The product should provide optional deeper detail without obscuring the primary story. | Should | A learner can open and dismiss details without losing the current step. |
| Annotations must be usable without hover-only input. | Must | Keyboard or equivalent controls can access required annotation content. |

### FR-06: Formative knowledge checks

| Requirement | Priority | Acceptance criteria |
| --- | --- | --- |
| The lesson must include formative checks aligned with stated learning objectives. | Must | Each question maps to one or more outcome IDs in this PRD. |
| Feedback must explain the relevant reasoning. | Must | A wrong answer receives more than a correctness marker. |
| Learners must be able to revisit relevant lesson content after feedback. | Must | Feedback includes a clear review or replay path. |
| The product must not present quiz results as clinical or academic certification. | Must | Completion language makes the formative scope clear. |

### FR-07: Accessibility and learner control

| Requirement | Priority | Acceptance criteria |
| --- | --- | --- |
| Core controls must support keyboard operation. | Must | A keyboard-only learner can begin, pause, navigate, replay, access required annotations, and complete a knowledge check. |
| The product must provide a reduced-motion path for essential lesson content. | Must | A learner can understand the major sequence without continuous or forced motion. |
| The product must not communicate required meaning through colour alone. | Must | State and flow meaning also use direction, labels, patterns, position, or text. |
| The product must expose readable text alternatives for essential visual information. | Must | Required concepts remain available outside the primary 3D representation. |
| The product should preserve settings or clearly state when they reset. | Should | Learner control preferences behave predictably in a session. |

### FR-08: Error handling and support

| Requirement | Priority | Acceptance criteria |
| --- | --- | --- |
| The product must give a clear recovery action when a critical lesson asset or view cannot load. | Must | The learner receives an understandable message and can retry, continue with an alternative, or return safely. |
| The product must not lose the learner’s lesson context during a recoverable error. | Must | Recovery returns to the active lesson or clearly restarts with notice. |
| The product should expose concise help for controls and lesson scope. | Should | A learner can find help without leaving the experience. |

## Product-level non-functional requirements

Detailed budgets and test methods will be defined in Engineering, Design, and Accessibility specifications. These requirements establish the product expectation now.

| ID | Requirement | Priority | Acceptance principle |
| --- | --- | --- | --- |
| NFR-01 | Performance | Must | The primary lesson is responsive and visually stable on the documented reference environment. |
| NFR-02 | Reliability | Must | Core learner actions do not cause crashes, unrecoverable state, or misleading progression. |
| NFR-03 | Accessibility | Must | Essential learning tasks are supported through the approved accessibility path. |
| NFR-04 | Scientific integrity | Must | Medical claims, labels, flows, and simplifications are reviewed and traceable. |
| NFR-05 | Privacy | Must | The MVP does not require unnecessary personal data or health information. |
| NFR-06 | Security | Should | The public experience avoids obvious risks from untrusted content, dependencies, and configuration. |
| NFR-07 | Maintainability | Must | Shared lesson behavior and lesson content follow the documented architecture and can be changed safely. |
| NFR-08 | Observability | Should | Validation-relevant product events can be measured in a privacy-respecting way once analytics are approved. |
| NFR-09 | Compatibility | Must | Supported browsers, devices, and fallback behavior are explicitly documented before release. |

## User stories

| ID | User story | Priority |
| --- | --- | --- |
| US-01 | As a learner new to circulation, I want to see where the heart and lungs are before I follow blood flow, so that the route has spatial meaning. | Must |
| US-02 | As a learner, I want the lesson to show one understandable flow step at a time, so that I do not lose track of the route. | Must |
| US-03 | As a learner, I want to pause and replay a step, so that I can learn at my own pace. | Must |
| US-04 | As a learner, I want to inspect primary structures and learn their function, so that labels become meaningful. | Must |
| US-05 | As a learner, I want feedback after a knowledge check, so that I know how to correct a misunderstanding. | Must |
| US-06 | As a keyboard or reduced-motion user, I want an equivalent way to complete the essential lesson, so that visual interaction is not a barrier. | Must |
| US-07 | As an educator, I want to pause and revisit a circulation stage, so that I can explain the process to a group. | Should |
| US-08 | As a future content author, I want the circulation lesson to use reusable patterns, so that a later body-system lesson does not require copying its implementation. | Must |

## Prioritization

| Tier | Meaning | Included MVP examples |
| --- | --- | --- |
| Must | Required to prove the core learning journey responsibly. | Orientation, major circulation route, step-based flow, pause/replay, primary annotations, formative check, essential accessibility path, error recovery. |
| Should | Valuable if it does not compromise Must scope or quality. | Direct revisit of completed steps, deeper optional details, educator-friendly controls, privacy-preserving validation events. |
| Could | Helpful future enhancement after MVP validation. | Search, pronunciation, multiple learner levels, advanced comparison views, clinical context panels. |
| Won’t (MVP) | Explicitly deferred. | All body systems, pathology simulations, AI tutor, accounts, social features, payments, full curriculum mapping, VR mode. |

## Assumptions

| ID | Assumption | Risk if false | Validation approach |
| --- | --- | --- | --- |
| A-01 | A focused cardiovascular story is meaningful to target learners. | The MVP may not address a high-priority learning gap. | Interview learners and educators before scope lock. |
| A-02 | A visual sequence plus formative practice can improve comprehension versus disconnected explanation alone. | The interaction may add effort without learning value. | Use task-based learner validation. |
| A-03 | The project can obtain appropriate source material and review for MVP content. | Medical integrity gate cannot be met. | Identify sources and review path early. |
| A-04 | The target experience can run on a realistic supported baseline. | The product excludes intended users or becomes unstable. | Define reference environment and prototype early. |
| A-05 | The lesson model can be separated from one-off visual logic. | The MVP becomes a demo rather than a platform proof. | Review architecture during implementation. |

## Dependencies

| Dependency | Why it matters | Owner / status |
| --- | --- | --- |
| Medical-content source and review process | Validates anatomy, physiology, labels, and simplifications. | TBD |
| Learner and educator validation plan | Tests the product hypothesis and usability. | TBD |
| Design and accessibility specification | Defines controls, readability, motion, and alternative paths. | Future PRD/UX work |
| Engineering architecture | Defines lesson data, rendering, state, performance, and recovery behavior. | Future engineering work |
| 3D assets and asset-license policy | Enables visual representation without rights or performance issues. | TBD |
| Support policy | Defines browsers, devices, network conditions, and fallback expectations. | TBD |

## Risks and mitigations

| Risk | Impact | Mitigation |
| --- | --- | --- |
| Scope expands to all systems before MVP validation | Delayed delivery and reduced quality | Maintain Must/Should/Could/Won’t boundaries; require PRD change approval. |
| Visual complexity confuses learners | Reduced learning value | Test comprehension, reveal detail progressively, prioritize clear cues. |
| Medical inaccuracies or oversimplifications | Loss of trust and possible harm | Source claims, document simplifications, obtain appropriate review. |
| 3D performance excludes learner devices | Accessibility and usability failure | Define reference devices, progressive loading, fallbacks, and budgets. |
| Scroll-driven design removes learner agency | Disorientation and inaccessible experience | Require pause, replay, step state, navigation, and reduced-motion path. |
| Accessibility is deferred | Core users cannot access the lesson | Treat accessibility as a release gate from the first prototype. |
| AI-generated content introduces errors | Scientific or product-quality failure | Apply human review, source checks, and documented acceptance criteria. |
| Reusable engine is overdesigned before validation | Unnecessary complexity | Build only the abstractions demonstrated by the cardiovascular MVP. |

## PRD chapter plan

This master document is the entry point. The following focused documents will be created as Milestone 2 proceeds.

| Planned document | Purpose |
| --- | --- |
| `USER_PERSONAS.md` | Detailed personas, needs, contexts, accessibility considerations, and jobs to be done. |
| `USER_JOURNEYS.md` | End-to-end learner and educator flows, including errors and accessibility paths. |
| `MVP_SCOPE.md` | Definitive MVP boundaries, requirements mapping, feature priority, and release slices. |
| `FUNCTIONAL_REQUIREMENTS.md` | Expanded behavior specifications and acceptance criteria for every MVP capability. |
| `NON_FUNCTIONAL_REQUIREMENTS.md` | Performance, accessibility, reliability, privacy, compatibility, and quality requirements. |
| `CONTENT_AND_LESSON_REQUIREMENTS.md` | Lesson structure, medical-content handoff, annotations, assessments, and review process. |
| `RELEASE_AND_VALIDATION_PLAN.md` | Prototype, validation, release-gate, feedback, and iteration plan. |
| `RISKS_AND_ASSUMPTIONS.md` | Maintained risk register and assumption log. |

## Decisions required before implementation

- [ ] Name the primary learner segment for MVP validation.
- [ ] Define the initial support policy: browsers, device class, network assumptions, and fallback path.
- [ ] Confirm the medical-source and reviewer pathway for circulation content.
- [ ] Approve the exact cardiovascular learning-objective depth and list of structures in scope.
- [ ] Decide whether a first public version is educator-led, self-guided, or both.
- [ ] Define the privacy boundary for analytics and feedback collection.

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-27 | AnatomIQ Project Team | Initial master PRD and cardiovascular MVP requirements draft. |

## Review checklist

- [x] Problem, hypothesis, goals, non-goals, and intended users are defined.
- [x] Cardiovascular MVP experience and functional requirements are specified.
- [x] Product-level non-functional requirements, user stories, priorities, dependencies, risks, and assumptions are included.
- [x] MVP scope deliberately excludes premature platform expansion.
- [x] PRD chapter plan and implementation-blocking decisions are identified.
- [x] AI Context is complete.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Plan, design, implement, or validate the AnatomIQ cardiovascular MVP as a learner-controlled, medically responsible, reusable circulation lesson. |
| Constraints | Stay within MVP scope; preserve learning objectives, scientific integrity, accessibility, learner agency, privacy, performance, and documentation-first workflow. Treat Must requirements and release gates as non-negotiable unless an approved exception exists. |
| Inputs | This PRD; linked Vision documents; Project Constitution; and the relevant future UX, design, engineering, medical, and validation specifications. |
| Outputs | A focused requirement, design, task, implementation, test plan, or validation report mapped to a requirement ID, user need, or learner outcome. |
| Do not assume | All body systems, pathology simulations, medical review, analytics, support policy, detailed anatomy scope, or implementation technology are approved. Do not invent evidence, sources, numeric targets, or acceptance results. |
| Validation | Verify the work maps to an in-scope requirement, preserves the primary circulation journey, meets applicable release gates, identifies dependencies and assumptions, and documents any exception or unresolved decision. |
