<!--
COMP 330 Instructional Example Artifact

This Markdown file is an instructional example showing professional engineering evidence patterns, workflow visibility, repository organization, and planning/governance expectations.

Teams should adapt this structure to their actual project, repository evidence, risks, workflow, and operational maturity. Do not preserve the example entries unchanged.

The authoritative operational version of this artifact belongs inside the team GitHub repository and should evolve throughout the semester.
-->

# Scope Example

**Purpose:** Defines what the team is building now, what is intentionally out of scope, and what may be deferred for later.

**Typical repository location:** `/docs/planning/scope.md`

## Engineering Guidance

Scope decisions should support engineering focus, release defensibility, operational stability, and realistic delivery expectations.

Strong engineering teams intentionally defer risky, poorly understood, weakly validated, or weakly governed features rather than overcommit beyond their evidence and review capacity.

Scope artifacts should support release decisions and engineering coordination — not justify unrealistic feature volume or presentation-driven commitments.

## Cycle Target

| Item | Description |
|---|---|
| Current cycle | Cycle 1 |
| Release goal | Demonstrate a narrow, reviewable student-support request workflow using synthetic data |
| Primary user workflow | Student submits a support request; staff user views and updates request status |
| Scope owner | Example: Planning Lead |
| Last updated | YYYY-MM-DD |

## In Scope

| ID | Scope Item | Reason Included | Related Requirement / Issue | Operational / Governance Concern |
|---|---|---|---|---|
| S-001 | Student can submit a support request | Required for the main vertical slice | FR-001 / #1 | Input validation and basic audit visibility required |
| S-002 | Staff user can view submitted requests | Needed to close the basic workflow loop | FR-002 / #2 | Access assumptions must be documented |
| S-003 | Request status can be updated manually | Supports visible lifecycle progress without over-automating | FR-003 / #3 | Status changes should be traceable |

## Out of Scope

| ID | Out-of-Scope Item | Reason Excluded | Possible Future Action |
|---|---|---|---|
| OOS-001 | Live integration with university systems | Requires private data, institutional approval, and stronger governance | Simulate with synthetic data |
| OOS-002 | Automated assignment of requests to real staff | Requires access control, workflow policy, and operational approval | Revisit after manual workflow is stable |
| OOS-003 | Production deployment | Course project does not have institutional production authorization | Demonstrate release-readiness evidence only |

## Deferred Candidates

Deferred work should often include features requiring additional testing, operational evidence, governance review, AI-boundary clarification, runtime visibility, or architectural maturity before acceptance.

| ID | Candidate | Evidence Needed Before Accepting | Target Cycle / Status |
|---|---|---|---|
| D-001 | AI category suggestion | Need Cycle 1 workflow evidence, validation plan, human approval boundary, and AI-use disclosure | Cycle 2 candidate |
| D-002 | Admin dashboard | Need stable request model and clear decision about useful metrics | Cycle 2 candidate |
| D-003 | Email notification simulation | Need test evidence and failure-handling assumptions | Backlog |

## Scope Review Questions

| Question | Current Answer |
|---|---|
| Is the scope small enough to engineer well? | Example: Yes, limited to one vertical slice |
| What is intentionally not being built? | Live integrations, production deployment, automatic routing |
| What evidence would justify expanding scope? | Passing tests, reviewed PRs, stable requirements, risk mitigation, operational visibility |
| What scope item creates the most release risk? | AI category suggestion, because validation and governance are immature |

## Reviewability Check

Another engineering team should be able to inspect this scope evidence and understand what the team chose to build, what it intentionally deferred, and why those boundaries support release defensibility.
