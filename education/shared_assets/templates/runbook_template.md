# Runbook Template

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Template  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/operations/runbook.md` or `/docs/runbook.md`

## Purpose

This lightweight runbook helps a team explain how to build, run, observe, troubleshoot, recover, and support its software system.

The goal is not bureaucracy.

The goal is operational clarity.

Another engineering team should be able to inspect the runbook and understand how to run, diagnose, support, recover, and evaluate the current release without relying on private explanation from the original team.

---

## Course Principle

The repository is the proof source.

Operational claims should remain traceable to repository-visible evidence such as issues, pull requests, tests, CI runs, logs, release notes, ADRs, defects, AI-use evidence, and known limitations when appropriate.

The runbook should point to commands, logs, tests, issues, release notes, and known limitations that make operational claims reviewable.

---

## 1. System and Runbook Information

| Field | Team Response |
|---|---|
| Team Number / Team Name | |
| Repository URL | |
| Project / System Name | |
| Cycle / Release Version | Cycle 1 / Cycle 2 / Final Release |
| Runbook Owner | |
| Last Updated | |
| Primary Support Contact / Role | |
| Primary Communication Channel | |

---

## 2. System Overview

Briefly describe what the system does, who uses it, and what workflow or problem it supports.

| Prompt | Team Response |
|---|---|
| What does the system do? | |
| Who are the primary users or roles? | |
| What is the main workflow or vertical slice? | |
| What is in scope for this release? | |
| What is intentionally out of scope or deferred? | |
| What systems, APIs, data files, models, or external services does it depend on? | |

---

## 3. Quick Start: Build, Run, and Test

Document the shortest reliable path for another engineer to run the system from a clean checkout.

Commands should be current and tested.

Quick-start instructions should assume a clean environment and should not depend on undocumented tribal knowledge, local-only setup, or instructor intervention.

| Step | Command / Location | Expected Result |
|---|---|---|
| Clone repository | | Repository is available locally. |
| Install dependencies | | Required packages or tools are installed. |
| Configure environment | | Environment variables, config files, or accounts are ready. |
| Build | | Build completes without errors. |
| Run application | | Application starts successfully. |
| Run automated tests | | Tests complete with visible pass/fail evidence. |
| Run demo path | | Core demo workflow can be completed. |

---

## 4. Configuration and Environment Requirements

| Configuration Item | Required? | Where Defined | Notes / Safe Handling |
|---|---|---|---|
| Runtime / language version | | | Example: Python version, Node version, Java version, C compiler, etc. |
| Environment variables | | | Do not place secrets in the repository. |
| Accounts / test users | | | Use synthetic or demo accounts only. |
| Database / storage | | | Include setup, seed data, and reset instructions if applicable. |
| External APIs / AI tools | | | Document model/tool name, purpose, limits, and fallback behavior. |
| Local files / sample data | | | Use synthetic sample data only. |

---

## 5. Normal Operation

Describe the normal operating path. Focus on what should happen when the system is healthy.

| Workflow / Operation | Expected Behavior | Evidence to Check |
|---|---|---|
| Main user workflow | | Demo script, test evidence, logs, or screenshots. |
| Important validation or refusal path | | Evidence that the system says no at the right time. |
| Administrative or support action | | Who may perform it and what evidence is recorded. |
| AI-assisted workflow, if applicable | | AI-use log, prompt/output notes, review evidence, or validation cases. |

---

## 6. Observability and Runtime Evidence

List the evidence the team can use to understand runtime behavior. At student-project scale, this may be logs, request IDs, test output, CI runs, screenshots, or documented observations.

| Signal / Artifact | Where It Lives | What It Tells Us | Example / Notes |
|---|---|---|---|
| Application logs | | Important events, outcomes, failures, or recovery paths. | |
| Request IDs / audit IDs | | Connects one user action to related logs, errors, or defects. | |
| CI/CD results | | Shows build/test checks and visible pass/fail evidence. | |
| Test evidence | | Shows what behavior was verified. | |
| AI usage or cost notes | | Shows AI calls, model/tool usage, token/cost awareness, or limits. | |
| Known limitations / release notes | | Explains current risk boundaries and release decisions. | |
| Operational metric or health signal | Monitoring note, dashboard, timing evidence, or known threshold | Helps identify degraded behavior before complete failure. | Example: response latency increase before timeout failures |

---

## 7. Common Failure Modes and Diagnosis

Use this table to turn mystery failures into diagnosable engineering facts.

Diagnosis should prioritize observable evidence, reproducibility, and workflow traceability over assumptions or memory-based debugging.

Add rows as the team learns from testing, demos, defects, or production-like use.

| Symptom | Likely Cause | Evidence to Check | Recovery / Next Action | Owner |
|---|---|---|---|---|
| Application will not start | | Build output, setup logs, README, dependency versions | | |
| Core demo path fails | | Logs, request ID, defect log, recent PRs, test evidence | | |
| Validation rejects valid input | | Requirements, acceptance criteria, logs, failing test case | | |
| Invalid input is accepted | | Boundary tests, validation code, defect log | | |
| External API / AI service failure | | Timeout logs, error class, retry behavior, cost/rate-limit evidence | | |
| Test or CI failure | | CI logs, recent commits, changed files, test output | | |

---

## 8. Incident Response and Recovery Procedure

For this course, an incident can be a broken demo, failed release check, data corruption risk, security concern, AI behavior failure, or other high-impact defect.

| Step | Action | Evidence / Output |
|---|---|---|
| 1. Confirm impact | Identify what failed, who is affected, and whether the main workflow is blocked. | Issue, defect entry, screenshot, log, or CI result. |
| 2. Preserve evidence | Capture logs, request IDs, input data, error messages, failing test output, and recent changes. | Saved evidence path or linked issue. |
| 3. Stabilize | Stop risky action, disable failing feature, revert change, activate safe mode if available, or use documented workaround. | Mitigation note or rollback reference. |
| 4. Diagnose | Identify likely root cause using evidence, not guesses. | Root-cause note in defect log or postmortem. |
| 5. Fix or defer | Fix now if release-blocking; otherwise document limitation, workaround, owner, and next action. | PR, issue, release note, or known limitation. |
| 6. Prove recovery | Run relevant tests, CI checks, manual verification, or regression checks. | Test output, CI run, or evidence link. |

Recovery claims should remain reviewable through tests, logs, CI evidence, release notes, issue history, or operational validation evidence when appropriate.

---

## 9. Rollback, Disable, or Safe Mode Plan

Describe what the team can do if a change creates unacceptable risk.

Not every student project has formal deployment rollback, but every team should know how to return to a safer state.

Teams should identify the fastest safe path to restore stability, even if functionality must be temporarily reduced or disabled.

Teams should prefer safe degradation and controlled recovery over unstable feature preservation.

| Risk Scenario | Safe Action | Who Decides? | Evidence / Notes |
|---|---|---|---|
| Broken build or failed CI | | | |
| Core workflow failure | | | |
| High-severity security or data issue | | | |
| AI tool produces unsafe or unreliable output | | | |
| External dependency unavailable or too costly | | | |

---

## 10. Security, Data, and AI Governance Notes

Identify what data the system stores, displays, logs, or sends to external services.

Do not include secrets, private credentials, or unnecessary sensitive data in the repository, logs, prompts, screenshots, or sample data.

For AI-assisted functionality, document what AI is allowed to do, what requires human review, and what evidence proves verification.

If the system can take actions, document permission boundaries, approval points, audit evidence, and recovery steps.

AI-assisted functionality should remain reviewable, testable, governable, observable, and operationally explainable before being trusted in release workflows.

| Governance Question | Team Response |
|---|---|
| What sensitive or important data exists? | |
| What data must never be logged or sent to AI tools? | |
| What actions require human approval? | |
| What AI-assisted work must be disclosed and verified? | |
| What security or governance risks remain? | |

---

## 11. Known Limitations and Support Notes

| Limitation / Risk | User or Team Impact | Workaround / Mitigation | Owner | Next Action |
|---|---|---|---|---|
| | | | | |
| | | | | |
| | | | | |

---

## 12. Operational Readiness Checklist

- [ ] A clean checkout can be built or run using documented steps.
- [ ] Required configuration, environment variables, accounts, and sample data are documented.
- [ ] The main demo path is repeatable and tied to requirements or release notes.
- [ ] Important failure paths have safe user messages and diagnosable evidence.
- [ ] Logs, request IDs, CI output, or test evidence can explain important behavior.
- [ ] Known limitations include impact, mitigation, owner, and next action.
- [ ] AI-assisted work, if used, is disclosed, reviewed, verified, and bounded.
- [ ] Security, data, and permission concerns are documented honestly.
- [ ] The runbook has been reviewed by someone other than the original author.
- [ ] Another engineering team could reproduce the demo path, diagnose major failures, and understand release limitations using the repository evidence.

---

## 13. Change History

| Date | Change | Reason | Owner |
|---|---|---|---|
| | | | |
| | | | |

---

## Final Takeaway

A runbook is not extra paperwork.

It is evidence that the team can operate, diagnose, recover, and responsibly own the software after the happy-path demo ends.
