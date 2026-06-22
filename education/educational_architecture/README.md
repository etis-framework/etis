# Educational Architecture

## Purpose

The `educational_architecture` directory defines how the ETIS (Engineering Trustworthy Intelligent Systems) framework is taught, adapted, sequenced, and consumed within educational settings.

This directory is the architectural center of the ETIS Educational Ecosystem.

Its purpose is to prevent ETIS education from becoming a loose collection of course materials, assignments, slides, rubrics, and templates. Instead, this directory defines the educational system that governs how ETIS concepts are transformed into teachable, assessable, reusable, and sustainable learning experiences.

Educational architecture is treated as a first-class ETIS artifact.

It is not administrative support material.

It is the design system for teaching trustworthy engineering.

---

## Mission

The mission of `educational_architecture` is to preserve the educational structure, rationale, learning pathways, design principles, and implementation boundaries required to teach ETIS responsibly over time.

This directory explains how the ETIS book, shared educational assets, learning models, student starter kits, and course implementations relate to one another.

The goal is to ensure that future educational work remains coherent, maintainable, and aligned with the core ETIS thesis:

Future engineers must learn to define intent, engineer context, bound authority, verify behavior, operate reality, explain decisions, and own outcomes.

---

## Educational Architecture Philosophy

Software engineering education is no longer limited to teaching students how to build working software.

Modern engineering education must teach students how to create systems that can be understood, reviewed, governed, operated, improved, and trusted over time.

That requires intentional educational architecture.

Without educational architecture, courses tend to become collections of lectures, assignments, examples, and grading instruments. Over time, those materials drift. Terminology becomes inconsistent. Assignments lose their relationship to learning outcomes. Reusable assets become trapped inside course-specific implementations. Students complete tasks without understanding the engineering system those tasks belong to.

The ETIS Educational Ecosystem avoids that failure mode by explicitly designing the educational system.

---

## Directory Role

This directory defines the educational brain of Phase II.

It answers questions such as:

* How should ETIS be taught?
* How do different audiences consume the 39-chapter ETIS book?
* What educational principles govern asset creation?
* How do learning models support professional transformation?
* How do course implementations consume shared assets?
* Where do ownership boundaries exist?
* What should remain stable as the ecosystem grows?

This directory should be consulted before creating new educational assets, new course implementations, new starter kits, or new learning pathways.

---

## Current Directory Contents

```text
educational_architecture/

├── README.md

├── ETIS_Educational_Architecture.md

├── educational_design_principles.md

├── audience_learning_paths.md

└── 39_chapter_learning_map.md
```

Each file has a distinct responsibility.

---

## File Responsibilities

### README.md

This file is the entry point for the `educational_architecture` directory.

It explains the purpose, structure, ownership boundaries, and governance role of the directory.

This file should remain stable and should not become a dumping ground for detailed learning maps, course schedules, or implementation-specific guidance.

---

### ETIS_Educational_Architecture.md

This is the master educational architecture document.

It defines the overall educational system for ETIS Phase II.

It should explain:

* The educational mission of ETIS
* The relationship between the ETIS book and the Educational Ecosystem
* The professional transformation model
* The role of shared assets
* The role of learning models
* The role of student starter kits
* The role of adoption examples
* Educational ownership boundaries
* Governance principles
* Long-term evolution strategy

This document should be treated as the primary architecture specification for ETIS education.

---

### educational_design_principles.md

This file defines the design principles that govern ETIS educational assets and implementations.

It should answer:

What rules should guide the creation of ETIS educational content?

Examples of design principles include:

* Teach systems, not isolated tasks
* Teach evidence, not paperwork
* Teach engineering judgment, not procedural compliance
* Teach responsible AI collaboration, not AI dependency
* Preserve engineering memory
* Prefer reusable assets over duplicated materials
* Maintain Loyola provenance until multiple implementations exist

This file should guide asset creation, course design, and future expansion.

---

### audience_learning_paths.md

This file defines how different audiences consume ETIS.

Not every audience should consume all 39 chapters in the same way.

Different audiences have different needs, levels of maturity, time constraints, and professional responsibilities.

Potential audiences include:

* Undergraduate software engineering students
* Graduate students
* Capstone teams
* Professional engineers
* Software architects
* Engineering leaders
* Governance and review boards
* Organizational training programs

This file should define appropriate learning paths without weakening the authority of the full ETIS book.

---

### 39_chapter_learning_map.md

This file maps the 39-chapter ETIS book into educational use.

It is not merely a table of contents.

It explains how the chapters support different educational pathways, implementations, and maturity levels.

For example, Loyola COMP330 may emphasize Parts I and II while selectively introducing Parts III and IV.

Other implementations may emphasize governance, operations, architecture, AI oversight, or organizational stewardship.

This file helps instructors and adopters understand how to teach from the book without assuming that every course must cover every chapter equally.

---

## Relationship to the ETIS Book

The ETIS book remains complete, frozen, and authoritative.

The Educational Ecosystem does not replace the book.

It translates the book into educational architecture, learning paths, reusable assets, implementation models, and student engineering environments.

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

---

## Relationship to Learning Models

The `learning_models` directory contains specific models of professional development and engineering maturity.

The `educational_architecture` directory governs how those models fit into the broader educational system.

Learning models may include:

* Professional Transformation Model
* Engineering Maturity Model
* Two-Cycle Engineering Model
* Software Engineering Learning Progression

Educational architecture explains how these models relate to course design, asset design, assessment, and student development.

---

## Relationship to Shared Assets

The `shared_assets` directory contains reusable educational assets.

The `educational_architecture` directory explains why those assets exist and how they should be governed.

Shared assets include:

* Playbooks
* Templates
* Workflows
* AI Engineering assets
* Assessment assets

Educational architecture defines the learning purpose and ownership model behind those assets.

Shared assets provide the reusable educational building blocks.

---

## Relationship to Student Starter Kits

The `student_starter_kit` directory contains assembled engineering environments for learners.

Student Starter Kits are products.

They are not collections of unrelated documents.

Educational architecture governs what starter kits are supposed to accomplish, how they relate to shared assets, and how they support student transformation.

Starter kits should help students practice repository-centered engineering in a realistic, structured, and reviewable environment.

---

## Relationship to Adoption Examples

The `adoption_examples` directory contains concrete implementations of the ETIS Educational Ecosystem.

The current flagship implementation is:

```text
adoption_examples/
└── loyola_comp330/
```

Loyola COMP330 is the flagship implementation, but it is not the Educational Ecosystem itself.

COMP330 consumes educational architecture.

COMP330 consumes shared assets.

COMP330 contributes educational assets.

COMP330 preserves implementation provenance.

Course-specific material belongs inside the adoption example. Reusable assets belong outside the adoption example.

---

## Ownership Boundaries

This directory owns educational architecture.

It does not own every educational asset.

The ownership boundaries are:

```text
educational_architecture/
```

Owns educational system design, learning pathways, design principles, and chapter consumption architecture.

```text
learning_models/
```

Owns specific learning progression and maturity models.

```text
shared_assets/
```

Owns reusable educational assets.

```text
student_starter_kit/
```

Owns assembled student engineering environments.

```text
adoption_examples/
```

Owns implementation-specific course materials.

These boundaries should be preserved to prevent duplication and drift.

---

## Governance Rules

The following governance rules apply to this directory.

### Educational architecture is intentional.

Educational structure should be designed, not allowed to emerge accidentally.

### The ETIS book remains authoritative.

Educational architecture adapts the book for teaching but does not override it.

### Markdown is authoritative.

Markdown files are the source of truth for educational architecture.

### Do not duplicate shared assets.

This directory may describe shared assets but should not contain the assets themselves.

### Do not bury implementation-specific material here.

Course-specific details belong in `adoption_examples`.

### Preserve learning relationships.

Educational documents should explain how ideas, assets, audiences, and implementations relate to one another.

### Avoid premature generalization.

Loyola COMP330 provenance should remain visible until multiple implementations exist.

### Optimize for long-term stewardship.

Architecture should support future growth without requiring frequent restructuring.

---

## Directory Status

The `educational_architecture` directory contains the core documents needed to govern ETIS education.

These files establish:

* The master educational architecture
* The educational design principles
* Audience learning paths
* The 39-chapter learning map
* Ownership boundaries for educational architecture

This directory should now be treated as architecturally stable.

Future changes should clarify the educational architecture rather than duplicate material owned by `learning_models`, `shared_assets`, `student_starter_kit`, or `adoption_examples`.

---

## Future Evolution

This directory may evolve as the ETIS Educational Ecosystem expands.

Possible future additions include:

* Instructor adoption guide
* Educational implementation model
* Course design reference architecture
* Assessment architecture
* Portfolio architecture
* Capstone adoption pathway
* Professional workshop pathway

Future additions should be made only when they clarify educational architecture rather than duplicate material owned elsewhere.

---

## Core Thesis

Educational architecture is as important as educational content.

Without architecture, educational ecosystems become collections of disconnected materials.

With architecture, educational assets become a governed system for developing future trustworthy engineers.

The `educational_architecture` directory exists to preserve that system.
