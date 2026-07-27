# AnatomIQ Mission

| Field | Value |
| --- | --- |
| Document ID | AQ-MIS-001 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-27 |
| Last updated | 2026-07-27 |
| Review cadence | Before MVP scope approval and each major product release |
| Related documents | [Project Vision](PROJECT_VISION.md), [Project Constitution](../00-Constitution/PROJECT_CONSTITUTION.md) |

## Purpose

This document states what AnatomIQ commits to do now and over time. While the Project Vision describes the future AnatomIQ seeks to create, this Mission defines the product’s practical purpose, the people it serves, and the standards that shape daily prioritization.

## Scope

### In scope

- The mission statement and its supporting commitments.
- The learner value AnatomIQ is responsible for delivering.
- Decision criteria for product, content, and experience choices.

### Out of scope

- Feature-level requirements and release commitments.
- Revenue, organizational structure, or implementation technology.
- Medical diagnosis, treatment, or personalized healthcare guidance.

## Mission statement

**AnatomIQ makes human anatomy and physiology easier to understand by giving learners accurate, interactive, and accessible ways to explore how body structures relate and function together.**

We translate complex biological systems into learner-controlled visual journeys that connect location, process, vocabulary, and meaning—without sacrificing scientific integrity or treating the learner as a passive viewer.

## Who we serve

AnatomIQ serves people who need to build or strengthen a mental model of the human body, especially when static diagrams and disconnected explanations are not enough.

| Group | What AnatomIQ helps them do |
| --- | --- |
| Biology learners | Visualize foundational concepts and connect terminology to real structure and function. |
| Pre-medical learners | Understand sequences and relationships needed for later study and assessment. |
| Health-science learners | Reinforce lectures, laboratory study, and textbook learning with a navigable visual model. |
| Educators | Explain difficult processes in a shared, controllable visual environment. |
| Independent learners | Explore reliable foundational anatomy at a self-directed pace. |

The mission does not promise equal depth for every audience in every release. It commits the project to make audience, level, and limitations explicit.

## How AnatomIQ creates value

### Turn abstractions into observable relationships

AnatomIQ shows anatomical structures in spatial context and physiological events in sequence. A learner should be able to see how a chamber, valve, vessel, organ, nerve, or tissue relates to its role in a larger system.

### Turn observation into understanding

The product combines guided explanation with meaningful interaction, such as pausing, replaying, inspecting annotations, predicting an outcome, and checking comprehension. Interaction must help a learner reason, not merely produce activity.

### Turn complexity into a path learners can follow

The experience begins with orientation and introduces complexity progressively. It should make difficult material approachable without hiding important caveats or presenting simplified models as complete reality.

### Turn medical information into trustworthy educational content

AnatomIQ uses traceable sources, appropriate review, transparent scope, and careful wording. It makes no claim to diagnose, prescribe, or replace professional learning or care.

## Mission commitments

### 1. Make every lesson purposeful

Each lesson begins with explicit learning objectives and ends with a meaningful way for the learner to confirm or revisit their understanding. Content that cannot explain its learning purpose does not belong in the core experience.

### 2. Teach systems, not disconnected facts

Where possible, show cause, effect, direction, timing, and relationship. A correct label alone is not sufficient when a learner also needs to understand what the structure does in the system.

### 3. Protect scientific accuracy

Use medically responsible language, indicate simplifications, and require evidence or qualified review for medical claims. When accuracy and dramatic presentation conflict, accuracy wins.

### 4. Respect different learners

Provide learner control, clear navigation, accessible alternatives, and a progressive path through complexity. Do not require a particular device, movement tolerance, or prior knowledge to access essential concepts.

### 5. Build capabilities that scale across systems

The cardiovascular MVP is a focused proof point. Shared lesson, annotation, camera, interaction, assessment, and content capabilities should make it easier—not harder—to teach another body system accurately.

### 6. Be transparent about limitations

State what a lesson covers, what it simplifies, and what it does not provide. Never confuse a visualization with clinical reality, a learning check with competency assessment, or a planned feature with a released one.

## Everyday prioritization guide

When choosing between valid pieces of work, prioritize the item that best satisfies the following order:

1. Removes a meaningful learner misunderstanding.
2. Strengthens accuracy, accessibility, safety, or trust.
3. Completes the end-to-end cardiovascular MVP learning journey.
4. Creates a reusable capability for future body-system lessons.
5. Improves reliability, performance, or maintainability.
6. Improves visual polish after the learning need is already met.

The team should decline or defer work that is impressive but does not provide demonstrated educational value, creates unreviewed medical claims, excludes learners, or locks the project into one-off implementation.

## Mission in practice

| Situation | Mission-aligned response |
| --- | --- |
| A heart animation looks impressive but hides valve timing | Simplify or redesign it until the relevant sequence is understandable. |
| A learner cannot tolerate continuous camera movement | Offer reduced-motion and step-based alternatives that preserve the learning objective. |
| A contributor proposes a new body system | Define its learning objectives and reuse the lesson model before building custom interactions. |
| A feature suggests a disease outcome | Require an appropriately scoped source, review path, limitation statement, and non-diagnostic framing. |
| A visual decision increases load time or unstable frame rate | Apply a performance budget, progressive loading, or a lower-cost representation. |

## What success looks like

AnatomIQ is fulfilling its mission when learners can explain a process more clearly after interacting with a lesson, educators can integrate it as a trustworthy supplement, and the project can grow its content without weakening accuracy, accessibility, or maintainability.

Specific measurable outcomes are defined in the forthcoming Success Criteria and Product Requirements documents. The mission acts as the qualitative standard behind those measures.

## Open questions

- [ ] What level of reading and scientific vocabulary will the cardiovascular MVP assume by default?
- [ ] Which accessibility accommodations must be validated with representative learners before a public MVP demonstration?
- [ ] What evidence threshold should be required before claiming an improvement in learner understanding?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-27 | AnatomIQ Project Team | Initial mission draft. |

## Review checklist

- [x] Mission statement distinguishes current commitment from long-term vision.
- [x] Intended learners and the value delivered to them are defined.
- [x] Commitments align with the Project Constitution.
- [x] A practical prioritization guide and examples are included.
- [x] Limitations and non-clinical boundaries are explicit.
- [x] AI Context is complete.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Use this mission to prioritize and evaluate proposed AnatomIQ work in terms of concrete learner value and responsible delivery. |
| Constraints | Maintain scientific integrity, accessibility, learner control, honest scope, and the reusable lesson-engine direction. |
| Inputs | This document, [Project Vision](PROJECT_VISION.md), [Project Constitution](../00-Constitution/PROJECT_CONSTITUTION.md), and relevant approved specifications. |
| Outputs | A prioritized proposal, task, or implementation that clearly connects to a learner need and a mission commitment. |
| Do not assume | That feature requests are mission-aligned merely because they are 3D, interactive, or visually impressive. Do not make medical or learning-effectiveness claims without evidence. |
| Validation | Confirm the work strengthens an end-to-end learning outcome, serves a named learner need, preserves stated protections, and can be explained using the Everyday Prioritization Guide. |
