# AnatomIQ Asset Pipeline

| Field | Value |
| --- | --- |
| Document ID | AQ-ENG-010 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before asset production, content import, and release candidate review |
| Related documents | [3D Art Direction](../05-Design/3D_ART_DIRECTION.md), [Lighting and Materials](../05-Design/LIGHTING_AND_MATERIALS.md), [Audio Direction](../05-Design/AUDIO_DIRECTION.md), [Performance Strategy](PERFORMANCE_STRATEGY.md) |

## Purpose

This document defines the asset pipeline for AnatomIQ. The pipeline must support efficient intake, review, optimization, and delivery of 3D, texture, audio, and documentation assets.

## Scope

### In scope

- Asset categories and intake rules.
- Naming and organization expectations.
- Optimization and packaging guidance.
- Review and validation checkpoints.

### Out of scope

- Specific toolchain or export format choices.
- Vendor-specific storage policies.
- Full DCC workflow implementation details.

## Pipeline goals

- Make assets easy to find, review, and replace.
- Support the reusable lesson engine rather than one-off imports.
- Keep performance and accessibility implications visible.

## Asset categories

| Category | Examples |
| --- | --- |
| 3D models | body, organ, vessel, nerve, scene props |
| Textures | surface maps, labels, overlays |
| Audio | cues, ambience, narration |
| Reference images | source images, sketches, mood references |
| Documentation assets | diagrams, flowcharts, explanatory visuals |

## Pipeline stages

1. Ingest source or created asset.
2. Verify naming, ownership, and intended use.
3. Check whether the asset supports the lesson objective.
4. Optimize for performance and readability.
5. Validate accessibility and visual clarity.
6. Store in the correct folder or package.
7. Reference the asset from the relevant data or lesson document.

## Asset rules

- Assets must be named consistently and be easy to trace back to their source or owner.
- Imported assets should not bypass the content review process.
- Optimization should preserve educational clarity.
- Assets that affect performance or readability must be tested in context.

## Acceptance criteria

- [ ] Asset intake and review steps are explicit.
- [ ] Optimization and traceability expectations are covered.
- [ ] The pipeline supports the reusable lesson model.
- [ ] AI Context is current.

## Open questions

- [ ] Which assets should be versioned in the repository versus stored externally?
- [ ] What are the minimum naming and folder conventions for incoming anatomical assets?
- [ ] How much manual review is needed before an asset can be used in a lesson?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial Asset Pipeline draft for the engineering bible. |

## Review checklist

- [ ] Asset categories and stages are explicit.
- [ ] Naming and traceability are defined.
- [ ] Performance and accessibility considerations are included.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the asset pipeline for AnatomIQ so media can be reviewed, optimized, and delivered consistently. |
| Constraints | Preserve traceability, readability, and performance across all assets. |
| Inputs | 3D Art Direction, Lighting and Materials, Audio Direction, Performance Strategy. |
| Outputs | Asset workflow, organization rules, or validation checkpoints. |
| Do not assume | Imported assets are automatically suitable for educational use. |
| Validation | Confirm every asset can be traced, reviewed, and linked to the relevant lesson context. |