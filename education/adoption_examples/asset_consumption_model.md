# Asset Consumption Model

## Purpose

This document defines how educational implementations consume assets within the ETIS (Engineering Trustworthy Intelligent Systems) Educational Ecosystem.

The purpose of this model is to establish clear relationships between ETIS educational components while preventing duplication, fragmentation, and architectural drift.

Educational implementations should consume ETIS assets rather than recreate them.

This document explains how that consumption occurs.

---

## Core Philosophy

ETIS is an ecosystem.

Educational ecosystems are assembled from interconnected assets.

Not every implementation should create its own materials from scratch.

Instead, implementations should intentionally consume, adapt, and contribute educational assets while preserving ownership boundaries.

The objective is sustainable educational reuse.

---

## Core Principle

Educational implementations should consume ETIS assets rather than own them.

The implementation assembles a learning experience.

The ecosystem supplies the building blocks.

This distinction is critical.

---

## Asset Consumption Architecture

All ETIS implementations should follow the same high-level consumption model.

```text
ETIS Book
        ↓
Educational Architecture
        ↓
Learning Models
        ↓
Shared Assets
        ↓
Student Starter Kits
        ↓
Educational Implementations
        ↓
Learner Experience
```

Each layer consumes the layers above it.

The relationship is intentionally directional.

---

## Educational Layers

The ETIS Educational Ecosystem contains six layers.

### Layer 1: ETIS Book

The ETIS book is the authoritative engineering framework.

The book defines:

* Principles
* Engineering philosophy
* Engineering methods
* Governance concepts
* Operational thinking
* Stewardship concepts

The book is authoritative.

Educational assets adapt the book.

Educational assets do not replace the book.

---

### Layer 2: Educational Architecture

Educational architecture defines how ETIS is taught.

Examples include:

```text
educational_architecture/

README.md

ETIS_Educational_Architecture.md

educational_design_principles.md

audience_learning_paths.md

39_chapter_learning_map.md
```

Educational architecture provides teaching structure.

Educational implementations consume this architecture.

---

### Layer 3: Learning Models

Learning models define learner development.

Examples include:

```text
learning_models/

ETIS_Learning_Models.md

professional_transformation_model.md

engineering_maturity_model.md

software_engineering_learning_progression.md

two-cycle_engineering_model/
```

Learning models explain how learners mature.

Implementations consume these models.

---

### Layer 4: Shared Assets

Shared assets provide reusable educational intellectual property.

Examples include:

```text
shared_assets/

playbooks/

templates/

workflows/

ai_engineering/

assessment/
```

Shared assets are intentionally reusable.

They are consumed by implementations.

---

### Layer 5: Student Starter Kits

Student Starter Kits provide assembled engineering environments.

Examples include:

```text
student_starter_kit/

comp330/
```

Starter kits are educational products.

They are consumed by implementations.

---

### Layer 6: Educational Implementations

Educational implementations assemble the learner experience.

Examples include:

```text
adoption_examples/

loyola_comp330/
```

Implementations orchestrate educational assets.

They do not redefine them.

---

## Asset Ownership Model

Each educational component has ownership responsibilities.

| Component                | Owns                                       |
| ------------------------ | ------------------------------------------ |
| ETIS Book                | Engineering framework                      |
| Educational Architecture | Teaching architecture                      |
| Learning Models          | Learner development                        |
| Shared Assets            | Reusable educational intellectual property |
| Student Starter Kits     | Structured practice environments           |
| Adoption Examples        | Local implementation context               |

Ownership should remain clear.

---

## Consumption Is Not Copying

The following patterns should be avoided.

### Poor Pattern

```text
COMP330 creates its own requirements template.

Another course creates its own requirements template.

A third course creates another requirements template.
```

This creates duplication.

---

### Healthy Pattern

```text
shared_assets/templates/
        ↓
Consumed by COMP330
        ↓
Consumed by Course B
        ↓
Consumed by Course C
```

One reusable asset.

Multiple consumers.

---

## The Consumption Rule

When creating a new educational artifact, implementations should ask:

```text
Does this already exist somewhere else?
```

If yes:

Consume it.

If no:

Create it locally.

Then ask:

```text
Can another implementation use this without significant modification?
```

If yes:

Consider promoting it later.

If no:

Keep it local.

---

## Educational Asset Lifecycle

Assets should move through a deliberate lifecycle.

```text
Implementation Need
        ↓
Local Asset Creation
        ↓
Demonstrated Value
        ↓
Review For Reuse
        ↓
Markdown Normalization
        ↓
Provenance Preservation
        ↓
Shared Asset Promotion
```

This lifecycle prevents uncontrolled growth.

---

## Promotion Criteria

An implementation asset should generally satisfy several criteria before promotion.

### Criterion 1: Reuse Potential

Can multiple implementations use it?

### Criterion 2: Minimal Local Assumptions

Does it depend heavily on one institution?

### Criterion 3: Stable Purpose

Is its educational purpose well understood?

### Criterion 4: Clear Ownership

Can future adopters understand where it came from?

### Criterion 5: Markdown Authority

Can it become a Markdown-native ETIS asset?

Only then should promotion occur.

---

## Loyola COMP330 Consumption Example

The current flagship implementation demonstrates the model.

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
Loyola COMP330
```

COMP330 assembles these assets into a semester-long learning experience.

COMP330 should not duplicate them.

---

## Example Consumption Scenario

A future COMP330 implementation might consume:

### Educational Architecture

```text
audience_learning_paths.md

39_chapter_learning_map.md
```

### Learning Models

```text
professional_transformation_model.md

engineering_maturity_model.md

software_engineering_learning_progression.md

two-cycle_engineering_model/
```

### Shared Assets

```text
requirements_review_playbook.md

risk_register_template.md

ai_use_log_template.md

release_readiness_workflow.md
```

### Student Starter Kit

```text
student_starter_kit/comp330/
```

The implementation then adds local materials.

Examples:

```text
Fall 2027 syllabus

Weekly schedule

Assignment due dates

Class slides

Instructor announcements
```

This separation is intentional.

---

## Local Assets

Some assets should remain local.

Examples include:

* Syllabi
* Semester schedules
* Assignment due dates
* Classroom slides
* Instructor observations
* Semester-specific announcements

These assets support the implementation.

They are not educational infrastructure.

---

## Instructor Tools

Instructor tools often begin locally.

Examples include:

* Repository analysis scripts
* Assessment automation
* Reporting tools
* Dashboard generation

These tools should initially remain inside the implementation.

Example:

```text
adoption_examples/
└── loyola_comp330/
    └── instructor_tools/
```

If multiple implementations can use them without major changes, they may later be promoted elsewhere.

---

## Provenance Rules

Every asset should preserve provenance.

Assets should identify:

* Origin institution
* Origin implementation
* Educational purpose
* Relationship to ETIS
* Relationship to reusable assets

Provenance preserves educational memory.

---

## Anti-Patterns

The following anti-patterns should be actively avoided.

### Asset Duplication

Creating multiple versions of the same asset.

### Asset Hoarding

Keeping reusable assets inside implementations.

### Premature Generalization

Promoting assets before reuse is demonstrated.

### Hidden Dependencies

Depending on undocumented materials.

### Institutional Erasure

Removing provenance too early.

### Framework Drift

Allowing implementations to redefine ETIS.

These anti-patterns increase complexity and reduce maintainability.

---

## Relationship to Implementation Governance

This document explains **how assets move through the ecosystem**.

`implementation_governance.md` explains **how implementations remain healthy over time**.

The two documents are complementary.

---

## Future Evolution

This model should remain relatively stable.

New educational implementations may appear.

New shared assets may emerge.

New student starter kits may be created.

However, the underlying consumption relationships should remain simple.

Growth should increase capability, not complexity.

---

## Core Thesis

Educational implementations should assemble ETIS rather than recreate ETIS.

The ecosystem supplies reusable educational infrastructure.

Implementations consume that infrastructure and create local learning experiences.

That separation between reusable assets and local implementation is what allows ETIS to grow without fragmenting.
