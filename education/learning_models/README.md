# Learning Models

## Purpose

The `learning_models` directory contains the progression models that explain how learners develop within the ETIS (Engineering Trustworthy Intelligent Systems) Educational Ecosystem.

These models describe the movement from student participation toward professional engineering responsibility.

The purpose of this directory is to make learner development explicit, intentional, and reusable across educational implementations.

Learning models help instructors, students, adopters, and reviewers understand not only what learners are doing, but how they are expected to mature over time.

---

## Mission

The mission of `learning_models` is to define how ETIS education develops trustworthy engineers.

ETIS education is not only about content coverage.

It is about professional transformation.

Learners should progressively develop the ability to:

* Define intent
* Engineer context
* Bound authority
* Verify behavior
* Operate reality
* Explain decisions
* Own outcomes

The learning models in this directory provide the structure for that transformation.

---

## Directory Role

This directory owns learner development architecture.

It does not own course materials, shared educational assets, rubrics, starter kits, or implementation-specific schedules.

Those belong elsewhere.

The role of this directory is to define durable models of learner progression that can inform:

* Course design
* Assignment sequencing
* Project checkpoints
* Assessment design
* Classroom exercises
* Instructor feedback
* Student reflection
* Professional development pathways

---

## Current Directory Contents

```text
learning_models/

├── README.md

├── ETIS_Learning_Models.md

├── professional_transformation_model.md

├── engineering_maturity_model.md

├── software_engineering_learning_progression.md

└── two-cycle_engineering_model/
```

Each file has a distinct responsibility.

---

## File Responsibilities

### README.md

This file is the entry point for the `learning_models` directory.

It explains the purpose, structure, ownership boundaries, and educational role of the learning model subsystem.

---

### ETIS_Learning_Models.md

This is the master learning models document.

It explains how the individual learning models relate to one another and how they support the broader ETIS Educational Ecosystem.

It should define the overall learner development architecture.

---

### professional_transformation_model.md

This file defines the central professional transformation pathway.

The current transformation model is:

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

This model explains the professional identity shift ETIS is designed to produce.

---

### engineering_maturity_model.md

This file defines observable stages of engineering maturity.

It should help instructors and learners understand how engineering behavior improves over time.

This model may include maturity across areas such as:

* Intent definition
* Context quality
* Repository discipline
* Evidence creation
* Review participation
* AI responsibility
* Release readiness
* Operational thinking
* Accountability

---

### software_engineering_learning_progression.md

This file defines how students progress through software engineering capability development.

It should connect learning activities, engineering artifacts, reviews, assignments, and project milestones to growth in engineering responsibility.

This model should help answer:

How does a learner move from knowing concepts to practicing trustworthy engineering?

---

### two-cycle_engineering_model/

This directory contains the Two-Cycle Engineering Model.

The model distinguishes between two major learning phases:

```text
Cycle 1: Can it work?

Cycle 2: Can it survive?
```

Cycle 1 focuses on feasibility, basic implementation, team coordination, and initial engineering discipline.

Cycle 2 focuses on evidence, quality, reviewability, operational readiness, risk, release defense, and sustainability.

This model is foundational to the Loyola COMP330 implementation and may be reused by future implementations.

---

## Relationship to Educational Architecture

The `educational_architecture` directory defines how ETIS is taught at the system level.

The `learning_models` directory defines how learners mature within that system.

Relationship model:

```text
Educational Architecture
        ↓
Learning Models
        ↓
Educational Design
        ↓
Assignments, Reviews, Assets, and Starter Kits
        ↓
Learner Transformation
```

Educational architecture defines the system.

Learning models define the developmental arc.

---

## Relationship to Shared Assets

Shared assets teach specific behaviors, artifacts, workflows, AI practices, and assessment mechanisms.

Learning models explain why those assets matter developmentally.

For example:

* Playbooks support professional behavior development.
* Templates support evidence maturity.
* Workflows support process discipline.
* AI Engineering assets support responsible human-AI collaboration.
* Assessment assets evaluate maturity and responsibility.

Learning models help connect these assets to learner growth.

---

## Relationship to Student Starter Kits

Student Starter Kits provide structured environments where learners practice ETIS behaviors.

Learning models explain the intended growth that should occur as students use those environments.

The starter kit is where learners practice.

The learning models explain what maturity that practice should develop.

---

## Relationship to Adoption Examples

Educational implementations consume learning models.

The current flagship implementation is:

```text
adoption_examples/
└── loyola_comp330/
```

COMP330 uses learning models to support:

* Team project sequencing
* Assignment design
* Cycle 1 and Cycle 2 expectations
* Repository-centered engineering
* Release readiness
* Engineering reflection
* Professional growth

Future implementations may adapt learning models while preserving the underlying professional transformation goal.

---

## Learning Model Philosophy

ETIS learning models are developmental, not merely descriptive.

They are intended to guide transformation.

A learner should not only know more at the end of an ETIS experience.

A learner should practice differently.

A learner should review differently.

A learner should communicate differently.

A learner should use AI differently.

A learner should defend decisions differently.

A learner should understand engineering responsibility differently.

The models in this directory make that progression visible.

---

## What Belongs Here

The following belong in this directory:

* Learner progression models
* Professional transformation models
* Engineering maturity models
* Developmental frameworks
* Cycle-based learning models
* Cross-course learning progression models

These assets should be durable and reusable across implementations.

---

## What Does Not Belong Here

The following do not belong in this directory:

* Course schedules
* Assignment instructions
* Rubrics
* Templates
* Repository setup guides
* Student project files
* Instructor analysis scripts
* Implementation-specific reports

Those assets belong in `adoption_examples`, `shared_assets`, `student_starter_kit`, or future instructor tooling locations.

---

## Governance Rules

The following governance rules apply to this directory.

### Learning models should describe progression.

They should explain how learners mature over time.

### Learning models should remain reusable.

They should not be overly tied to one course unless explicitly identified as implementation-specific.

### Learning models should support assessment.

They should help instructors evaluate growth in engineering responsibility.

### Learning models should support reflection.

They should help students understand their own development.

### Learning models should preserve ETIS principles.

They should remain aligned with evidence, governance, context, review, operations, stewardship, and accountability.

### Learning models should avoid unnecessary complexity.

Models should clarify learning, not overwhelm readers.

---

## Future Evolution

This directory may evolve as the Educational Ecosystem expands.

Possible future additions include:

* Instructor development model
* Reviewer maturity model
* AI engineering maturity model
* Release defense maturity model
* Engineering portfolio maturity model
* Organizational learning model
* Capstone maturity pathway

Future additions should be made only when they clarify learner development in a way not already covered by existing models.

---

## Core Thesis

ETIS education is professional transformation.

The `learning_models` directory exists to make that transformation visible, intentional, assessable, and repeatable.

A student should not simply finish an ETIS learning experience with more information.

A student should finish with a stronger engineering identity.
