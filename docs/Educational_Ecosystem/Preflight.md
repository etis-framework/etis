---
hide:
  - toc
---

# ETIS Preflight

**Phase-gate readiness analysis before formal engineering review**

ETIS Preflight helps student engineering teams determine whether their repository appears ready to enter a formal phase-gate review.

It is the readiness component of the [ETIS Engineering Education Suite](Engineering_Education_Suite.md).

Preflight uses analytical heuristics, rules, repository inspection, and phase-specific expectations to check whether required evidence is present and whether that evidence has the basic shape expected at the current point in the engineering lifecycle.

It does not grade the project and it does not perform the formal engineering review.

---

## What Preflight Checks

Preflight is phase-gate aware. The expected evidence changes as the team progresses through the course.

Depending on the gate, readiness analysis may include areas such as:

- repository organization;
- expected engineering artifacts;
- requirements and acceptance evidence;
- architecture and decision records;
- team roles and governance evidence;
- AI-use and verification records;
- test and verification evidence;
- release and operational evidence;
- Git/GitHub workflow and traceability;
- phase-specific completeness and basic artifact shape.

The goal is not to prove that the engineering work is correct.

The goal is to identify obvious readiness gaps before the team submits the repository for formal review.

---

## A Sophisticated Readiness Check, Not a Gate Decision

A traditional checklist can answer whether a box was checked.

Preflight goes further by examining repository evidence and applying phase-aware analytical rules. It helps teams recognize when an artifact is missing, incomplete, structurally weak, or inconsistent with the basic evidence expected for that gate.

That remains different from engineering judgment.

A repository can pass basic readiness checks and still contain weak decisions, unconvincing evidence, unresolved risk, or incorrect reasoning. Those concerns belong in developmental review and formal engineering review.

---

## Relationship to Engineering Studio

[ETIS Engineering Studio](Engineering_Studio.md) and Preflight are complementary but independent.

Preflight provides final readiness guidance about whether expected gate evidence is present and basically reviewable.

Studio uses controlled engineering reviewers to look at the team's frozen evidence more holistically, ask questions, challenge reasoning, and help students develop engineering judgment before formal review.

Studio does not simply replay Preflight findings. Its review board examines the engineering evidence through its own controlled reviewer perspectives.

---

## Relationship to Formal Phase-Gate Review

After the team is ready, the formal review is conducted through the instructor-facing [ETIS Engineering Review Center](Engineering_Review_Center.md).

The formal gate uses the evidence established by the course-designated Git tag.

Preflight can help a team avoid arriving at that review with missing or obviously malformed evidence. It does not determine whether the team passes the gate.

The instructor remains the academic authority.

---

## Flagship Use

The COMP 330/474 flagship implementation uses Preflight as part of a larger two-cycle phase-gate model.

Students can use Preflight before formal submission to identify readiness concerns while they still have time to improve the repository.

[Explore the COMP 330/474 Flagship Implementation →](Flagship_Implementation.md)

---

## Public Reference Tool

The COMP 330/474 ETIS Preflight implementation is published openly so students can understand and run the readiness checks that apply to their repository.

[Open ETIS Preflight Repository ↗](https://github.com/etis-framework/comp330-submission-preflight){ .md-button }

Course-specific requirements remain authoritative. Another institution may adapt the readiness model to its own phase gates, repository structure, and educational objectives.

---

## Bottom Line

Preflight asks a deliberately narrow question:

> **Is the repository ready to enter formal engineering review?**

It helps students find basic evidence and readiness gaps early while preserving the distinction between automated readiness analysis, developmental engineering judgment, and instructor-led formal review.
