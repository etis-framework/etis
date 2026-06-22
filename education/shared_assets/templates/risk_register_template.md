# Risk Register Template

**Classification:** ETIS Educational Ecosystem Shared Asset  
**Category:** Template  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/planning/risk-register.md`  
**Primary Evidence Owner:** Planning & Process Lead, with backup owner identified in the role matrix

## Purpose

This template tracks risks that could affect scope, schedule, quality, security, governance, team performance, operational readiness, or release readiness.

A risk register is a living engineering artifact. It should help the team see uncertainty early, assign ownership, choose mitigation actions, and make honest release decisions.

---

## Engineering Guidance

Keep the risk register current throughout both cycles. A stale risk register is not useful evidence.

Use plain language. A reviewer should understand the risk, trigger, mitigation, owner, and current status without interviewing the team.

Any team member may add or update a risk. The assigned owner is responsible for keeping the risk accurate at assignment and release checkpoints.

AI may be used to brainstorm missing risks, but the team must decide which risks are real, relevant, and in scope.

Risks should remain visible, actionable, and connected to engineering evidence, workflow maturity, operational understanding, and release decisions.

Risk artifacts should support engineering review, release readiness, governance awareness, and operational understanding. They should not merely create the appearance of process maturity.

Another engineering team should be able to inspect the risk evidence and understand major engineering, governance, operational, and release concerns without relying on private explanation from the original team.

---

## Project Information

| Item | Team Response |
|---|---|
| Project Name |  |
| Team Number / Team Name |  |
| Repository URL |  |
| Cycle / Assignment |  |
| Last Updated |  |
| Primary Owner |  |
| Backup Owner |  |

---

## Risk Register

Use this table as a living artifact. Add, close, or update risks as evidence changes.

Some risks may justify scope reduction, additional review, release delay, operational mitigation, or deferred functionality before release approval.

Significant risks should remain traceable through issues, pull requests, ADRs, release notes, postmortems, operational evidence, or related repository workflow artifacts when appropriate.

| ID | Risk Description | Category | Trigger / Early Warning | Probability | Impact | Mitigation / Response | Owner | Status | Evidence / Link |
|---|---|---|---|---|---|---|---|---|---|
| R-001 | Team is unfamiliar with selected framework, slowing implementation. | Technical / Schedule | Prototype task takes more than estimated or blocks another story. | Medium | High | Create small spike issue; assign two students; document decision and learning. | Planning Lead | Open | Issue #8; ADR-001 |
| R-002 | AI-assisted implementation may introduce behavior the team cannot adequately explain, review, govern, validate, or operationally support. | AI / Quality | PR contains code no team member can walk through. | Medium | High | Require AI-use disclosure, reviewer walkthrough, and test evidence before merge. | Quality Lead | Monitoring | AI log; PR checklist |
| R-003 | Cycle 1 scope may be too broad for available team capacity. | Scope | Multiple stories remain unstarted one week before release prep. | High | High | Cut lower-priority features; protect vertical slice; update release notes. | Team Lead | Open | `scope.md`; backlog |
| R-004 | Demo path depends on manual setup that may fail during presentation. | Release | System requires unclear local steps or missing seed data. | Medium | Medium | Document setup steps; create seed data; rehearse demo; capture fallback screenshots. | Operations & Evidence Lead | Open | README; `demo-script.md` |
| R-005 | Private or sensitive data is accidentally used in testing. | Security / Governance | Real names, IDs, grades, or private records appear in repo or prompts. | Low | High | Use synthetic data only; review test data; document data rule in architecture. | Architecture & Development Lead | Monitoring | `data-context.md` |
| R-006 | Runtime failures are difficult to diagnose because of weak logging or observability evidence. | Operations / Observability | Team cannot explain or reproduce important failures during testing or review. | Medium | Medium | Improve logging, runtime diagnostics, operational evidence, and troubleshooting guidance. | Operations & Evidence Lead | Monitoring | `/docs/observability/` |
|  |  |  |  |  |  |  |  |  |  |

---

## Risk Categories

| Category | Use When |
|---|---|
| Scope | The team may be trying to build too much or has unclear boundaries. |
| Schedule | Work may not finish because of dependencies, availability, or late integration. |
| Technical | Technology, architecture, API, integration, or implementation risk exists. |
| Quality | Testing, validation, defects, reliability, or maintainability risk exists. |
| AI | AI-assisted work may introduce hallucinations, weak tests, unclear logic, or scope creep. |
| Security / Governance | Permissions, private data, auditability, approval, or unsafe action risk exists. |
| Team / Process | Ownership, communication, meetings, reviews, or contribution risk exists. |
| Release / Operations | Demo, deployment, setup, observability, logging, runtime diagnostics, recovery behavior, supportability, operational maturity, or known limitation risk exists. |

---

## Risk Status Values

Accepted risks should still remain visible and documented in release notes, operational guidance, or presentation evidence when they materially affect release behavior or limitations.

| Status | Meaning |
|---|---|
| Open | Risk is active and needs monitoring or action. |
| Monitoring | Risk is possible; owner is watching triggers. |
| Mitigating | Team is actively reducing probability or impact. |
| Accepted | Team consciously accepts the risk and documents why. |
| Closed | Risk no longer applies or has been resolved with evidence. |

---

## Checkpoint Questions

- What is the highest risk this week?
- What changed since the last checkpoint?
- Which risk is most likely to affect the release?
- Which risk should be converted into an issue, test, ADR, or known limitation?
- Which risks should be discussed in the presentation or release notes?
- Which risks could affect operational stability, observability, recovery behavior, or release defensibility?

---

## Bottom Line

Risk evidence should make uncertainty visible while there is still time to act. A strong risk register helps the team make better scope, quality, release, governance, and operational decisions.
