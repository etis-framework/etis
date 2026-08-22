---
hide:
  - toc
---

<div style="text-align:center; margin-bottom:1.5rem;">
  <img src="../../assets/etis-logo.svg"
       alt="ETIS"
       style="width:320px; max-width:60%; height:auto;">
</div>

# ETIS Student Resources

**Professional engineering practice, responsible AI use, evidence, teamwork, and career readiness**

ETIS Student Resources help students practice software engineering as professional engineering work in the AI era.

Students are not simply asked to build software.

They are expected to create evidence that their work can be understood, reviewed, governed, operated, improved, and trusted over time.

> The model is not the system.  
> The repository is not just code.  
> Engineering work must leave evidence.

The ETIS Engineering Platform provides the practical workspace. Engineering Stages ES-100 through ES-114, templates, LMU/COICP examples, governance assets, and Project Workspaces help students produce reviewable engineering evidence instead of isolated assignment artifacts.

---

## Start Here

| Resource | Use It For |
|---|---|
| [From Data Structures to Engineering Judgment](../Books/engineering-judgment/index.md) | Develop professional engineering judgment using data structures and algorithms as the technical teaching vehicle |
| [ETIS Books](../Books/index.md) | Explore the Framework Reference Work and Professional Computing Series |
| [COMP-WP-001](../publications/education-papers/comp-wp-001.md) | Understand why software engineering matters more in the AI era |
| [COMP-WP-002](../publications/education-papers/comp-wp-002.md) | Build a credible professional engineering portfolio |
| [COMP-WP-003](../publications/education-papers/comp-wp-003.md) | Work effectively on an engineering team |
| [COMP-WP-004](../publications/education-papers/comp-wp-004.md) | Use AI professionally |
| [COMP-WP-005](../publications/education-papers/comp-wp-005.md) | Connect course work to long-term engineering growth |
| [Platform Overview](../Platform/Platform.md) | Learn how the Platform supports ETIS student work |
| [Launch the Engineering Platform ↗](https://platform.etisframework.org) | Enter the working project environment |
| [Student Professional Engineering Guide](Educational_Products.md#student-product) | Obtain deeper practical guidance |

Course requirements vary by implementation. Your instructor or course LMS determines which ETIS books, publications, tools, and resources are required.

---

## Professional Computing and Engineering Judgment

The **ETIS Professional Computing Series** provides longer-form works for developing professional computing judgment.

Its inaugural title, *From Data Structures to Engineering Judgment*, is intentionally not a conventional data structures textbook, programming guide, or algorithms reference. It uses data structures and algorithms as the technical vehicle for learning how engineers reason about representation, performance, tradeoffs, evidence, verification, system consequences, AI-assisted work, and professional responsibility.

The goal is not simply to know which structure or algorithm to choose. The goal is to be able to explain **why** a choice is appropriate, what assumptions and boundaries it depends on, what evidence supports it, and what consequences follow from it.

[Explore *From Data Structures to Engineering Judgment* →](../Books/engineering-judgment/index.md)

[Explore the ETIS Professional Computing Series →](../Books/ETIS_Professional_Computing_Series.md)

---

## What Makes ETIS Student Work Different

Traditional pattern:

```text
Receive assignment
↓
Build software
↓
Submit final artifact
↓
Receive grade
```

ETIS pattern:

```text
Define intent
↓
Plan work
↓
Engineer context
↓
Use AI responsibly
↓
Build and verify
↓
Preserve evidence
↓
Review and defend
↓
Improve from feedback
```

The goal is not only to finish the project.

The goal is to become a trustworthy engineer.

---

## Student Transformation Model

```text
Student
↓
Responsible Engineer
↓
Reviewer
↓
Architect
↓
Release Defender
↓
Operational Thinker
↓
Future Trustworthy Engineer
```

Each stage requires stronger evidence, better judgment, and greater ownership.

---

## A Professional Repository Pattern

The Engineering Platform illustrates a professional repository structure in which responsibilities are separated clearly:

| Area | Responsibility |
|---|---|
| `docs/` | Think, decide, explain, and preserve evidence |
| `src/` | Build the system |
| `tests/` | Verify behavior |
| `data/` | Support realistic use and evaluation |
| `scripts/` | Automate repeatable work |

The most important area is often `docs/`.

That is where intent, assumptions, decisions, reviews, risks, and release evidence become visible.

Your course repository may adapt this structure. Follow the repository model and evidence requirements established by your instructor rather than assuming that every ETIS course uses the Platform Project Workspace directly.

[Explore the Platform Overview →](../Platform/Platform.md)

[Launch the Engineering Platform ↗](https://platform.etisframework.org)

---

## Student Engineering Systems

ETIS student-facing systems help you prepare evidence and develop engineering judgment before formal phase-gate review.

### ETIS Preflight

[ETIS Preflight](Preflight.md) checks whether the evidence expected for the current phase gate is present and has the basic shape needed for review.

Use it to find readiness gaps while you still have time to improve the repository.

Passing a readiness check does not prove that an engineering decision is correct. You remain responsible for the quality, accuracy, completeness, and meaning of the evidence you submit.

[Open ETIS Preflight Repository ↗](https://github.com/etis-framework/comp330-submission-preflight){ .md-button }

### ETIS Engineering Studio

[ETIS Engineering Studio](Engineering_Studio.md) is the team learning environment for deeper engineering review.

Your team can create frozen evidence snapshots as the project evolves. Every student on the team sees the same snapshot evidence, but each student can ask questions and interact independently with the controlled engineering reviewers.

Use Studio to:

- conduct mini-reviews before the formal gate;
- ask why a reviewer surfaced a fact or concern;
- defend a decision with repository evidence;
- challenge a reviewer when the evidence supports a different conclusion;
- identify risks, unknowns, and unresolved decisions;
- strengthen your reasoning before the tagged submission;
- open relevant Engineering Platform stages, Starter Kit guidance, or LMU/COICP examples when additional help is needed.

The reviewers do not give you the answer. They coach and challenge you so that **you** remain the engineer.

Your instructor provisions the course environment and determines which ETIS systems your course uses.

---

## Engineering Evidence Package

Student repositories should include evidence such as:

- requirements and assumptions;
- acceptance criteria;
- planning artifacts;
- task plans and schedules;
- team roles and working agreements;
- architecture descriptions and ADRs;
- AI-use logs;
- AI-verification notes;
- code and architecture review evidence;
- test plans, cases, and results;
- defect logs and quality notes;
- security and data-handling notes;
- release-readiness evidence;
- demo scripts and known limitations;
- operational notes and runbooks;
- observability plans;
- postmortem and improvement evidence.

This is not paperwork.

It is how engineering work becomes reviewable.

---

## Repository-Centered Engineering

A strong repository should answer:

- What are we building?
- Why are we building it?
- What assumptions are we making?
- What decisions did we make?
- What evidence supports our claims?
- What risks remain?
- How did we use AI?
- How did we verify the work?
- Is the system ready to release, demonstrate, or operate?
- What should improve next?

If those answers are not visible, the engineering work is incomplete.

---

## AI Use and Verification

AI may support:

- brainstorming;
- requirements refinement;
- design alternatives;
- code generation;
- test generation;
- documentation drafting;
- defect analysis;
- review preparation;
- operational planning.

Students remain responsible for the work.

Professional expectations include:

- disclose meaningful AI assistance;
- verify generated artifacts;
- preserve evidence of verification;
- reject unsupported or incorrect output;
- understand submitted work;
- defend the engineering decision;
- respect data, security, licensing, and authorization boundaries.

AI proposes.

Engineers verify.

[Read COMP-WP-004 — Using AI Professionally →](../publications/education-papers/comp-wp-004.md)

---

## Team Engineering

Strong teams make work visible.

They preserve:

- roles and responsibilities;
- working agreements;
- communication plans;
- decisions;
- risks;
- blockers;
- review outcomes;
- ownership boundaries.

Roles create primary accountability, not silos.

Review creates shared responsibility, not ceremonial approval.

[Read COMP-WP-003 — Working Effectively on an Engineering Team →](../publications/education-papers/comp-wp-003.md)

---

## Reviews and Defenses

Students should be prepared to defend:

- requirements choices;
- scope decisions;
- architecture tradeoffs;
- AI-assisted work;
- testing strategy;
- quality evidence;
- security assumptions;
- release readiness;
- operational risks;
- known limitations.

Engineering work is not complete until it can be defended.

---

## Individual Accountability

Students should be able to explain:

- what they personally contributed;
- what the team produced;
- what evidence supports the work;
- what AI helped create;
- how AI output was verified;
- what risks remain;
- what they would improve next.

The strongest students do not merely say, “It works.”

They show why the work should be trusted.

---

## Professional Portfolio Value

A strong ETIS repository can become professional portfolio evidence.

It can show future employers that a student can:

- work in a team;
- reason about requirements;
- make architectural decisions;
- use AI responsibly;
- test and verify systems;
- handle defects and quality issues;
- think about security and operations;
- prepare release evidence;
- explain tradeoffs;
- improve from review.

Students should leave the course with evidence of engineering ability—not only a grade.

[Read COMP-WP-002 — Building a Professional Engineering Portfolio →](../publications/education-papers/comp-wp-002.md)

---

## Student Product

| Product | Purpose |
|---|---|
| **ETIS Student Professional Engineering Guide** | Deeper guidance for professional behavior, responsible AI use, repository evidence, review, release defense, and portfolio development |

[Explore Educational Products →](Educational_Products.md)

---

## How to Use Student Resources

1. Read the Education Papers and any ETIS book assigned or relevant to your course.
2. Understand repository-centered engineering.
3. Use the Engineering Platform Project Workspace or the course-specific repository environment designated by your instructor.
4. Organize evidence before producing too much code.
5. Use ETIS Preflight before formal gates to identify readiness gaps in the expected repository evidence.
6. Use Engineering Studio when available to conduct developmental mini-reviews, ask questions, challenge findings, and strengthen engineering judgment.
7. Use AI responsibly and visibly.
8. Preserve decisions, tests, reviews, and release evidence.
9. Prepare to defend engineering work.
10. Improve the repository as the project matures and translate the evidence into portfolio and interview stories.

The objective is not to fill folders.

The objective is to make engineering work understandable, reviewable, and trustworthy.

---

## Student Doctrine

- Educational work should resemble professional engineering work.
- AI can produce artifacts; engineers create trust.
- The model is not the system.
- The repository is an engineering memory system.
- Engineering work must leave evidence.
- Undisclosed and unverified AI dependency is an engineering risk.
- Requirements, decisions, tests, reviews, releases, and operations should be traceable.
- Engineering work is not complete until it can be defended.
- Tools change; engineering behaviors endure.
- Students should graduate with evidence of engineering ability rather than evidence of course completion.

---

## Bottom Line

ETIS Student Resources help students move from building software to practicing engineering.

The successful ETIS student does not merely produce a working project.

The student produces credible evidence that the work can be trusted.
