# Student Success Pattern

## Provenance

Origin: Loyola University Chicago COMP 330 — Software Engineering  
Original Context: COMP 330 team software engineering project  
ETIS Category: Shared Asset — Playbook  
Authoritative Format: Markdown  

This guide originated as a COMP 330 course asset and has been normalized as an ETIS shared playbook. It preserves Loyola COMP 330 provenance while making the guidance reusable across ETIS-aligned educational implementations.

---

## Purpose

This guide summarizes the habits that help student engineering teams succeed in ETIS-aligned software engineering courses.

The course rewards steady engineering evidence, responsible AI use, professional communication, and honest release judgment.

It does not reward last-minute artifact production or unsupported confidence.

---

## Core Idea

Successful teams do not merely produce more artifacts.

They build a visible engineering trail that shows:

* What they intended
* What they changed
* What they verified
* What risks remain
* What AI assistance was used
* Why the release should be trusted

The goal is not volume.

The goal is credible engineering evidence.

---

## Course Operating Model

Use the course platform to understand what to do each week.

Use GitHub to prove what the team actually did.

In COMP 330, Sakai explains workflow, expectations, modules, assignments, and resources.

GitHub stores the authoritative engineering evidence:

* Decisions
* Requirements
* Plans
* Issues
* Pull requests
* Tests
* Defects
* Release notes
* AI-use evidence
* Operational maturity artifacts

The repository `README.md` should serve as the professional front door to the project and link to major engineering evidence.

---

## The Success Pattern

| Habit | What It Means | Evidence You Should Produce |
|---|---|---|
| Start weekly | Read the current module before the work begins. | Updated issues, team notes, and clear next steps. |
| Build evidence continuously | Do not wait until the deadline to document work. | Repository updates, issues, branches, pull requests, changed files, test notes, and decisions as work occurs. |
| Keep scope small | Protect a controlled vertical slice before expanding. | Explicit included scope, deferred scope, and release limitations. |
| Use AI responsibly | Use AI to accelerate thinking and artifact production, but verify, govern, and own the result. | AI-use log entries, review notes, rejected output, and validation evidence. |
| Review like engineers | Treat reviews as quality gates, not personal criticism. | Pull requests, review comments, fixes, and merge rationale. |
| Make risks visible | Expose uncertainty early instead of hiding it. | Risk register entries, defect log updates, mitigations, owners, and status. |
| Tell the truth about readiness | A demo is not enough; release claims need evidence. | Release notes, known limitations, test evidence, CI results, release/version evidence, and presentation evidence links. |

---

## Weekly Team Rhythm

A strong weekly rhythm should include the following actions.

* Review the current course module and assignment expectations.
* Confirm who owns each active task, artifact, review, or risk.
* Update GitHub issues, pull requests, and repository artifacts during the week.
* Use AI where helpful, then verify the result against requirements, architecture, security, and tests.
* Record important decisions, risks, defects, and limitations while they are fresh.
* Capture important runtime behavior, observability findings, operational concerns, or recovery issues as they emerge.
* End each week knowing what changed, what evidence exists, what is blocked, and what comes next.

Professional rule:

> Engineering evidence should be reviewable without requiring verbal clarification from the original team.

---

## What Successful Teams Do Early

Successful teams usually:

* Form roles quickly
* Establish communication expectations
* Build a repository structure early
* Keep the first scope intentionally small
* Start requirements before implementation accelerates
* Identify assumptions and open questions
* Create issues before large code changes
* Use pull requests as review evidence
* Record AI use when it materially affects the work
* Prepare evidence continuously instead of rushing at the deadline

---

## What Successful Teams Do During the Project

Successful teams usually:

* Keep the repository current
* Link work to requirements, issues, risks, or decisions
* Review code and artifacts before treating them as accepted
* Add tests as behavior becomes important
* Update documentation when the system changes
* Surface blockers early
* Revisit scope based on evidence
* Track defects and limitations honestly
* Prepare release evidence before presentations

---

## What Successful Teams Do Near Release

Successful teams usually:

* Freeze or stabilize scope before the release deadline
* Verify important behavior
* Document known limitations
* Update release notes
* Connect presentation claims to repository evidence
* Rehearse the demo from a stable release state
* Explain what was deferred and why
* Reflect on what Cycle 1 taught them before planning Cycle 2

---

## Avoid These Failure Patterns

Avoid:

* Treating the Word submission as the evidence instead of an index to GitHub
* Creating documents at the deadline that were not used to guide actual work
* Letting AI produce code, tests, or documents the team cannot explain
* Adding features while core workflow, tests, risks, or release notes are weak
* Presenting confident claims without repository evidence behind them
* Treating presentations or demos as proof instead of repository-supported engineering evidence
* Allowing one person to silently carry the project while others remain invisible
* Expanding scope because the team feels behind instead of narrowing scope to protect quality

---

## Repository Success Standard

A successful student repository should make it possible for another engineer to answer:

* What problem is this team solving?
* What scope did the team choose?
* What requirements were accepted?
* What risks were known?
* What changed during implementation?
* What was reviewed?
* What was tested?
* What AI assistance was used?
* What limitations remain?
* What evidence supports release readiness?

If the repository cannot answer these questions, the team likely needs stronger engineering evidence.

---

## AI Success Standard

AI use is expected in modern engineering work.

Successful teams do not hide AI use and do not trust it blindly.

They:

* Use AI to accelerate thinking
* Review the output
* Modify weak suggestions
* Reject unsafe or unsupported recommendations
* Verify accepted work
* Record meaningful AI assistance
* Own the final result

The standard is not whether AI was used.

The standard is whether the team used AI professionally.

---

## Release Success Standard

A successful release is not merely a working demonstration.

A successful release is supported by:

* Requirements evidence
* Test evidence
* Review evidence
* Defect and limitation evidence
* AI-use evidence
* Release notes
* Risk disposition
* Operational awareness
* Clear presentation evidence

A demo can show behavior.

The repository must support the engineering claim.

---

## Key Idea

Successful teams do not produce more artifacts for the sake of volume or appearance.

They build a visible engineering trail that shows what they intended, what they changed, what they verified, what risks remain, and why the release should be trusted.
