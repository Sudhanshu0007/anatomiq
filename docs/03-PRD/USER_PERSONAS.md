# AnatomIQ User Personas

| Field | Value |
| --- | --- |
| Document ID | AQ-PRD-002 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-27 |
| Last updated | 2026-07-27 |
| Review cadence | Before learner validation, MVP scope lock, and each major target-audience change |
| Related documents | [Product Requirements Document](PRODUCT_REQUIREMENTS_DOCUMENT.md), [Project Vision](../01-Vision/PROJECT_VISION.md), [Educational Philosophy](../01-Vision/EDUCATIONAL_PHILOSOPHY.md), [Success Criteria](../01-Vision/SUCCESS_CRITERIA.md) |

## Purpose

This document defines the provisional user personas for AnatomIQ’s cardiovascular MVP. Personas make target learners, educators, their goals, and their constraints concrete enough to guide scope, journey, interaction, content, and validation decisions.

These personas are working hypotheses, not market research or demographic claims. They must be validated and revised through interviews, observation, accessibility review, and learner testing before being treated as authoritative.

## Scope

### In scope

- Primary and secondary learner personas for the cardiovascular MVP.
- An educator persona whose needs affect facilitation and classroom use.
- Accessibility and context-of-use considerations.
- Jobs to be done, needs, pain points, and success signals.
- Research questions that must validate or revise the personas.

### Out of scope

- Personas for every future body system or paid product tier.
- Individual medical histories, diagnosis, or health data.
- Claims about the size, behavior, or purchasing power of any audience.
- A substitute for recruiting and testing with real representative learners.

## Persona design principles

1. A persona represents a recurring learning context and need, not a stereotype.
2. Needs, constraints, and desired outcomes matter more than age, country, or device alone.
3. Accessibility is a normal product context, not a separate edge case.
4. The MVP may optimize for one primary persona while remaining respectful and usable for others.
5. Every persona statement marked as an assumption requires validation before it drives a high-cost decision.

## Persona summary

| Persona | Role in MVP | Primary job | Product priority |
| --- | --- | --- | --- |
| Aarav — foundational anatomy learner | Primary | Build a correct mental model of blood circulation for study and revision. | Must optimize |
| Maya — early health-science learner | Secondary | Connect lecture terminology to structure-function relationships. | Must support |
| Priya — educator and facilitator | Secondary | Explain circulation to a group while controlling pace and focus. | Should support |
| Sam — learner using accessibility alternatives | Cross-cutting | Access the same essential circulation concepts without depending on continuous motion, colour, or pointer-only input. | Must support |

The names are fictional labels used only to make the profiles memorable. They do not imply a fixed identity, region, gender, or background.

## Primary persona — Aarav, foundational anatomy learner

### Snapshot

| Attribute | Provisional profile |
| --- | --- |
| Learning context | Secondary-school biology, entrance-exam preparation, or early self-directed anatomy study. |
| Prior knowledge | Recognizes broad terms such as heart, lungs, arteries, and veins; may not reliably trace circulation or explain pulmonary versus systemic routes. |
| Typical device context | Often uses a personal laptop or mobile device; may have uneven internet speed and no prior experience with 3D interfaces. |
| Time available | Short revision sessions before or after classes, with occasional longer study time. |
| Motivation | Wants to understand the concept well enough to answer questions, revise efficiently, and feel less intimidated by anatomy. |

### Core job to be done

> When a diagram or textbook explanation leaves circulation confusing, help me see the route and understand why each stage follows the next, so that I can explain it without only memorizing a list of names.

### Goals

- Locate the heart and lungs in a body context.
- Follow the major route of blood in the correct direction.
- Distinguish the broad role of the right and left sides of the heart.
- Understand the relationship between the lungs, oxygenation, and systemic circulation.
- Pause and repeat difficult parts without starting from the beginning.

### Pain points

- Static diagrams show many labels at once and make the route hard to follow.
- Terms such as pulmonary artery and pulmonary vein can seem contradictory when learned as isolated facts.
- A video may move too fast or prevent inspection of a structure at the moment it matters.
- A complex 3D interface can be intimidating if controls are unexplained.
- The learner may confuse colour conventions with the actual definitions of arteries and veins.

### Product requirements implied by this persona

- Establish orientation before detail.
- Introduce terminology progressively and attach it to visible function.
- Make flow direction explicit through arrows, sequence, labels, position, or other non-colour cues.
- Provide pause, replay, progress state, and direct review paths.
- Keep entry low-friction and do not require an account for core learning.
- Use concise explanations first, with deeper content available on demand.

### Success evidence

After the lesson, Aarav can:

- trace the taught major circulation route in the correct broad order;
- explain why blood travels to the lungs and then returns to the heart;
- distinguish the primary taught role of arteries, veins, and capillaries;
- locate a relevant explanation or replay point without help.

### Assumptions to validate

- [ ] Learners at this level prefer a guided story before a free-exploration mode.
- [ ] The chosen vocabulary level is understandable without a glossary-first approach.
- [ ] A laptop-first experience is appropriate for the primary validation setting.
- [ ] The lesson can fit meaningfully into a short study session without oversimplifying the model.

## Secondary persona — Maya, early health-science learner

### Snapshot

| Attribute | Provisional profile |
| --- | --- |
| Learning context | Early undergraduate nursing, physiotherapy, allied-health, or other health-science study. |
| Prior knowledge | Has encountered formal anatomy terminology and basic circulation but needs stronger spatial and causal integration. |
| Typical device context | Uses a laptop for study, often alongside lecture slides, notes, a textbook, or laboratory material. |
| Motivation | Wants a trustworthy supplement that makes lecture concepts easier to visualize and revisit. |

### Core job to be done

> When I know the names of structures but cannot picture how they operate together, help me connect terminology, location, direction, and function so that I can reason through a process instead of reciting it.

### Goals

- Review circulation efficiently before or after a lecture.
- Link chambers, valves, major vessels, and lungs to the route of blood.
- Use the lesson to identify a misunderstanding before an assessment or practical session.
- Access enough contextual detail to reinforce formal study without turning the lesson into an exhaustive atlas.

### Pain points

- Lecture material may alternate between high-level diagrams and terminology-heavy detail without a visual bridge.
- Existing 3D viewers may show structure but not the temporal process or explanation.
- Simplified resources may omit distinctions that matter to formal study.
- Learner trust falls if sources, limits, and simplifications are unclear.

### Product requirements implied by this persona

- State the lesson’s level, scope, and simplified model clearly.
- Pair concise core explanations with optional deeper annotations.
- Keep route, structure, and function connected at each lesson stage.
- Provide medically traceable content and avoid unsupported clinical extensions.
- Make replay and targeted step review efficient rather than forcing a full restart.

### Success evidence

After the lesson, Maya can:

- explain the major route using appropriate taught terminology;
- identify which details were intentionally simplified;
- use the lesson to resolve a specific lecture-related confusion;
- distinguish the platform’s educational model from a complete clinical simulation.

### Assumptions to validate

- [ ] Optional deeper detail is sufficient for this learner group in the MVP.
- [ ] The same core lesson can support Maya without creating a separate advanced experience.
- [ ] Content-source transparency affects trust and adoption for this group.

## Secondary persona — Priya, educator and facilitator

### Snapshot

| Attribute | Provisional profile |
| --- | --- |
| Teaching context | Biology classroom, tutoring session, introductory lecture, or small-group revision. |
| Prior knowledge | Comfortable explaining basic circulation and selecting supplementary material. |
| Typical device context | Classroom display, shared laptop, projector, or guided group session. |
| Motivation | Make an abstract process visible, pace explanation around learner questions, and supplement existing teaching materials. |

### Core job to be done

> When I introduce or revisit circulation with a group, give me a trustworthy visual model that I can pause, replay, and discuss so that learners can follow the sequence together.

### Goals

- Start the lesson quickly with clear scope and controls.
- Pause at meaningful stages and explain what learners are seeing.
- Revisit a previous step when a question arises.
- Use a knowledge check as a discussion prompt, not only an individual test.
- Know the lesson’s intended level, sources, and limitations.

### Pain points

- Video content can move at a fixed pace and be difficult to inspect.
- Complex interactive tools may be unreliable or require too much setup in a teaching session.
- Unclear medical accuracy or scope creates risk for an educator.
- A visually busy scene may not work on a projector or for a group sitting far from the display.

### Product requirements implied by this persona

- Controls must be visible, reliable, and understandable without a tutorial-heavy setup.
- Pause, replay, reset, and major-step navigation must work predictably.
- Text and annotations must remain readable in a shared-display context.
- The lesson must identify its objectives, level, scope, and meaningful simplifications.
- Core value must not depend on one learner’s personal account or saved state.

### Success evidence

Priya can:

- begin and control the primary lesson flow without technical assistance;
- pause at a selected point and explain the taught concept to a group;
- answer a learner’s request to revisit a route segment;
- identify what the lesson is designed to teach and what it does not cover.

### Assumptions to validate

- [ ] Educators will use the MVP as a supplement rather than requiring a full teacher dashboard.
- [ ] A single self-guided interface can support group facilitation with limited additional controls.
- [ ] Projected readability can be met without a dedicated presentation mode in the MVP.

## Cross-cutting persona — Sam, learner using accessibility alternatives

### Snapshot

Sam represents learners whose access to the experience depends on alternative input, reduced-motion settings, non-colour cues, readable text, captions, assistive technology, or a combination of these. Sam is not one uniform type of learner; the persona prevents the team from treating accessibility as a later add-on.

### Core job to be done

> When the lesson uses movement, 3D visuals, colour, or pointer interactions, give me an equivalent way to understand and control the essential circulation concept so that I can complete the same learning objective.

### Potential contexts to design and test for

- Keyboard-only navigation or switch-like input.
- Reduced-motion preference, vestibular sensitivity, migraine triggers, or attention needs that make continuous camera movement difficult.
- Colour-vision differences or grayscale viewing.
- Screen-reader use or a need for text-based descriptions of essential visual information.
- Low vision, magnification, and contrast needs.
- Temporary constraints such as a broken mouse, small screen, slow connection, or noisy environment.

### Product requirements implied by this persona

- Essential lesson controls must be keyboard-operable with visible focus.
- Flow meaning must not depend on red/blue colour alone.
- Essential sequence meaning must remain available in a reduced-motion or step-based mode.
- Required annotations must not be hover-only.
- Essential visual concepts require readable text alternatives or descriptions aligned with the lesson objective.
- Accessibility paths must be tested as first-class flows, not assumed to work because controls exist.

### Success evidence

Sam can:

- start, pause, navigate, replay, access annotations, and complete the knowledge check through supported alternatives;
- understand the taught route and oxygenation-state change without depending solely on motion or colour;
- recover from a control or loading problem without losing the lesson.

### Assumptions to validate

- [ ] The chosen alternatives preserve enough spatial and temporal meaning for the MVP learning objectives.
- [ ] Keyboard and reduced-motion testing will reveal the highest-priority barriers early enough to correct them.
- [ ] The initial 3D approach can be made compatible with the project’s accessibility commitments.

## Shared jobs to be done

| Job ID | Job statement | Primary personas |
| --- | --- | --- |
| JTBD-01 | When circulation feels like a list of facts, help me see it as a route with purpose so that I can explain the sequence. | Aarav, Maya, Sam |
| JTBD-02 | When a visual sequence moves too quickly or becomes confusing, let me control the pace and revisit the relevant point. | Aarav, Maya, Priya, Sam |
| JTBD-03 | When I see a structure, explain what it does in the current process so that terminology has meaning. | Aarav, Maya, Sam |
| JTBD-04 | When I am unsure whether I understand, give me low-stakes feedback tied to the exact concept I need to review. | Aarav, Maya, Sam |
| JTBD-05 | When I teach or discuss the process with others, let me control the visual model and return to earlier steps reliably. | Priya |

## Design implications by persona

| Product area | Aarav | Maya | Priya | Sam |
| --- | --- | --- | --- | --- |
| Entry | Simple, low-jargon objective and control hint | State level and scope | Fast start and lesson overview | Clear keyboard and reduced-motion access |
| Story pacing | Strong guided progression | Direct review of selected steps | Pause and group discussion | Step-based alternative, no forced motion |
| Content depth | Concise default with definitions | Optional deeper context | Clear teaching prompts and limits | Textual equivalent of essential concepts |
| Navigation | Obvious progress and replay | Efficient return to a concept | Predictable controls on a shared screen | Keyboard focus and non-hover access |
| Assessment | Low-stakes, explanatory feedback | Reasoning-oriented checks | Discussion-ready prompts | Equivalent operable question formats |

## Anti-personas and explicit exclusions

An anti-persona clarifies whom the MVP is not designed to serve as its primary solution.

| Anti-persona | Why the MVP is not designed for this use |
| --- | --- |
| Clinician seeking patient-specific guidance | AnatomIQ is educational and must not diagnose, triage, or prescribe. |
| Specialist seeking a complete surgical or diagnostic simulator | The MVP teaches foundational circulation, not high-fidelity clinical procedure or imaging interpretation. |
| Learner seeking an exhaustive atlas of every structure | The MVP intentionally teaches a bounded circulation model. |
| User seeking unrestricted free-form 3D modeling | AnatomIQ is a guided educational experience, not a general-purpose anatomy model editor. |

## Persona validation plan

Before locking the MVP scope, the team should seek lightweight evidence from representative learners and at least one educator.

| Question | Method | Evidence needed |
| --- | --- | --- |
| Is the circulation route a meaningful and difficult learning problem for the primary learner? | Short interview and pre-task | Repeated descriptions of confusion or a demonstrated gap. |
| Does the proposed vocabulary level fit the learner? | Think-aloud lesson review | Learners understand the sequence without unexplained terms blocking progress. |
| Do learners prefer or benefit from guided progression, exploration, or a blend? | Prototype comparison or moderated session | Observed ability to complete objectives and explain why. |
| Can educators use the controls in a teaching context? | Facilitated walkthrough | Educator can start, pause, replay, and explain without rescue. |
| Do accessibility alternatives preserve the learning outcome? | Keyboard, reduced-motion, and assistive-technology checks with relevant users where possible | Essential tasks are completed and concept understanding remains available. |

## Open questions

- [ ] Which persona is the first validation priority: secondary-school learner, entrance-exam learner, or early health-science learner?
- [ ] What regional curricula, language preferences, or access constraints should influence the initial learner model?
- [ ] Which accessibility experiences can be directly tested before the first public prototype?
- [ ] Should the educator flow be a first-MVP requirement or a validation-only use case?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- |
| 0.1.0 | 2026-07-27 | AnatomIQ Project Team | Initial provisional MVP personas and validation plan. |

## Review checklist

- [x] Primary, secondary, educator, and cross-cutting accessibility personas are defined.
- [x] Personas focus on learning context, goals, constraints, and jobs rather than stereotypes.
- [x] Product implications and success evidence are specified for each persona.
- [x] Anti-personas prevent scope drift into clinical or specialist simulation use cases.
- [x] Assumptions and validation questions are explicit.
- [x] AI Context is complete.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Use these personas to make the cardiovascular MVP understandable for foundational learners, useful for early health-science learners and educators, and accessible through equivalent core paths. |
| Constraints | Treat personas as provisional hypotheses; do not invent demographics, research findings, medical needs, or accessibility compliance. Do not design for anti-persona use cases without an approved scope change. |
| Inputs | This document, the master PRD, Product and Educational Philosophy, user-research findings, and relevant accessibility requirements. |
| Outputs | A user journey, feature requirement, interface decision, test plan, or validation question that names the persona, job to be done, and desired learner outcome. |
| Do not assume | That one interaction style works for every learner, that device ownership guarantees access, or that a fictional persona represents all learners in a group. |
| Validation | Confirm the design solves a named persona need, supports the primary learner without excluding Sam’s essential path, and identifies assumptions that need evidence. |
