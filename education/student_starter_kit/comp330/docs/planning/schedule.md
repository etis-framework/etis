<!--
COMP 330 Instructional Example Artifact

This Markdown file is an instructional example showing professional engineering evidence patterns, workflow visibility, repository organization, and planning/governance expectations.

Teams should adapt this structure to their actual project, repository evidence, risks, workflow, and operational maturity. Do not preserve the example entries unchanged.

The authoritative operational version of this artifact belongs inside the team GitHub repository and should evolve throughout the semester.
-->

# Schedule Example

**Purpose:** Tracks milestones, checkpoints, review windows, and target dates. Keep this lightweight and realistic.

**Typical repository location:** `/docs/planning/schedule.md`

## Engineering Guidance

Schedules should support engineering coordination, release readiness, review timing, and operational stability rather than artificial deadline optimism.

Schedule adjustments based on evidence, defects, review findings, or operational concerns are expected professional engineering behavior.

Milestones and checkpoints should align with visible repository evidence, pull requests, review activity, tests, and release readiness.

## Milestones and Checkpoints

| Date | Milestone / Checkpoint | Expected Evidence | Owner | Status |
|---|---|---|---|---|
| YYYY-MM-DD | Team launch complete | Team charter, roles, repo setup, AI policy, README | Example: Team Lead | Current |
| YYYY-MM-DD | Requirements checkpoint | Requirements, acceptance criteria, open questions, traceability updates | Example: Requirements Lead | In progress |
| YYYY-MM-DD | Architecture checkpoint | Architecture overview, diagram, ADRs if needed | Example: Architecture Lead | Not started |
| YYYY-MM-DD | Integration checkpoint | Issues, PRs, review evidence, early test evidence | Example: Development Lead | Not started |
| YYYY-MM-DD | Operational readiness review | Logging, observability evidence, recovery assumptions, runtime diagnostics | Example: QA Lead | Not started |
| YYYY-MM-DD | Release readiness checkpoint | Tests, defects, release notes, known limits, release/version evidence | Example: Release Lead | Not started |

## Weekly Cadence

| Meeting Day / Time | Meeting Mode | Cadence Owner | Notes Location |
|---|---|---|---|
| Tuesdays after class | In person / Zoom | Example: Project Coordinator | `/docs/team/meetings/` |
| Fridays asynchronous | GitHub issue / PR review | Example: Review Lead | GitHub Issues and Pull Requests |

## Schedule Risks

| Risk | Impact | Mitigation |
|---|---|---|
| Review is delayed until the end of the cycle | Late defects and weak release evidence | Require PR review throughout the week |
| Test evidence appears after feature claims | Release claims become hard to defend | Tie tests to traceability and release notes |
| Operational evidence is deferred too long | Failures are hard to diagnose during release review | Add logging and observability checkpoint |

## Reviewability Check

Another engineering team should be able to inspect the schedule evidence and understand the current release trajectory and major delivery assumptions.
