# ETIS Student Starter Kit

## Purpose

The **ETIS Student Starter Kit** provides repository-centered engineering environments that students use to initialize projects within ETIS-aligned courses.

A Student Starter Kit is not a folder of sample files.

A Student Starter Kit is an assembled engineering environment designed to help students practice professional software engineering from the beginning of a project.

The goal is to establish professional engineering habits early rather than introducing engineering practices only after implementation has already begun.

Students begin with an engineering operating environment that already incorporates evidence expectations, repository organization, review structures, AI accountability, and operational thinking.

---

## Mission

The mission of the Student Starter Kit is to translate ETIS educational architecture into student engineering practice.

The starter kit helps students experience software engineering as a professional engineering discipline rather than a collection of disconnected assignments.

Each starter kit is intentionally designed to reinforce the core principles of **Engineering Trustworthy Intelligent Systems (ETIS)**.

The objective is not to accelerate coding.

The objective is to establish trustworthy engineering behaviors.

---

## Educational Goals

Student starter kits are designed to help students learn how to:

* Establish professional engineering environments
* Organize repositories intentionally
* Preserve engineering evidence
* Govern AI-assisted work
* Work effectively in teams
* Document important decisions
* Support engineering claims with evidence
* Prepare systems for review
* Think operationally from the beginning
* Defend engineering decisions

Students should learn that repositories are engineering systems rather than code storage locations.

---

## Core Philosophy

A Student Starter Kit is a product.

It is not a document collection.

It is not a code sample.

It is not merely a project template.

It is an intentionally assembled engineering environment.

The starter kit should help students understand that software engineering requires structure, evidence, review, accountability, and operational awareness.

---

## Educational Philosophy

The Student Starter Kit is grounded in several ETIS principles.

> AI proposes; engineers verify.

> Everything important leaves evidence.

> Governance is architecture.

> Context is control.

> The model is not the system.

> A demo is not operational proof.

These principles shape how repositories are organized, how teams collaborate, and how engineering work is documented throughout a project.

---

## Repository-Centered Engineering

The repository serves as the authoritative engineering record.

Students are expected to preserve evidence across the engineering lifecycle rather than accumulating artifacts at the end of a project.

Engineering evidence may include:

* Requirements
* Assumptions
* Risks
* Architecture decisions
* AI-use records
* Reviews
* Pull requests
* Testing evidence
* Release evidence
* Operational assumptions
* Observability notes
* Runbooks
* Postmortems
* Final engineering defenses

The repository should allow a reviewer to understand:

* What was intended
* What was built
* What changed
* What was reviewed
* What was tested
* What remains risky
* Why the team believes the system is defensible

This reflects a core ETIS concept:

> Repositories preserve engineering memory.

---

## Engineering Workflow Philosophy

Engineering work should remain visible throughout the repository lifecycle.

Typical engineering progression includes:

```text
Issue
↓
Branch
↓
Commit
↓
Pull Request
↓
Review
↓
Validation
↓
Merge
↓
Evidence Updated
↓
Release Readiness
↓
Operational Learning
```

Students are taught that engineering artifacts should remain connected throughout the project.

Traceability is not documentation overhead.

Traceability is a mechanism for understanding why work exists, how it evolved, and how engineering decisions can be defended.

---

## Available Starter Kits

Starter kits may vary by course, audience, or educational implementation.

Current implementation:

```text
comp330/
```

Future starter kits may include:

```text
graduate/

capstone/

professional_workshop/
```

The architecture intentionally supports expansion while maintaining consistency across ETIS educational experiences.

New starter kits should be created only when the learning environment requires a materially different structure.

---

## Relationship to the Educational Ecosystem

The Student Starter Kit is one component of the broader ETIS Educational Ecosystem.

```text
ETIS Book
      ↓
Educational Architecture
      ↓
Learning Models
      ↓
Shared Assets
      ↓
Student Starter Kit
      ↓
Student Engineering Practice
      ↓
Professional Engineering Formation
```

Starter kits translate ETIS principles into daily engineering habits.

---

## Relationship to Shared Assets

Student Starter Kits consume shared assets.

They should not permanently duplicate reusable educational intellectual property.

Reusable educational assets belong in:

```text
shared_assets/
```

Examples include:

* Playbooks
* Templates
* Workflows
* AI Engineering guidance
* Assessment assets

Starter kits may include placeholders, student-facing copies, or implementation-specific versions when necessary for usability.

However, the authoritative reusable asset should remain in `shared_assets`.

---

## Relationship to Adoption Examples

Adoption examples explain how a starter kit is used in a specific educational implementation.

The current flagship implementation is:

```text
adoption_examples/
└── loyola_comp330/
```

The starter kit provides the student engineering environment.

The adoption example provides the course implementation context.

The flagship implementation proves the doctrine.

It does not become the doctrine.

The COMP330 starter kit should never become the universal ETIS starter kit.

Future implementations should inherit ETIS principles while adapting to their own educational environments.

Institutions should inherit ETIS doctrine, not ETIS implementations.

In simple terms:

```text
student_starter_kit/comp330/
```

is where students practice engineering.

```text
adoption_examples/loyola_comp330/
```

explains how the course uses that practice environment.

---

## Relationship to Learning Models

Starter kits should support ETIS learning models.

A starter kit should help students progress from:

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

The starter kit should also support movement through engineering maturity levels.

It should help students move from task completion toward evidence-based, reviewable, and accountable engineering practice.

---

## What Belongs Here

The following belong in this directory:

* Student-facing repository starter kits
* Starter kit architecture documentation
* Starter kit design principles
* Starter kit evolution guidance
* Implementation-specific starter kit variants
* Student practice environments

These assets should directly support student engineering practice.

---

## What Does Not Belong Here

The following do not belong in this directory:

* Course syllabi
* Weekly schedules
* Instructor slides
* Instructor-only analysis scripts
* Rubrics
* Course-specific assignment instructions
* Master shared asset sources
* Educational architecture documents
* Learning model documents

Those assets belong elsewhere in the Educational Ecosystem.

---

## Starter Kit Design Responsibilities

A Student Starter Kit should help learners practice the following responsibilities.

### Define intent

Students should have a place to preserve requirements, assumptions, scope, and acceptance criteria.

### Engineer context

Students should have a place to document architecture, decisions, team roles, planning, risks, and system understanding.

### Bound authority

Students should have a place to document permissions, AI usage, security expectations, and role responsibilities.

### Verify behavior

Students should have a place to preserve test plans, test cases, CI evidence, defect logs, and verification notes.

### Operate reality

Students should have a place to preserve runbooks, observability notes, incident response notes, and operational assumptions.

### Explain decisions

Students should have a place to preserve ADRs, review notes, release notes, and engineering presentation evidence.

### Own outcomes

Students should have a place to show release readiness, known limitations, risk disposition, and final engineering reflection.

---

## Evidence-Centered Learning

The starter kit should help students learn that claims require evidence.

Students should not merely claim:

```text
The project works.
```

They should learn to show:

* What was required
* What was built
* What was tested
* What was reviewed
* What risks remain
* What AI assistance was used
* What limitations are known
* What evidence supports release readiness

The starter kit should make this evidence easier to create and review.

---

## AI-Aware Engineering

Modern student engineering work will often involve AI assistance.

The starter kit should support responsible AI use by providing locations for:

* AI policy
* AI-use log
* AI verification notes
* AI-assisted review evidence
* Human accountability documentation

AI should be treated as a bounded engineering collaborator.

Students remain responsible for understanding, verification, integration, and final outcomes.

---

## Guiding Principle

Student repositories should answer a simple question:

> If another engineer inherited this project tomorrow, could they understand it, review it, operate it, improve it, and defend it?

If the answer is no, additional engineering evidence is likely needed.

---

## Governance Rules

The following governance rules apply to Student Starter Kits.

### Starter kits are products.

They should be intentionally designed and maintained.

### Starter kits support practice.

They should help students perform engineering work, not merely read about it.

### Starter kits should preserve structure.

The organization should remain stable enough that instructors and students can rely on it.

### Starter kits should avoid unnecessary complexity.

The structure should teach engineering discipline without overwhelming students.

### Starter kits should consume shared assets.

Reusable educational content should remain in `shared_assets`.

### Starter kits should preserve provenance.

The current flagship starter kit originates from Loyola COMP 330.

### Starter kits should evolve from evidence.

Changes should be based on instructional experience, student difficulty, repository analysis, and instructor review.

---

## Future Evolution

Additional starter kits may be added over time.

Possible future starter kits include:

* Graduate software engineering starter kit
* Capstone starter kit
* AI governance starter kit
* Professional workshop starter kit
* Organizational training starter kit

New starter kits should be created only when the learning environment requires a materially different structure.

Do not create new starter kits merely because a new implementation exists.

Where possible, implementations should reuse or adapt existing starter kits.

---

## Core Thesis

A Student Starter Kit is the bridge between ETIS educational architecture and student engineering practice.

It turns trustworthy engineering principles into a working repository environment.

The goal is not to give students files.

The goal is to give students a structured environment where they can learn to think, work, review, verify, release, and reflect like responsible engineers.
