<!--
COMP 330 Instructional Example Artifact

This Markdown file is an instructional example showing professional engineering evidence patterns, workflow visibility, repository organization, and planning/governance expectations.

Teams should adapt this structure to their actual project, repository evidence, risks, workflow, and operational maturity. Do not preserve the example entries unchanged.

The authoritative operational version of this artifact belongs inside the team GitHub repository and should evolve throughout the semester.
-->

# Task Plan Example

**Purpose:** Lightweight work decomposition and iteration planning tied to GitHub Issues, milestones, workflow evidence, and release progress.

**Typical repository location:** `/docs/planning/task-plan.md`

## Engineering Guidance

Task planning should support visible engineering coordination, workflow traceability, review readiness, and realistic release progress.

Planning evidence should evolve continuously as work changes, risks emerge, defects appear, or operational understanding improves.

Work should remain visible through repository issues, branches, pull requests, reviews, and updated engineering evidence rather than private coordination alone.

## Current Iteration / Checkpoint

| Item | Value |
|---|---|
| Cycle | Cycle 1 |
| Planning checkpoint | Requirements-to-architecture checkpoint |
| Target date | YYYY-MM-DD |
| Planning owner | Example: Project Coordinator |
| Last updated | YYYY-MM-DD |

## Work Breakdown

| Work ID | Work Area | Task | Owner | Backup | Related Issue | Estimate | Status | Evidence Needed |
|---|---|---|---|---|---|---|---|---|
| WB-001 | Request workflow | Create request submission form | Example: Dev A | Example: Dev B | #1 | 2-4 hrs | In progress | PR, review, test evidence |
| WB-002 | Request workflow | Validate required fields | Example: Dev B | Example: Dev A | #2 | 1-2 hrs | Not started | Test case, PR, validation screenshot |
| WB-003 | Requirements | Update acceptance criteria for request submission | Example: Requirements Lead | Example: QA Lead | #4 | 1 hr | Current | Updated requirements and traceability |
| WB-004 | Operations | Add basic runtime logging for failed submissions | Example: QA Lead | Example: Dev A | #12 | 2-4 hrs | Planned | Log evidence, test note, release note |

## Evidence Guidance

Evidence may include pull requests, reviews, tests, screenshots, CI results, release notes, observability evidence, ADRs, defects, operational findings, or updated planning artifacts.

## Current Blockers

| Blocker | Impact | Owner | Next Action | Target Resolution |
|---|---|---|---|---|
| Staff-view requirements are not fully clear | Could delay list-view design | Example: Requirements Lead | Ask clarification question and update FR-002 | YYYY-MM-DD |
| Logging insufficient to diagnose failures | Operational debugging delayed | Example: QA Lead | Add runtime logging and observability evidence | YYYY-MM-DD |

## Next Team Checkpoint

| Question | Team Answer |
|---|---|
| What must be completed before the next meeting? | Finish PR #5 and update TC-001 / TC-002 evidence |
| What needs review? | Request form validation and traceability update |
| What risk needs attention? | AI category suggestion should remain deferred until governance is clearer |
| What evidence must be updated? | Requirements, traceability, risk register, test evidence |
| What repository workflow evidence must be visible? | Issues #1, #2, #12; PR #5; review comments; updated planning files |

## Reviewability Check

Another engineering team should be able to inspect the task-planning evidence and understand current engineering priorities, workflow progress, and coordination status.
