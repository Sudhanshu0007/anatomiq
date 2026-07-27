# AnatomIQ Success Criteria

| Field | Value |
| --- | --- |
| Document ID | AQ-VIS-004 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-27 |
| Last updated | 2026-07-27 |
| Review cadence | Before MVP release, after each learner validation cycle, and at each major release |
| Related documents | [Project Vision](PROJECT_VISION.md), [Mission](MISSION.md), [Product Philosophy](PRODUCT_PHILOSOPHY.md), [Educational Philosophy](EDUCATIONAL_PHILOSOPHY.md), [Project Constitution](../00-Constitution/PROJECT_CONSTITUTION.md) |

## Purpose

This document defines what success means for AnatomIQ. It provides outcome-oriented criteria for the cardiovascular MVP and a reusable measurement framework for later releases.

Success is not defined by visual complexity, page count, number of body systems, time spent in the product, or the presence of 3D technology. AnatomIQ succeeds when it helps learners build clearer, accurate mental models in an accessible and trustworthy experience.

## Scope

### In scope

- Success dimensions and criteria for product validation.
- Initial MVP release gates.
- Measurement principles and evidence standards.
- Signals that indicate progress, risk, or failure.

### Out of scope

- Final numeric targets before the target learner group and validation method are selected.
- Marketing claims of improved academic or clinical performance.
- Detailed analytics architecture, data schema, or privacy policy.
- Feature-level test plans and performance budgets, which belong in later specifications.

## Success definition

The cardiovascular MVP is successful when a representative learner can complete a clear, medically responsible, accessible journey through blood circulation; explain its major route and purpose better than before the lesson; and revisit information without losing control or context.

The platform direction is successful when this lesson can serve as a reliable foundation for additional body-system lessons without duplicating core product behavior or lowering the project’s standards.

## Success dimensions

| Dimension | Core question | Success means |
| --- | --- | --- |
| Learning value | Did the learner build a more accurate mental model? | Learners can locate, trace, explain, and distinguish the lesson’s key concepts. |
| Scientific integrity | Is the lesson medically responsible? | Claims, visual representations, and simplifications are traceable, reviewed, and clearly scoped. |
| Usability and agency | Can learners understand and control the experience? | Learners can orient, progress, pause, replay, and recover without undue confusion. |
| Accessibility | Can learners access the essential educational value through supported alternatives? | Essential concepts and controls are not dependent on a single sensory or input method. |
| Technical quality | Does the product reliably support attention and learning? | The experience is stable, responsive, and performant on the supported reference environment. |
| Reusability | Does the MVP prove a platform rather than a one-off demo? | Lesson content and shared capabilities are sufficiently separated to support another system. |
| Trust | Does the product communicate its scope and limitations honestly? | Learners and educators can identify what is taught, simplified, and not provided. |
| Documentation health | Can a collaborator or AI agent implement and review work consistently? | Decisions, requirements, and acceptance criteria are current, linked, and usable. |

## Cardiovascular MVP outcomes

The MVP must teach a deliberately bounded circulation story. The final Product Requirements Document will define the exact scope, but the initial outcome set is:

| Outcome ID | Learner outcome | Evidence of success |
| --- | --- | --- |
| LO-CV-01 | Identify the heart, lungs, and major body context relevant to the circulation journey. | Learner can locate or name the structures in a contextual task. |
| LO-CV-02 | Trace the route of deoxygenated blood from the body through the right side of the heart to the lungs. | Learner correctly orders or explains the route with a visual reference removed or reduced. |
| LO-CV-03 | Trace the route of oxygenated blood from the lungs through the left side of the heart to the body. | Learner correctly orders or explains the route and direction of flow. |
| LO-CV-04 | Distinguish the broad roles of arteries, veins, and capillaries in the taught route. | Learner matches a structure type to its relationship with the circulation route. |
| LO-CV-05 | Explain, at the intended learner level, why pulmonary and systemic circulation are connected. | Learner gives a simple cause-and-effect explanation rather than only reciting labels. |

These outcomes are educational targets, not evidence of medical or professional competency.

## MVP release gates

The MVP must not be represented as ready for public demonstration until every applicable gate is satisfied or an explicit, time-bounded exception is recorded.

### 1. Educational readiness

- [ ] The lesson has approved, assessable learning objectives.
- [ ] Every major scene and interaction supports at least one objective.
- [ ] The lesson provides orientation, focused explanation, learner-controlled review, and formative practice.
- [ ] Practice questions map to content actually taught in the lesson.
- [ ] Feedback explains the reasoning and links learners to relevant review material.
- [ ] Representative learner feedback has been collected and acted on, or a documented plan explains why it cannot yet be collected.

### 2. Scientific and content readiness

- [ ] Medical claims, labels, and sequence representations have traceable sources.
- [ ] The intended level of simplification is documented.
- [ ] Simplifications that could cause misunderstanding are disclosed in context.
- [ ] Required medical or subject-matter review has occurred.
- [ ] The lesson does not provide diagnosis, treatment recommendations, or personalized medical advice.

### 3. Usability and agency readiness

- [ ] Learners can determine what system and lesson step they are viewing.
- [ ] Core navigation, pause, replay, and reset behavior are discoverable and work predictably.
- [ ] A learner can recover from a wrong click, rapid scroll, interrupted animation, or accidental navigation.
- [ ] Important explanations are available without waiting for a time-limited animation.
- [ ] Usability testing identifies no unresolved blocker that prevents the primary learning journey.

### 4. Accessibility readiness

- [ ] Core lesson controls are operable by keyboard.
- [ ] Focus order and visible focus states are verified.
- [ ] Information is not conveyed only by color, motion, sound, or hover behavior.
- [ ] Reduced-motion behavior preserves the essential explanation.
- [ ] Text alternatives, captions, and descriptions are provided where required by the accessibility specification.
- [ ] Contrast, readability, and target size meet the defined design and accessibility standards.

### 5. Technical readiness

- [ ] The supported reference environment and minimum support policy are documented.
- [ ] Critical paths are tested for loading failures, slow networks, unsupported graphics capability, and recovery.
- [ ] The experience meets its approved performance budgets on reference hardware.
- [ ] No known crash, data-loss, navigation, or rendering defect blocks the primary lesson.
- [ ] Error states communicate what happened and offer a meaningful next action.

### 6. Platform and documentation readiness

- [ ] Lesson content is separated from reusable engine behavior at the documented level.
- [ ] The lesson’s camera states, annotations, sequence, interactions, and assessment are documented.
- [ ] Shared capabilities and lesson-specific exceptions are identified.
- [ ] Relevant architecture, design, medical, and AI-context documents are linked and current.
- [ ] A future contributor can identify the next work item and its acceptance criteria without guessing.

## Measurement principles

### Measure understanding, not only engagement

Engagement signals—time spent, scroll depth, replays, or clicks—can help diagnose experience quality but cannot prove learning. Pair behavioral signals with objective-aligned tasks, observations, and learner feedback.

### Use the smallest responsible measurement set

Collect only data needed to answer a defined product question. Prefer anonymized, aggregate, or voluntary feedback. Do not collect personal health information for core learning validation.

### Compare before and after where feasible

For early validation, use a short pre-lesson task and an equivalent post-lesson task aligned to the same objectives. Interpret results cautiously: a small sample can reveal confusion and direction, but not establish broad educational efficacy.

### Combine quantitative and qualitative evidence

Numbers identify patterns; observation and interviews help explain them. A learner who answers correctly but cannot explain their reasoning may be guessing. A learner who pauses or replays may be struggling—or may be using the product well.

### Make uncertainty explicit

Document sample size, learner profile, test conditions, missing data, and known bias. Avoid claims that the available evidence cannot support.

## Initial measurement framework

Numeric targets are intentionally marked `TBD` until the primary learner segment, validation setting, and baseline are selected.

| Dimension | Indicator | Method | Initial target | Interpretation |
| --- | --- | --- | --- | --- |
| Learning value | Objective-aligned post-lesson task performance | Short task or think-aloud after the lesson | TBD | Indicates whether the taught model can be applied. |
| Learning value | Improvement from pre-lesson task | Comparable before/after task | TBD | Suggests learning within the tested session; not long-term retention. |
| Understanding quality | Explanation of circulation route and purpose | Interview, written explanation, or recorded response | TBD | Reveals causal understanding and misconceptions. |
| Usability | Completion of primary journey without facilitator rescue | Observed usability session | TBD | Identifies navigation or comprehension blockers. |
| Agency | Successful pause, replay, and step revisit | Task-based usability session | TBD | Checks whether learner controls are discoverable and reliable. |
| Accessibility | Completion of core tasks using supported alternatives | Keyboard, reduced-motion, and assistive-technology checks | Required release gate | Confirms essential access, not optional polish. |
| Trust | Learner can identify the lesson’s scope and limitation | Post-lesson prompt | TBD | Checks for misleading interpretations. |
| Technical quality | Blocking defects and performance-budget compliance | Test suite and reference-device testing | Required release gate | Ensures the platform does not interrupt learning. |
| Reusability | Effort to model a second sample lesson using shared capabilities | Internal implementation exercise | TBD | Tests whether the MVP created a reusable foundation. |

## Leading indicators and warning signs

| Signal | Interpretation | Recommended response |
| --- | --- | --- |
| Learners repeatedly replay one step and then answer correctly | May indicate useful self-paced learning or unclear first explanation. | Observe sessions and clarify the step if confusion is evident. |
| Learners reach the end but cannot explain the route | Completion is not producing the intended model. | Revisit orientation, sequence cues, explanation, and practice. |
| Learners confuse red/blue color with artery/vein identity | Visual convention may be teaching a misconception. | Add explicit explanation and non-color cues. |
| Learners cannot find pause or replay | Agency controls are not discoverable. | Improve hierarchy, onboarding, labels, and keyboard affordances. |
| A high-detail scene reduces performance or orientation | Detail is exceeding its educational value. | Simplify, use progressive detail, or provide a lower-cost mode. |
| New lessons require duplicated logic | The engine boundary is not adequately reusable. | Document and refactor shared capability before scaling content. |
| Content reviewers dispute a representation | The medical model or simplification is unclear. | Pause release, trace sources, revise the model, and record the decision. |

## Non-success conditions

The project must not call an MVP successful merely because it has a functioning 3D model, a polished animation, social-media interest, a completed roadmap item, or high engagement. The project has not met its standard if any of the following are true:

- learners commonly leave with an inaccurate model of the taught route;
- essential controls or explanations are inaccessible to a supported learner group;
- the product presents unsupported medical claims or conceals material simplifications;
- the primary journey is unstable, disorienting, or unusable on the stated reference environment;
- the cardiovascular lesson works only through hardcoded, non-reusable behavior without an accepted rationale;
- documentation cannot explain the product’s intended behavior, evidence, limitations, or next decisions.

## Reporting cadence

| Event | Required review |
| --- | --- |
| Before first internal prototype review | Confirm educational objectives, core flow, scope limitations, and validation plan. |
| After each learner validation round | Record findings, changes made, unresolved risks, and implications for criteria. |
| Before a public demo or MVP release | Evaluate all release gates and document any approved exceptions. |
| After a major release | Review evidence, update targets, revise risks, and decide next investment. |

## Open questions

- [ ] Who are the first representative learners, and how will they be recruited ethically?
- [ ] What pre/post tasks best assess the cardiovascular MVP without becoming a formal examination?
- [ ] What reference devices and browsers define the initial support policy?
- [ ] Which qualified subject-matter reviewers can validate the MVP’s medical content?
- [ ] What privacy-preserving analytics, if any, are necessary for early product learning?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-27 | AnatomIQ Project Team | Initial success criteria draft. |

## Review checklist

- [x] Success is defined in learning, scientific, usability, accessibility, technical, platform, trust, and documentation dimensions.
- [x] Cardiovascular MVP outcomes and release gates are included.
- [x] Measurement principles avoid unsupported effectiveness claims and unnecessary data collection.
- [x] Early targets are explicitly marked TBD pending research design.
- [x] Warning signs and non-success conditions prevent superficial completion metrics.
- [x] AI Context is complete.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define, test, and report whether AnatomIQ work creates accurate learner value in a usable, accessible, trustworthy, and reusable product. |
| Constraints | Do not equate engagement, visual polish, or feature completion with learning success. Do not invent numeric targets, medical validation, learner-research results, or accessibility compliance. |
| Inputs | This document, the Project Constitution, approved lesson objectives, usability findings, medical-review results, accessibility checks, and technical test results. |
| Outputs | A validation plan, release-readiness report, improvement proposal, or documented evidence summary linked to the relevant success dimension and release gate. |
| Do not assume | That completion proves comprehension, that a small sample proves broad effectiveness, or that untested alternatives satisfy accessibility requirements. |
| Validation | Evaluate applicable MVP release gates, cite the evidence available, identify gaps and exceptions, and clearly state whether the decision is ready, blocked, or needs further validation. |
