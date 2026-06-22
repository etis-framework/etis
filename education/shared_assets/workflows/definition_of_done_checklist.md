# Definition of Done Checklist

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Workflow  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/release/definition-of-done.md`

## Purpose

Use this checklist before each major cycle delivery, release package, or presentation.

The checklist helps a team decide whether work is actually done, not merely coded, demonstrated once, or documented after the fact.

The repository remains the authoritative evidence source.

Another engineering team should be able to inspect the repository evidence and understand what changed, what was reviewed, what was tested, what risks remain, and why the current release is defensible.

---

## Team and Delivery Information

| Field | Team Response |
|---|---|
| Team Number / Name | |
| Repository URL | |
| Delivery / Assignment | |
| Release / Cycle | |
| Checklist Date | |
| Checklist Owner | |

---

## How to Use This Checklist

- Complete this checklist before submitting a cycle package or presenting a release.
- Mark an item done only when the team can point to repository evidence.
- If an item is not applicable, mark it `N/A` and briefly explain why.
- If an item is incomplete, record the gap, owner, risk, and next action.
- Do not treat the checklist as paperwork. Use it as a release-readiness control.
- A completed checklist should reflect the actual engineering state of the release, including known limitations, unresolved risks, operational concerns, and deferred work.

---

## Definition of Done Checklist

A delivery is done when the team can explain what changed, why it changed, what evidence supports it, what risks remain, and who owns the next action.

| Done? | Check Area | Definition of Done | Evidence Location | Owner |
|---|---|---|---|---|
| ☐ | Scope and Requirements | Completed work is tied to current requirements, acceptance criteria, and intentionally deferred scope. | `/docs/requirements/`; `/docs/planning/traceability.md` | |
| ☐ | Task and Issue Traceability | Major work items connect to issues/tasks, owners, branches, commits, and pull requests. | GitHub Issues, PRs, `/docs/planning/traceability.md` | |
| ☐ | Architecture Fit | Implementation remains consistent with the architecture or documented architecture changes and ADRs. | `/docs/architecture/`; `/docs/decisions/` | |
| ☐ | Code and Configuration | Code/config changes are committed, organized, readable, and free of obvious dead code, secrets, or local-only assumptions. | `/src/`; `/scripts/`; config files; PR diffs | |
| ☐ | Pull Request Review | Meaningful changes were reviewed before merge, with comments, risks, decisions, or rationale visible. | GitHub Pull Requests; review comments | |
| ☐ | Testing Evidence | Relevant unit, integration, system, manual, regression, or AI validation evidence exists and is current. | `/docs/testing/`; `/tests/`; `/test-evidence/` | |
| ☐ | CI/CD Evidence | Build/test workflow status is visible; failed, skipped, or missing checks are explained. | `/.github/workflows/`; `/docs/testing/ci-evidence.md` | |
| ☐ | Defect Status | Known defects are logged, classified, owned, and dispositioned as fixed, mitigated, deferred, accepted, or removed from scope. | `/docs/quality/defect-log.md` | |
| ☐ | AI Use and Verification | AI-assisted work is disclosed, reviewed, modified as needed, and verified by humans. | `/docs/ai/ai-use-log.md`; PR notes | |
| ☐ | Security and Data Handling | Sensitive data, permissions, dependencies, external services, and AI/tool boundaries have been reviewed. | `/docs/security/`; risk register | |
| ☐ | Observability / Operations | Important runtime behavior, failures, setup, recovery, and operational support notes are documented where relevant. | `/docs/observability/`; `/docs/operations/runbook.md` | |
| ☐ | Recovery / Rollback Readiness | Important failures, risky changes, or degraded dependencies have a documented recovery, rollback, disablement, or safe-mode path where appropriate. | `/docs/operations/runbook.md`; release notes; rollback notes | |
| ☐ | Release Notes / Known Limits | Release notes explain what changed, what works, known limitations, residual risks, and next steps. | `/docs/release/release-notes.md`; known limitations | |
| ☐ | README / Navigation | README and repository navigation help another engineer understand, run, test, and review the project. | `README.md`; docs README files | |
| ☐ | Presentation Readiness | Presentation claims are backed by repository evidence, demo path is rehearsed, and backup evidence exists. | `/docs/release/presentation-index.md`; demo script | |

---

## Gap / Risk Log

Use this table for any checklist item that is incomplete, risky, deferred, or intentionally accepted for the current delivery.

| Item | Gap / Risk | Impact | Owner | Disposition | Next Action / Evidence |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## Final Readiness Decision

Select one.

- [ ] Ready to submit / present: all critical items are complete, evidence exists, and remaining risks are documented.
- [ ] Ready with known limitations: the release is defensible, but limitations, mitigations, and deferred work must be clearly stated.
- [ ] Not ready: a critical build, test, demo, security, evidence, or ownership gap must be corrected before submission or presentation.

| Field | Team Response |
|---|---|
| Final Readiness Decision | |
| Decision Rationale | |
| Approved By / Team Role | |
| Date | |

The rationale should explain remaining risks, mitigations, operational concerns, deferred work, and why the current release remains defensible.

---

## Final Takeaway

Done means reviewable, testable, traceable, governable, and explainable.

If the team cannot point to evidence, the work is not professionally done yet.
