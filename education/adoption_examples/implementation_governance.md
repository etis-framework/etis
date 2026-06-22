# Implementation Governance

## Purpose

This document defines how ETIS (Engineering Trustworthy Intelligent Systems) educational implementations are governed over time.

The purpose of implementation governance is to preserve alignment between local educational implementations and the broader ETIS Educational Ecosystem.

Educational implementations are intentionally adaptable.

However, adaptability should not become fragmentation.

Implementation governance provides a framework for allowing local flexibility while preserving the integrity of ETIS.

---

## Core Philosophy

Educational implementations should evolve.

They should not drift.

Evolution is intentional.

Drift is accidental.

Implementation governance exists to help educational adopters make intentional decisions about what should remain stable, what may change locally, and what may eventually become reusable across the ETIS ecosystem.

The goal is sustainable adaptation.

---

## Governance Principle

ETIS is one educational ecosystem with many implementations.

The framework remains stable.

Implementations adapt to local context.

The framework should not be redefined every time a new implementation appears.

Instead, implementations should consume, apply, evaluate, and contribute back to ETIS.

---

## Governance Objectives

Implementation governance has five objectives.

### Preserve educational alignment

Ensure implementations remain connected to the ETIS philosophy and educational goals.

### Preserve ownership boundaries

Ensure reusable educational assets do not become trapped inside local implementations.

### Preserve provenance

Ensure future adopters understand where educational assets originated.

### Preserve educational memory

Ensure implementations remain understandable over time.

### Support responsible evolution

Ensure educational improvements can be incorporated without destabilizing ETIS.

---

## Governance Architecture

Implementation governance operates across three layers.

```text
Stable ETIS Foundation
        ↓
Reusable Educational Assets
        ↓
Local Educational Implementations
```

Each layer changes at a different rate.

---

## Layer 1: Stable ETIS Foundation

This layer changes slowly.

It provides long-term stability.

Examples include:

* ETIS book
* Educational architecture
* Learning models

This layer should remain relatively stable.

Changes should occur infrequently and intentionally.

---

## Layer 2: Reusable Educational Assets

This layer changes occasionally.

Examples include:

* Playbooks
* Templates
* Workflows
* AI Engineering assets
* Assessment assets

This layer grows as educational experience accumulates.

Assets should only enter this layer after demonstrating reuse potential.

---

## Layer 3: Local Educational Implementations

This layer changes frequently.

Examples include:

* Course schedules
* Assignments
* Rubrics
* Slides
* Classroom exercises
* Instructor notes
* Local analysis tools

Local adaptation is expected at this layer.

---

## Governance Questions

Every implementation should regularly answer the following questions.

### Is this still aligned with ETIS?

### Is this implementation-specific or reusable?

### Are we preserving provenance?

### Is educational evidence understandable to future adopters?

### Are we creating unnecessary duplication?

These questions help implementations remain healthy over time.

---

## What Implementations May Change

Implementations may adapt:

* Reading emphasis
* Chapter sequencing
* Weekly schedules
* Assignment structure
* Classroom exercises
* Project scope
* Rubrics
* Local tooling
* Instructor notes

These changes allow implementations to fit local educational environments.

---

## What Implementations Should Not Change

Implementations should not alter the foundational ETIS philosophy.

Core expectations should remain stable.

Examples include:

* Evidence-centered engineering
* Repository-centered engineering
* Human accountability
* Responsible AI usage
* Review culture
* Operational awareness
* Long-term stewardship

These principles should remain visible regardless of implementation.

---

## Provenance Requirements

Every implementation should preserve provenance.

At minimum, implementations should identify:

### Institution

Example:

```text
Loyola University Chicago
```

### Course or program

Example:

```text
COMP 330 — Software Engineering
```

### Audience

Examples:

* Undergraduate students
* Graduate students
* Professional learners

### Relationship to ETIS

Implementations should identify which ETIS assets are being consumed.

### Local adaptations

Implementations should document important local decisions.

Provenance preserves educational memory.

---

## Local Adaptation Documentation

Implementations should make local adaptations visible.

Future adopters should be able to understand:

* What changed
* Why it changed
* What problem it solved
* Whether the adaptation may be useful elsewhere

Adaptations should not remain hidden inside slides, emails, or instructor memory.

---

## Asset Ownership Boundaries

Clear ownership boundaries reduce educational drift.

### Educational Architecture

Defines how ETIS is taught.

### Learning Models

Define how learners develop.

### Shared Assets

Provide reusable educational intellectual property.

### Student Starter Kits

Provide assembled practice environments.

### Adoption Examples

Provide implementation context.

Each implementation should respect these boundaries.

---

## Reuse Promotion Model

Implementations will create new assets.

Not every asset should become part of ETIS.

An asset should generally remain local until reuse is demonstrated.

Promotion path:

```text
Local Asset
        ↓
Demonstrated Value
        ↓
Review For Reuse
        ↓
Normalize To Markdown
        ↓
Preserve Provenance
        ↓
Promote To Shared Assets
```

Promotion should be intentional.

---

## Instructor Tool Governance

Educational implementations may create instructor-specific tooling.

Examples include:

* Repository analysis scripts
* Assessment automation
* Reporting scripts
* Dashboard generation
* Review support tools

These tools should initially remain implementation-specific.

For example:

```text
adoption_examples/
└── loyola_comp330/
    └── instructor_tools/
```

If multiple implementations can use the tools without significant modification, they may eventually be promoted elsewhere.

---

## Educational Memory Preservation

Implementations should preserve educational memory.

Future adopters should be able to answer:

* What was taught?
* Why was it taught?
* What evidence was expected?
* What tools were used?
* What worked well?
* What changed over time?

Educational memory should not depend on a single instructor.

---

## Growth Without Fragmentation

Growth is expected.

Fragmentation is not.

Healthy growth looks like:

```text
Shared Foundation
        ↓
Multiple Implementations
        ↓
Shared Learning
        ↓
Improved Educational Assets
```

Unhealthy growth looks like:

```text
Multiple Implementations
        ↓
Multiple Frameworks
        ↓
Duplicated Assets
        ↓
Conflicting Philosophies
```

The goal is a single ecosystem with many implementations.

---

## Relationship to Loyola COMP330

The current flagship implementation is:

```text
adoption_examples/
└── loyola_comp330/
```

COMP330 provides the initial implementation experience for ETIS.

Its role is to:

* Demonstrate ETIS adoption
* Generate educational evidence
* Generate reusable assets
* Preserve Loyola provenance
* Inform future implementations

COMP330 is an implementation, not the framework itself.

---

## Future Evolution

Over time, ETIS may support many implementations.

Examples include:

* Undergraduate courses
* Graduate courses
* Capstone programs
* Professional workshops
* AI governance programs
* Organizational training programs

Implementation governance should scale with that growth without increasing complexity unnecessarily.

The framework should remain stable while implementations diversify.

---

## Core Thesis

ETIS implementations should be free to adapt without becoming disconnected.

Implementation governance exists to preserve that balance.

The framework remains stable.

The implementations evolve.

The ecosystem learns.
