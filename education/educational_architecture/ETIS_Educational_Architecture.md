# ETIS Educational Architecture

## Purpose

This document defines the educational architecture for the ETIS (Engineering Trustworthy Intelligent Systems) Educational Ecosystem.

The purpose of this architecture is to transform ETIS from a completed book into a teachable, reusable, governable, and sustainable educational system.

The ETIS book remains the authoritative knowledge source. The Educational Ecosystem defines how that knowledge is taught, sequenced, practiced, assessed, adapted, and preserved across educational implementations.

This document is the master educational architecture reference for Phase II.

---

## How to Use This Document

This document should be read as the architectural guide for ETIS education.

It is intended for instructors, curriculum designers, educational adopters, and project stewards who need to understand how the ETIS book becomes an educational system.

This document does not replace detailed learning maps, audience pathways, shared asset documentation, course materials, or student starter kit guidance. Instead, it explains how those pieces relate to one another.

Readers should use this document to understand:

* The purpose of the ETIS Educational Ecosystem
* The relationship between the ETIS book and educational implementations
* The major educational architecture components
* The role of shared assets and starter kits
* The professional transformation model
* The ownership boundaries that prevent duplication and drift

---

## Mission

The mission of the ETIS Educational Ecosystem is to prepare future engineers to build, govern, operate, review, and steward trustworthy intelligent systems.

Software engineering education must now extend beyond teaching students how to build working software.

Future engineers must learn to create systems that can be:

* Understood
* Reviewed
* Governed
* Operated
* Improved
* Defended
* Trusted over time

The Educational Ecosystem exists to teach those capabilities intentionally.

---

## Core Educational Thesis

AI capability increases engineering responsibility.

As AI systems become more capable, engineers do not become less responsible.

They become more responsible for defining intent, engineering context, bounding authority, verifying behavior, preserving evidence, explaining decisions, and owning outcomes.

The ETIS Educational Ecosystem exists to teach that responsibility.

---

## Relationship to the ETIS Book

The ETIS book is complete, frozen, and authoritative.

The Educational Ecosystem does not rewrite the book.

The Educational Ecosystem translates the book into educational structures.

Relationship model:

```text
ETIS Book
    ↓
Educational Architecture
    ↓
Learning Models
    ↓
Shared Assets
    ↓
Educational Implementations
    ↓
Student Starter Kits
    ↓
Student Engineering Practice
```

The book defines the framework.

Educational architecture defines how the framework is taught.

Shared assets provide reusable educational building blocks.

Adoption examples demonstrate concrete implementation.

Student Starter Kits provide assembled engineering environments for learners.

---

## Educational System Architecture

The ETIS Educational Ecosystem is organized around the following structure:

```text
education/

├── README.md

├── educational_architecture/

├── learning_models/

├── shared_assets/

├── student_starter_kit/

└── adoption_examples/
```

Each directory represents a distinct architectural responsibility.

---

## Directory Responsibilities

### educational_architecture/

Defines how ETIS is taught.

Owns:

* Educational architecture
* Educational design principles
* Audience learning paths
* Chapter learning maps
* Educational ownership boundaries

This directory governs the educational system itself.

---

### learning_models/

Defines models of learner development and professional progression.

Owns:

* Professional Transformation Model
* Engineering Maturity Model
* Two-Cycle Engineering Model
* Software Engineering Learning Progression

This directory explains how learners mature over time.

---

### shared_assets/

Contains reusable educational assets.

Owns:

* Playbooks
* Templates
* Workflows
* AI Engineering assets
* Assessment assets

This directory provides reusable educational building blocks.

---

### student_starter_kit/

Contains assembled student engineering environments.

Owns:

* Starter kit structure
* Student-facing repository environments
* Practice scaffolding
* Engineering workspace organization

Student Starter Kits are products, not document collections.

---

### adoption_examples/

Contains implementation-specific educational examples.

Owns:

* Course-specific materials
* Institution-specific implementations
* Syllabi
* Weekly schedules
* Assignments
* Rubrics
* Slides
* Implementation notes

The current flagship implementation is Loyola COMP330.

---

## Flagship Implementation

Loyola University Chicago COMP 330 — Software Engineering is the flagship ETIS educational implementation.

COMP330 is important because it serves as the initial real-world educational implementation of ETIS Phase II.

However, COMP330 is not the Educational Ecosystem itself.

COMP330:

* Consumes educational architecture
* Consumes shared assets
* Uses learning models
* Uses the Student Starter Kit
* Contributes new educational assets
* Preserves Loyola provenance

Course-specific materials belong in:

```text
adoption_examples/loyola_comp330/
```

Reusable assets belong outside COMP330, usually in:

```text
shared_assets/
```

This boundary prevents reusable educational intellectual property from becoming trapped inside one course implementation.

---

## Professional Transformation Architecture

The ETIS Educational Ecosystem is organized around professional transformation.

The target progression is:

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

This progression is not merely aspirational.

It should influence:

* Course design
* Assignment sequencing
* Starter kit structure
* Assessment rubrics
* Classroom exercises
* Review practices
* Student reflection
* Instructor feedback

The educational goal is not only for students to complete software projects.

The educational goal is for students to mature into engineers capable of taking responsibility for trustworthy systems.

---

## Educational Responsibility Model

ETIS education should teach learners to:

### Define intent

Students must learn to clarify what a system is supposed to accomplish and why it matters.

### Engineer context

Students must learn that context shapes system behavior, AI behavior, review quality, operational readiness, and governance.

### Bound authority

Students must learn to define what people, systems, tools, and AI agents are allowed to do.

### Verify behavior

Students must learn that claims require evidence.

### Operate reality

Students must learn that systems must survive use, failure, change, and operational constraints.

### Explain decisions

Students must learn to make decisions understandable to others.

### Own outcomes

Students must learn that engineering responsibility cannot be delegated away.

---

## Educational Design Philosophy

ETIS education should teach systems rather than isolated tasks.

Traditional software engineering education often emphasizes deliverables.

ETIS emphasizes the relationships among deliverables, decisions, evidence, review, governance, operations, and accountability.

Students should understand not only what artifact they are creating, but why that artifact matters within the engineering system.

A requirements document is not paperwork.

It is intent preservation.

An architecture document is not a diagram.

It is decision structure.

A test plan is not a checklist.

It is evidence design.

A release readiness review is not a presentation.

It is an engineering defense.

A postmortem is not a blame document.

It is organizational learning.

---

## Educational Asset Architecture

Educational assets are first-class ETIS artifacts.

They should be intentionally created, named, governed, normalized, versioned, and preserved.

Authoritative format:

```text
Markdown (.md)
```

Distribution format:

```text
PDF (.pdf)
```

Optional editable format:

```text
Word (.docx)
```

Markdown is the source of truth.

Word and PDF files may exist during transition, distribution, or archival use, but they are not authoritative.

---

## Shared Asset Architecture

Shared assets are reusable educational intellectual property.

They are organized into five categories:

```text
shared_assets/

├── playbooks/

├── templates/

├── workflows/

├── ai_engineering/

└── assessment/
```

Each category has a distinct educational purpose.

### Playbooks

Teach professional engineering behaviors.

Core question:

How should engineers behave?

### Templates

Teach engineering evidence creation.

Core question:

What evidence should engineers create?

### Workflows

Teach engineering flow and process.

Core question:

How does engineering work move through a system?

### AI Engineering

Teach responsible human-AI collaboration.

Core question:

How should engineers responsibly collaborate with AI?

### Assessment

Teach evaluation of engineering maturity.

Core question:

How do we evaluate engineering responsibility?

---

## Student Starter Kit Architecture

Student Starter Kits are assembled engineering environments.

They are products.

They are not document folders.

A Student Starter Kit should provide learners with a structured environment for practicing repository-centered engineering.

The current flagship starter kit is:

```text
student_starter_kit/comp330/
```

Starter Kits may contain:

* Repository structure
* Documentation folders
* Source folders
* Test folders
* Script folders
* Data folders
* Evidence folders
* README guidance
* Starter policies
* Engineering scaffolding

Student Starter Kits consume shared assets but should not permanently duplicate them.

The starter kit is where students practice.

Shared assets are where reusable educational intellectual property lives.

---

## Repository-Centered Engineering

Repository-centered engineering is central to ETIS education.

The repository is not merely where code is stored.

The repository is where engineering evidence accumulates.

Students should learn to use repositories to:

* Define intent
* Preserve requirements
* Document architecture
* Record decisions
* Track risks
* Show testing evidence
* Capture AI usage
* Conduct reviews
* Prepare releases
* Preserve operational knowledge

The repository becomes the student’s engineering memory system.

This is one of the most important educational shifts in ETIS.

---

## Evidence-Centered Education

ETIS education should teach students that important engineering claims require evidence.

Students should not merely say:

“The system works.”

They should be able to show:

* Requirements evidence
* Design evidence
* Test evidence
* Review evidence
* Traceability evidence
* AI verification evidence
* Release readiness evidence
* Operational readiness evidence

Evidence-centered education prepares students for professional engineering environments where decisions must be reviewed, defended, audited, and improved.

---

## AI-Assisted Engineering Education

AI is a major educational concern within ETIS.

Students should learn to use AI responsibly, but they should not learn to outsource engineering responsibility.

AI may assist with:

* Brainstorming
* Drafting
* Code explanation
* Test generation
* Review preparation
* Documentation improvement
* Risk identification
* Alternative analysis

However, students remain responsible for:

* Understanding
* Verification
* Accuracy
* Decisions
* Integration
* Evidence
* Final outcomes

The governing principle is:

```text
AI proposes; engineers verify.
```

AI should be taught as a bounded engineering collaborator, not an authority.

---

## Two-Cycle Engineering Model

The Two-Cycle Engineering Model is foundational to the COMP330 implementation and may be reused in future implementations.

The model distinguishes between two major project learning phases.

### Cycle 1

Cycle 1 asks:

```text
Can it work?
```

Students focus on establishing core feasibility, basic functionality, team coordination, and initial engineering structure.

### Cycle 2

Cycle 2 asks:

```text
Can it survive?
```

Students focus on quality, reviewability, operational readiness, traceability, release readiness, risk, and sustainability.

This model teaches students that working software is not the finish line.

A system must also be maintainable, reviewable, governable, and operationally credible.

---

## 39-Chapter Consumption Architecture

The ETIS book contains 39 chapters.

Not every educational implementation should consume all 39 chapters equally.

Different audiences require different pathways.

For example, COMP330 primarily emphasizes Parts I and II while selectively introducing Parts III and IV.

Other implementations may emphasize:

* AI governance
* Operational readiness
* Architecture review
* Release governance
* Incident response
* Human oversight
* Stewardship

The purpose of educational architecture is to preserve the authority of the complete ETIS book while allowing responsible educational adaptation.

---

## Audience Architecture

ETIS may serve multiple audiences over time.

Potential audiences include:

* Undergraduate software engineering students
* Graduate software engineering students
* Capstone teams
* Early-career software engineers
* Professional engineers
* Software architects
* Technical leads
* Engineering managers
* AI governance teams
* Review boards
* Organizational training programs

These audiences should not all receive identical learning paths.

Audience learning paths should be designed intentionally.

---

## Assessment Architecture

Assessment in ETIS should evaluate engineering maturity, not merely task completion.

Students should be assessed on their ability to:

* Define intent
* Create evidence
* Explain decisions
* Work professionally
* Manage risk
* Use AI responsibly
* Review engineering work
* Demonstrate release readiness
* Think operationally
* Own outcomes

Assessment should mirror professional engineering evaluation.

The central question should not be only:

```text
Did the software work?
```

The better question is:

```text
Is the engineering work understandable, reviewable, governable, sustainable, and trustworthy?
```

---

## Instructor Architecture

The ETIS Educational Ecosystem should eventually support instructors beyond the original COMP330 implementation.

Instructor-facing materials may include:

* Course setup guidance
* Weekly sequencing guidance
* Assignment guidance
* Rubric guidance
* Classroom exercises
* Starter kit usage guidance
* Assessment guidance
* Adoption notes
* Implementation patterns

Instructor materials should help adopters teach ETIS without requiring them to reconstruct the educational architecture from scratch.

---

## Classroom Exercise Architecture

Classroom exercises should reinforce ETIS behaviors through practice.

Potential exercise areas include:

* Requirements review
* Architecture review
* AI usage review
* Pull request review
* Release readiness defense
* Risk review
* Incident response
* Postmortem analysis
* Operational readiness review

Exercises should help students practice engineering judgment, not merely recall concepts.

---

## Ownership Boundaries

Clear ownership boundaries prevent educational drift.

### Educational architecture owns system design.

It defines how ETIS is taught.

### Learning models own progression models.

They explain how learners mature.

### Shared assets own reusable artifacts.

They contain reusable teaching assets.

### Student Starter Kits own assembled practice environments.

They give students structured engineering spaces.

### Adoption examples own implementation-specific materials.

They preserve course-specific and institution-specific context.

These boundaries should be preserved unless a significant architectural event justifies change.

---

## Provenance

The current educational assets originate primarily from Loyola University Chicago COMP330.

This provenance should be preserved.

Loyola provenance matters because it records the implementation history of the Educational Ecosystem.

Educational assets should not be prematurely generalized.

Reusable assets may become more implementation-neutral over time, but their origin should remain traceable.

---

## Related Documents

This document is part of the `educational_architecture` directory.

Related documents include:

* `educational_design_principles.md`
* `audience_learning_paths.md`
* `39_chapter_learning_map.md`

Those documents provide more detailed guidance on educational design rules, audience-specific pathways, and chapter-level learning use.

---

## Core Thesis

The ETIS Educational Ecosystem exists because trustworthy engineering must be taught intentionally.

Future engineers will not be judged solely by whether they can produce software.

They will be judged by whether they can define intent, engineer context, bound authority, verify behavior, operate reality, explain decisions, and own outcomes.

This architecture exists to make that education possible, repeatable, governable, and sustainable.

