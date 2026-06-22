# Postmortem Template

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Template  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/postmortems/cycle-1-postmortem.md`

## Purpose

Use this template after Cycle 1 and, when appropriate, after the final cycle to convert project evidence into engineering learning.

A postmortem is not a blame exercise. It is an engineering learning artifact.

The team uses evidence from the cycle to identify what happened, why it happened, what operational assumptions failed or succeeded, and what must improve next.

The postmortem should be concise, specific, evidence-based, and tied to repository artifacts.

---

## Related Evidence Locations

Postmortems should reference evidence such as:

- `/docs/planning/`
- `/docs/testing/`
- `/docs/release/`
- `/docs/quality/`
- `/docs/ai/`
- `/docs/observability/`
- `/docs/operations/`
- GitHub Issues
- Pull Requests
- Release notes
- Defect log
- Risk register

Postmortems should support engineering learning, operational understanding, and release improvement. They should not merely satisfy process expectations.

---

## Engineering Guidance

- Base claims on evidence, not memory or personal impressions.
- Separate symptoms from root causes.
- Identify what the team will change in Cycle 2 or the next release.
- Keep the tone professional and blameless while still being honest.
- Use AI as a reviewer or brainstorming aid if helpful, but the team owns the final analysis.
- Adapt this template to actual evidence, failures, risks, and improvement opportunities rather than preserving example text unchanged.

---

## 1. Team and Cycle Information

| Item | Team Response |
|---|---|
| Team Number | |
| Team Name | |
| Repository URL | |
| Cycle Reviewed | Cycle 1 / Final Cycle / Other |
| Postmortem Date | |
| Facilitator / Owner | |
| Attendees | |
| Absent Team Members | |
| Primary Evidence Reviewed | Release notes, defect log, test evidence, issues, PRs, risk register, AI-use log |

---

## 2. Executive Summary

| Prompt | Team Response |
|---|---|
| What did the team set out to accomplish? | |
| What did the team actually complete? | |
| What was the most important engineering lesson from this cycle? | |
| What must improve in the next cycle or next release? | |
| What evidence most influenced the team’s release-readiness judgment? | |
| What residual risks, deferred work, or operational limitations remained at release time? | |

---

## 3. Evidence Reviewed

| Evidence Area | Repository Path or Link | What It Showed |
|---|---|---|
| Requirements / Scope | `/docs/requirements/` | Example: some acceptance criteria were still too broad. |
| Planning / Estimates | `/docs/planning/` | Example: integration work took longer than expected. |
| Architecture / ADRs | `/docs/architecture/` and `/docs/architecture/adr/` | Example: data ownership needed clearer boundaries. |
| Issues / Pull Requests | GitHub Issues and Pull Requests | Example: some work bypassed issue tracking. |
| Testing / Defects | `/docs/testing/` and `/docs/quality/` | Example: tests covered happy path but not error cases. |
| Release Evidence | `/docs/release/` | Example: known limitations were documented clearly. |
| AI-Use Evidence | `/docs/ai/ai-use-log.md` | Example: AI was useful for test ideas but required human correction. |
| Observability / Operations | `/docs/observability/` and `/docs/operations/` | Example: runtime failures were difficult to diagnose without additional logging or operational evidence. |

---

## 4. What Went Well

| Observation | Evidence | Why It Mattered |
|---|---|---|
| Example: Weekly status meetings kept the team aligned. | Meeting notes; task board updates | Risks were identified before the release deadline. |
| | | |
| | | |

---

## 5. What Did Not Go Well

Professional engineering teams document important failures and weaknesses honestly because hidden problems usually become larger operational risks later.

| Issue / Problem | Evidence | Impact |
|---|---|---|
| Example: Pull requests were opened too late for meaningful review. | PR timestamps; release notes | Reduced time for testing and defect correction. |
| | | |
| | | |

---

## 6. Root Cause Analysis

Identify causes that the team can control or improve. Avoid stopping at symptoms such as “we ran out of time.”

Good root-cause analysis should identify controllable engineering, workflow, review, testing, communication, or operational factors rather than stopping at schedule pressure alone.

The goal is not to identify who failed. The goal is to identify what engineering systems need improvement.

| Symptom | Likely Root Cause | Evidence | Corrective Action |
|---|---|---|---|
| Example: Feature finished late | Task was too large and had hidden dependencies | Issue history; estimate notes | Break similar work into smaller issues with earlier integration checkpoint. |
| | | | |
| | | | |

---

## 7. Cycle 2 / Next Release Improvement Plan

| Improvement Candidate | Reason / Evidence | Owner | Target Evidence |
|---|---|---|---|
| Example: Add regression tests for request status changes | Defect found during demo preparation | Quality & Review Lead | `/docs/testing/final-test-evidence.md`; PR link |
| Example: Improve logging for failed request updates | Hard to diagnose runtime failure | Operations & Evidence Lead | `/docs/observability/observability-plan.md` |
| Example: Improve fallback behavior when AI suggestions fail or are unavailable | Manual recovery workflow unclear during testing | Architecture & Development Lead | `/docs/operations/`; ADR; release notes |
| | | | |

---

## 8. Team Process Review

| Question | Team Response |
|---|---|
| Did the team maintain a weekly 15-30 minute status cadence? | |
| Were roles and backups effective? | |
| Was work visible in GitHub Issues before implementation? | |
| Were pull requests reviewed before merge? | |
| Did all team members own visible engineering evidence? | |
| What team working agreement needs to change? | |

---

## 9. AI-Use Reflection

| Prompt | Team Response |
|---|---|
| Where did AI help the team most? | |
| Where did AI produce weak, wrong, incomplete, or risky output? | |
| How did the team verify AI-assisted work? | |
| What AI-use practice should change in the next cycle? | |
| Did any AI-assisted work create review, governance, operational, or maintainability concerns that required additional engineering oversight? | |

---

## 10. Required Repository Updates After the Postmortem

| Artifact to Update | Required Action | Owner |
|---|---|---|
| `/docs/planning/risk-register.md` | Add new risks, update severity, identify owner and mitigation. | Planning & Process Lead |
| `/docs/planning/re-estimation.md` | Record what changed and how estimates should improve. | Planning & Process Lead |
| `/docs/planning/task-plan.md` | Create Cycle 2 or next-release action items. | Planning & Process Lead |
| `/docs/testing/` | Add tests or validation evidence based on defects and release gaps. | Quality & Review Lead |
| `/docs/architecture/` or ADRs | Document architecture changes or deferred design decisions. | Architecture & Development Lead |
| `/docs/ai/ai-use-log.md` | Record AI use in postmortem analysis or improvement planning. | Operations & Evidence Lead |
| GitHub Issues | Create issues for approved improvement actions. | Team Lead / Assigned Owners |
| `/docs/observability/` or `/docs/operations/` | Improve operational visibility, logging, runbooks, or recovery guidance when gaps were identified. | Operations & Evidence Lead |

---

## 11. Postmortem Completion Checklist

- [ ] Postmortem is specific, evidence-based, and blameless.
- [ ] At least three evidence sources were reviewed.
- [ ] Root causes are separated from symptoms.
- [ ] Cycle 2 or next-release improvement candidates are scoped realistically.
- [ ] Owners and target evidence are identified for improvement actions.
- [ ] Related GitHub Issues, planning files, risks, tests, release notes, and AI-use logs are updated as needed.
- [ ] Another engineering team could inspect the postmortem evidence and understand the major lessons without relying on private explanation from the original team.

---

## Final Takeaway

A postmortem is one of the main ways engineering teams convert experience into maturity.

Professional teams do not use postmortems to assign blame. They use them to preserve learning, improve systems, reduce future risk, and strengthen operational judgment.
