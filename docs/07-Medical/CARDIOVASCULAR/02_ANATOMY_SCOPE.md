# AnatomIQ Cardiovascular Anatomy Scope

| Field | Value |
| --- | --- |
| Document ID | AQ-MED-004 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before scene authoring and before medical review |
| Related documents | [Overview](00_OVERVIEW.md), [Learning Objectives](01_LEARNING_OBJECTIVES.md), [Physiology Scope](03_PHYSIOLOGY_SCOPE.md), [Scene-by-Scene Specification](05_SCENE_BY_SCENE_SPECIFICATION.md), [Sources and Medical Review](09_SOURCES_AND_MEDICAL_REVIEW.md) |

## Purpose

This document defines the cardiovascular anatomy included in the MVP. It identifies which structures must appear, which are optional, and what anatomical depth is excluded.

## Scope

### In scope

- Heart, lungs, and major route structures.
- Broad vessel categories relevant to the lesson.
- Orientation structures needed for the body context.

### Out of scope

- Full vessel branching tree.
- Detailed chamber wall anatomy and microscopic structure.
- Disease anatomy and pathology.

## Required structures

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

## Anatomy rules

- Structures must support the approved route model.
- Anatomical names should be consistent across scenes, annotations, and assessments.
- The anatomy model should be clear enough to teach without implying full anatomical completeness.
- Optional detail must not obscure the primary route.

## Acceptance criteria

- [ ] The required structures are explicitly listed.
- [ ] The scope matches the MVP route and objectives.
- [ ] Excluded anatomy is clearly kept out of the lesson package.
- [ ] AI Context is current.

## Open questions

- [ ] Are the valves named in the MVP anatomy scope or kept as optional depth only?
- [ ] Should the body orientation include only thoracic context or a broader body frame?
- [ ] Which anatomical labels are required at each scene versus later in the lesson?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial cardiovascular anatomy scope draft. |

## Review checklist

- [ ] Required structures are explicit.
- [ ] In-scope and out-of-scope anatomy are separated.
- [ ] The anatomy scope aligns with the route and objectives.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the anatomical scope for the cardiovascular MVP lesson. |
| Constraints | Do not expand into full branching detail, pathology, or unsupported structures. |
| Inputs | Overview, Learning Objectives, Physiology Scope, Content and Lesson Requirements. |
| Outputs | Anatomy scope and required structure list. |
| Do not assume | More anatomical detail is automatically in scope for the MVP. |
| Validation | Confirm the listed structures are sufficient to teach the approved route. |