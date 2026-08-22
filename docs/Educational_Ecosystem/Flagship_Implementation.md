---
hide:
  - toc
---

<div style="text-align:center; margin-bottom:1.5rem;">
  <img src="../../assets/etis-logo.svg"
       alt="ETIS"
       style="width:320px; max-width:60%; height:auto;">
</div>

# ETIS COMP 330/474 Flagship Implementation

**A real-world educational laboratory for evidence-centered, AI-responsible software engineering**

The Loyola University Chicago COMP 330/474 implementation is the flagship ETIS educational implementation and feedback system.

It shows how ETIS operates in a real software engineering course—and how the Educational Ecosystem improves when tested through real students, teams, projects, constraints, reviews, and engineering evidence.

> Educational laboratories are where educational frameworks become trustworthy.

The ETIS Engineering Platform strengthens the implementation by providing a professional reference and implementation environment for staged engineering work. Teams use its Engineering Stages ES-100 through ES-114, templates, LMU/COICP reference examples, and governance assets to strengthen how they engineer their work. Project-specific engineering evidence is preserved in each team’s course repository.

---

## Purpose

The flagship implementation demonstrates how ETIS can be taught, operated, reviewed, and improved inside an academic software engineering course.

It is not the definition of ETIS.

It is a reference implementation and evidence-generating laboratory.

```text
ETIS Doctrine
↓
Education Papers and Educational Ecosystem
↓
Flagship Implementation
↓
Engineering Evidence and Feedback
↓
ETIS Improvement
```

---

## Implementation Context

| Area | Detail |
|---|---|
| **Institution** | Loyola University Chicago |
| **Courses** | COMP 330 — Software Engineering; COMP 474 — Software Engineering |
| **Instructor and ETIS Steward** | William T. O’Connell |
| **Course Model** | 15-week semester |
| **Enrollment Model** | Mixed undergraduate and graduate enrollment |
| **Team Model** | Engineering teams of approximately five to six students |
| **Graduate Student Model** | Graduate students intentionally distributed across teams, often in leadership roles |
| **Project Model** | One team project matured across the semester |
| **Engineering Model** | Two-cycle ETIS engineering model |
| **Review Model** | Six engineering phase gates |
| **Repository Model** | Private team GitHub repositories created from the COMP 330 course starter kit and used as the authoritative engineering record |
| **AI Model** | AI encouraged throughout the lifecycle and governed through ETIS principles |
| **Platform Model** | ETIS Engineering Platform used as a professional reference and implementation environment providing stages, templates, examples, and governance assets |

---

## Professional Provenance

The flagship implementation is informed by approximately four decades of software engineering experience, including IBM Distinguished Engineer and IBM CTO for Quality and Delivery Excellence experience across hundreds of organizations and client engagements.

That provenance matters because ETIS is not only an academic framework.

It carries professional engineering lessons into the classroom and asks students to experience software engineering as disciplined, reviewable, evidence-centered work.

---

## Core Thesis

COMP 330/474 is a bidirectional educational laboratory.

```text
ETIS informs the course.
The course tests ETIS.
The learners transform.
The evidence improves the next offering.
```

The course operationalizes ETIS doctrine.

The classroom tests educational assumptions.

Student repositories preserve evidence.

The semester generates feedback.

The framework and course improve.

---

## What the Implementation Demonstrates

The flagship implementation demonstrates that students can practice professional engineering behaviors in an academic course when the course is designed around evidence, review, accountability, and operational thinking.

Students can:

- work in engineering teams;
- use AI responsibly;
- maintain repository-centered evidence;
- make and defend requirements decisions;
- reason about architecture;
- perform reviews;
- produce test evidence;
- evaluate quality;
- consider security and operations;
- defend release readiness;
- reflect on improvement.

The implementation does not prove that every institution should copy Loyola’s course structure.

It demonstrates that ETIS doctrine can be implemented in a real educational environment.

---

## Two-Cycle Engineering Model

The flagship course compresses a much broader ETIS lifecycle into a semester-sized instructional path.

A semester cannot examine every ETIS chapter or lifecycle concern with equal depth. The Educational Ecosystem therefore supports different teaching models and durations. COMP 330/474 selects a deliberate path through the framework using a two-cycle delivery model.

```text
Cycle 1
Project launch → first release

Cycle 2
Operational enhancement → continued engineering responsibility
```

The first five phase gates form Cycle 1, moving the team from project launch through its initial release.

The sixth phase gate begins Cycle 2 as an operational enhancement. Students must work on a system that now exists, has accumulated engineering history, and carries continuing responsibility.

This structure reflects the broader movement of ETIS from the system-construction concerns emphasized in Volume I toward the operations, governance, oversight, and stewardship concerns emphasized in Volume II.

It does not attempt to compress the entire ETIS Framework into six gates.

> **Release changes the nature of engineering responsibility. It does not end it.**

A working demo is not operational proof.

---

## Six Engineering Phase Gates

The course uses six engineering phase gates to distribute accountability across the semester.

Phase gates prevent the course from collapsing into end-of-semester compression. They create recurring moments when students must present evidence, receive challenge, disposition findings, and improve the work.

Phase gates support:

- requirements accountability;
- planning accountability;
- architecture accountability;
- AI responsibility;
- testing and quality accountability;
- release readiness;
- operational thinking;
- team ownership.

The goal is not ceremony.

The goal is visible engineering maturity.

---

## Repository-Centered Engineering

GitHub supports the implementation because it is widely used and well suited to repository-centered work.

But ETIS is not defined by GitHub.

The repository functions as an engineering memory system.

Students preserve evidence such as:

- requirements;
- assumptions;
- plans;
- team roles;
- architecture decisions;
- AI-use logs;
- AI-verification notes;
- issues and pull requests;
- reviews;
- test evidence;
- defects;
- release notes;
- operational notes;
- postmortems and improvement records.

The tool can change.

The engineering behavior must endure.

Within the flagship implementation, the repository also becomes the shared evidence base for the ETIS Engineering Education Suite. Preflight checks phase-gate readiness, Engineering Studio supports repeated developmental review and engineering-judgment practice, and the Engineering Review Center supports the instructor's formal phase-gate review.

These systems improve visibility, continuity, and engineering feedback. They do not replace professional review, student responsibility, engineering judgment, or instructor authority.

---

## Engineering Platform and Engineering Education Suite

The Engineering Platform gives teams a repeatable lifecycle and evidence architecture.

Students can use Platform stages to understand what work comes next, templates and reference patterns to structure important artifacts, governance guidance to make AI-assisted work visible and reviewable, and LMU/COICP examples to calibrate the shape of professional engineering evidence.

The Engineering Education Suite then operates around the team's own authoritative course repository.

### ETIS Preflight

Before formal gate submission, Preflight uses phase-aware analytical heuristics and rules to identify whether expected evidence is present and has the basic shape needed for review.

### ETIS Engineering Studio

Throughout the phase, teams can create frozen evidence snapshots whenever a developmental review would help. The controlled engineering reviewers inspect the same team evidence, ask questions, challenge assumptions, and guide students toward stronger reasoning. When students need additional help, Studio can link them directly to relevant Platform stages, Starter Kit material, or LMU/COICP examples in a separate tab.

The reviewers coach and guide. They do not provide the engineering answer.

### ETIS Engineering Review Center

At the formal gate, the designated Git tag establishes the submitted evidence boundary. The instructor review environment analyzes that tagged evidence and provides rubric-aligned evidence, confidence, summaries, findings, and lineage back to the repository sources that support the analysis.

The instructor remains the academic authority.

### Developmental and Formal Review Remain Separate

An instructor can see Studio review history and student/reviewer dialogue, but the formal phase-gate analysis is based on the evidence presented at the gate. Studio conversations are not silently incorporated into the gate evidence.

```text
Engineer the work
      ↓
Use Studio repeatedly as evidence evolves
      ↓
Use Preflight to check gate readiness
      ↓
Tag the formal phase-gate submission
      ↓
Engineering Review Center analyzes tagged evidence
      ↓
Instructor exercises academic judgment
```

The sequence is intentionally not rigid. A team may return to Studio many times and may run Preflight more than once before the final tag.

> **Flagship Implementation — COMP 330/474 Software Engineering**
> COMP 330/474 combines the ETIS Framework, Engineering Platform, course-specific team repositories, and the Engineering Education Suite into the flagship classroom implementation of the ETIS educational model. Student teams progress through six phase-gate reviews across a two-cycle semester model while preserving the repository as the authoritative record of their engineering work.

[Explore the Engineering Education Suite →](Engineering_Education_Suite.md)

[Explore Engineering Studio →](Engineering_Studio.md)

[Explore the Platform Overview →](../Platform/Platform.md)

[Launch the Engineering Platform ↗](https://platform.etisframework.org)

[Browse the ETIS Engineering Platform Starter Kit Repository ↗](https://github.com/etis-framework/etis-starter-kit)

[View the COMP 330 Fall 2026 Starter Kit ↗](https://github.com/etis-framework/comp330-f26-starter-kit)

---

## Education Papers in the Flagship Course

The ETIS Education Papers provide a professional reading sequence for the course:

- [COMP-WP-001](../publications/education-papers/comp-wp-001.md) establishes why software engineering matters more in the AI era.
- [COMP-WP-002](../publications/education-papers/comp-wp-002.md) shows students how to turn course work into portfolio evidence.
- [COMP-WP-003](../publications/education-papers/comp-wp-003.md) establishes the professional team model.
- [COMP-WP-004](../publications/education-papers/comp-wp-004.md) defines responsible AI-assisted engineering.
- [COMP-WP-005](../publications/education-papers/comp-wp-005.md) connects course practices to long-term professional growth.

Together, these papers orient students before and during the engineering work.

---

## AI-Supported, Evidence-Governed Work

AI is encouraged throughout the lifecycle.

Students may use AI for ideation, drafting, code support, testing, documentation, review preparation, and operational reasoning.

But AI use must remain governed.

Students are expected to:

- disclose meaningful AI assistance;
- verify AI-generated artifacts;
- preserve evidence of verification;
- understand the work they submit;
- defend AI-supported decisions;
- avoid hidden dependency.

AI use is not an academic violation.

Undisclosed and unverified AI dependency is an engineering risk.

---

## Graduate Student Leadership

Graduate students are intentionally distributed across teams.

This creates a stronger team-learning model and gives graduate students opportunities to practice leadership, coordination, review, and technical judgment.

The role is not simply to do more work.

The role is to help the team mature.

Graduate student leadership supports:

- team accountability;
- project planning;
- technical decision-making;
- peer mentoring;
- review readiness;
- release-defense preparation;
- professional communication.

---

## Professional Portfolio Evidence

The flagship implementation encourages students to create repositories that can continue as professional portfolio evidence.

A strong repository can demonstrate that a student can:

- work in a team;
- reason about requirements;
- make design decisions;
- use AI responsibly;
- verify system behavior;
- respond to review;
- prepare release evidence;
- think operationally;
- improve from feedback.

Students should leave with more than a grade.

They should leave with credible evidence.

[Read COMP-WP-002 — Building a Professional Engineering Portfolio →](../publications/education-papers/comp-wp-002.md)

---

## Educational Feedback System

Each offering can reveal:

- where students struggle;
- where instructors need better guidance;
- where assignments need clearer sequencing;
- where AI policy needs refinement;
- where assessment needs stronger evidence;
- where repository structures need improvement;
- where ETIS doctrine needs clearer teaching pathways.

The course does not merely consume ETIS.

The course improves ETIS.

---

## What Other Institutions Should Learn

Institutions should study the flagship implementation to understand how ETIS can be operationalized.

They should not mechanically copy it.

Local adoption should consider:

- academic calendar;
- course level;
- student background;
- class size;
- tooling environment;
- institutional policy;
- AI expectations;
- assessment model;
- project scale;
- instructor capacity.

The right question is not:

> How do we copy COMP 330?

The right question is:

> How do we implement ETIS doctrine responsibly in our environment?

---

## Public Implementation Product

| Product | Purpose |
|---|---|
| **ETIS COMP 330 Flagship Implementation Guide** | Real-world reference for instructors, departments, universities, and institutional adopters |

The website introduces the implementation model.

The guide provides deeper implementation detail.

[Explore Educational Products →](Educational_Products.md)

---

## Implementation Boundary

The Loyola implementation is an adoption example.

It is not the ETIS architecture.

It is evidence, not doctrine.

```text
Educational products teach ETIS.
Focused publications orient the learner.
Adoption examples demonstrate ETIS in practice.
```

This boundary protects ETIS from becoming overfit to one course, university, semester model, or instructor.

---

## Bottom Line

The COMP 330/474 flagship implementation shows ETIS operating in a real educational environment.

It demonstrates that students can learn software engineering as professional, evidence-centered, AI-responsible work.

It also shows that a course can become an educational laboratory in which the framework, instructor, students, and engineering evidence improve one another over time.
