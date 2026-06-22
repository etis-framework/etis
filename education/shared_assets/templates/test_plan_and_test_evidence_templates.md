# Test Plan and Test Evidence Templates

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Template  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/testing/`

## Purpose

These templates help teams plan tests, document test cases, record execution evidence, and link defects, requirements, pull requests, operational evidence, and release readiness.

Testing is engineering and operational evidence.

A test plan should show what must be proven, what was tested, what failed, what changed, and what risks remain.

---

## Core Rule

Testing evidence should support review, release decisions, operational understanding, and risk visibility.

The goal is not paperwork.

The goal is inspectable evidence that another reviewer can follow without interviewing the team.

---

## 1. How to Use These Templates

Use the master test plan as the umbrella artifact.

Use separate test case/evidence files when details become too large for the plan.

Adapt the structures to actual workflows, risks, and system maturity rather than preserving example content unchanged.

| Artifact | Purpose | Typical GitHub Location | Primary Owner |
|---|---|---|---|
| Master Test Plan | Defines test scope, strategy, test types, responsibilities, traceability, and release-readiness criteria. | `/docs/testing/test-plan.md` | Quality & Review Lead |
| Test Case / Evidence Files | Records individual test cases, results, screenshots/logs if useful, linked issues/PRs, and pass/fail evidence. | `/docs/testing/test-cases/TC-###-short-title.md` | Quality & Review Lead; assigned tester/developer |
| Test Execution Summary | Summarizes what ran, what passed, what failed, what defects were opened, and what remains risky for release. | `/docs/testing/test-summary.md` or `/docs/testing/final-test-evidence.md` | Quality & Review Lead |
| CI/CD Evidence | Shows automated build/test workflow status and links to GitHub Actions runs or PR checks. | `/docs/testing/ci-evidence.md`; `/.github/workflows/ci.yml` | Quality & Review Lead; Architecture & Development Lead |
| Defect Links | Defects should be tracked in GitHub Issues or the defect log, then linked from test evidence. | GitHub Issues; `/docs/quality/defect-log.md` | Quality & Review Lead |

Ownership note: Any team member may update test artifacts. The assigned owner is responsible for ensuring the artifact is current, accurate, linked, and ready at the appropriate project checkpoint.

---

# Master Test Plan Template

**File Name:** `/docs/testing/test-plan.md`  
**Role:** Umbrella document for the team testing strategy and release confidence evidence.

## Project Information

| Field | Team Response |
|---|---|
| Project Name | |
| Team | |
| Version / Cycle | Cycle 1 / Cycle 2 |
| Last Updated | |
| Primary Owner | Quality & Review Lead |
| Backup Owner | |

---

## Test Scope

| In Scope | Out of Scope | Reason / Notes |
|---|---|---|
| Primary Cycle 1 workflow: submit request, review request, update status, view status | Full production security hardening | Cycle 1 focuses on controlled vertical slice. |
| Requirement acceptance criteria for top user stories | Real university data or live university system integration | Synthetic data only for course project. |
| | | |

---

## Test Types Planned

| Test Type | Purpose | When Used | Example Evidence | Owner |
|---|---|---|---|---|
| Unit | Check one function, component, or rule in isolation. | When logic can be tested without the full system. | Validation rule test; utility function test. | Assigned developer; Quality & Review Lead verifies. |
| Integration | Check that components work together across boundaries. | API, database, service, or module interactions. | Submit request API saves expected data and returns expected status. | Assigned developer/tester. |
| System / End-to-End | Check a complete user workflow. | Demo path and release readiness. | Student submits request; reviewer updates; student sees status. | Quality & Review Lead. |
| Regression | Prove a fixed defect or prior behavior stays fixed. | After a bug fix or risky change. | Test linked to GitHub Issue #__. | Defect owner. |
| Manual / Exploratory | Check usability, edge cases, and behavior not automated yet. | Early Cycle 1 and presentation prep. | Manual test notes with steps, result, screenshot/log if useful. | Assigned tester. |
| AI Validation, if applicable | Check AI-assisted behavior remains bounded, explainable, observable, governable, reviewable, and operationally safe. | Category suggestions, draft responses, missing-info prompts, generated tests/code. | Golden cases; rejected unsafe suggestion; human approval evidence. | Quality & Review Lead; AI evidence owner. |
| Operational / Observability | Verify important failures, runtime behavior, logging, diagnostics, recovery expectations, or operational visibility. | Assignment 6, release readiness, or risky workflows. | Postmortem evidence; runtime logs; observability screenshots; operational review notes. | Quality & Review Lead; operations/release owner. |

---

## Requirement-to-Test Traceability

Traceability should make it possible for another engineering reviewer to understand how important system behavior, risks, and release claims were validated.

| Requirement ID | Requirement Summary | Test ID(s) | Test Type | Evidence Location | Status |
|---|---|---|---|---|---|
| FR-001 | Student can submit a support request. | TC-001 | System / Integration | `/docs/testing/test-cases/TC-001-submit-request.md` | Planned |
| FR-002 | Reviewer can update request status. | TC-002 | System | `/docs/testing/test-cases/TC-002-update-status.md` | Planned |
| NFR-001 | System handles missing required fields safely. | TC-003 | Unit / Negative | `/docs/testing/test-cases/TC-003-required-fields.md` | Planned |
| | | | | | |

---

## Test Environment and Data

| Item | Team Answer | Notes |
|---|---|---|
| Environment | Local development / hosted demo / other | State where tests run. |
| Test Data | Synthetic sample data only | Do not use private student or university data. |
| Build/Test Command | | Example: `npm test`, `pytest`, `mvn test`, `dotnet test`. |
| CI/CD Workflow | | Link GitHub Actions workflow when available. |

---

## Release Readiness Criteria

- [ ] Primary demo workflow has supporting test evidence.
- [ ] Known defects are fixed, mitigated, deferred, or accepted with owner and rationale.
- [ ] AI-assisted code, tests, documentation, or behavior has been reviewed and verified.
- [ ] CI/CD or local test evidence is visible and linked.
- [ ] Release notes honestly describe what works, what does not, and what risks remain.
- [ ] Release/version evidence clearly identifies the repository state associated with the reviewed release.
- [ ] The team can explain why the current release was considered safe enough, reviewable enough, and governable enough to present or release.

---

# Test Case and Evidence Template

**File Name Pattern:** `/docs/testing/test-cases/TC-###-short-title.md`  
**Role:** One file per meaningful test case or test evidence record. Small related checks may be grouped when that is clearer.

## Test Case Information

| Field | Team Response |
|---|---|
| Test ID | TC-001 |
| Test Name | Submit support request |
| Related Requirement(s) | FR-001 |
| Related Issue / PR | Issue #__; PR #__ |
| Test Type | Unit / Integration / System / Regression / Manual / AI Validation |
| Owner | |
| Last Run | |
| Status | Planned / Pass / Fail / Blocked |

---

## Preconditions

- Test data exists: sample student account and sample support category.
- Application is running locally or in the agreed test environment.

---

## Test Steps and Expected Results

| Step | Action | Expected Result | Actual Result / Evidence |
|---|---|---|---|
| 1 | Open the request form. | Form loads with required fields visible. | |
| 2 | Submit request with valid title, category, and description. | Request is saved and confirmation is displayed. | |
| 3 | Open reviewer view. | New request appears with correct status and data. | |

---

## Evidence Links

| Evidence Type | Link or Location |
|---|---|
| Automated test file | `/tests/...` |
| Screenshot / log / output | `/test-evidence/...` |
| CI/CD run | GitHub Actions link |
| Related defect if failed | GitHub Issue #__ |

---

## Result and Notes

| Result | Decision | Notes |
|---|---|---|
| Pass / Fail / Blocked | Accept / Fix / Defer / Retest | Brief explanation and next action. |

---

## AI Validation Addendum, If Applicable

| Validation Question | Expected Boundary | Observed Behavior | Human Decision |
|---|---|---|---|
| Did AI suggest an appropriate category? | Suggestion only; human reviewer decides. | | |
| Did AI expose private or unsafe data? | No private data; synthetic data only. | | |
| Did AI produce a response that required human approval? | Draft response cannot be sent automatically. | | |
| What happens if the AI/tool response is unavailable, unsafe, or incorrect? | System falls back safely to human review or controlled workflow. | | |

---

# Test Execution Summary Template

**File Name:** `/docs/testing/test-summary.md` or `/docs/testing/final-test-evidence.md`  
**Role:** Summarizes testing status for an assignment checkpoint, Cycle 1 release, or final release.

## Summary Information

| Field | Team Response |
|---|---|
| Cycle / Checkpoint | Assignment 4 / Assignment 5 / Final Release |
| Summary Date | |
| Owner | Quality & Review Lead |
| Test Window | |
| Repository Version / Commit | |
| Overall Release Confidence | High / Medium / Low with explanation |

---

## Execution Summary

| Test Type | Planned | Run | Passed | Failed / Blocked | Notes |
|---|---:|---:|---:|---:|---|
| Unit | | | | | |
| Integration | | | | | |
| System / End-to-End | | | | | |
| Regression | | | | | |
| Manual / Exploratory | | | | | |
| AI Validation, if applicable | | | | | |
| Operational / Observability | | | | | |

---

## Open Defects and Release Risks

| Defect / Risk ID | Severity | Status | Owner | Release Decision | Evidence / Link |
|---|---|---|---|---|---|
| Issue #__ | High / Medium / Low | Open / Fixed / Deferred / Accepted | | Mitigate / Defer / Block release | |

---

## Release Decision

Release decisions should be based on evidence, residual risk visibility, operational understanding, and engineering judgment — not presentation confidence alone.

| Decision | Rationale | Required Follow-Up |
|---|---|---|
| Ready / Ready with limitations / Not ready | Explain using evidence, not confidence. | List owners and next actions. |

---

## Appendix A: Suggested Testing Repository Structure

```text
/docs
  /testing
    test-plan.md
    test-summary.md
    final-test-evidence.md
    ci-evidence.md
    /test-cases
      TC-001-submit-request.md
      TC-002-update-status.md
      TC-003-required-fields.md
  /quality
    defect-log.md

/tests
  automated test files, organized by the team's technology stack

/test-evidence
  screenshots, logs, exported reports, or manual evidence when useful

/.github
  /workflows
    ci.yml
```

Important distinction: GitHub Issues track defects, tasks, and follow-up work. Files under `/docs/testing/` document the test strategy and evidence. Pull requests should link to both when a change is reviewed.

---

## Appendix B: Quick Quality Checklist

- [ ] Every major requirement has at least one planned test or validation method.
- [ ] Tests include important negative and boundary cases, not only the happy path.
- [ ] Failed tests create visible defects, follow-up issues, operational review actions, or release decisions rather than disappearing.
- [ ] AI-assisted output is treated as unverified until reviewed, tested, and explained by the team.
- [ ] Test evidence is linked to requirements, issues, pull requests, release notes, and known limitations.
- [ ] The final release decision is based on evidence, not on whether the demo happened to work once.
- [ ] Another engineering team should be able to inspect the testing evidence and understand the release confidence without relying on private explanation from the original team.

---

## Final Takeaway

Testing is not the last step before a demo.

Testing is engineering evidence that supports release judgment, defect management, operational understanding, and professional accountability.
