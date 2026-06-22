# GitHub Workflow and Traceability Quick Reference

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Workflow  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/workflow/github-workflow-traceability.md`

## Purpose

Use this quick reference while working.

It is not a substitute for engineering judgment. It is a reminder of the minimum workflow and traceability habits expected in an ETIS-aligned student engineering repository.

---

## Professional Workflow

```text
Issue → Branch → Commit → Pull Request → Review → Checks → Merge → Evidence Updated
```

| Step | Minimum Evidence |
|---|---|
| Issue | Why the work exists, what outcome is expected, owner, priority, and related requirement if applicable. |
| Branch | Clear branch name tied to purpose or issue, such as `feature/12-login-validation`. |
| Commit | Meaningful commit messages describing engineering changes. |
| Pull Request | Summary, linked issue, tests performed, risks, AI use, screenshots/logs if useful. |
| Review | Another team member checks correctness, tests, risk, architecture fit, AI use, and evidence. |
| Checks | CI or validation evidence is visible and passing, or failures are explained honestly. |
| Merge | Approved changes merge to `main`; related docs/evidence are updated. |

---

## Linking Syntax

| Need | Use This |
|---|---|
| Reference an issue | `Issue #12` or `#12` |
| Close an issue from PR | `Closes #12` |
| Reference a PR | `PR #8` |
| Reference a commit | Use the short commit hash or GitHub commit link |
| Reference evidence file | Link directly to `/docs/...` file in the repository |
| Reference test evidence | Link to CI run, test file, or `/test-evidence/` artifact |

---

## Pull Request Checklist

- What changed?
- Why was the change needed?
- What issue, requirement, risk, or defect does it connect to?
- What tests or validation were performed?
- What architecture or security concerns exist?
- Was AI used materially? If yes, is the AI-use log updated?
- Are dependencies or configuration changes reviewed?
- Is documentation or release evidence updated if needed?
- Is the change small enough to review responsibly?
- Why was the change considered safe enough to merge into the operational system?

---

## What Good Traceability Looks Like

```text
Requirement
  → Acceptance Criteria
  → Issue
  → Branch
  → Pull Request
  → Review
  → Tests
  → Release Notes
  → Release Version / Tag
  → Known Limitations
```

---

## Assignment Evidence Map

| Assignment | Evidence to Check Before Submission |
|---|---|
| A1 | README, team charter, roles, working agreements, AI policy, initial requirements, GitHub setup. |
| A2 | Planning docs, scope, task plan, estimates, schedule, risk register, traceability, issues/milestones. |
| A3 | Architecture overview, component responsibilities, API contracts, diagram, architecture review, security/governance notes. |
| A4 | Changed files, PRs, reviews, CI workflow, test evidence, AI code review, dependency review, defect visibility. |
| A5 | Release notes, known limitations, final test evidence, defect log, presentation index, traceability summary. |
| A6 | Runbook, observability evidence, runtime evidence, security/governance evidence, postmortem, final release notes, residual risks, recovery expectations, and operational fallback assumptions when appropriate. |

---

## AI-Use Log Minimum Fields

| Field | Question It Answers |
|---|---|
| Tool / Date | What tool or model was used and when? |
| Task | What was AI asked to help with? |
| Accepted Output | What was accepted into the project after human review? |
| Rejected Output | What was rejected and why? |
| Human Edits | What did the team change before accepting the output? |
| Verification | What tests, reviews, comparisons, or evidence support the accepted artifact? |
| Risk / Limitation | What AI-related uncertainty remains? |
| Owner / Reviewer | Who is accountable for the correctness, governance, and operational behavior of the accepted work? |

---

## Red Flags

- Large unreviewed PRs with no linked issue.
- Claims that something works with no test evidence.
- README out of date, missing operational context, or missing evidence links.
- AI use mentioned vaguely but not traceable to accepted work and verification.
- Release notes that hide known limitations or defects.
- Architecture decisions documented only in chat, not repository evidence.
- Large architecture or operational decisions discussed only in chat or meetings without repository evidence.
- CI failing without explanation.
- Team cannot explain code, tests, or documents that AI helped produce.
- Evidence exists only for presentation appearance rather than supporting real engineering review or operational understanding.

---

## Quick Submission Review

- Can a reviewer find the assignment evidence in under two minutes?
- Are all required files current and linked from README or the submitted review package?
- Are issue, PR, test, AI-use, and release evidence connected?
- Are limitations, defects, and risks honest?
- Would another engineering team understand what happened without a private explanation?
- Is the repository evidence reviewable without requiring private explanation from the original team?

---

## Final Reminder

GitHub evidence should survive the semester.

Do not build evidence only for a deadline.

Maintain it as the project matures.
