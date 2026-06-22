<!--
COMP 330 Instructional Example Artifact

This Markdown file is an instructional example showing professional engineering evidence patterns, workflow visibility, repository organization, and planning/governance expectations.

Teams should adapt this structure to their actual project, repository evidence, risks, workflow, and operational maturity. Do not preserve the example entries unchanged.

The authoritative operational version of this artifact belongs inside the team GitHub repository and should evolve throughout the semester.
-->

# Estimates Example

**Purpose:** Records rough effort estimates, assumptions, uncertainty, and risk triggers. Estimates should use ranges, not false precision.

**Typical repository location:** `/docs/planning/estimates.md`

## Engineering Guidance

Estimates should support engineering planning, risk visibility, staffing awareness, review capacity, operational validation, and release expectations rather than create artificial certainty.

Review, testing, debugging, governance, operational validation, and integration work are often underestimated compared to initial implementation effort.

Strong engineering teams revise estimates when evidence changes rather than protecting unrealistic plans.

## Estimate Summary

| Item | Value |
|---|---|
| Current cycle | Cycle 1 |
| Estimate owner | Example: Planning Lead |
| Last updated | YYYY-MM-DD |
| Overall confidence | Medium |

## Task Estimates

| Task / Work ID | Short Description | Low | Likely | High | Assumptions | Risk Trigger | Owner |
|---|---|---:|---:|---:|---|---|---|
| WB-001 | Request submission form | 2 hrs | 3 hrs | 5 hrs | Simple form, no external integration | Validation complexity grows | Example: Dev A |
| WB-002 | Required-field validation | 1 hr | 2 hrs | 4 hrs | Rules remain simple | Edge cases increase | Example: Dev B |
| WB-004 | Staff request list view | 3 hrs | 5 hrs | 8 hrs | Request data model stays stable | Filtering/sorting added too early | Example: Dev C |
| WB-010 | Runtime diagnostics and logging improvements | 2 hrs | 4 hrs | 8 hrs | Existing failures can be reproduced | Logging gaps block troubleshooting | Example: QA Lead |

## Estimate Assumptions

| ID | Assumption | Impact if Wrong | Owner |
|---|---|---|---|
| A-001 | Team can use synthetic data only | May require redesign if real data is expected | Example: Product Owner |
| A-002 | AI category suggestion remains deferred for Cycle 1 | Review and governance workload stays manageable | Example: Architecture Lead |
| A-003 | Basic logging is sufficient for release review | Additional operational evidence may be needed | Example: QA Lead |

## Estimate Risks

| Risk | Why It Matters | Related Evidence |
|---|---|---|
| Integration takes longer than implementation | UI and data behavior often fail at boundaries | Risk R-001; PR review notes |
| AI assistance reduces drafting time but increases review time | Generated output still requires validation, explanation, governance, and ownership | AI-use log; Risk R-002 |
| Operational diagnostics are underestimated | Failures may be hard to reproduce or explain during release review | Risk R-004; `/docs/observability/` |

## Notes

- AI may reduce drafting or implementation time, but it can increase review, validation, debugging, governance, integration, and operational validation time.
- Update this file when evidence shows the original estimate was wrong.
- Estimates should help teams make realistic engineering decisions, not justify optimistic schedules or presentation-driven promises.
