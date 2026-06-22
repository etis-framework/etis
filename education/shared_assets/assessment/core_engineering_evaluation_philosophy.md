# Core Engineering Evaluation Philosophy

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Assessment  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Primary Audience:** Instructors, reviewers, teaching assistants, and educational adopters  
**Status:** Normalized shared assessment asset  

---

## Purpose

This document defines the core engineering evaluation philosophy used within ETIS-aligned software engineering education.

It originated in Loyola University Chicago COMP 330 — Software Engineering and has been normalized as a reusable ETIS assessment asset.

The purpose of this document is to explain how engineering work should be evaluated when the educational goal is not merely working software, but trustworthy engineering practice.

ETIS assessment evaluates whether a team can produce engineering work that is:

- Reviewable
- Testable
- Maintainable
- Governable
- Operationally understandable
- Professionally defensible

The course or implementation may require concise submission documents, presentations, or milestone packets, but those artifacts are not the full engineering record.

The repository remains the primary source of engineering evidence.

---

## Core Principle

A working demo is not enough.

Professional engineering requires visible evidence that the team:

- Understood the problem
- Controlled the work
- Reviewed changes
- Verified behavior
- Disclosed meaningful AI assistance
- Understood operational behavior
- Identified remaining risks and limitations
- Can explain the engineering decisions behind the work

A polished presentation does not compensate for weak engineering evidence.

A working feature does not compensate for missing review, testing, traceability, or accountability.

A generated artifact does not become trustworthy until humans review, verify, understand, and accept responsibility for it.

---

## Evaluation Philosophy

ETIS assessment evaluates engineering maturity rather than artifact volume.

Students should understand that the question is not simply:

```text
Did the team submit the required files?
```

The better question is:

```text
Can the team make credible engineering claims and support those claims with reviewable evidence?
```

Engineering evaluation therefore focuses on the relationship among intent, decisions, evidence, verification, risk, AI use, operational awareness, and professional accountability.

---

## What ETIS Evaluation Values

ETIS-aligned evaluation values the following.

### Engineering evidence over unsupported claims

Teams should support important claims with requirements, architecture, tests, reviews, traceability, release notes, operational notes, or other repository evidence.

### Reviewability over private or undocumented work

Engineering work should be inspectable by others.

### Realistic scope over feature volume

A smaller system with defensible evidence is stronger than a larger system with unclear ownership and weak verification.

### Human ownership of AI-assisted work

AI may assist, but teams remain responsible for correctness, maintainability, security, governance, testing, and release readiness.

### Operational honesty

Teams should be honest about defects, limitations, risks, deferred work, supportability, and operational assumptions.

### Continuous repository discipline

Engineering evidence should accumulate throughout the lifecycle rather than appear as a deadline documentation dump.

### Professional communication

Teams should communicate clearly, take ownership, and make decisions understandable to reviewers.

### Operational understanding

Teams should show awareness of setup, runtime behavior, observability, recovery, support, and future maintenance when appropriate to the assignment phase.

---

## How Assignments Are Evaluated

Each assignment should be treated as a phase gate in the software development lifecycle.

A phase gate is not just a grading checkpoint.

It is an engineering review point.

The expected submission may be a concise document, form, or presentation that indexes the team evidence. However, the actual engineering record should remain in the repository.

Repository-visible evidence may include:

- Issues
- Branches
- Pull requests
- Reviews
- Tests
- Defect logs
- Architecture Decision Records
- Release notes
- Runbooks
- Observability notes
- Security or governance notes
- AI-use evidence
- Traceability links

Each phase gate evaluates whether engineering intent, workflow discipline, repository evidence, operational maturity, and release defensibility are becoming more credible over time.

---

## Evaluation Focus by Assignment Type

| Evaluation Focus | Common Use | Primary Question |
|---|---|---|
| Phase-Gate Engineering Reviews | Early and middle lifecycle assignments | Can the team make engineering intent, decisions, workflow, evidence, and risk visible at this stage? |
| Release and Operational Readiness Reviews | Release, presentation, peer review, and final defense assignments | Can the team defend a release using evidence, testing, operational maturity, governance, and professional judgment? |

---

## AI-Assisted Engineering Expectation

AI use is encouraged when it strengthens engineering work.

The evaluation standard is not whether AI was used.

The evaluation standard is whether the team used AI responsibly.

Teams should be able to show that meaningful AI assistance was:

- Disclosed
- Reviewed
- Verified
- Bounded
- Protected from sensitive data exposure
- Integrated intentionally
- Owned by the team

AI-assisted outputs must remain reviewable, governable, testable, maintainable, operationally understandable, and professionally defensible before acceptance into release evidence.

```text
AI proposes; engineers verify.
```

---

## Performance Bands

The following bands describe engineering practice quality.

They are not merely writing-quality categories. They describe the credibility of the engineering evidence and the maturity of the team’s engineering behavior.

| Band | Meaning |
|---|---|
| Exceptional Engineering Practice | Evidence is complete, current, easy to inspect, technically credible, and demonstrates professional ownership beyond minimum expectations. |
| Strong Engineering Practice | Evidence is clear, mostly complete, aligned to the assignment purpose, and shows disciplined team execution. |
| Acceptable Engineering Practice | Core expectations are met, but evidence may be uneven, shallow, late, or difficult to inspect in places. |
| Weak Engineering Practice | Important evidence is missing, disconnected, unclear, unreviewed, or not credible enough to support the team’s claims. |

---

## Instructor Judgment

Rubrics guide evaluation, but professional judgment remains necessary.

Teams may earn strong credit with different technical choices when their decisions are justified and supported by evidence.

Conversely, a polished demo or attractive document does not compensate for:

- Weak engineering evidence
- Hidden defects
- Undisclosed or unreviewed AI output
- Poor repository discipline
- Unsupported release claims
- Unclear ownership
- Missing verification
- Unrealistic operational assumptions

The evaluator should ask whether another engineer could inspect the repository, understand the work, evaluate the evidence, and reasonably trust the team’s claims.

---

## Student-Facing Evaluation Message

Students should understand the evaluation model clearly.

A useful student-facing summary is:

```text
You are not being evaluated only on whether the software appears to work.
You are being evaluated on whether your team can make professional engineering claims and support those claims with evidence.
```

That evidence should be visible, current, understandable, and connected across the repository.

---

## Relationship to ETIS Assessment Assets

This document defines the evaluation philosophy.

Related assessment assets may include:

- Phase-gate engineering review rubrics
- Release and operational readiness rubrics
- Engineering maturity models
- Peer review instruments
- Repository analysis tools
- Portfolio assessment guidance

This document should remain stable as the philosophical anchor for ETIS-aligned assessment.

---

## Core Thesis

Evaluation is based on reviewable engineering evidence, not unsupported claims or last-minute documentation.

The goal is not to reward teams for producing more files.

The goal is to help learners become engineers who can define intent, engineer context, bound authority, verify behavior, operate reality, explain decisions, and own outcomes.
