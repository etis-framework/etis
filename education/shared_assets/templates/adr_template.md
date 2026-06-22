# Architecture Decision Record Template

**Classification:** ETIS Educational Ecosystem Shared Asset  
**Category:** Template  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/architecture/adr/ADR-001-short-title.md`

## Purpose

Use one ADR file for each significant architecture or engineering decision.

ADRs explain why a decision was made, what alternatives were considered, what tradeoffs were accepted, and what evidence supports the choice.

ADRs should support engineering understanding, review, governance, and operational reasoning. They should not create documentation volume for its own sake.

---

## Engineering Guidance

Create ADRs for meaningful architecture, governance, operational, observability, security, AI-boundary, or release-impacting decisions.

Keep each ADR short enough to review in a pull request.

Use one ADR per decision so the decision history remains traceable and easy to update.

If a later decision replaces this one, mark this ADR as Superseded and link to the new ADR.

The sample structures and examples in this template illustrate professional engineering decision documentation patterns. Teams should adapt ADR content to their actual system decisions rather than preserve example text unchanged.

Another engineering team should be able to inspect the ADR and understand the decision context without relying on private explanation from the original team.

---

## Recommended File Naming

```text
/docs/architecture/adr/ADR-001-short-title.md
```

Use sequential numbers: `ADR-001`, `ADR-002`, `ADR-003`.

Use lowercase words separated by hyphens after the number.

Examples:

```text
ADR-001-database-selection.md
ADR-002-api-style.md
ADR-003-ai-integration-approach.md
```

Link ADRs from the architecture overview, README, review evidence, or release artifacts when appropriate.

---

# ADR-___: [Decision Title]

## ADR Metadata

| Field | Team Response |
|---|---|
| ADR ID | ADR-___ |
| Decision title | [Short title] |
| Status | Proposed / Accepted / Superseded |
| Date | [YYYY-MM-DD] |
| Owner | [Primary owner] |
| Related issues / PRs | Issue #__; PR #__; review note; test evidence |

---

## 1. Context

[What problem, constraint, risk, or design pressure caused this decision? Include only the background needed to understand the choice.]

---

## 2. Decision

[State the decision clearly. Avoid vague wording. A reviewer should be able to tell exactly what the team chose.]

---

## 3. Alternatives Considered

[List the realistic alternatives considered. Include “do nothing” or “defer” if that was a serious option.]

Documenting rejected alternatives is valuable because it makes tradeoffs, constraints, and review reasoning visible to future reviewers.

---

## 4. Rationale and Tradeoffs

[Explain why this decision is appropriate for the current cycle. What benefits does it create? What costs, constraints, or future work does it introduce?]

The rationale should help reviewers understand why the decision was considered safe enough, governable enough, and maintainable enough for the current release scope.

---

## 5. Consequences

[What changes because of this decision? Consider implementation, testing, security, observability, operational recovery, maintainability, release readiness, schedule, and team skills.]

If AI-assisted workflows or AI-generated components are involved, explain how review, validation, approval boundaries, and operational oversight are maintained.

---

## 6. Risks and Follow-Up Work

[List risks, open questions, deferred work, or review actions created by the decision.]

---

## 7. Evidence Links

[Link to relevant requirements, issues, pull requests, tests, review notes, AI-use log entries, observability evidence, diagrams, release notes, or operational evidence.]

---

## Sample ADR Row for the Architecture Overview Index

| ADR ID | Decision Title | Status | Owner | File / Evidence Link |
|---|---|---|---|---|
| ADR-001 | Use SQLite for Cycle 1 persistence | Accepted | Architecture & Development Lead | `/docs/architecture/adr/ADR-001-sqlite-persistence.md` |

---

## Good ADR Topics

- Database or persistence approach
- Frontend/backend/API architecture
- Authentication or role model
- AI integration approach and approval boundaries
- Testing strategy for a risky workflow
- Deployment or runtime environment decision
- Logging, observability, or audit evidence approach
- Boundary decisions about what the system intentionally will not automate or operationalize

---

## Avoid ADRs For

- Variable names
- Formatting changes
- Tiny refactors
- Button colors
- Small bug fixes
- Decisions no one reviewed or that do not affect architecture, risk, quality, or maintainability

---

## Bottom Line

An ADR should preserve the reasoning behind an important decision. It should make the decision reviewable, traceable, and understandable after the original discussion is forgotten.
