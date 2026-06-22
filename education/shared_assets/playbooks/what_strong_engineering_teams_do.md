# What Strong Engineering Teams Do

## Provenance

Origin: Loyola University Chicago COMP 330 — Software Engineering  
Original Context: COMP 330 team software engineering project  
ETIS Category: Shared Asset — Playbook  
Authoritative Format: Markdown  

This guide originated as a COMP 330 course asset and has been normalized as an ETIS shared playbook. It preserves Loyola COMP 330 provenance while making the guidance reusable across ETIS-aligned educational implementations.

---

## Purpose

This guide describes the behavior patterns expected of strong engineering teams in ETIS-aligned educational settings.

It is not a grading checklist by itself.

It is a practical standard for how professional teams make work visible, reviewable, testable, operationally understandable, and trustworthy.

---

## Core Principle

Strong teams do not wait for deadlines to discover whether the project works.

They build evidence continuously, communicate clearly, keep scope realistic, and make engineering decisions visible in GitHub as the authoritative project record.

The repository `README.md` should act as the professional front door linking to major engineering evidence and release artifacts.

---

## Strong Teams Usually

Strong engineering teams usually:

* Keep the repository current throughout the cycle
* Commit small, reviewable changes tied to issues, requirements, tasks, pull requests, and traceability evidence
* Use pull requests to expose rationale, risks, tests, reviews, and AI-use notes
* Connect requirements, tasks, architecture decisions, tests, defects, release notes, and presentation claims
* Review, govern, and verify AI-assisted work before accepting it
* Record how AI-assisted results were validated
* Document risks, tradeoffs, deferred scope, and known limitations honestly
* Update evidence as work happens, not as a last-minute documentation exercise
* Test important behavior early and repeatedly, including failure and boundary cases
* Make important runtime behavior, failures, operational assumptions, and recovery expectations visible as the system matures
* Communicate blockers before they become emergencies
* Prepare demos from stable releases supported by repository evidence, not last-minute hope

---

## Strong Teams Avoid

Strong engineering teams avoid:

* Dumping documentation into GitHub only at the deadline
* Merging code no one reviewed, tested, or understands
* Treating AI output as automatically correct or professionally owned by the tool
* Hiding defects, unfinished work, security concerns, or release risks
* Creating impressive slides without repository evidence
* Expanding scope when the core workflow is still fragile
* Producing artifacts for appearance rather than as evidence used to guide real engineering work
* Letting one person silently carry the project while the rest of the team becomes invisible
* Treating the demo as proof instead of a demonstration supported by evidence

---

## Operational Habits That Matter

Professional engineering evidence should be reviewable without requiring verbal clarification from the original team.

| Habit | What It Looks Like | Why It Matters |
|---|---|---|
| Small changes | Focused commits and pull requests | Makes review, testing, and rollback easier |
| Visible ownership | Primary and backup owners for artifacts and work areas | Prevents hidden work and single-person dependency |
| Continuous evidence | Artifacts updated as decisions and changes occur | Turns the repository into the authoritative engineering record |
| Risk honesty | Defects, limitations, and deferred scope are visible | Builds trust and supports mature release decisions |
| AI accountability | AI use is disclosed, reviewed, modified, tested, and owned | Keeps acceleration from becoming unmanaged risk |
| Stable demos | Demo paths are rehearsed from release evidence | Prevents presentation theater, unsupported release claims, and late-cycle chaos |

---

## Questions Strong Teams Ask Weekly

Strong teams regularly ask:

* What changed in the repository this week, and is the evidence visible?
* What requirement, risk, defect, or decision does this work connect to?
* What did AI help produce, and how did humans verify it?
* What is currently most likely to break the release or presentation?
* What should be cut, deferred, or simplified to protect quality?
* Could another engineer inspect the repository and understand our current state?
* What operational, observability, security, governance, or recovery concerns are emerging as the system matures?

---

## Strong Teams Make Work Inspectable

A strong team should be able to show:

* Current scope
* Current risks
* Current defects
* Current release claims
* Current testing evidence
* Current AI-use evidence
* Current ownership
* Current known limitations

If the team can only explain the project verbally, the repository evidence is too weak.

---

## Strong Teams Keep Scope Defensible

Strong teams do not treat feature volume as the definition of success.

They protect quality by asking:

* Is the core workflow stable?
* Is the evidence current?
* Are tests meaningful?
* Are risks visible?
* Are known limitations honest?
* Can the team defend the release?

A smaller defensible release is stronger than a larger fragile one.

---

## Strong Teams Use AI Professionally

Strong teams may use AI extensively, but they do not surrender responsibility.

They use AI to:

* Generate alternatives
* Identify gaps
* Critique requirements
* Suggest tests
* Review code
* Improve documentation
* Prepare release notes

They still:

* Review outputs
* Verify claims
* Test generated code
* Reject weak suggestions
* Disclose meaningful use
* Own the final decision

AI proposes.

Engineers verify.

---

## Strong Teams Prepare Releases With Evidence

Strong teams understand that release readiness is not the same as demo readiness.

Before presenting a release, they should be able to show:

* What works
* What changed
* What was tested
* What defects remain
* What limitations exist
* What AI contributed
* What risks remain
* What evidence supports the release claim

The presentation should be a guided tour of evidence, not the proof source itself.

---

## Instructor Expectation

A strong team is not the team with the most artifacts or the most code.

A strong team is the team whose work can be inspected, explained, tested, reviewed, and trusted.

---

## Core Thesis

Strong engineering teams make trust inspectable.

They do not rely on private explanations, hidden work, optimistic claims, or last-minute polish.

They create visible engineering evidence that allows others to understand, review, validate, operate, and improve the system.
