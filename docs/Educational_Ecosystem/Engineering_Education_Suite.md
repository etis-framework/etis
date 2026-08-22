---
hide:
  - toc
---

# ETIS Engineering Education Suite

**Phase-gate-aware educational systems for readiness, engineering judgment, and formal review**

The ETIS Engineering Education Suite is an integrated set of course systems designed for semester software engineering education.

The suite supports three distinct educational needs:

| Capability | Primary Persona | Core Question |
|---|---|---|
| **[ETIS Preflight](Preflight.md)** | Student team | Are we ready for formal phase-gate review? |
| **[ETIS Engineering Studio](Engineering_Studio.md)** | Students and student teams | Do we understand and have evidence for our engineering decisions? |
| **[ETIS Engineering Review Center](Engineering_Review_Center.md)** | Instructor | What does the evidence submitted for this phase gate actually demonstrate? |

The three capabilities are designed to work together, but they are modular. An adopting institution may use the complete suite or one or more components according to its instructional model.

The suite supports engineering analysis, developmental review, and instructor evaluation; it does not replace the instructor's academic judgment or authority. Evidence, findings, confidence assessments, summaries, and rubric-aligned analysis are inputs to instructor decision-making, not autonomous grading decisions.

The suite is **instructor-operated and course-configured**. It is not a public self-service application environment. Students use the capabilities provisioned and authorized for their course, section, team, and repositories.

---

## One Engineering Lifecycle, Three Different Roles

Preflight, Engineering Studio, and the Engineering Review Center are all **phase-gate aware**.

What they inspect, what evidence they expect, and how they analyze the work changes with the current phase gate. They also retain awareness of prior phase-gate analysis so that a team is not reviewed as if its project began at the current checkpoint.

The systems apply that context differently.

### ETIS Preflight — Readiness

Preflight uses analytical heuristics, rules, repository inspection, and phase-specific evidence expectations to determine whether the repository appears ready to enter formal review.

It asks whether expected evidence is present and whether that evidence has the basic shape needed for review.

It does **not** perform the formal phase-gate review.

### ETIS Engineering Studio — Judgment Development

Engineering Studio is the student-team learning environment.

Teams may create frozen evidence snapshots whenever a developmental review would help. Students can then interact independently with a controlled multidisciplinary engineering review board working from the same evidence.

The reviewers examine the repository holistically, surface facts and concerns, ask questions, challenge assumptions, probe reasoning, and guide students toward relevant ETIS resources. They coach and mentor; they do not provide the engineering answer.

### ETIS Engineering Review Center — Formal Review

The Engineering Review Center is the instructor-facing formal phase-gate environment.

At the gate, the course-designated Git tag establishes the formal evidence boundary. The review environment analyzes that evidence and provides rubric-aligned evidence, confidence, summaries, findings, and traceable lineage back to the repository sources that support the analysis.

The instructor remains the academic and evaluation authority.

---

## Developmental Review and Formal Review Stay Separate

ETIS intentionally separates learning before the gate from evaluation at the gate.

Engineering Studio may help a team improve through many developmental snapshots and reviewer conversations. An instructor may see the review history and student/reviewer dialogue for educational context.

The formal phase-gate review, however, is based on the evidence actually submitted at the gate. Studio conversations are not silently incorporated into the formal evidence decision.

This preserves a critical engineering principle:

> **The evidence presented for formal review must stand on its own.**

---

## Shared Controlled Review Board

Engineering Studio and the Engineering Review Center use the same controlled reviewer perspectives so that engineering expectations remain coherent across the semester.

The reference Studio includes six perspectives:

- Chief Architect / chair;
- Security Engineer;
- Verification Lead;
- Operations Lead;
- Human Impact Reviewer;
- Red Team.

Their role changes with context.

| Environment | Reviewer Role |
|---|---|
| **Engineering Studio** | Mentor, coach, challenger, and evidence-grounded reviewer |
| **Engineering Review Center** | Formal engineering review-board member analyzing submitted gate evidence |

The reviewers are bounded advisers. They do not become the engineering authority, fabricate evidence, or replace instructor judgment.

---

## Connection to the ETIS Engineering Platform

The Engineering Education Suite does not duplicate the [ETIS Engineering Platform](../Platform/Platform.md).

The Platform provides Engineering Stages ES-100 through ES-114, reusable templates, governance assets, evidence patterns, Project Workspace guidance, and completed LMU/COICP reference examples.

Engineering Studio can guide students to relevant Platform resources when the evidence shows that additional engineering guidance is needed. Students open those resources separately, study the appropriate stage, template, or example, and then return to their own work.

The relationship is intentional:

```text
ETIS Framework
    Defines the engineering discipline
        ↓
ETIS Educational Ecosystem
    Adapts the discipline to a course model
        ↓
ETIS Engineering Platform
    Provides stages, templates, patterns, and examples
        ↓
Student Team Repository
    Preserves the team's authoritative project evidence
        ↓
Engineering Education Suite
    Readiness + judgment development + formal review
        ↓
Instructor Judgment
```

Studio can point to knowledge and examples. It does not substitute those examples for the student's own engineering reasoning.

---

## The Semester Model Is an Educational Adaptation of ETIS

The ETIS Framework covers a broader lifecycle than any single semester can examine deeply.

The [Educational Ecosystem](Educational_Ecosystem.md) therefore supports different teaching models and durations. Instructors select an instructional path through the broader ETIS lifecycle appropriate to the course level, duration, and learning objectives.

The [COMP 330/474 flagship implementation](Flagship_Implementation.md) uses a two-cycle delivery model. The first five phase gates move teams from project launch through an initial release. The sixth begins an operational enhancement cycle that reinforces the continuing engineering responsibility emphasized as ETIS moves from the concerns of Volume I into the operational, governance, oversight, and stewardship concerns emphasized in Volume II.

> **Release changes the nature of engineering responsibility. It does not end it.**

The six-gate flagship model is a deliberate semester implementation, not a claim that the complete ETIS lifecycle contains only six gates.

---

## Adoption Model

The suite was developed around the COMP 330/474 Software Engineering flagship implementation at Loyola University Chicago and is designed so other universities can adopt the educational model for their own students and teams.

Adoption is not the same as downloading a consumer application.

An institution or instructor configures the course environment, identity, teams, repository authorization, phase-gate model, AI services, privacy and retention controls, and operating responsibilities appropriate to the local environment.

Institutions may adopt:

- ETIS educational doctrine without any ETIS software;
- ETIS course resources and the Engineering Platform;
- one or more Engineering Education Suite components;
- or the complete integrated suite.

[Explore Institutional Adoption →](Institutional_Adoption.md)

[Study the COMP 330/474 Flagship Implementation →](Flagship_Implementation.md)

---

## Bottom Line

The ETIS Engineering Education Suite is not a three-step grading pipeline.

It separates three professional questions that should remain distinct:

**Preflight:** Is the evidence ready to be reviewed?  
**Engineering Studio:** Can the students reason about and defend the engineering work?  
**Engineering Review Center:** What does the evidence submitted at the gate demonstrate?

Across all three, the repository preserves the evidence, the reviewers remain bounded, the current phase gate provides context, and human engineering judgment remains authoritative.
