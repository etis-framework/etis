# Demo and Presentation Readiness Checklist

**Classification:** ETIS Educational Ecosystem Asset  
**Category:** Workflow  
**Origin:** Loyola University Chicago COMP 330 — Software Engineering  
**Authoritative Format:** Markdown  
**Typical Repository Location:** `/docs/release/demo-presentation-readiness.md`

## Purpose

Use this checklist before a Cycle 1 release presentation or final Cycle 2 release presentation.

The presentation should be a guided tour of repository evidence. The live demo should be short, controlled, and supported by release notes, tests, defect/risk review, AI-use disclosure, known limitations, and operational evidence where appropriate.

A strong team does not ask reviewers to trust a demo.

A strong team shows the system, the evidence, and the limits.

Another engineering team should be able to understand the release claim, evidence, architecture, risks, known limitations, operational posture, and AI-assisted workflow decisions without relying on verbal explanation alone.

---

## Core Principle

The repository is the proof source.

Slides are structure.

The running system and evidence artifacts carry the argument.

A temporary demo failure should not invalidate repository evidence, release reasoning, or engineering reviewability.

---

## What the Presentation Must Prove

| Area | Expectation |
|---|---|
| Product clarity | The team can explain the problem, users, scope, and working vertical slice. |
| Controlled demo | The main user path works and at least one risk, validation, refusal, or boundary path is understood. |
| Engineering evidence | Repository artifacts support claims about requirements, architecture, tests, defects, AI use, risks, observability, operational readiness, release readiness, and recovery awareness where relevant. |
| Professional honesty | Known limitations, deferred work, residual operational concerns, bounded trust assumptions, and residual risks are stated clearly. |
| Team learning | The team can explain what changed, what was learned, and what should improve next. |

---

## Readiness Checklist

Before presentation day, verify each item below. Use the final column to record the repository link, file path, issue, pull request, or evidence location.

| Check | Ready? | Evidence Location / Notes |
|---|---|---|
| Repository README is current and points to the major evidence areas. | ☐ | |
| Release notes are complete and identify what shipped, what did not ship, known limits, and release judgment. | ☐ | |
| Requirements and acceptance criteria are current enough to support the demo claim. | ☐ | |
| Traceability connects key requirement(s) to issue/task, test/evaluation, demo step, and release evidence. | ☐ | |
| Major presentation claims are traceable through repository-visible evidence such as issues, pull requests, tests, ADRs, release notes, AI-use evidence, defects, risks, or operational artifacts when appropriate. | ☐ | |
| Architecture overview and major decisions are current enough to explain the system. | ☐ | |
| Test evidence is present: automated tests, manual checks, system checks, or AI validation where relevant. | ☐ | |
| Defects and risks are classified, owned, fixed, deferred, mitigated, or accepted with rationale. | ☐ | |
| AI-use log is updated and shows what AI helped produce and how humans verified it. | ☐ | |
| Team can explain why accepted AI-assisted work was considered reviewable, governable, testable, maintainable, and operationally supportable. | ☐ | |
| Demo path has been tested from a fresh start or clean setup. | ☐ | |
| Demo accounts, seed data, browser tabs, commands, and fallback materials are ready. | ☐ | |
| Each speaker owns a clear claim and knows which evidence supports it. | ☐ | |
| Team can answer: what is the highest risk, what did tests prove, what did AI touch, and what would we fix next? | ☐ | |

---

## Recommended 15-Minute Presentation Spine

Teams may adjust timing slightly, but the presentation should stay focused and evidence-backed.

| Target Time | Segment | Focus |
|---|---|---|
| 1-2 min | Problem and scope | Who has the need? What did this cycle promise? What was intentionally deferred? |
| 2-3 min | System and architecture | Show the major workflow, components, data, interfaces, and key decisions at a high level. |
| 3-4 min | Live demo | Show one main path and one boundary/risk path. Keep it controlled and repeatable. |
| 3-4 min | Repository evidence | Show release notes, tests, defects/risks, AI-use log, and traceability links. |
| 1-2 min | Reflection and next steps | What changed, what was learned, what remains risky, and what the next engineering move should be. |

---

## Demo Strategy

### One main path

Show the core user story from start to finish.

Do not wander through every screen.

### One risk path

Show at least one validation, refusal, error handling, boundary case, or limitation.

### One evidence link

Connect the demo to a requirement ID, test, defect, pull request, release note, or known limitation.

### Backup plan

Have screenshots, a recorded clip, seed data, or manual fallback notes ready.

A live demo can fail. The engineering evidence still needs to survive.

---

## Cycle-Specific Emphasis

| Presentation | Primary Question | Evidence Emphasis |
|---|---|---|
| Cycle 1 Release | Can the team build and present a controlled first release? | Working vertical slice, requirements, architecture, tests, defects, AI-use log, release notes, known limitations. |
| Final Cycle Release | Can the team prove engineering maturity after Cycle 1? | What changed after feedback, stronger testing, observability, security/governance, risk disposition, AI-use reflection, final release judgment, rollback/recovery understanding, supportability evidence, and release-defensibility reasoning. |

---

## Speaker Ownership

Do not let one person carry the entire story.

Each speaker should own a specific claim, artifact, and transition.

An example flow:

| Speaker Role | Responsibility |
|---|---|
| Team Lead | Opening, scope, release claim, transitions, closing. |
| Product / Requirements Owner | User story, acceptance criteria, deferred scope. |
| Architecture / Development Owner | System structure, repository organization, major decisions. |
| Quality / Review Owner | Tests, defects, AI-use evidence, known limitations. |
| Demo Driver | Controlled demo path, backup plan, and evidence handoff. |

Each speaker should understand both the claim they present and the repository evidence supporting that claim.

---

## Common Presentation Failure Modes

- Showing a demo but no evidence.
- Walking randomly through screens instead of proving a user workflow.
- Claiming “everything works” without tests, limitations, or defect review.
- Hiding AI usage or being unable to explain AI-assisted work.
- One speaker doing all the talking while others appear disconnected.
- Slides become the product while the repository and system disappear.
- Major risks, defects, known limitations, or operational concerns are hidden.
- The team cannot trace presentation claims back to repository evidence.

---

## Final Takeaway

A strong presentation makes the reviewer more confident after asking hard questions.

Show the system.

Show the evidence.

Show the limits.

The repository is the proof source; the presentation is the guided tour.
