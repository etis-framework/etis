# ETIS Student Starter Kit Architecture

## Purpose

This document defines the architecture of Student Starter Kits within the ETIS (Engineering Trustworthy Intelligent Systems) Educational Ecosystem.

The purpose of this architecture is to establish how ETIS translates educational theory into student engineering practice.

Student Starter Kits provide the environment where learners repeatedly practice trustworthy engineering behaviors.

They are the operational bridge between educational design and student engineering work.

---

## Core Philosophy

A Student Starter Kit is a product.

It is not a repository template.

It is not a collection of files.

It is not a starter assignment.

It is an intentionally assembled engineering environment.

The objective is to create environments where students naturally practice ETIS principles as part of their daily engineering activities.

The environment itself should teach engineering.

---

## Educational Role

Student Starter Kits occupy a specific position within the ETIS Educational Ecosystem.

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
Professional Transformation
```

Student Starter Kits operationalize ETIS.

The completed Instructor Course Package sits alongside the Student Starter Kit.

The Instructor Course Package designs, operates, and stewards educational systems.

The Student Starter Kit provides the engineering environment where students repeatedly practice those systems.

Their relationship can be summarized as:

```text
Instructor Course Package

↓

Student Starter Kit

↓

Student Engineering Practice

↓

Professional Transformation
```

The two systems are intentionally complementary.

One teaches instructors how to create trustworthy engineers.

The other provides environments where students repeatedly practice becoming trustworthy engineers.

They transform educational concepts into engineering habits.

---

## Core Educational Problem

Traditional software engineering courses often begin with an empty repository.

Students then gradually discover:

* Documentation
* Testing
* Architecture
* Reviews
* Traceability
* Operational thinking

These disciplines often appear late in the project.

ETIS intentionally reverses this pattern.

Students should begin inside an engineered environment that already expects professional engineering behavior.

The starter kit reduces educational randomness.

---

## Architectural Goals

Student Starter Kits exist to achieve several goals.

### Goal 1: Normalize Professional Engineering Structure

Students should encounter professional engineering organization immediately.

### Goal 2: Teach Repository-Centered Engineering

Repositories should function as engineering memory systems.

### Goal 3: Teach Evidence-Centered Engineering

Claims should be supported by evidence.

### Goal 4: Teach Responsible AI Collaboration

AI should be treated as a bounded collaborator.

### Goal 5: Teach Reviewability

Engineering work should be understandable by others.

### Goal 6: Teach Operational Thinking

Students should think beyond implementation.

### Goal 7: Teach Accountability

Students should own outcomes.

---

## Architectural Components

Every Student Starter Kit consists of three layers.

```text
Engineering Workspace
        ↓
Engineering Evidence System
        ↓
Engineering Learning System
```

Each layer serves a different purpose.

---

## Layer 1: Engineering Workspace

This is the visible repository structure students interact with.

Examples may include:

```text
README.md

docs/

src/

tests/

scripts/

data/
```

The workspace organizes engineering activities.

This layer should remain intentionally simple.

---

## Layer 2: Engineering Evidence System

This layer defines what evidence students are expected to preserve.

Examples include:

* Requirements
* Assumptions
* Risks
* Architecture
* Decisions
* AI-use logs
* Test evidence
* Review evidence
* Release evidence
* Operational assumptions

Students should learn that evidence accumulates continuously.

Evidence should not be generated at the end of the semester.

---

## Layer 3: Engineering Learning System

This layer connects repository activities to educational outcomes.

Repository activities should reinforce:

* Professional transformation
* Engineering maturity
* Review skills
* AI accountability
* Operational awareness
* Stewardship

The environment itself should help learners mature.

---

## The Seven Engineering Responsibilities

Every Student Starter Kit should reinforce seven ETIS responsibilities.

```text
Define Intent

Engineer Context

Bound Authority

Verify Behavior

Operate Reality

Explain Decisions

Own Outcomes
```

These responsibilities should be visible throughout the engineering environment.

---

## Design Philosophy

Student Starter Kits should embody several design characteristics.

### Visible

Students should be able to easily understand where work belongs.

### Understandable

The environment should not overwhelm beginners.

### Reviewable

Engineering evidence should be easy to inspect.

### Sustainable

The structure should remain useful throughout the entire project lifecycle.

### AI-Aware

Responsible AI practices should be integrated naturally.

### Operationally Conscious

Students should think beyond implementation.

### Evolvable

The environment should support future growth without structural instability.

---

## Repository-Centered Engineering

Student Starter Kits reinforce one of the foundational ETIS concepts:

> Repositories preserve engineering memory.

Repositories should contain more than code.

They should preserve:

* Intent
* Decisions
* Evidence
* Reviews
* Risks
* Tests
* Operational assumptions
* Reflection

Students should gradually understand that engineering memory is one of their primary responsibilities.

---

## Evidence-Centered Engineering

Student Starter Kits should teach students that evidence is continuous.

Evidence may include:

```text
Requirements
↓
Architecture
↓
Implementation
↓
Tests
↓
Reviews
↓
Release Evidence
↓
Operational Learning
```

Every phase should leave evidence behind.

---

## AI-Aware Engineering

Student Starter Kits should support responsible AI usage.

Students should have clear places to preserve:

* AI policies
* AI-use logs
* Verification notes
* Human review evidence

The starter kit should reinforce:

> AI proposes; engineers verify.

AI should not become an invisible participant.

---

## Relationship to Learning Models

Student Starter Kits consume learning models.

Learning models explain how students develop.

Starter kits provide environments where that development occurs.

Examples include:

* Professional Transformation Model
* Engineering Maturity Model
* Software Engineering Learning Progression
* Two-Cycle Engineering Model

The starter kit operationalizes those models.

---

## Relationship to Shared Assets

Student Starter Kits consume shared assets.

Shared assets remain authoritative.

Examples include:

```text
shared_assets/

playbooks/

templates/

workflows/

ai_engineering/

assessment/
```

Student Starter Kits may surface these assets in student-friendly ways.

They should not permanently duplicate them.

---

## Relationship to Adoption Examples

Adoption examples explain how starter kits are used.

The current flagship implementation is:

```text
adoption_examples/
└── loyola_comp330/
```

The adoption example explains instructional use.

The starter kit provides the student environment.

The relationship is complementary.

The flagship implementation proves the doctrine.

It does not become the doctrine.

The COMP330 starter kit should never become the universal ETIS starter kit.

Future educational implementations should inherit ETIS principles while adapting to their own environments.

Institutions should inherit ETIS doctrine, not ETIS implementations.

---

## Architectural Boundaries

Student Starter Kits do not own:

* Course schedules
* Syllabi
* Rubrics
* Instructor slides
* Instructor analysis tools
* Educational architecture
* Learning models
* Shared asset sources

Student Starter Kits own the student engineering environment.

---

## Growth Model

New starter kits should only be created when educational environments materially differ.

Examples may include:

* Undergraduate software engineering
* Graduate software engineering
* Capstone programs
* Professional workshops
* AI governance programs

Different semesters alone should not create new starter kits.

---

## Governance Rules

The following rules should remain stable.

### Starter kits are products.

### Starter kits teach through structure.

### Starter kits should consume shared assets.

### Starter kits should preserve provenance.

### Starter kits should avoid unnecessary complexity.

### Starter kits should evolve from educational evidence.

### Starter kits should support long-term maintainability.

These rules help preserve architectural consistency.

---

## Layer Separation Rules

The Student Starter Kit intentionally separates engineering activities into distinct layers.

```text
docs/     → Think

src/      → Build

tests/    → Verify

data/     → Support

scripts/  → Automate
```

These responsibilities should remain distinct.

Do not duplicate engineering evidence across layers.

Do not move educational artifacts into implementation layers.

Do not allow tooling implementations to become educational doctrine.

This separation helps preserve long-term maintainability.

---

## Future Evolution

Future enhancements may include:

* Multiple starter kit variants
* Discipline-specific starter kits
* Professional training starter kits
* AI governance starter kits

Growth should occur intentionally.

The architecture should remain simple.

---

## Core Thesis

Student Starter Kits are where ETIS becomes practice.

They provide environments where students repeatedly exercise the habits of trustworthy engineering.

The goal is not to provide files.

The goal is to create engineering environments that help learners define intent, engineer context, bound authority, verify behavior, operate reality, explain decisions, and own outcomes.

That repeated practice is what ultimately produces trustworthy engineers.
