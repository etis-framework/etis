# Executable Verification Package

## Purpose

This directory contains executable tests used to verify engineering behavior.

Unlike the `docs/` directory, these artifacts are executed by tools rather than primarily read by humans.

The goal is to verify engineering claims through repeatable execution.

Keep tests simple, understandable, and maintainable.

Do not over-engineer them.

---

## Test Areas

| Directory | Purpose |
|-----------|---------|
| `unit/` | Verifies individual components in isolation |
| `integration/` | Verifies interactions between components |

---

## Relationship To ETIS Philosophy

Testing answers one question:

> How do we know our engineering claims are true?

Executable tests provide evidence that expected behavior actually occurred.

Students should continuously ask:

- What behavior are we verifying?
- What assumptions are we validating?
- What failures should be detected?
- What evidence are we creating?

Tests should remain understandable.

Complicated tests often become unmaintainable tests.

---

## Relationship To `docs/testing/`

`docs/testing/` teaches testing.

`tests/` performs testing.

The two directories intentionally complement each other.

```text
docs/testing/

↓

Testing Intent

↓

tests/

↓

Testing Execution
```

---

## Review Questions

Teams should periodically ask:

- Are important behaviors being tested?
- Are tests understandable?
- Are tests maintainable?
- Are failures easy to diagnose?

---

## Engineering Standard

Engineering claims should be supported by repeatable verification.