# Adoption Examples

## Purpose

The `adoption_examples` directory contains concrete educational implementations of the ETIS (Engineering Trustworthy Intelligent Systems) Educational Ecosystem.

This directory shows how ETIS can be adopted, adapted, and taught in real educational settings.

Adoption examples are not the Educational Ecosystem itself.

They are implementation records that demonstrate how the ETIS book, educational architecture, learning models, shared assets, and student starter kits can be applied within a specific course, institution, program, workshop, or training environment.

---

## Mission

The mission of `adoption_examples` is to preserve implementation-specific educational practice while maintaining a clear relationship to the broader ETIS framework.

Each adoption example should show how a specific educational setting uses ETIS to teach trustworthy engineering.

Adoption examples help future instructors and adopters understand:

* What was taught
* Why it was taught
* How the course or program was structured
* Which ETIS assets were used
* Which implementation-specific materials were created
* What should remain local to the implementation
* What may eventually become reusable across implementations

---

## Core Philosophy

ETIS should be adaptable without becoming fragmented.

Different institutions, programs, courses, instructors, and professional contexts will teach ETIS differently.

That variation is expected.

However, variation should occur within a governed educational architecture.

Adoption examples preserve local implementation context without allowing course-specific materials to overwrite the shared ETIS ecosystem.

The goal is not to force every adopter to teach ETIS identically.

The goal is to preserve enough structure that each implementation remains aligned with trustworthy engineering.

---

## Directory Role

This directory owns implementation-specific educational examples.

It does not own shared assets.

It does not own master learning models.

It does not own the ETIS book.

It does not own the Student Starter Kit architecture.

It records how those assets are used in specific educational contexts.

---

## Current Directory Structure

```text
adoption_examples/

├── README.md

└── loyola_comp330/
```

The current flagship implementation is:

```text
adoption_examples/loyola_comp330/
```

Future implementations may include:

```text
adoption_examples/

├── loyola_comp330/

├── graduate_software_engineering/

├── capstone_program/

├── professional_workshop/

├── ai_governance_training/

└── organizational_training/
```

Future examples should be added only when they represent a real implementation or a carefully designed adoption model.

---

## Flagship Implementation

Loyola University Chicago COMP 330 — Software Engineering is the flagship ETIS educational implementation.

It is currently located at:

```text
adoption_examples/loyola_comp330/
```

COMP330 is important because it provides the initial real-world implementation context for ETIS Phase II.

However, COMP330 is not the Educational Ecosystem itself.

COMP330:

* Consumes educational architecture
* Consumes learning models
* Consumes shared assets
* Uses the Student Starter Kit
* Preserves Loyola provenance
* Contributes new educational assets
* Demonstrates how ETIS can operate in a semester-long software engineering course

---

## What Belongs Here

The following belong in `adoption_examples`:

* Course-specific implementations
* Institution-specific implementations
* Program-specific adoption examples
* Workshop implementation examples
* Training implementation examples
* Local syllabi
* Weekly schedules
* Assignment sequences
* Course-specific rubrics
* Course slides
* Implementation notes
* Instructor observations
* Local adaptation decisions
* Local tooling and analysis scripts when implementation-specific
* Reflection and lessons learned artifacts

This directory should preserve the context needed to understand how ETIS was actually adopted.

---

## What Does Not Belong Here

The following do not belong directly in `adoption_examples`:

* Reusable playbooks
* Reusable templates
* Reusable workflows
* Reusable AI Engineering guidance
* Reusable assessment assets
* Master learning models
* Student starter kit architecture
* Generic ETIS educational architecture
* The ETIS book manuscript

Those assets belong elsewhere in the Educational Ecosystem.

If a local implementation creates an asset that later becomes broadly reusable, it may be normalized and promoted to `shared_assets`.

---

## Relationship to Educational Architecture

The `educational_architecture` directory defines how ETIS is taught at the system level.

The `adoption_examples` directory shows how that architecture is implemented in specific settings.

Relationship model:

```text
Educational Architecture
        ↓
Learning Models
        ↓
Shared Assets
        ↓
Student Starter Kits
        ↓
Adoption Examples
        ↓
Local Educational Practice
```

Educational architecture provides the governing structure.

Adoption examples demonstrate local application.

---

## Relationship to Learning Models

Adoption examples consume learning models.

Learning models explain how learners develop.

Adoption examples show how that development is supported in a specific context.

For example, Loyola COMP330 uses:

* Professional Transformation Model
* Engineering Maturity Model
* Software Engineering Learning Progression
* Two-Cycle Engineering Model

Other implementations may use the same models differently depending on audience, instructional time, and educational goals.

---

## Relationship to Shared Assets

Adoption examples consume shared assets.

Shared assets should not be duplicated inside adoption examples unless there is a clear implementation-specific reason.

For example, a course may reference:

* Playbooks
* Templates
* Workflows
* AI Engineering assets
* Assessment assets

If a course modifies a shared asset for local use, the local version should remain clearly identified as implementation-specific.

If the modification has broader value, it may later be considered for promotion back into `shared_assets`.

---

## Relationship to Student Starter Kits

Adoption examples may use Student Starter Kits.

A starter kit provides a structured engineering environment for learners.

The adoption example explains how that starter kit is used within a specific course, workshop, or program.

The starter kit is the student practice environment.

The adoption example is the implementation context.

---

## Local Adaptation Rules

Adoption examples may adapt:

* Sequencing
* Assignments
* Weekly schedules
* Reading emphasis
* Classroom exercises
* Local rubrics
* Instructor notes
* Project structure
* Workshop timing
* Program constraints

Adoption examples should not alter:

* Core ETIS principles
* The authority of the ETIS book
* The ownership boundaries of shared assets
* The distinction between implementation-specific material and reusable assets
* The principle that Markdown is authoritative
* The requirement to preserve provenance

Adaptation is expected.

Architectural drift is not.

---

## Provenance

Every adoption example should preserve provenance.

An adoption example should clearly identify:

* Institution or organization
* Course, program, workshop, or training context
* Intended audience
* Instructor or steward when appropriate
* Term or version when appropriate
* Relationship to ETIS
* Relationship to shared assets
* Local adaptations

Provenance matters because implementation history is educational memory.

---

## Implementation Structure

Educational implementations should remain flexible.

Implementations may organize materials differently based on institutional needs.

Examples may include:

* Syllabi
* Weekly schedules
* Assignments
* Rubrics
* Slides
* Implementation notes
* Instructor tools

The exact organization is intentionally implementation dependent.

The implementation should prioritize understandability over structural consistency.

---

## Instructor Tools and Analysis Scripts

Some adoption examples may include instructor tools.

These may include scripts, reports, or analysis utilities that support a specific implementation.

For example, COMP330 may include Python scripts that analyze student GitHub repositories after assignments.

Such tools should initially remain inside the relevant adoption example when they are implementation-specific.

A likely location is:

```text
adoption_examples/
└── loyola_comp330/
    └── instructor_tools/
        └── repository_analysis/
```

These tools may later be promoted into a reusable instructor package or shared assessment infrastructure if multiple implementations can use them without significant local assumptions.

The governing rule is:

Implementation-specific tools begin inside the implementation.

Reusable educational infrastructure may later be promoted.

---

## Promotion Path for Reusable Assets

Adoption examples may generate new educational assets.

When an implementation-specific asset proves broadly useful, it may move through the following path:

```text
Local implementation asset
        ↓
Reviewed for reuse
        ↓
Normalized into Markdown
        ↓
Provenance preserved
        ↓
Promoted to shared_assets
        ↓
Consumed by multiple implementations
```

Promotion should be deliberate.

Not every local course artifact should become a shared ETIS asset.

---

## Governance Rules

The following governance rules apply to this directory.

### Preserve implementation context.

Adoption examples should remain understandable as real educational implementations.

### Do not bury reusable assets here.

Reusable assets should live in `shared_assets`.

### Do not prematurely generalize.

Local materials should remain local until reuse is demonstrated.

### Preserve provenance.

Implementation history is educational memory.

### Keep local adaptations visible.

Future adopters should understand what was changed and why.

### Avoid uncontrolled expansion.

New adoption examples should represent meaningful implementations, not speculative placeholders.

---

## Future Evolution

This directory may grow as ETIS is adopted in additional settings.

Future adoption examples may include:

* Undergraduate software engineering courses
* Graduate software engineering courses
* Capstone programs
* AI governance workshops
* Professional development programs
* Organizational training programs
* Government or public-sector training programs

Growth should occur through governed adoption, not accumulation.

Each new adoption example should explain how it uses ETIS and what makes the implementation distinct.

---

## Core Thesis

ETIS adoption should be adaptable, but not uncontrolled.

The `adoption_examples` directory exists to preserve real implementation practice while protecting the integrity of the broader Educational Ecosystem.

Each adoption example should show how ETIS can be taught in context without allowing local context to fragment the framework.
