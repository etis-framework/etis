# Phase-Gate Engineering Review Rubric

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Assessment  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Primary Audience:** Instructors, reviewers, teaching assistants, and student teams  
**Status:** Normalized shared assessment asset  

---

## Purpose

This rubric evaluates whether a team is developing software through disciplined engineering phase gates.

It originated in Loyola University Chicago COMP 330 — Software Engineering and has been normalized as a reusable ETIS assessment asset.

Phase-gate reviews are not primarily about feature volume.

They evaluate whether the team can make intent, workflow, decisions, risks, AI use, repository evidence, and engineering maturity visible at the right point in the lifecycle.

A phase gate should help answer:

```text
Is the team practicing engineering in a way that can be reviewed, improved, and trusted?
```

---

## Common Use

This rubric is intended for early and middle software engineering lifecycle reviews.

In the COMP 330 implementation, it was designed for assignments such as:

- Project launch
- Planning and estimation
- Architecture and review
- Construction, integration, and AI code review

Other implementations may adapt the rubric to equivalent phase gates.

---

## Evaluation Principle

Rubric criteria should be evaluated relative to the current lifecycle phase and assignment maturity expectations.

Exceptional practice for an early project launch phase is not the same as exceptional practice for a later release phase.

The evaluator should ask whether the work is mature enough for the phase being reviewed.

---

## Rubric

| Evaluation Area | Exceptional Practice | Strong Practice | Acceptable Practice | Weak / Missing Practice |
|---|---|---|---|---|
| Lifecycle / Phase Fit | Artifacts directly support the current phase gate and show maturity appropriate to the assignment stage. | Most artifacts support the phase gate and show clear progress. | Basic phase expectations are present but uneven or shallow. | Work is generic, misaligned, missing, or treated as paperwork. |
| Repository Organization | Repository is easy to inspect; evidence locations are obvious and current. | Repository is mostly organized with clear evidence locations. | Repository contains evidence, but navigation requires effort. | Repository structure prevents efficient review, onboarding, troubleshooting, or engineering continuity. |
| Engineering Evidence | Evidence is specific, traceable, reviewable, and demonstrates operational awareness and supportability appropriate to the phase. | Evidence supports most claims and is generally current. | Evidence exists but is partial, weakly linked, or uneven. | Claims are unsupported or evidence is missing or not credible. |
| Requirements / Scope / Planning | Scope, assumptions, estimates, risks, and tradeoffs are visible and realistic for the phase. | Most planning artifacts are clear and useful. | Planning exists but is incomplete, optimistic, or weakly connected to work. | Planning is absent, unrealistic, or disconnected from execution. |
| Architecture / Design Reasoning | Boundaries, responsibilities, interfaces, decisions, risks, and governance concerns are clearly explained where relevant. | Design reasoning is mostly clear and supports implementation. | Design artifacts exist but omit important rationale or risks. | Architecture is vague, decorative, contradictory, or missing. |
| Workflow / GitHub Discipline | Issues, branches, commits, pull requests, reviews, and evidence show controlled professional workflow. | Workflow is mostly visible and disciplined. | Workflow exists but is inconsistent or weakly documented. | Work bypasses review, lacks traceability, or appears as last-minute dumping. |
| AI Use and Verification | AI assistance is disclosed, reviewed, verified, and owned; risks are addressed honestly. | AI use is disclosed and mostly verified. | AI use is mentioned, but verification is thin or inconsistent. | AI output is accepted blindly, undisclosed, or not understood. |
| Team Ownership / Communication | Roles, ownership, communication rhythm, and accountability are visible and professional. | Team ownership is mostly clear. | Ownership is present but uneven or incomplete. | Ownership is unclear; team work appears uncoordinated or hidden. |
| Professional Quality | Artifacts are concise, current, internally consistent, operationally useful, and written for reviewers, maintainers, and future engineers. | Artifacts are mostly clear and professional. | Artifacts are understandable but inconsistent, too verbose, or too thin. | Artifacts are unclear, careless, stale, or not professionally reviewable. |

---

## Assignment-Specific Emphasis

The same rubric may be applied differently depending on the phase gate.

| Assignment or Phase | Primary Emphasis |
|---|---|
| Project Launch | Team identity, roles, communication rhythm, repository setup, initial evidence locations, AI-use expectations, and launch readiness. |
| Planning and Estimation | Requirements clarity, scope boundaries, traceability, task planning, estimates, risks, schedules, and tradeoff decisions. |
| Architecture and Review | Architecture overview, component responsibilities, interfaces, data or context ownership, ADRs, AI/tool boundaries, peer review, and design refinement. |
| Construction and Integration | Implementation traceability, pull request discipline, code review, CI/CD evidence, AI code review, dependency/security awareness, and test evidence. |

---

## Evidence Review Guidance

When applying this rubric, reviewers should look for repository-visible evidence.

Strong phase-gate evidence may include:

- README guidance
- Requirements
- Acceptance criteria
- Scope boundaries
- Assumptions and open questions
- Risk register
- Estimates
- Schedule
- Traceability
- Architecture overview
- ADRs
- Issues
- Branches
- Pull requests
- Review comments
- Test evidence
- AI-use log
- AI verification notes

The submission document should index this evidence.

It should not replace it.

---

## Common Weak Patterns

The following weak patterns should be actively identified.

- Submitting a document that describes work but does not point to repository evidence.
- Creating artifacts at the deadline rather than using them to guide the work.
- Using AI to produce polished text or code without verification.
- Treating GitHub as file storage instead of an engineering control system.
- Making large claims that are not supported by issues, pull requests, tests, reviews, or decisions.
- Creating architecture diagrams without explaining boundaries, responsibilities, or tradeoffs.
- Creating requirements that are not connected to implementation, testing, or release evidence.
- Showing team roles without visible ownership or follow-through.

---

## Reviewer Interpretation

This rubric should guide professional judgment.

It should not be used mechanically.

A team may use a different technical approach and still demonstrate strong engineering practice if the work is clear, evidence-backed, reviewable, and aligned with the phase.

A team may produce polished documents and still demonstrate weak engineering practice if repository evidence is missing, disconnected, or not credible.

---

## Relationship to Release Readiness Assessment

This rubric evaluates early and middle lifecycle maturity.

A separate release and operational readiness rubric should be used when teams are defending releases, presentations, operational maturity, and final engineering claims.

Phase-gate review asks:

```text
Is the team building engineering maturity at this stage?
```

Release readiness review asks:

```text
Can the team responsibly defend this release?
```

---

## Core Thesis

Phase-gate evaluation is based on reviewable engineering evidence, not unsupported claims or last-minute documentation.

Professional engineering is measured by disciplined workflow, reviewable evidence, responsible decision-making, operational awareness, and the ability for others to understand, validate, maintain, and evolve the system.
