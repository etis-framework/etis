# Architecture Overview Template

**Classification:** ETIS Educational Ecosystem Shared Asset  
**Category:** Template  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/architecture/architecture-overview.md`

## Purpose

This umbrella artifact describes the current system structure: major components, responsibilities, interfaces, data/context ownership, AI/tool boundaries, governance points, risks, and evidence links.

The architecture overview should help another engineering team inspect the repository and understand how the system is organized.

Architecture exists to support engineering review, implementation decisions, operational understanding, and release readiness. It is not merely diagram production.

---

## Engineering Guidance

Keep this document current and practical.

Use this as the architecture overview, not as the home for every architecture decision.

Document significant decisions as separate Architecture Decision Record (ADR) files and link them in the ADR index below.

Update this file when implementation changes system boundaries, responsibilities, data flow, AI/tool use, security assumptions, observability expectations, recovery behavior, or operational maturity.

The sample entries in this template illustrate professional architecture communication and evidence patterns. Teams should adapt the structure to their actual system rather than preserve example content unchanged.

---

## Architecture Overview vs. ADRs

| Artifact | Purpose | Typical Repository Location |
|---|---|---|
| Architecture overview | Explains what the system is now: structure, components, boundaries, workflows, data/context, AI/tool use, risks, and evidence links. | `/docs/architecture/architecture-overview.md` |
| ADR files | Explain why important architecture decisions, tradeoffs, boundaries, or governance choices were made. Use one ADR per meaningful decision. | `/docs/architecture/adr/ADR-001-short-title.md` |

Link the architecture overview from the repository README and related release or review evidence when appropriate.

---

## 1. Project Information

| Item | Team Response |
|---|---|
| Project name |  |
| Team number / team name |  |
| Repository URL |  |
| Architecture owner |  |
| Backup owner |  |
| Last updated |  |
| Cycle 1 vertical slice / current release focus |  |

---

## 2. System Overview

[Briefly describe what the system does, who uses it, the primary workflow, and the current release focus. Keep this to one short paragraph.]

The overview should help reviewers understand why the current architecture is considered stable enough, governable enough, and reviewable enough for the current release scope.

---

## 3. Users, Roles, and Permissions

| User / Role | Primary Goals | Allowed Actions | Limitations / Approvals |
|---|---|---|---|
| Student requester | Submit and track support request | Create request; view status; add clarification | Cannot approve or close own request |
| Support reviewer | Triage and resolve requests | Assign category/status; request clarification; add resolution note | High-risk actions require team administrator approval |
|  |  |  |  |
|  |  |  |  |

---

## 4. Architecture Diagram

[Insert or link the current architecture diagram. Recommended file: `/docs/architecture/architecture-diagram.png`.]

Show users/roles, client/UI, services/modules, data stores, external services, AI/tool boundaries, approval points, and logging/audit evidence where relevant.

Keep the diagram simple enough that another engineering team can understand the system structure, responsibilities, risks, and operational boundaries without interviewing you.

---

## 5. Component Responsibility Map

| Component | Owns / Responsible For | Must Not Own | Inputs / Outputs | Evidence Link |
|---|---|---|---|---|
| Request UI | Collect request details and show status | Business triage rules | Input: form data; Output: API request | Issue #__; PR #__; test __ |
| Workflow service | Validate and update request state | Direct UI rendering | Input: request action; Output: updated status | Issue #__; PR #__; test __ |
|  |  |  |  |  |
|  |  |  |  |  |

---

## 6. Interfaces, APIs, and Tool Boundaries

| Interface / Tool | Producer | Consumer | Contract / Behavior | Failure / Security Notes |
|---|---|---|---|---|
| `POST /requests` | Request UI | API / service layer | Creates request with category, description, contact method | Validate required fields; reject unsafe input |
| AI category suggestion, if used | AI assistant | Support reviewer | Suggests category only; human reviewer decides | Log suggestion; no automatic status change |
| Operational logging / observability | Application services | Operations/review workflow | Records important runtime behavior and errors | Avoid sensitive data exposure; validate logs remain reviewable |
|  |  |  |  |  |

---

## 7. Data and Context Ownership

| Data / Context | Authoritative Source | Sensitive? | Allowed Use | Retention / Logging |
|---|---|---|---|---|
| Request record | Application database / sample data | Potentially | Workflow status and resolution | Log status changes; do not use real student data |
| AI prompt context, if used | Synthetic request text only | No real private data | Suggest category or missing information | Record prompt purpose and verification in AI-use log |
|  |  |  |  |  |
|  |  |  |  |  |

---

## 8. AI / Tool Boundary and Governance Model

| Boundary Question | Team Answer | Human Approval Point | Evidence Location |
|---|---|---|---|
| Read: What data/context can AI or tools see? |  | Who confirms this is allowed? | `/docs/ai/ai-use-log.md` |
| Infer: What suggestions or conclusions are allowed? |  | Who reviews the suggestion? | `/docs/architecture/architecture-overview.md` |
| Change: Can the system change records or state? |  | Who approves the action? | `/docs/architecture/architecture-overview.md` |
| Log: What inputs, outputs, decisions, and errors are recorded? |  | Who reviews the evidence? | `/docs/testing/` or `/docs/release/` |
| Recover: What operational fallback exists if AI suggestions fail or are unavailable? |  | Who approves fallback behavior? | `/docs/operations/` or `/docs/release/` |

---

## 9. Testing and Review Implications

| Architecture Claim | What Must Be Tested or Reviewed | Owner | Evidence Link |
|---|---|---|---|
| Request state transition | Valid and invalid status changes |  | Test case / PR / issue |
| Role boundary | Student cannot perform reviewer actions |  | Test case / review note |
| AI suggestion, if used | Suggestion is reviewed before action |  | AI-use log / manual test |
| Operational observability | Important failures and runtime conditions are diagnosable |  | `/docs/observability/`; test evidence |
|  |  |  |  |

---

## 10. ADR Index

List one row for each significant Architecture Decision Record affecting system structure, operational behavior, AI boundaries, governance, security assumptions, or release maturity.

ADRs should be stored as individual files in `/docs/architecture/adr/`.

| ADR ID | Decision Title | Status | Owner | File / Evidence Link |
|---|---|---|---|---|
| ADR-001 | Database / persistence approach | Accepted |  | `/docs/architecture/adr/ADR-001-database-selection.md` |
| ADR-002 | AI integration approach | Proposed |  | `/docs/architecture/adr/ADR-002-ai-integration-approach.md` |
|  |  |  |  |  |
|  |  |  |  |  |

---

## 11. Known Architecture Risks and Open Questions

| ID | Risk / Question | Impact | Owner | Next Action |
|---|---|---|---|---|
| AR-001 | Data model may need to support status history in Cycle 2. | Medium |  | Decide during postmortem. |
| AR-002 | External API dependency not yet approved. | High |  | Avoid in Cycle 1 or document ADR. |
|  |  |  |  |  |
|  |  |  |  |  |

---

## Final Check

- [ ] The overview explains the current system structure without becoming a dumping ground for every decision.
- [ ] Every significant decision is linked through the ADR index.
- [ ] Architecture claims connect to issues, pull requests, tests, reviews, AI-use logs, or release evidence.
- [ ] AI/tool boundaries and human approval points are explicit when relevant.
- [ ] Data/context ownership is documented.
- [ ] Operational, observability, security, and governance implications are visible where relevant.
- [ ] Another engineering team could inspect the architecture evidence without relying on private explanation from the original team.

---

## Bottom Line

Architecture artifacts should support engineering understanding, review, governance, and operational reasoning. A useful architecture overview makes system structure, boundaries, decisions, and risks visible enough for another engineer to understand and improve the system.
