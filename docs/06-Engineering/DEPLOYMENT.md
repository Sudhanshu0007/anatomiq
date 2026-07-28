# AnatomIQ Deployment

| Field | Value |
| --- | --- |
| Document ID | AQ-ENG-013 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before release candidate approval, environment changes, and public deployment |
| Related documents | [System Architecture](SYSTEM_ARCHITECTURE.md), [Performance Strategy](PERFORMANCE_STRATEGY.md), [Testing Strategy](TESTING_STRATEGY.md), [Non-Functional Requirements](../03-PRD/NON_FUNCTIONAL_REQUIREMENTS.md) |

## Purpose

This document defines the deployment approach for AnatomIQ. Deployment must support predictable release, validation, and rollback behavior for the MVP.

## Scope

### In scope

- Build and release flow.
- Environment promotion expectations.
- Release readiness and rollback considerations.
- Public MVP delivery boundaries.

### Out of scope

- Infrastructure vendor selection.
- CI/CD platform-specific configuration.
- Production monitoring tool configuration.

## Deployment principles

- Deployment should be predictable and repeatable.
- Release readiness depends on documentation, testing, and performance checks.
- The public MVP must not be deployed before the critical journeys are validated.
- Rollback or safe-exit paths must exist for release problems.

## Deployment stages

| Stage | Purpose |
| --- | --- |
| Local development | Verify changes in the working environment |
| Shared review | Validate changes against the documentation and tests |
| Release candidate | Freeze scope and verify readiness gates |
| Public MVP | Deliver the validated cardiovascular experience |

## Deployment rules

- Do not promote a release that fails required journey, accessibility, or recovery checks.
- Documentation updates should accompany meaningful product changes.
- Performance and asset concerns should be reviewed before public release.
- The deployment process should support future body systems without a redesign.

## Release readiness inputs

- Approved or accepted documentation for the milestone scope.
- Passing validation for the target journeys.
- Confirmed performance and fallback behavior.
- Clear knowledge of what is intentionally out of scope.

## Acceptance criteria

- [ ] The deployment path is predictable and staged.
- [ ] Release readiness depends on documented validation.
- [ ] The process supports safe release and rollback thinking.
- [ ] AI Context is current.

## Open questions

- [ ] What environment set should be used for the first public MVP release?
- [ ] What should the rollback boundary be if a release fails after deployment?
- [ ] Which deployment checks are manual versus automated for the MVP?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial Deployment draft for the engineering bible. |

## Review checklist

- [ ] Deployment stages and rules are explicit.
- [ ] Release readiness depends on documentation and validation.
- [ ] Safe release and rollback expectations are included.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Define the deployment approach for AnatomIQ so the MVP can be released predictably and safely. |
| Constraints | Do not deploy before the critical journeys and release checks are validated. |
| Inputs | System Architecture, Performance Strategy, Testing Strategy, Non-Functional Requirements. |
| Outputs | Deployment stages, readiness criteria, or rollback considerations. |
| Do not assume | A build is ready for public use without validation and documentation alignment. |
| Validation | Confirm the release can be promoted safely through the defined deployment stages. |