# Implementation Package

## Purpose

This directory contains the implementation of the system.

Implementation transforms engineering intent into engineering behavior.

This directory should contain source code rather than engineering evidence.

Engineering evidence belongs in `docs/`.

Implementation should remain understandable, maintainable, and reviewable.

Do not over-engineer the structure.

Allow the implementation to evolve naturally as complexity increases.

---

## Relationship To The Engineering Lifecycle

Implementation consumes engineering decisions created elsewhere in the repository.

```text
Requirements

↓

Planning

↓

Architecture

↓

Implementation

↓

Testing

↓

Release
```

Implementation should remain connected to engineering evidence throughout the project.

---

## Relationship To ETIS Philosophy

The model is not the system.

Implementation is where engineering decisions become executable reality.

Students should continuously ask:

- Does the implementation match requirements?
- Does the implementation match the architecture?
- Is the implementation understandable?
- Is unnecessary complexity emerging?

Implementation should never become disconnected from engineering evidence.

---

## Implementation Expectations

Source code should be:

- understandable
- maintainable
- reviewable
- testable
- appropriately documented

Avoid unnecessary complexity.

Prefer clarity over cleverness.

---

## Documentation Expectations

If implementation decisions become significant, document them in the appropriate location under `docs/`.

Do not bury important engineering decisions inside source code.

---

## Review Questions

Teams should periodically ask:

- Can another engineer understand the implementation?
- Is complexity increasing unnecessarily?
- Is implementation still aligned with requirements?
- Is implementation still aligned with architecture?

---

## Engineering Standard

Strong implementations remain understandable long after they are written.