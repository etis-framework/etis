<!--
COMP 330 Instructional Example Artifact

This Markdown file is an instructional example showing professional engineering evidence patterns, workflow visibility, repository organization, and planning/governance expectations.

Teams should adapt this structure to their actual project, repository evidence, risks, workflow, and operational maturity. Do not preserve the example entries unchanged.

The authoritative operational version of this artifact belongs inside the team GitHub repository and should evolve throughout the semester.
-->

# Re-Estimation Notes Example

**Purpose:** Records how the team updates plans based on evidence, not wishful thinking.

**Typical repository location:** `/docs/planning/re-estimation.md`

## Engineering Guidance

Re-estimation is expected professional engineering behavior when evidence changes assumptions, scope understanding, operational complexity, review workload, or release confidence.

AI-assisted implementation may accelerate drafting while simultaneously increasing review, debugging, governance, integration, and operational validation workload.

Re-estimation artifacts should document real engineering learning and changing evidence — not retroactively justify unrealistic planning decisions.

## Re-Estimation Summary

| Item | Value |
|---|---|
| Current cycle | Cycle 1 |
| Re-estimation date | YYYY-MM-DD |
| Re-estimation owner | Example: Planning Lead |
| Evidence reviewed | Defects / PRs / tests / runtime evidence / observability findings / estimates / blockers / feedback / postmortem |

## What Changed?

| Area | Original Plan | New Understanding | Change Made | Evidence |
|---|---|---|---|---|
| Request workflow | Complete full admin dashboard | Dashboard is too large for Cycle 1 | Defer dashboard, keep status update workflow | Issue #8, Risk R-005 |
| AI support | Add AI category suggestion in Cycle 1 | Validation and governance evidence are immature | Move to deferred candidate | Risk R-003, AI-use log |
| Runtime visibility | Rely on console output only | Failures are difficult to diagnose during review | Add basic logging task | Risk R-004, Issue #12 |

## Estimate Updates

| Task / Work ID | Original Estimate | Updated Estimate | Reason for Change | Owner |
|---|---:|---:|---|---|
| WB-001 | 3 hrs | 5 hrs | Validation and error handling took longer | Example: Dev A |
| WB-004 | 4 hrs | 8 hrs | Staff list view needs clearer requirements and test data | Example: Dev C |
| WB-010 | 0 hrs | 4 hrs | Operational diagnostics were missing from original plan | Example: QA Lead |

## Scope Decisions

| Decision | Reason | Impact | Evidence / Link |
|---|---|---|---|
| Delay AI-generated recommendations from release | Validation and governance evidence incomplete | Reduce release risk and maintain reviewability | ADR-004, Risk R-003 |
| Defer admin analytics dashboard | Current scope already stretches review capacity | Keeps Cycle 1 focused on one defensible workflow | Scope D-002, Issue #8 |
| Add basic operational logging | Runtime failures were not diagnosable enough | Improves release confidence and reviewability | Risk R-004, Issue #12 |

## Next Actions

| Action | Owner | Target Date | Evidence Needed |
|---|---|---|---|
| Update scope and traceability | Example: Planning Lead | YYYY-MM-DD | Updated `scope.md`, `traceability.md` |
| Create logging issue | Example: QA Lead | YYYY-MM-DD | Issue #12, PR, operational evidence |
| Update release notes with deferred AI behavior | Example: Release Lead | YYYY-MM-DD | Release notes, AI-use log, known limitations |

## Reviewability Check

Another engineering team should be able to inspect the re-estimation evidence and understand why planning decisions changed over time.
