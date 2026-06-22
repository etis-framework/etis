# AI Use and Disclosure Expectations Guide

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** AI Engineering  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Implementation Provenance:** COMP330 Flagship Implementation  
**Authoritative Format:** Markdown  
**Purpose:** Student-facing expectations for meaningful AI-use disclosure and verification

---

## Purpose

This guide defines expectations for AI use and disclosure in ETIS-aligned software engineering work.

The original version of this asset was created for Loyola University Chicago COMP 330 — Software Engineering. It has been normalized as an ETIS AI Engineering shared asset while preserving COMP330 provenance.

AI tools are encouraged because professional software engineering is now AI-assisted.

The expectation is not to avoid AI.

The expectation is to use AI responsibly, disclose meaningful use, verify results, and own the final engineering work.

---

## Core Principle

AI may help produce requirements, plans, code, tests, documentation, reviews, release notes, and presentation materials.

The team still owns:

* Correctness
* Architecture fit
* Maintainability
* Security
* Testing
* Governance
* Operational impact
* Release readiness

```text
AI generated it.
```

is never an engineering defense.

The professional question is whether the result was reviewed, verified, understood, and responsibly accepted.

AI-generated output is proposed engineering material until humans review, validate, govern, and intentionally accept it into the operational system.

---

## Appropriate AI Use

AI may be used to support engineering work throughout the software development lifecycle.

Appropriate uses include:

* Brainstorming requirements, user stories, acceptance criteria, risks, edge cases, and test ideas
* Reviewing artifacts for ambiguity, missing assumptions, weak traceability, or unclear ownership
* Drafting or improving code when the team reviews, tests, and understands the result
* Generating candidate tests, CI/CD workflow drafts, documentation, README content, release notes, and demo scripts
* Assisting with observability ideas, operational diagnostics, runbooks, postmortems, release-readiness reviews, and governance analysis when the team validates the results
* Using AI as a reviewer, critic, tutor, or second set of eyes during engineering work

The standard is not whether AI was used.

The standard is whether the team used AI professionally.

---

## Unacceptable or Unprofessional AI Use

The following are unacceptable:

* Submitting AI-generated work the team cannot explain, defend, test, or maintain
* Using AI to create the appearance of engineering maturity without corresponding review, validation, testing, or operational evidence
* Merging AI-generated code without human review, testing, and architecture-fit judgment
* Inventing evidence, fake test results, fake citations, fake review comments, or fake repository history
* Using AI to hide defects, inflate progress, obscure contribution, or make unsupported claims
* Entering secrets, credentials, private data, real student data, or sensitive information into AI tools without explicit approval

AI may support learning.

AI may not replace learning.

---

## What Must Be Disclosed

Teams should disclose AI use when it materially helped create, review, modify, or decide project work.

Disclosure does not need to list every minor grammar edit.

Disclosure must capture meaningful engineering assistance.

Meaningful AI-use evidence should normally be captured inside the repository using:

* AI-use logs
* Pull requests
* Review artifacts
* Architecture decisions
* Release evidence
* Related engineering documentation

---

## Disclosure Categories

| Category | Examples that should be disclosed |
|---|---|
| Requirements / planning | AI helped draft requirements, identify missing assumptions, generate acceptance criteria, estimate tasks, or analyze risk. |
| Architecture / design | AI proposed components, interfaces, data flow, governance boundaries, tradeoffs, or ADR language. |
| Implementation | AI generated, refactored, debugged, or substantially modified code, configuration, scripts, or CI/CD files. |
| Testing / validation | AI generated tests, edge cases, adversarial cases, golden cases, test plans, or validation rubrics. |
| Review / security | AI assisted with code review, dependency review, security concerns, defect analysis, or release readiness checks. |
| Documentation / release | AI drafted or revised README content, release notes, runbooks, known limitations, presentation materials, or demo scripts. |

---

## Minimum AI-Use Log Entry

For meaningful AI assistance, the AI-use log should identify:

* Date
* Tool used
* Task or artifact affected
* What AI contributed
* What the team accepted, modified, or rejected
* How the result was verified
* Owner responsible for the final decision

AI-related engineering changes should also remain traceable through repository commits, pull requests, reviews, tests, and supporting evidence when applicable.

A typical AI-use log location is:

```text
/docs/ai/ai-use-log.md
```

---

## Good and Weak Disclosure Examples

| Disclosure Quality | Example |
|---|---|
| Good | Used AI to generate initial negative test ideas for REQ-04. Team selected three cases, rewrote them, added two tests, and verified they fail when the authorization rule is removed. |
| Good | Used AI to critique the architecture diagram for missing boundaries. Team accepted the concern about data ownership, updated architecture.md, and documented the decision in ADR-0003. |
| Weak | Used ChatGPT for coding. |
| Weak | AI helped with documentation. |
| Weak | AI generated the architecture. |

Good disclosure explains what AI helped with, what humans did with it, and how the team verified the final result.

Weak disclosure hides engineering responsibility behind vague wording.

---

## Verification Expectations

AI-assisted work must be verified before acceptance.

### Code

Code must be reviewed through pull requests, engineering review, and human validation before merge, especially if AI generated or significantly modified it.

### Architecture and design

AI-generated architecture or design suggestions should be evaluated for architectural consistency, maintainability, operational supportability, governance, and long-term engineering impact.

### Testing

Tests should prove important behavior, failure paths, and acceptance criteria rather than only the happy path.

AI-generated tests must be inspected because they may mirror assumptions or reinforce implementation mistakes.

### Security and governance

Security, data handling, dependency, permission, and governance concerns must be inspected when AI touches implementation or workflow behavior.

### Documentation

Documentation created with AI must be accurate, current, and consistent with the repository.

### Release claims

AI-assisted release notes, summaries, or presentations must be supported by repository evidence.

Polished wording is not release evidence.

---

## Sensitive Data Rule

Do not place any of the following into AI tools without explicit approval:

* Secrets
* Passwords
* Tokens
* Credentials
* Private user data
* Real student data
* Confidential information
* Unnecessary sensitive content

Use synthetic data unless explicitly approved.

When in doubt, remove, mask, or synthesize the data before using AI assistance.

---

## Team Accountability Standard

The team may use AI throughout the software development lifecycle, but the team must be able to explain the submitted work.

The team must be able to point to evidence showing:

* What AI helped produce
* What humans accepted
* What humans modified
* What humans rejected
* How the result was verified
* Who owned the final decision

The team is responsible for defects, security issues, poor design choices, missing tests, and unsupported claims even when AI contributed.

---

## Pull Request Disclosure Guidance

When AI materially affects a change, the pull request should identify:

* What AI helped produce or review
* Which files or artifacts were affected
* What the team changed after AI assistance
* How the result was tested or reviewed
* Any remaining risks or limitations

Example:

```text
AI was used to suggest initial validation logic and negative test cases for REQ-04. The team modified the generated code, added three tests, reviewed the authorization boundary manually, and verified the tests fail when the authorization rule is removed.
```

This creates reviewable engineering evidence.

---

## Student Reflection Guidance

Students may also use AI-use evidence in reflection.

Useful reflection questions include:

* Where did AI improve our engineering process?
* Where did AI create risk or confusion?
* What AI suggestions did we reject?
* How did we verify accepted AI output?
* Did AI change our architecture, scope, tests, or release claims?
* Could another team understand our AI-assisted decisions from repository evidence?

Reflection should connect AI use to engineering maturity.

---

## Bottom Line

AI use is expected.

Blind trust is not.

Professional engineering teams use AI to accelerate engineering work while preserving human judgment, verification, review discipline, governance, operational accountability, and ownership.

AI should make engineering more reviewable, not less.

---

## Core Thesis

AI assistance does not reduce engineering responsibility.

It increases the need for evidence, disclosure, review, verification, and accountability.

A team may use AI throughout the project, but the team must still be able to explain, defend, test, maintain, and own the final engineering work.
