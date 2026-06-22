# Release and Operational Readiness Rubric

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Assessment  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Primary Audience:** Instructors, reviewers, teaching assistants, and student teams  
**Status:** Normalized shared assessment asset  

---

## Purpose

This rubric evaluates whether a team can close a release professionally.

It originated in Loyola University Chicago COMP 330 — Software Engineering and has been normalized as a reusable ETIS assessment asset.

Release and operational readiness reviews are not primarily about presentation polish or feature count.

They evaluate whether the team can defend release claims using:

- Testing evidence
- Repository evidence
- Operational readiness
- Governance awareness
- AI accountability
- Honest engineering judgment

A release review should help answer:

```text
Can the team responsibly stand behind this release?
```

---

## Common Use

This rubric is intended for release-oriented assessments.

In the COMP 330 implementation, it was designed for assignments such as:

- Cycle 1 release, presentation, and peer review
- Final cycle release, operational maturity, presentation, and peer review

Other implementations may adapt the rubric to equivalent release gates, final project defenses, capstone reviews, or professional workshop evaluations.

---

## Evaluation Principle

Rubric criteria should be evaluated relative to the current lifecycle phase and assignment maturity expectations.

A Cycle 1 release may demonstrate a controlled vertical slice with honest limitations.

A final release should show greater maturity, deeper evidence, stronger operational awareness, and clearer learning from prior review.

The evaluator should ask whether the release claims are credible for the maturity stage being reviewed.

---

## Rubric

| Evaluation Area | Exceptional Practice | Strong Practice | Acceptable Practice | Weak / Missing Practice |
|---|---|---|---|---|
| Release Story and Scope | Release clearly explains what works, what changed, what was deferred, and why the scope is defensible. | Release story is clear with minor gaps. | Release scope is understandable but incomplete or optimistic. | Release claims are vague, inflated, or unsupported. |
| Validation and Test Evidence | Testing evidence is current, meaningful, traceable, and includes important success, failure, boundary, regression, or AI validation cases. | Testing evidence supports most important claims. | Testing exists but is shallow, partial, or hard to connect to requirements. | Testing evidence is missing, weak, or mostly demo-based. |
| Defects and Known Limitations | Defects, limitations, residual risks, mitigations, owners, and next actions are honest and reviewable. | Most defects and limitations are visible and responsibly handled. | Some risks are documented but not fully analyzed. | Risks or defects are hidden, minimized, or unmanaged. |
| Operational Readiness | Runbook, setup, observability, logging, recovery, supportability guidance, and release evidence help another engineer operate or diagnose the system. | Operational evidence is mostly clear and useful. | Operational evidence exists but has gaps. | Operational readiness is absent or treated as an afterthought; another engineer could not reliably deploy, diagnose, support, recover, or review the system. |
| Security / Governance / Data Handling | Permissions, data handling, AI/tool boundaries, approval points, and security concerns are reviewed and documented. | Most governance concerns are addressed. | Governance is present but incomplete or generic. | Security or governance concerns are missing or not credible. |
| AI Accountability | AI-assisted work is disclosed, verified, bounded, and reflected on honestly, including failures and human decisions. | AI use and verification are mostly clear. | AI documentation exists but lacks depth or verification. | AI use is undisclosed, unverified, or not understood. |
| Repository as Proof Source | Presentation and submission claims point to lifecycle-traceable repository evidence, including requirements, issues, pull requests, tests, logs, release notes, ADRs, and engineering decisions. | Most claims are backed by repository evidence. | Some claims are supported; others require verbal explanation. | Repository does not support the release narrative. |
| Presentation and Professional Defense | Presentation is concise, evidence-driven, operationally realistic, and prepared for technical questions. | Presentation is clear and mostly evidence-based. | Presentation explains the demo but weakly defends evidence or tradeoffs. | Presentation is mostly unsupported claims, polish, or demo optimism. |
| Cycle Learning and Maturity | Team shows learning from prior cycle evidence, defects, review, postmortem, and re-estimation. | Team shows meaningful improvement. | Some improvement is visible but not well connected to evidence. | Little learning or maturity improvement is visible. |

---

## Assignment-Specific Emphasis

| Assignment or Phase | Primary Emphasis |
|---|---|
| Cycle 1 Release | Controlled vertical-slice release, testing evidence, defect review, known limitations, release notes, presentation readiness, and peer review. |
| Final Release | Cycle 2 maturity improvement, observability, operational readiness, security/governance, AI accountability, runbook evidence, final release defense, and professional reflection. |

---

## What Strong Release Evidence Looks Like

Strong release evidence should allow another engineer or reviewer to inspect the repository and understand the release without relying only on a live demo or verbal explanation.

Strong evidence includes:

- Release notes that explain what changed, what works, known limitations, and evidence links.
- Test evidence that proves important behavior, not just the happy-path demo.
- Defects and risks that are visible, triaged, owned, and honestly dispositioned.
- Repository navigation that guides reviewers to requirements, architecture, tests, CI/CD evidence, AI-use evidence, and release artifacts.
- Presentation materials that guide reviewers through the evidence rather than replace it.
- Operational notes that help another engineer run, diagnose, support, or improve the system.
- Security, governance, and data-handling notes appropriate to project scope.
- AI accountability evidence showing what assistance was accepted, modified, rejected, and verified.

---

## Common Weak Patterns

The following weak patterns should be actively identified.

- A demo works once, but testing evidence is thin or missing.
- Known limitations are hidden to make the release look stronger.
- Presentation claims cannot be traced to repository evidence.
- AI-generated work is not disclosed, reviewed, or validated.
- Operational readiness, runbook, observability, or recovery thinking is missing.
- Release notes summarize features but do not explain evidence, risks, or limitations.
- Teams rely on verbal explanation because the repository cannot support the release narrative.
- Final release work does not show learning from prior defects, feedback, or postmortems.

---

## Reviewer Interpretation

This rubric should guide professional judgment.

It should not be applied as a mechanical checklist.

A team can have a modest feature set and still demonstrate strong release readiness if the scope is honest, evidence-backed, tested, reviewable, and operationally understandable.

A team can have an impressive demo and still demonstrate weak release readiness if the repository cannot support the claims.

---

## Relationship to Phase-Gate Assessment

This rubric evaluates release and operational readiness.

A separate phase-gate engineering review rubric should be used for earlier lifecycle checkpoints such as launch, planning, architecture, and construction.

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

Evaluation is based on reviewable, lifecycle-traceable engineering evidence and operational readiness.

It is not based on unsupported claims, presentation polish, feature count, or last-minute documentation.

A professional release is not proven by a demo.

A professional release is defended through evidence.
