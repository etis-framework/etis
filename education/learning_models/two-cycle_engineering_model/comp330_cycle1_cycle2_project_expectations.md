# COMP 330 Two-Cycle Engineering Project Model

Software Engineering in the AI Era

Loyola University Chicago

An ETIS Educational Ecosystem Flagship Implementation

---

## Provenance

This document originated from Loyola University Chicago COMP 330 — Software Engineering.

It serves as the flagship implementation of the ETIS Two-Cycle Engineering Model.

While many concepts may eventually become reusable educational assets, this document intentionally preserves COMP330 provenance because it reflects a specific educational implementation.

Future ETIS educational implementations may adapt the model while preserving the underlying principles.

---

## Core Idea

The COMP 330 project is not two coding deadlines.

Cycle 1 proves that the team can build a controlled vertical slice with evidence.

Cycle 2 proves that the team can learn from Cycle 1, improve the system, and make a defensible final release judgment.

---

## 1. Purpose of the Two-Cycle Project Model

The COMP 330 project is organized as two development cycles because professional software engineering is not a one-shot coding exercise.

Teams must learn to define the problem, make commitments, build a controlled first release, review evidence, learn from defects and feedback, and then mature the system.

The two-cycle model intentionally separates first-release capability from engineering maturity.

A working Cycle 1 demo matters, but it is not the end of the project. The stronger professional question is what the team learned from Cycle 1 and how that evidence changed Cycle 2 decisions.

### Cycle 1: Controlled Vertical Slice

Cycle 1 asks:

```text
Can it work?
```

The team demonstrates that it can organize, plan, architect, construct, review, test, and release a small working system with evidence.

### Cycle 2: Evidence-Based Maturity

Cycle 2 asks:

```text
Can it survive?
```

The team uses postmortem evidence, defects, risks, estimates, testing gaps, review feedback, and presentation feedback to improve quality, security, governance, observability, and release readiness.

---

## 2. Team Size, Team Formation, and Team Engineering Expectations

Teams will be formed by Week 2.

The expected team size is usually four to five students.

A three-person team can work, but it is fragile.

A six-person team is possible, but it should be treated as the upper limit because coordination overhead and hidden work increase quickly.

Software engineering is a team discipline.

Everyone on the team is a developer and engineering contributor first. Every student is expected to contribute to implementation, review, testing, documentation, and repository evidence.

Additional operational roles exist to make ownership visible, not to excuse anyone from technical contribution.

Every team member must own visible repository work.

Repository-visible workflow evidence should include issues, branches, pull requests, reviews, commits, and traceability links as the project matures.

Every team member must participate in review and evidence creation.

Every team member must understand the system well enough to explain the team's main engineering claims.

Every role must have a primary owner and a backup so the team does not fail when one person is unavailable.

> **Professional warning**  
> Uneven contribution is common in student teams and in industry teams. COMP 330 does not assume every team works perfectly. It requires visible ownership, weekly status checks, GitHub evidence, pull requests, reviews, peer feedback, and role accountability so contribution problems become visible early instead of appearing at the deadline.

---

## 3. Professional Responsibility Roles

The following five operational roles should be assigned to students.

Smaller teams may combine roles.

Larger teams may split responsibilities if approved by the instructor.

The role model is intentionally lightweight. It creates accountability without turning the project into bureaucracy.

| Role | Primary Responsibility | Typical GitHub Evidence Owned |
|---|---|---|
| Team Lead | Meeting cadence, team coordination, decision visibility, milestone readiness, team accountability | `/docs/team/team-charter.md`, `/docs/team/working-agreements.md`, meeting notes, milestone checklists |
| Planning & Process Lead | Scope, task plan, estimates, risks, schedule, issue hygiene, progress tracking | `/docs/planning/`, GitHub Issues, `/docs/planning/risk-register.md`, `/docs/planning/traceability.md` |
| Architecture & Development Lead | Architecture coherence, repository structure, implementation coordination, technical decision records | `/src`, `/docs/architecture/`, `/docs/decisions/`, `README.md` |
| Quality & Review Lead | Testing, pull request discipline, review evidence, CI/CD checks, defect tracking, validation evidence | `/tests`, `/docs/testing/`, `/docs/reviews/`, `/.github/workflows/`, `/docs/quality/` |
| Operations & Evidence Lead | Release evidence, observability, known limitations, AI-use evidence, final evidence index, presentation evidence readiness | `/docs/release/`, `/docs/observability/`, `/docs/ai/`, `/docs/security/`, security-governance checklist |

Role ownership means responsibility for correctness, completeness, and readiness of the evidence at the proper point in the cycle.

It does not mean the owner is the only person allowed to update the artifact.

Any team member may update any evidence artifact when doing legitimate project work.

The owner is responsible for making sure the artifact is accurate, current, reviewable, and linked to the rest of the project evidence when the milestone arrives.

### Ownership Rules

| Ownership Level | Responsibility |
|---|---|
| Primary owner | Accountable for keeping the artifact correct and ready |
| Backup owner | Able to step in if the primary owner is unavailable |
| All team members | Allowed and expected to update evidence when their work affects it |
| Team | Responsible for reviewing important evidence before submission or presentation |

---

## 4. Minimum Weekly Cadence Meetings

Each team must run a minimum weekly cadence meeting.

This can be on Zoom or in person, on any day and time the team chooses.

The purpose is not to hold a long engineering design session.

The purpose is to keep status, ownership, blockers, commitments, and evidence visible.

When done correctly, the weekly cadence meeting should usually take 15 to 30 minutes, with a target closer to 15 minutes.

Longer design discussions, debugging sessions, architecture debates, or pair-programming work should be scheduled separately.

### Recommended Cadence Agenda

Each weekly cadence meeting should answer:

1. What did each person complete since the last checkpoint?
2. What is each person doing next?
3. What is blocked, unclear, risky, or behind schedule?
4. What GitHub evidence changed?
5. What agreement or decision did the team make?
6. What repository evidence, issue updates, pull requests, or documentation changes are required before the next checkpoint?
7. What must be ready before the next class, milestone, or submission?

GitHub evidence may include:

* Issues
* Branches
* Pull requests
* Tests
* Documentation
* AI-use log entries
* Architecture decisions
* Release evidence

> **Cadence rule**  
> A cadence meeting is a status and accountability checkpoint. It is not the place to design the entire architecture, debug a hard failure, or debate every implementation option. Those are real engineering meetings, but they should be scheduled separately.

---

## 5. Cycle 1 Expectations: Controlled Vertical Slice

Cycle 1 is intentionally longer than the raw implementation size of the default project would require in industry.

A professional team assigned a small version of this project might implement much of the basic functionality quickly.

COMP 330 slows the work down on purpose because students are learning the full engineering discipline around the work, not just the code.

Cycle 1 is the crawl phase.

The team is learning how to form, define scope, create evidence, make estimates, document architecture, use GitHub professionally, review AI-assisted work, test the system, and present a release.

Weekly progress is still required.

Teams that wait until the deadline will struggle because late work leaves no time for review, testing, integration, defect correction, or evidence cleanup.

### Cycle 1 Minimum Expectations

By the end of Cycle 1, the team should have:

* Formed the team and assigned roles, with backups identified
* Created and used the GitHub repository as the authoritative engineering record
* Established the repository `README.md` as the professional front door to the project and major engineering evidence
* Defined a Cycle 1 vertical slice and kept it intentionally small
* Documented requirements, acceptance criteria, assumptions, risks, and out-of-scope decisions
* Maintained task plan, estimates, schedule, traceability, and team commitments
* Made architecture, interfaces, data/context ownership, and governance boundaries reviewable
* Completed implementation through issues, branches, pull requests, reviews, and tests
* Disclosed, reviewed, verified, and owned AI use
* Presented the Cycle 1 release with evidence, known limitations, risks, and lessons learned

### Cycle 1 Professional Standard

Cycle 1 does not prove that the system is mature.

Cycle 1 proves that the team can create a controlled, reviewable, evidence-backed first release.

---

## 6. Cycle 2 Expectations: Evidence-Based Maturity

Cycle 2 is shorter and should not become a feature binge.

It is not a restart.

It is also not a promise to complete every improvement idea listed in the project overview.

Cycle 2 work must be selected and scoped based on evidence from Cycle 1.

The Cycle 1 postmortem is the decision point.

Teams should use defects, missed estimates, weak tests, review feedback, architecture pain, AI-use issues, presentation questions, and known limitations to choose the highest-value maturity work.

The goal is to improve the credibility of the system, not simply add sparkle.

### Cycle 2 Minimum Expectations

During Cycle 2, the team should:

* Review Cycle 1 evidence before choosing Cycle 2 work
* Identify root causes, not just symptoms
* Re-estimate remaining and new work based on actual Cycle 1 performance
* Select a small number of maturity targets the team can complete and prove
* Improve tests, defects, architecture, observability, runtime visibility, security/governance, AI-use controls, or release documentation as appropriate
* Document what was intentionally deferred and why
* Prepare a final release argument supported by repository evidence
* Identify the repository state associated with major releases using release tags, versions, or equivalent release markers when appropriate

### Cycle 2 Professional Standard

Cycle 2 proves whether the team can learn.

A mature Cycle 2 release should show improved engineering judgment, stronger evidence, clearer release claims, and more realistic awareness of operational risk.

---

## 7. Evidence Ownership by Role and Cycle

The table below connects operational roles to the main evidence they are expected to keep healthy.

These are ownership lanes, not walls.

Teammates may and should help each other, but the owner is accountable for readiness at each milestone.

Engineering evidence should be reviewable without requiring verbal clarification from the original team.

| Role | Evidence Owned | Why It Matters |
|---|---|---|
| Team Lead | Team charter, working agreements, meeting notes, milestone readiness | Keeps team decisions, communication rhythm, and submission readiness visible |
| Planning & Process Lead | Scope, task plan, estimates, risk register, schedule, traceability | Keeps work bounded, sequenced, owned, and connected to requirements |
| Architecture & Development Lead | Architecture package, decision records, repository structure, implementation coordination | Keeps the design understandable, changeable, and aligned with implementation |
| Quality & Review Lead | Tests, defect log, pull request review evidence, CI/CD evidence, validation evidence | Keeps quality claims backed by inspection, tests, reviews, and defect discipline |
| Operations & Evidence Lead | AI-use log, release notes, known limitations, observability evidence, security/governance evidence, final evidence index | Keeps release claims, AI accountability, operational maturity, and final presentation evidence defensible |

---

## 8. How This Compares to Industry Practice

Industry teams often operate with short status rituals, explicit ownership, issue tracking, pull requests, build checks, release notes, and postmortems.

COMP 330 uses a classroom version of that pattern.

The goal is not to imitate every industry tool or ceremony.

The goal is to practice the engineering habits that make team software controllable.

Professional engineering maturity includes operational stewardship, accountable review behavior, honest risk communication, and evidence that another engineer can independently inspect.

In professional teams, a 15-minute status check is not where all engineering work happens.

It is where the team synchronizes.

The real work happens in issues, design notes, pull requests, tests, reviews, documentation updates, and focused working sessions.

COMP 330 expects the same distinction.

Professional teams also experience uneven contribution, missed estimates, unclear ownership, and communication failures.

The professional response is not denial.

The professional response is visibility: identify the problem, adjust responsibilities, document risks, and make sure the evidence reflects reality.

---

## 9. What Is Not Acceptable

The following behaviors are not acceptable in COMP 330 project work:

* Waiting until the deadline to create GitHub evidence
* Treating the project as separate individual parts that are never integrated
* Using AI-generated work that the team cannot explain or verify
* Skipping reviews because the code appears to work
* Holding vague meetings with no decisions, owners, or next actions
* Submitting a polished document that does not point to repository evidence
* Presenting a demo while hiding known limitations, defects, or risks
* Treating the final presentation as proof instead of repository-supported engineering evidence
* Allowing one or two students to carry the project while others remain invisible

---

## 10. What Teams Should Do Immediately

Teams should do the following as soon as project work begins:

1. Confirm team membership by Week 2.
2. Select a team name and primary communication channel.
3. Assign the five professional responsibility roles and identify backups.
4. Choose the default project or propose an instructor-approved alternative.
5. Schedule the weekly cadence meeting.
6. Create the GitHub repository and minimum folder structure.
7. Draft the team charter, role matrix, working agreements, and AI-use policy.
8. Define the Cycle 1 vertical slice and the first small set of issues.
9. Identify which evidence artifacts each role owner must keep current before the first submission.

---

## Relationship to the ETIS Learning Models

This document operationalizes the Two-Cycle Engineering Model inside the Loyola COMP330 flagship implementation.

It connects directly to the broader ETIS learning model architecture.

### Professional Transformation Model

The two-cycle model helps students move from:

```text
Student
↓
Responsible Engineer
↓
Reviewer
↓
Release Defender
```

Cycle 1 introduces responsible engineering behavior.

Cycle 2 strengthens reviewability, release defense, and operational awareness.

### Engineering Maturity Model

Cycle 1 primarily moves students from task completion toward structured participation.

Cycle 2 moves students toward evidence-based engineering and reviewable engineering judgment.

### Software Engineering Learning Progression

The two-cycle model gives the learning progression a project rhythm.

Cycle 1 emphasizes orientation, intent formation, engineering structure, and initial construction.

Cycle 2 emphasizes improved construction, verification, release defense, operational awareness, and professional reflection.

---

## Final Takeaway

The project succeeds when the team can show both a useful system and the engineering evidence behind it.

A professional team does not ask others to trust a demo.

It shows the requirements, design, review, tests, risks, AI-use decisions, release notes, and maturity evidence that make the demo credible.
