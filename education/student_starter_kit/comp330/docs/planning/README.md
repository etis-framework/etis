<!--
COMP 330 Instructional Example Artifact

This Markdown file is an instructional example showing professional engineering evidence patterns, workflow visibility, repository organization, and planning/governance expectations.

Teams should adapt this structure to their actual project, repository evidence, risks, workflow, and operational maturity. Do not preserve the example entries unchanged.

The authoritative operational version of this artifact belongs inside the team GitHub repository and should evolve throughout the semester.
-->

# Planning Package Example

**Purpose:** Index the team’s planning evidence for the current development cycle.

**Typical repository location:** `/docs/planning/README.md`

## Engineering Guidance

Planning artifacts are living engineering evidence that evolve as requirements, risks, defects, tests, estimates, architecture decisions, and operational understanding change.

These artifacts should support engineering coordination, workflow visibility, release planning, operational understanding, and reviewability — not merely create the appearance of process maturity.

Important planning decisions, scope changes, risks, and release assumptions should remain discoverable through the repository README and related engineering evidence when appropriate.

Planning answers one engineering question:

> How will we organize engineering work responsibly?

Planning is not project management bureaucracy.

Planning is engineering accountability.

Good planning creates visibility.

Good planning creates focus.

Good planning creates realistic expectations.

Good planning continuously adapts as evidence changes.

The planning workflow intentionally follows this progression:

```text
Scope

↓

Traceability

↓

Task Planning

↓

Estimates

↓

Risks

↓

Schedule

↓

Re-estimation
```

Planning should continuously become more accurate as engineering evidence accumulates.

Planning should reduce uncertainty, not create false certainty.

## Planning Artifacts

| Artifact | Purpose | Current Status | Owner |
|---|---|---|---|
| [`scope.md`](scope.md) | Defines what is in scope, out of scope, and intentionally deferred | Draft / Current / Needs update | Example: Planning Lead |
| [`traceability.md`](traceability.md) | Connects requirements to issues, tasks, tests, PRs, release evidence, and operational findings | Draft / Current / Needs update | Example: Requirements Lead |
| [`task-plan.md`](task-plan.md) | Lightweight work decomposition and iteration plan | Draft / Current / Needs update | Example: Project Coordinator |
| [`estimates.md`](estimates.md) | Estimate ranges, assumptions, confidence, and risk triggers | Draft / Current / Needs update | Example: Planning Lead |
| [`risk-register.md`](risk-register.md) | Tracks major risks, triggers, mitigations, owners, and status | Draft / Current / Needs update | Example: Risk Owner |
| [`schedule.md`](schedule.md) | Milestones, checkpoints, review windows, and target dates | Draft / Current / Needs update | Example: Delivery Lead |
| [`re-estimation.md`](re-estimation.md) | Records planning changes based on evidence and learning | Draft / Current / Needs update | Example: Planning Lead |

## Planning Summary

Example summary:

> Cycle 1 focuses on a narrow request-submission workflow using synthetic data. The team is intentionally deferring live university-system integration, AI recommendation behavior, and administrative analytics until stronger requirements, validation evidence, and governance boundaries exist. Current top risks are integration effort, AI-review quality, and limited runtime diagnostic visibility.

## Current Planning Priorities

| Priority | Reason | Related Evidence |
|---|---|---|
| Complete the request-submission vertical slice | Establish a working end-to-end workflow before expanding scope | FR-001, Issue #1, PR #5 |
| Keep AI category suggestion deferred | Governance and validation evidence are not mature enough | D-001, Risk R-003 |
| Improve basic runtime diagnostics | Failures need to be diagnosable during release review | Risk R-004, `/docs/observability/` |

## Reviewability Check

Another engineering team should be able to inspect the planning evidence and understand the project direction, priorities, and major risks without relying on private explanation from the original team.
