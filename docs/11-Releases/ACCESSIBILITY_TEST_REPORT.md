# AnatomIQ Accessibility Test Report

| Field | Value |
| --- | --- |
| Document ID | AQ-REL-005 |
| Version | 0.1.0 |
| Status | Draft |
| Owner | AnatomIQ Project Team |
| Created | 2026-07-28 |
| Last updated | 2026-07-28 |
| Review cadence | After accessibility testing and before release decision review |
| Related documents | [Accessibility Specification](../04-UX/ACCESSIBILITY_SPECIFICATION.md), [Design Accessibility](../05-Design/DESIGN_ACCESSIBILITY.md), [Testing Strategy](../06-Engineering/TESTING_STRATEGY.md) |

## Purpose

This document records accessibility test findings for the release evidence pack. It should document keyboard, reduced-motion, text alternative, colour independence, and recovery validation results.

## Scope

### In scope

- Keyboard-only journey validation.
- Reduced-motion or step-based path validation.
- Colour independence and text alternative checks.
- Accessible recovery and focus behavior.

### Out of scope

- General usability findings that are not accessibility-related.
- Tool-specific accessibility audit configuration.
- Formal legal conformance claims without documented evidence.

## Report fields

| Field | Purpose |
| --- | --- |
| testArea | Keyboard, motion, colour, text, focus, recovery |
| method | How the check was performed |
| result | Pass, partial pass, or fail |
| evidence | Notes, screenshots, or session records |
| issue | Description of the problem if any |
| resolution | Fix, workaround, or accepted limitation |

## Reporting rules

- Record the actual observed result.
- Tie each finding to the relevant requirement or journey when possible.
- Do not mark accessibility as complete without explicit evidence.
- If a limitation remains, record it in the release evidence pack and known limitations.

## Acceptance criteria

- [ ] The report structure supports the required accessibility checks.
- [ ] Results are explicit and tied to evidence.
- [ ] Limitations are recorded honestly.
- [ ] AI Context is current.

## Open questions

- [ ] Which assistive technology combinations should be tested first?
- [ ] What is the minimum evidence required for a release-ready accessibility result?
- [ ] Should this report be split by test round or combined into one release report?

## Revision history

| Version | Date | Author/owner | Summary |
| --- | --- | --- | --- |
| 0.1.0 | 2026-07-28 | AnatomIQ Project Team | Initial accessibility test report template. |

## Review checklist

- [ ] The report structure covers the required accessibility checks.
- [ ] Results are explicit, tied to evidence, and honest.
- [ ] The report aligns with the accessibility specification and testing strategy.
- [ ] AI Context is current.

## AI Context

| Item | Value |
| --- | --- |
| Objective | Record accessibility test results for the release evidence pack. |
| Constraints | Do not claim accessibility success without explicit evidence. |
| Inputs | Accessibility Specification, Design Accessibility, Testing Strategy. |
| Outputs | Accessibility test results and limitation records. |
| Do not assume | Keyboard support or reduced-motion support is complete without testing. |
| Validation | Confirm the report captures pass/fail outcomes and evidence clearly. |