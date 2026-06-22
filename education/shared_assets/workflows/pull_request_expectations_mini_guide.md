# Pull Request Expectations Mini Guide

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Workflow  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/workflow/pull-request-expectations.md`

## Purpose

Use this guide when opening, reviewing, and merging pull requests in a team repository.

Pull requests are where private work becomes reviewable team-owned engineering evidence.

A pull request should explain what changed, why it changed, how it was tested, what risks remain, and what AI assistance was used or verified.

Important pull requests should remain traceable through linked requirements, issues, tests, defects, ADRs, release notes, AI-use evidence, operational artifacts, and known limitations when appropriate.

Another engineering team should be able to understand what changed, why it changed, what evidence supports it, what risks remain, and how the change affects the release without relying on private explanation from the original author.

---

## When to Open a Pull Request

Open a pull request when a focused unit of work is ready for team review.

Teams should:

- Keep pull requests small enough for another student to review seriously.
- Link the pull request to a requirement, issue, task, defect, or release item whenever possible.
- Avoid using pull requests as a last-minute dumping ground for unrelated changes.
- Prefer smaller, reviewable pull requests over large multi-purpose merges that reviewers cannot realistically evaluate.

---

## Pull Request Minimum Content

| Required Item | What Reviewers Should See |
|---|---|
| Purpose | A short explanation of the problem, requirement, defect, or task this pull request addresses. |
| Linked evidence | Issue, requirement, task, defect, ADR, test case, or release note connection when applicable. |
| Change summary | A concise list of the files or behaviors changed. |
| Testing / verification | Tests run, manual checks performed, CI/CD results, screenshots, logs, or known test gaps. |
| Risk notes | Anything reviewers should inspect carefully: architecture fit, edge cases, security, data handling, AI output, dependency changes, operational impact, observability impact, rollback concerns, supportability implications, or known limitations. |
| AI disclosure | What AI helped produce or review, what the team accepted or changed, and how the result was verified. |

---

## Good Pull Request Size

| Strong Pattern | Weak Pattern |
|---|---|
| One focused issue or feature path. | Several unrelated features, fixes, formatting changes, and documentation edits mixed together. |
| Reviewable diff that another team member can understand in one sitting. | Large diff that reviewers approve without actually understanding. |
| Clear test or evidence connection. | No clear way to tell whether the change was validated. |
| Architecture or requirement impact is explained. | Design impact is hidden inside code changes. |
| Review discussion reveals real engineering questions, clarification, or validation. | “LGTM” approval without meaningful review evidence. |

---

## Author Responsibilities Before Requesting Review

Before requesting review, the author should:

- Confirm the branch builds or runs as expected.
- Run relevant tests or clearly explain why tests were not run.
- Update related documentation, requirements, test evidence, defect logs, AI-use logs, or release notes when needed.
- Identify known limitations, risks, or follow-up work honestly.
- Ask reviewers to focus on specific concerns when the change has risk.
- Ensure the branch does not introduce undocumented operational assumptions, hidden configuration dependencies, or unrecoverable deployment behavior.

---

## Reviewer Responsibilities

| Review Area | Reviewer Question |
|---|---|
| Requirement fit | Does the change match the intended requirement, acceptance criterion, defect, or task? |
| Architecture fit | Does the change respect component responsibilities, interfaces, data ownership, and design decisions? |
| Correctness | Does the change handle normal, boundary, and failure cases? |
| Testing evidence | Do the tests or manual evidence support the claim? What remains untested? |
| Security / governance | Does the change affect permissions, data handling, approval boundaries, dependencies, or AI/tool authority? |
| Maintainability | Can the team understand, maintain, diagnose, and safely change this later? |
| Operational impact | Are observability, rollback, recovery, supportability, or deployment concerns visible when relevant? |
| AI accountability | If AI helped, was the output reviewed, modified where needed, tested, and owned by the team? |

---

## Merge Expectations

Do not merge only because the demo path works once.

Do not merge unresolved high-risk review concerns.

Do not merge AI-generated code that the team cannot explain, test, or maintain.

Merge only when the change is reviewed, validated, traceable, and safe enough to keep.

If a known risk remains, document it in the appropriate artifact before or immediately after merge.

Do not merge changes that reviewers cannot adequately explain, test, diagnose, or support operationally.

---

## Recommended Pull Request Template

The sample text below may be copied into `.github/pull_request_template.md`.

```markdown
## Purpose

What issue, requirement, defect, or task does this pull request address?

## Summary of Changes

- 
- 
- 

## Evidence / Testing

- Tests run:
- Manual checks:
- CI/CD evidence:
- Known gaps:
- Operational or observability impact:

## Review Focus

Please pay special attention to:

- 

## AI Assistance

- AI used? Yes / No
- What AI helped with:
- What humans changed or rejected:
- Verification performed:

## Risks / Follow-Up

- Known limitations:
- Deferred work:
- Related release note or defect entry:
```

---

## Quick Quality Gate

| Before Merge | Yes / No / N/A |
|---|---|
| Purpose and scope are clear. | |
| Linked issue, requirement, defect, or task is included where applicable. | |
| Relevant tests or manual evidence are documented. | |
| CI/CD status is visible or limitations are explained. | |
| AI assistance is disclosed and verified where applicable. | |
| Security, dependency, data, or governance concerns are reviewed. | |
| Operational, observability, rollback, or deployment concerns are documented where relevant. | |
| Documentation, test evidence, or release notes are updated if affected. | |
| Remaining risks or deferred work are visible. | |

---

## Final Takeaway

A pull request is not just a code diff.

It is a professional review gate that connects intent, implementation, evidence, AI accountability, and merge judgment.
