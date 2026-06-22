# Defect Log Template

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Template  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/quality/defect-log.md` or `/docs/testing/defect-log.md`

## Purpose

This template records defects found during review, testing, integration, demonstrations, AI-assisted development, release preparation, or operational rehearsal.

A defect is a discovered gap between expected behavior and actual behavior. The purpose of the defect log is not to shame the team. The purpose is to manage quality honestly and preserve evidence that supports review, release decisions, operational understanding, and quality transparency.

A successful demonstration does not eliminate unresolved defects, operational risks, governance concerns, or release limitations. The defect log should reflect the actual engineering state of the system.

---

## Artifact Ownership

| Field | Team Response |
|---|---|
| Project Name | |
| Team Number / Team Name | |
| Repository URL | |
| Cycle / Assignment | |
| Last Updated | |
| Primary Owner | Quality & Review Lead |
| Backup Owner | |

Any team member may report or update a defect. The assigned owner is responsible for ensuring the defect record is accurate at review and release checkpoints.

---

## Engineering Guidance

- Do not hide defects. Classify them and manage them.
- Use GitHub Issues for active defect work.
- Use this log as the evidence summary that tracks severity, status, owner, disposition, and release impact.
- Important defects, known limitations, release blockers, and mitigation evidence should remain discoverable through the repository README, release notes, and related engineering evidence.
- Defects may be fixed, mitigated, deferred, accepted, or removed from scope. The decision must be visible and defensible.
- Some defects may justify scope reduction, additional review, operational mitigation, release delay, or explicit known-limitation disclosure before release approval.
- AI-assisted implementation may accelerate feature creation while also increasing review, debugging, governance, testing, and operational validation workload.

Another engineering team should be able to inspect the defect evidence and understand major quality risks, release limitations, mitigation decisions, and operational concerns without relying on private explanation from the original team.

---

## Defect Log

Active work should also be tracked in GitHub Issues.

Significant defects should remain traceable through issues, pull requests, tests, reviews, release notes, postmortems, operational evidence, or related workflow artifacts when appropriate.

| ID | Defect Summary | Found In | Severity | Steps / Evidence | Owner | Status | Disposition | Related Issue / PR | Release Impact |
|---|---|---|---|---|---|---|---|---|---|
| D-001 | Request form accepts blank category. | Manual system test | Medium | Submit request with empty category; request is saved. | Quality Lead | Open | Fix before Cycle 1 release | Issue #__ | Blocks clean demo path |
| D-002 | Reviewer status update does not refresh student view until page reload. | Integration test / demo rehearsal | Low | Update status as reviewer; student view remains stale. | Developer | Mitigating | Document workaround or fix if time permits | Issue #__; PR #__ | Known limitation if not fixed |
| D-003 | AI-generated validation test only checks happy path. | AI code review | Medium | Generated test passes but misses invalid input case. | Quality Lead | Closed | Added negative test and updated AI-use log | PR #__ | Improved validation evidence |
| D-004 | Seed data setup steps are unclear for a new reviewer. | Release rehearsal | Low | Teammate cannot run demo without help. | Operations & Evidence Lead | Open | Update README and demo script | Issue #__ | Could affect presentation |
| D-005 | Unauthorized user can see admin page link in navigation. | Security review | High | Login as student role; admin link is visible. | Architecture & Development Lead | Open | Fix or remove before release | Issue #__ | Release blocker unless corrected |
| D-006 | Runtime failure logs do not contain enough detail to diagnose production-like issues. | Operational review / failure rehearsal | Medium | Failure reproduced but root cause unclear from logs. | Operations & Evidence Lead | Monitoring | Improve logging and operational diagnostics before final release. | Issue #__ | Weakens operational supportability |

---

## Severity Levels

| Severity | Meaning |
|---|---|
| Critical | System cannot be demonstrated, data may be unsafe, or a major workflow is unusable. |
| High | Core workflow, security, governance, operational supportability, observability, or release readiness is seriously affected. |
| Medium | Important behavior is incorrect or incomplete, but workaround or bounded impact exists. |
| Low | Minor defect, usability issue, documentation gap, or polish item. |

---

## Defect Status and Disposition

| Term | Meaning |
|---|---|
| Open | Defect has been identified but not resolved. |
| In Progress | Owner is actively working on the defect. |
| Closed | Fix, mitigation, or disposition has been completed and evidence exists. |
| Fixed | Code or artifact changed and test/review evidence supports closure. |
| Mitigated | Impact was reduced, but the defect may not be fully fixed. |
| Deferred | Team intentionally postpones the defect and documents why. |
| Accepted | Team accepts the defect and documents release impact, rationale, and risk. |
| Removed from Scope | Requirement or feature was intentionally removed to protect release stability, engineering quality, or operational maturity. |

Accepted or deferred defects should remain visible through release notes, operational guidance, presentation evidence, or known limitations when they materially affect release behavior or user expectations.

---

## Defect Review Questions

- Which defects block the Cycle 1 or final release?
- Which defects require tests or regression evidence?
- Which defects should appear in release notes as known limitations?
- Which defects were introduced or discovered through AI-assisted work?
- Which defects indicate a requirements, architecture, workflow, or review problem?
- Which defects affect operational supportability, observability, recovery, or security/governance?
- Which defects should trigger a postmortem action or Cycle 2 maturity target?

---

## Final Takeaway

A defect log is not a list of failures. It is evidence of quality discipline.

Professional teams do not hide defects. They classify them, assign owners, connect them to evidence, disposition them honestly, and use them to improve release judgment.
