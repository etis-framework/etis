# Requirements Template

**Classification:** ETIS Educational Ecosystem Shared Asset  
**Category:** Template  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/requirements/requirements.md`

## Purpose

This template defines system capabilities, scope, constraints, assumptions, and acceptance expectations.

Requirements should remain specific, testable, traceable, and updated as the team learns.

Requirements exist to guide engineering decisions, validation, review, release readiness, and operational understanding. They are not paperwork.

---

## Engineering Guidance

Keep this artifact lightweight and useful. Do not write a large specification just to fill space.

Use clear requirement identifiers such as `FR-001` and `NFR-001` so requirements can be traced to issues, tests, defects, and release notes.

Requirements exist to guide engineering decisions, validation, review, and release readiness.

AI tools may help identify gaps, edge cases, and weak acceptance criteria, but the team owns the final requirements.

Update this file whenever scope, assumptions, priorities, or acceptance expectations change.

The sample content in this template illustrates professional engineering structure and evidence patterns. Teams are expected to adapt the artifact to their actual project rather than copy example entries unchanged.

---

## 1. Project Information

| Item | Team Response |
|---|---|
| Project Name | [Enter value] |
| Team Number / Team Name | [Enter value] |
| Requirements Owner | [Enter value] |
| Backup Owner | [Enter value] |
| Version / Date | [Enter value] |
| Repository URL | [Enter value] |

---

## 2. System Overview

[Briefly describe the system, target users, and overall purpose. Keep this to one short paragraph.]

---

## 3. Cycle Scope

| Item | Team Response |
|---|---|
| Cycle 1 vertical slice | [Describe the small, demonstrable workflow the team will build first.] |
| Intentionally out of scope for Cycle 1 | [List features or ideas the team is explicitly deferring.] |
| Cycle 2 candidate improvements | [List maturity candidates such as better tests, observability, runtime visibility, security/governance, operational maturity, workflow depth, or selected features.] |
| Scope decision owner | [Name the person responsible for keeping scope current.] |

---

## 4. Assumptions, Constraints, and Open Questions

| ID | Type | Description | Status / Owner |
|---|---|---|---|
| A-001 | Assumption | Users will use synthetic sample data, not real student records. | Accepted / Team Lead |
| C-001 | Constraint | No live university systems or private institutional data may be used. | Required / Architecture & Development Lead |
| Q-001 | Open Question | Should request categories be fixed or configurable by an administrator? | Open / Requirements Owner |
|  |  |  |  |
|  |  |  |  |

---

## 5. Functional Requirements

Replace the sample rows with your team requirements. Keep each requirement small enough to implement, review, and test.

Requirements should support engineering review and release decisions by making expected behavior observable, testable, and explainable.

| ID | User / Role | Requirement | Priority | Acceptance Criteria | Related Evidence |
|---|---|---|---|---|---|
| FR-001 | Student requester | Student can submit a support request with category, description, and contact information. | High | Given valid required fields, the system saves the request and shows a confirmation with request status. | Issue #__; Test T-__ |
| FR-002 | Support reviewer | Reviewer can view submitted requests and update status. | High | Reviewer can change status from New to In Review or Resolved, and the status is visible to the requester. | Issue #__; Test T-__ |
| FR-003 | Support reviewer | Reviewer can request clarification from the student. | Medium | Reviewer can add a clarification note, and the request status indicates that student action is needed. | Issue #__; Test T-__ |
| FR-004 | Team administrator | Administrator can view requests by category or status. | Low | Administrator can filter the request list by at least one category or status value. | Issue #__; Test T-__ |
|  |  |  |  |  |  |

---

## 6. Non-Functional Requirements

| ID | Category | Requirement | Target / Acceptance Expectation | Evidence |
|---|---|---|---|---|
| NFR-001 | Usability | A first-time user can submit a request without training. | Main request form is understandable from labels and required-field messages. | Manual test notes |
| NFR-002 | Reliability | The system should not lose submitted request data during normal use. | Saved request remains available after refresh or restart, depending on chosen persistence design. | Test T-__ |
| NFR-003 | Security / Data | The project must use synthetic data only. | No real student records, grades, credentials, or private university data are stored. | Review checklist |
| NFR-004 | Maintainability | The team can explain major components and where changes belong. | Architecture document maps components to responsibilities. | `/docs/architecture/` |
| NFR-005 | Observability / Operations | Important operational failures should be diagnosable by the team. | Logs, validation output, or operational evidence help explain important failure conditions. | `/docs/observability/` |
|  |  |  |  |  |

---

## 7. AI-Assisted System Behavior, If Any

Complete this section only if the system includes user-facing AI behavior. AI use for development still belongs in the AI-use log.

AI-assisted system behavior should remain explainable, governable, reviewable, and consistent with the overall system architecture.

| ID | AI Behavior | Human Approval / Boundary | Acceptance Expectation | Evidence |
|---|---|---|---|---|
| AI-001 | System suggests a request category from the student description. | Suggestion only; reviewer may accept or override. | AI suggestion is displayed as a recommendation, not an automatic decision. | AI validation notes |
|  |  |  |  |  |

---

## 8. Requirement Traceability Summary

Update this table as issues, pull requests, tests, defects, release evidence, operational findings, and engineering decisions evolve.

| Requirement ID | GitHub Issue(s) | Pull Request(s) | Test / Validation Evidence | Release / Demo Evidence |
|---|---|---|---|---|
| FR-001 | Issue #__ | PR #__ | `/docs/testing/request-submit.md` | Demo step 1; `release-notes.md` |
| FR-002 | Issue #__ | PR #__ | `/docs/testing/status-update.md` | Demo step 2; `release-notes.md` |
| NFR-003 | Issue #__ | PR #__ | Security/governance checklist | `known-limitations.md` |
|  |  |  |  |  |

---

## 9. AI-Assisted Requirements Review Notes

Use this section when AI materially helps review, critique, rewrite, or expand requirements.

| Date | AI Tool Used | Prompt / Task Summary | Accepted / Rejected / Modified | Human Verification Notes | Related Repository Evidence |
|---|---|---|---|---|---|
| [Date] | [Tool] | Asked AI to identify missing edge cases for request submission. | Accepted two validation suggestions; rejected out-of-scope notification feature. | Team reviewed against Cycle 1 scope and updated FR-001 acceptance criteria. | Issue #12; PR #18; `/docs/testing/request-submit.md` |
|  |  |  |  |  |  |

---

## 10. Requirements Readiness Checklist

- [ ] Cycle 1 vertical slice is clear, small, and demonstrable.
- [ ] Each requirement is specific enough to implement and test.
- [ ] Acceptance criteria describe observable behavior.
- [ ] Out-of-scope and deferred items are explicit.
- [ ] Assumptions, constraints, risks, and open questions are visible.
- [ ] AI-assisted suggestions are disclosed and reviewed by humans.
- [ ] Requirements are traceable to issues, tests, release notes, or known limitations as the project evolves.
- [ ] Another engineering team could review the requirements and understand the intended system behavior without private explanation.

---

## Bottom Line

Requirements preserve engineering intent. They should help the team build the right system, review the right evidence, test the right behavior, and make defensible release decisions.
