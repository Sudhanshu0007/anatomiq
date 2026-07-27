# AnatomIQ Risks and Assumptions Register

| Field | Value |
| --- | --- |
| Document ID | AQ-PRD-009 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-27 |
| Last updated | 2026-07-27 |
| Review cadence | At each scope, validation, architecture, and release review |
| Related documents | [Product Requirements Document](PRODUCT_REQUIREMENTS_DOCUMENT.md), [MVP Scope](MVP_SCOPE.md), [Non-Functional Requirements](NON_FUNCTIONAL_REQUIREMENTS.md), [Release and Validation Plan](RELEASE_AND_VALIDATION_PLAN.md) |

## Purpose

This living register makes uncertainty visible before it becomes hidden scope, rework, or misleading claims. A risk is a possible negative event; an assumption is an unverified belief on which a decision depends.

## Rating system

| Rating | Likelihood / impact meaning |
| --- | --- |
| High | Likely or potentially severe enough to block safe, credible, or usable MVP release. |
| Medium | Plausible and material; requires monitoring and planned mitigation. |
| Low | Limited likelihood or impact; review periodically. |

## Risk register

| ID | Risk | Likelihood | Impact | Mitigation | Trigger / owner |
| --- | --- | --- | --- | --- | --- |
| R-01 | Scope expands from one circulation lesson into a whole-body build before validation. | High | High | Enforce MVP Scope and scope-change rules. | Any proposal for additional system/pathology feature; Project owner. |
| R-02 | Visual complexity creates confusion instead of understanding. | Medium | High | Progressive disclosure, learner testing, and objective-aligned scene review. | Learners cannot trace route or identify current step; Lesson owner. |
| R-03 | Medical content or simplification is inaccurate or misleading. | Medium | High | Source register, qualified review, simplification notes, and release gate. | Reviewer dispute or missing source; Content owner. |
| R-04 | Motion/3D interaction excludes some learners. | High | High | Keyboard, reduced-motion, text-equivalent, and colour-independent paths from prototype stage. | Core alternative journey fails; Accessibility owner. |
| R-05 | Performance or graphics support prevents use on target devices. | Medium | High | Define reference environment early; progressive loading and fallback; measure budgets. | Prototype misses budget or rendering fails; Engineering owner. |
| R-06 | Reusable engine is over-engineered before learning value is proven. | Medium | Medium | Build abstractions demonstrated by MVP; defer speculative platform features. | New abstraction lacks current lesson need; Engineering owner. |
| R-07 | Reusable engine is under-designed and forces copy-paste for later lessons. | Medium | Medium | Document lesson data boundary and perform second-lesson modeling exercise. | Cardiovascular-specific logic cannot be reused; Engineering owner. |
| R-08 | AI-generated content/code introduces factual, legal, or quality errors. | Medium | High | Human review, source verification, test evidence, and no invented claims. | Unverified generated output appears in release candidate; All owners. |
| R-09 | Learner validation is unavailable or unrepresentative. | Medium | Medium | Use small moderated sessions, educator review, transparent limitations, and defer strong claims. | No representative participants by R3; Product owner. |
| R-10 | Unclear licensing for models, textures, audio, or medical imagery. | Medium | High | Maintain asset register and use assets with documented permissions. | Asset has unknown origin/license; Asset owner. |
| R-11 | Privacy scope expands through analytics, accounts, or feedback collection. | Low | High | Data-minimization review before any collection; no account required for core lesson. | New event/data field proposed; Privacy owner. |
| R-12 | Documentation drifts from product behavior. | Medium | Medium | Update specs and acceptance criteria with material changes; review before release. | Implementation differs from approved doc; Project owner. |

## Assumption log

| ID | Assumption | Why it matters | Validation / decision needed | Status |
| --- | --- | --- | --- | --- |
| A-01 | The circulation route is a high-value problem for foundational anatomy learners. | Determines MVP topic. | Interview/test learners and educators. | Open |
| A-02 | A guided visual story plus practice helps learners more than disconnected content alone. | Underpins product hypothesis. | Task-based prototype evaluation. | Open |
| A-03 | A laptop-first reference environment is suitable for early validation. | Shapes interaction and performance plan. | Choose target cohort and device data. | Open |
| A-04 | An accessible reduced-motion path can preserve essential spatial/temporal learning. | Determines accessibility feasibility. | Prototype and test alternative journey. | Open |
| A-05 | Appropriate medical content review can be obtained before public release. | Required for integrity gate. | Identify reviewer and source plan. | Open |
| A-06 | The lesson engine can separate content from shared behavior without premature complexity. | Determines platform viability. | Architecture review and second-lesson exercise. | Open |
| A-07 | Educator-led use can be supported without a separate dashboard in the MVP. | Affects scope. | Educator walkthrough. | Open |
| A-08 | The MVP can provide sufficient value without accounts, personalization, or analytics. | Protects focus and privacy. | Validation plan and feedback needs review. | Open |

## Risk-response rules

- A High-impact risk without an active mitigation blocks the affected release stage.
- A changed assumption must trigger review of all dependent requirements and decisions.
- Closed risks and validated assumptions remain recorded with the evidence and date; they are not deleted.
- A risk that becomes an actual issue must be logged with impact, resolution, and any necessary PRD or ADR change.

## Open questions

- [ ] Who owns each risk area while the project is a solo effort, and how will external review responsibilities be assigned later?
- [ ] What asset-license format will the repository use?
- [ ] What is the escalation path if qualified medical review is unavailable before a desired demo date?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-27 | AnatomIQ Project Team | Initial MVP risk and assumption register. |

## Review checklist

- [x] Key product, medical, accessibility, performance, privacy, asset, AI, and documentation risks are listed.
- [x] Assumptions include validation paths and status.
- [x] Risk response rules are defined.
- [x] AI Context is complete.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Identify and reduce uncertainty before it produces unsafe, inaccessible, misleading, or unmaintainable MVP work. |
| Constraints | Do not close a risk or validate an assumption without evidence. Treat High-impact risks as release blockers unless an approved exception exists. |
| Inputs | This register, scope, requirements, validation findings, architecture decisions, asset register, and review results. |
| Outputs | A risk update, mitigation task, assumption-validation plan, issue record, or escalation decision. |
| Do not assume | That lack of visible failure means a risk is resolved, or that untested accessibility/medical/performance behavior is acceptable. |
| Validation | Update likelihood, impact, status, owner, evidence, and dependent documents after each material finding or decision. |
