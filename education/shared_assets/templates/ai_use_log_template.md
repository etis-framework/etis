# AI Use Log Template

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Template  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/ai/ai-use-log.md`

## Purpose

This template records meaningful AI assistance used during requirements, planning, architecture, implementation, testing, review, documentation, release preparation, operations, and reflection.

AI use is encouraged when it improves engineering work. The purpose of this log is not to create a confession form. The purpose is to preserve engineering evidence showing how AI-assisted work was supervised, reviewed, verified, governed, and owned by the team.

The team must be able to explain why each accepted AI-assisted result was considered maintainable, governable, reviewable, testable, operationally supportable, and appropriate for the current release scope.

---

## Core Principle

AI-generated output is proposed engineering material until humans review, validate, govern, and intentionally accept it into the engineering system.

The team owns the final result.

---

## Artifact Ownership

| Field | Team Response |
|---|---|
| Project Name | |
| Team Number / Team Name | |
| Repository URL | |
| Cycle / Assignment | |
| Last Updated | |
| Primary Owner | Operations & Evidence Lead |
| Backup Owner | |

Any team member may add entries. The owner is responsible for ensuring the log is accurate, current, reviewable, and ready at each deliverable checkpoint.

---

## Policy Summary

AI tools may be used throughout the full software development lifecycle when they help the team think, build, review, test, document, or improve the project.

AI-generated output remains draft material until the team reviews it, modifies it where needed, verifies it, and accepts responsibility for it.

The team must be able to explain any submitted requirement, design, code, test, document, diagram, release note, or decision, even when AI helped create it.

Private data, real student records, credentials, secrets, or sensitive institutional information must not be entered into AI tools.

AI use should not expand project scope without team approval, instructor awareness when needed, and updated planning evidence.

AI acceleration does not eliminate the need for review capacity, validation evidence, operational maturity, release discipline, or human accountability.

---

## What Must Be Logged

Log AI use when it materially affects a project artifact, engineering decision, repository change, submitted evidence, review finding, release claim, or operational judgment.

Routine spelling correction or minor grammar cleanup does not require a detailed entry unless it changes meaning.

| Area | Log when... |
|---|---|
| Requirements and planning | AI helped identify stakeholders, edge cases, acceptance criteria, risks, estimates, scope options, or tasks. |
| Architecture and design | AI suggested components, interfaces, data boundaries, technology choices, AI/tool boundaries, or tradeoffs. |
| Implementation | AI generated, transformed, debugged, refactored, or explained code that influenced the repository. |
| Testing and validation | AI suggested test cases, generated tests, reviewed coverage, identified edge cases, or analyzed failures. |
| Review and quality | AI helped critique code, architecture, security, maintainability, dependencies, defects, or release readiness. |
| Documentation and presentation | AI drafted or improved README content, release notes, diagrams, explanations, or presentation materials. |
| Operations and governance | AI helped analyze logs, propose runtime diagnostics, identify operational anomalies, suggest recovery behavior, draft runbooks, critique observability gaps, or review operational readiness. |

A useful entry is concise but specific. It identifies the tool, engineering purpose, artifact affected, accepted or rejected changes, human review performed, operational or governance considerations when relevant, and related repository evidence.

---

## AI Use Log

Use one row per meaningful AI-assisted activity.

| Date | Team Member | Tool / Model | SDLC Area | Artifact or File Affected | AI Task / Prompt Summary | Accepted / Modified / Rejected | Human Verification Performed | Related Issue / PR / Evidence |
|---|---|---|---|---|---|---|---|---|
| YYYY-MM-DD | | | Requirements | `/docs/requirements/requirements.md` | Asked AI to identify missing acceptance criteria for request submission workflow. | Modified | Team reviewed suggestions; accepted two criteria; rejected admin-reporting feature as out of scope. | Issue #__; PR #__; requirements review |
| YYYY-MM-DD | | | Implementation | `/src/...` | Generated first draft of validation helper. | Modified | Developer rewrote error handling; reviewer checked edge cases; tests added. | Issue #__; PR #__; test file |
| YYYY-MM-DD | | | Testing | `/docs/testing/...` | Brainstormed negative test cases for invalid input. | Accepted partly | Quality lead verified against acceptance criteria and added manual tests. | Issue #__; test evidence |
| YYYY-MM-DD | | | Operations / Governance | `/docs/observability/...` | Asked AI to critique missing runtime coverage and identify observability gaps. | Modified | Team reviewed suggestions; added error logging and recovery notes; rejected verbose user-tracking proposal. | Issue #__; ADR #__; release notes |

---

## Human Verification Checklist

Before accepting AI-assisted work into the repository or presentation evidence, the team should be able to answer:

- Can the responsible student explain the accepted output without reading from the AI response?
- Was the output checked against requirements, architecture, tests, and known constraints?
- Were hallucinated APIs, unsupported assumptions, hidden dependencies, or over-scoped suggestions removed?
- Was security, privacy, data handling, permission, and governance impact considered when relevant?
- Was the final accepted artifact reviewed by a human teammate before being treated as engineering evidence?
- Are related issues, pull requests, tests, or documentation links visible where appropriate?
- Could the team defend the accepted AI-assisted result during review, presentation, postmortem, or operational investigation?
- Does the team understand the operational behavior, limitations, observability impact, and recovery expectations associated with the accepted result?

---

## SDLC Classification Quick Guide

| SDLC Area | Examples |
|---|---|
| Requirements | User stories, acceptance criteria, ambiguity checks, edge cases, stakeholder questions |
| Planning | Scope options, task decomposition, risk identification, estimate assumptions, schedule risks |
| Architecture | Components, interfaces, data/context ownership, tool boundaries, ADR tradeoffs |
| Implementation | Code generation, refactoring, debugging, explanations, dependency suggestions |
| Testing | Test ideas, test data, automated tests, negative cases, validation checks |
| Review | Code review, AI-code critique, security review, maintainability review, PR review notes |
| Release | Release notes, known limitations, demo script, presentation outline, final evidence summary |
| Operations / Governance | Logs, observability, runtime diagnostics, permissions, approvals, audit evidence, recovery guidance, incident/postmortem analysis, governance review, operational readiness assessment |

---

## Final Takeaway

AI-assisted engineering is acceptable and expected when it improves engineering work responsibly.

Undisclosed, unreviewed, unverified, ungoverned, operationally unexplained, or poorly understood AI-assisted work is not professional engineering evidence.

Significant AI-assisted engineering work should remain traceable through issues, pull requests, reviews, tests, ADRs, release notes, postmortems, operational evidence, and related repository workflow artifacts when appropriate.

The AI use log exists to support engineering transparency, governance, reviewability, and accountable stewardship.
