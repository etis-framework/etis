# Professional Engineering Communication Guide

## Provenance

Origin: Loyola University Chicago COMP 330 — Software Engineering  
Original Context: COMP 330 team software engineering project  
ETIS Category: Shared Asset — Playbook  
Authoritative Format: Markdown  

This guide originated as a COMP 330 course asset and has been normalized as an ETIS shared playbook. It preserves Loyola COMP 330 provenance while making the guidance reusable across ETIS-aligned educational implementations.

---

## Purpose

This guide helps engineering teams communicate clearly, professionally, and with evidence across issues, pull requests, reviews, meetings, defects, release notes, operational artifacts, and presentations.

Professional engineering communication is not decoration. It is part of the engineering system.

Communication should help another engineer understand:

* What changed
* Why it changed
* What evidence supports the change
* What risks remain
* What decisions were made
* What actions are needed
* Who owns the next step

A project should not depend on private explanations from the original team.

---

## Core Standard

Professional engineering communication is:

* Concise
* Specific
* Evidence-based
* Action-oriented
* Respectful
* Reviewable
* Operationally useful

Good communication helps the team preserve intent, coordinate work, expose risk, review changes, and defend engineering claims.

---

## Communication as Engineering Evidence

In ETIS-aligned engineering work, communication is part of the repository evidence.

Engineering communication should preserve:

* Engineering intent
* Release reasoning
* Risk visibility
* Operational understanding
* Ownership
* Workflow continuity
* Review rationale
* AI-use accountability

Teams should write so another engineer can understand the project without needing a private explanation.

---

## Communication Rules

### Be specific.

Name the requirement, issue, file, test, defect, risk, decision, release, or operational concern.

### Be concise.

Write enough to be useful without obscuring the point.

### Be evidence-based.

Link to repository artifacts, pull requests, tests, logs, decisions, issues, or release evidence.

### Be action-oriented.

State what happened, what is needed, who owns it, and by when.

### Be professional.

Avoid blame, sarcasm, vague criticism, unsupported claims, and performative certainty.

---

## What Good Communication Looks Like

| Context | Weak Pattern | Professional Pattern |
|---|---|---|
| Issue title | Fix stuff | REQ-03: Validation fails when required document is missing |
| Pull request summary | Updated code | Implements REQ-03 validation, adds negative test, and updates defect log. |
| Review comment | This is bad | Authorization check happens after data update; move check before mutation and add regression test. |
| Defect note | It broke | Malformed input caused validation failure; logged as DEF-07, fixed in PR #18, regression test added. |
| Meeting note | Talked about testing | Decision: add integration test for approval flow. Owner: Maria. Target: Class 18. |
| Release note | More fixes | Reduced release risk by closing DEF-04 and DEF-07; known limitation remains for admin export. |
| Operational issue | System crashed | Timeout spike observed after deployment; issue linked to cache invalidation regression, logged as OPS-03, mitigated with rollback, observability gap remains under investigation. |

---

## Repository Communication Expectations

### Issues

Issues should describe:

* The work being requested
* Acceptance criteria
* Owner
* Status
* Related requirement, risk, defect, or decision

### Commits

Commits should be focused and understandable.

Avoid large unexplained change dumps.

### Pull Requests

Pull requests should explain:

* What changed
* Why it changed
* What was tested
* What evidence supports the change
* What risks remain
* Whether AI assisted the work

### Review Comments

Review comments should be:

* Specific
* Respectful
* Technical
* Evidence-based
* Tied to correctness, architecture, security, maintainability, testing, governance, or operations

### Release Notes

Release notes should explain:

* What changed
* What risk was reduced
* What remains limited
* Where evidence can be found
* Known operational issues
* Rollback implications when relevant
* Observability limitations when relevant
* Deferred governance concerns when relevant

Important repository communication should remain traceable through linked requirements, issues, tests, defects, ADRs, release notes, operational artifacts, and AI-use evidence when appropriate.

---

## Team Communication Expectations

### Raise blockers early.

A blocker reported late is often a planning failure, not a surprise.

### Document decisions where future teammates can find them.

Use meeting notes, ADRs, issues, pull requests, release notes, or other repository evidence.

### Use professional disagreement.

Challenge the work, risk, assumption, or evidence.

Do not attack the person.

### Confirm ownership after meetings.

Every important action should have an owner, date, and evidence location.

### Do not hide uncertainty.

Professional teams expose uncertainty so it can be managed.

Teams should prefer visible repository evidence and documented engineering reasoning over undocumented verbal communication.

---

## AI-Assisted Communication

AI tools may be used to improve clarity, summarize discussion, draft issue text, strengthen review comments, or polish documentation.

The team still owns the message.

Teams must:

* Verify that AI-generated summaries are accurate before using them as engineering evidence.
* Ensure AI does not invent decisions, test results, approvals, citations, or repository evidence.
* Use AI to make communication clearer, not to make weak evidence sound stronger.
* Disclose AI assistance when it materially contributes to submitted artifacts, review language, release notes, or presentation content.

AI-assisted communication should remain reviewable, attributable, evidence-backed, and professionally defensible.

Teams remain responsible for technical accuracy, operational claims, release reasoning, and governance implications regardless of AI assistance.

---

## Before You Submit or Merge

Use the following questions before submitting an artifact, merging a pull request, delivering a release note, or making an engineering presentation.

| Question | Yes / No / Evidence |
|---|---|
| Can another engineer understand what changed without asking you? |  |
| Is the claim supported by repository evidence? |  |
| Are risks, defects, or limitations stated honestly? |  |
| Is ownership clear? |  |
| Was AI-assisted content reviewed and verified? |  |
| Is the writing professional, concise, and action-oriented? |  |
| Would another engineer understand the operational impact, limitations, and risks from the communication alone? |  |

---

## Common Weak Patterns

Avoid:

* Vague issue titles
* Large unexplained commits
* Pull requests with no rationale
* Review comments that criticize without explaining
* Meeting notes without decisions or owners
* Release notes that list features but omit risks
* AI-polished writing that hides weak evidence
* Presentation claims unsupported by repository artifacts
* Operational claims without logs, notes, tests, or release evidence

---

## Instructor and Reviewer Use

Instructors and reviewers may use this playbook to evaluate whether team communication supports engineering review.

Strong communication should make a project easier to inspect.

Weak communication forces reviewers to reconstruct what happened from incomplete evidence.

---

## Bottom Line

Professional communication is not decoration.

It is how engineering teams coordinate work, preserve decisions, expose risk, review changes, and make software trustworthy.
