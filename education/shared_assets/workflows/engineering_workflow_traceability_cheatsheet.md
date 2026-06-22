# Engineering Workflow and Traceability Cheatsheet

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Workflow  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/workflow/engineering-workflow-traceability.md`

## Core Idea

Professional software engineering creates explainable history.

Every meaningful change should have a visible reason, a controlled branch, a reviewed pull request, supporting evidence, and a traceable release story.

---

## Why Traceability Matters

Traceability is the connection between intent, work, review, evidence, and release.

It lets another engineer answer:

- What changed?
- Why did it change?
- Who reviewed it?
- What evidence proves it works?
- Where is that evidence stored?

Traceability prevents invisible work from entering the project.

It connects requirements to issues, pull requests, tests, reviews, release notes, and operational evidence.

It makes AI-assisted work reviewable, explainable, and accountable.

It turns a demo claim into an engineering claim.

---

## Simple Professional Workflow Rule

```text
No issue → no branch → no pull request → no review → no merge.
```

This is not GitHub bureaucracy.

It is the minimum workflow needed to make team software visible, reviewable, and governed.

Direct commits to `main`, undocumented changes, or unreviewed AI-generated code weaken traceability and team accountability.

---

## Traceability Chain

| Step | Artifact | Purpose |
|---:|---|---|
| 1 | Requirement | What the system must do and how success is judged. |
| 2 | Issue | The specific task, defect, enhancement, or question to work on. |
| 3 | Branch | Isolated workspace tied to the issue. |
| 4 | Pull Request | Reviewable proposed change linked to issue and evidence. |
| 5 | Review + Tests | Human review, CI status, test notes, risk comments, AI disclosure. |
| 6 | Release Evidence | Release notes, known limitations, demo script, postmortem learning. |

---

## Example End-to-End Flow

| Artifact | Example |
|---|---|
| Requirement | REQ-03: Reviewer can approve or reject a request only after required fields are complete. |
| GitHub Issue | #42: Enforce required-field validation before approval. |
| Branch | `issue-42-approval-validation` |
| Pull Request | PR #18: Adds approval validation and tests. Includes `Closes #42`. |
| Review Evidence | Reviewer checks requirement fit, code, tests, security, AI use, and architecture consistency. |
| Test Evidence | T-07: Missing required fields block approval; CI run passes. |
| Release Evidence | `release-notes.md` identifies the approved workflow, validation evidence, and known limitations. |

---

## What Goes Where in GitHub

| Item | Where It Lives | Purpose |
|---|---|---|
| Ideas, tasks, defects, enhancements | GitHub Issues | Operational work queue. Issues explain why work exists. |
| Branches | Git branches | Safe isolated work areas tied to issues. |
| Pull requests | GitHub Pull Requests tab | Review gate before changes enter main. |
| Requirements | `/docs/requirements/` | Defines what the system must do and how acceptance is judged. |
| Planning and traceability | `/docs/planning/` | Scope, task plan, estimates, risks, schedule, traceability, and re-estimation. |
| Architecture and decisions | `/docs/architecture/` and `/docs/decisions/` | System structure and decision reasoning. |
| Testing and quality | `/docs/testing/` and `/docs/quality/` | Test strategy, test evidence, defects, CI evidence, and validation notes. |
| AI accountability | `/docs/ai/` | AI policy, AI-use log, verification notes, and disclosure evidence. |
| Release evidence | `/docs/release/` | Release notes, known limitations, presentation index, demo script, and final evidence package. |

---

## Issue, Branch, and Pull Request Naming

| Artifact | Recommended Form | Example |
|---|---|---|
| Issue title | Short action-oriented title | Fix approval validation edge case |
| Branch name | `issue-[number]-short-description` | `issue-42-approval-validation` |
| Pull request title | Clear summary of the change | Fix approval validation for required fields |
| Commit message | Concise change statement with issue reference | Fix approval validation for issue #42 |

---

## Pull Request Evidence Checklist

A pull request should make the change reviewable without requiring a private explanation in chat.

- Linked issue number, such as `Closes #42`.
- Short summary of what changed and why.
- Requirement or artifact path affected by the change.
- Tests run, CI status, or manual validation evidence.
- AI assistance disclosure, if applicable.
- Known limitations, risks, or follow-up work.
- Reviewer comments and author responses when changes are requested.

---

## Review Expectations

| Reviewer Asks | Why It Matters |
|---|---|
| Does this satisfy the issue or requirement? | Prevents random work from entering the system. |
| Is the change small enough to understand? | Large changes hide defects and weaken accountability. |
| Are tests or evidence included? | A claim without evidence is just an opinion. |
| Does the change fit the architecture? | Prevents design drift and accidental complexity. |
| Is AI use disclosed and verified? | Generated work still belongs to the team. |
| Can the team explain and maintain this later? | Professional engineering must survive beyond the author of the change. |

---

## Common Mistakes to Avoid

| Mistake | Why It Hurts the Team |
|---|---|
| Working directly on main | No safe separation of unfinished work and no review gate. |
| Doing work only discussed in chat | The work becomes invisible to the repository evidence trail. |
| Opening a pull request with no issue link | Reviewers cannot trace why the change exists. |
| Merging without test or validation evidence | The team relies on confidence instead of proof. |
| Using AI-generated code no one can explain | The team owns the risk even if AI produced the text. |
| Creating many empty placeholder files | This creates artifact theater instead of useful engineering evidence. |

---

## Final Student Rule

Before merge, answer five questions:

```text
What changed?
Why did it change?
Who reviewed it?
What evidence proves it works?
Where is that evidence stored?
```

---

## Final Takeaway

The repository is not just file storage.

It is the team’s engineering evidence system.

Strong teams make their work easy to inspect, review, explain, and improve.
