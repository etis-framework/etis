<!--
COMP 330 Instructional Example Artifact

This Markdown file is an instructional example showing professional engineering evidence patterns, workflow visibility, repository organization, and planning/governance expectations.

Teams should adapt this structure to their actual project, repository evidence, risks, workflow, and operational maturity. Do not preserve the example entries unchanged.

The authoritative operational version of this artifact belongs inside the team GitHub repository and should evolve throughout the semester.
-->

# Traceability Example

**Purpose:** Connects requirements to tasks, GitHub Issues, Pull Requests, tests, operational findings, and release evidence.

**Typical repository location:** `/docs/planning/traceability.md`

## Engineering Guidance

Traceability evidence should remain discoverable through the repository README, linked engineering artifacts, pull requests, and release evidence when appropriate.

Traceability should make it possible for another engineering reviewer to understand how important system behavior, risks, and release claims were validated.

## Traceability Table

| Requirement ID | Requirement Summary | GitHub Issue(s) | Task / Work Item | PR / Commit Evidence | Test / Validation / Operational Evidence | Release Evidence | Status |
|---|---|---|---|---|---|---|---|
| FR-001 | Student can submit a support request | #1 | WB-001: Build request form and validation | PR #5 | TC-001, TC-002, validation screenshot | Release Notes v0.1 | In progress |
| FR-002 | Staff user can view submitted requests | #2 | WB-004: Build request list view | PR #7 | TC-003, review notes | Release Notes v0.1 | Planned |
| FR-003 | Staff user can update request status | #3 | WB-006: Add manual status update | PR #9 | TC-004, defect D-002 | Release Notes v0.1 | Planned |
| NFR-001 | Important failures are diagnosable | #12 | WB-010: Add basic runtime logging | PR #14 | Log screenshot, operational review note | Known limitation / Release Notes | Open |

## Traceability Notes

- Every major requirement should eventually connect to issues, tasks, branches, pull requests, reviews, tests, release evidence, and operational findings when applicable.
- Every completed feature should connect to review, test, and release evidence.
- If a requirement is deferred, explain why and where that decision is recorded.
- AI-assisted implementation work should remain traceable through issues, pull requests, review evidence, AI-use logs, validation evidence, and release documentation when applicable.

## Deferred / Removed Requirements

| Requirement ID | Decision | Reason | Evidence / Decision Record |
|---|---|---|---|
| FR-999 | Deferred | Live student information system integration requires private data and institutional approval | Scope OOS-001; Risk R-005; ADR-003 |
| AI-001 | Deferred | AI category suggestion lacks sufficient validation and governance evidence for Cycle 1 | Scope D-001; AI-use log; Risk R-003 |

## Traceability Gaps

| Gap | Impact | Owner | Next Action |
|---|---|---|---|
| NFR-001 has limited evidence | Runtime failures may be hard to explain during release review | Example: Quality Lead | Add logging task and operational evidence |
| FR-003 lacks reviewed PR | Status workflow cannot be claimed as release-ready yet | Example: Development Lead | Complete PR and validation evidence |

## Reviewability Check

Another engineering team should be able to inspect the traceability evidence and understand how requirements evolved into implemented, reviewed, tested, and released engineering behavior.
