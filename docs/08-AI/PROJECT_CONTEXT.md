# AnatomIQ Project Context

| Field | Value |
| --- | --- |
| Document ID | AQ-AI-001 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | Before prompt writing, task creation, and major milestone changes |
| Related documents | [Project Vision](../01-Vision/PROJECT_VISION.md), [Product Philosophy](../01-Vision/PRODUCT_PHILOSOPHY.md), [Product Requirements Document](../03-PRD/PRODUCT_REQUIREMENTS_DOCUMENT.md), [System Architecture](../06-Engineering/SYSTEM_ARCHITECTURE.md), [Medical Content Standards](../07-Medical/MEDICAL_CONTENT_STANDARDS.md) |

## Purpose

This document gives AI collaborators the minimum project context needed to work safely and consistently on AnatomIQ. It is the entry point for AI-driven implementation, review, and task planning.

## Scope

### In scope

- Project summary and mission-aligned context.
- Milestone and documentation structure.
- Non-negotiable product constraints.
- AI collaboration boundaries.

### Out of scope

- Repeating every specification in full.
- Implementation details that belong in engineering documents.
- Medical claims that must live in the medical package.

## Project summary

AnatomIQ is a documentation-driven, reusable human anatomy learning platform. The MVP teaches one complete cardiovascular lesson first, then expands to other body systems through the same engine and content structure.

## AI working context

| Topic | Summary |
| --- | --- |
| Product goal | Help learners understand anatomy and physiology through a guided, interactive 3D learning experience |
| MVP focus | One complete cardiovascular circulation lesson |
| Reusability goal | Build a Human Body Engine and lesson engine that support later systems |
| Content rule | Medical content must be sourced, reviewed, and simplified responsibly |
| UX rule | Learners must keep control, orientation, and recovery paths |
| Engineering rule | Separate shared behavior from content-driven lesson data |

## AI collaboration boundaries

- Do not invent requirements that are not in approved documentation.
- Do not change medical scope without a matching document update.
- Do not add features that conflict with accessibility, learner control, or reuse.
- Do not claim tests, review, or approval that have not happened.

## Acceptance criteria

- [ ] The document gives AI collaborators enough context to work safely.
- [ ] The project summary matches the approved vision and PRD.
- [ ] The constraints are clear and aligned with the rest of the documentation set.
- [ ] AI Context is current.

## Open questions

- [ ] Which milestone documents should always be included in a prompt bundle for implementation work?
- [ ] How much project context should be repeated in prompts versus linked by document reference?
- [ ] Should AI context be mirrored in future body-system packages as well?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial project context draft for the AI bible. |

## Review checklist

- [ ] Project summary and MVP focus are explicit.
- [ ] AI collaboration boundaries are clear.
- [ ] The context matches the approved documentation set.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Give AI collaborators a concise, safe summary of AnatomIQ and its current documentation state. |
| Constraints | Do not invent scope, medical claims, or implementation details not approved in related documents. |
| Inputs | Project Vision, Product Philosophy, PRD, System Architecture, Medical Content Standards. |
| Outputs | Project summary, collaboration boundaries, or prompt-ready context. |
| Do not assume | The AI already knows the approved milestone structure or current source of truth. |
| Validation | Confirm the context matches the latest approved product, engineering, and medical documentation. |