# Evidence Index Template

**Classification:** ETIS Educational Ecosystem Asset

**Category:** Template

**Origin:** ETIS Educational Ecosystem

**Initial Implementation:** Loyola University Chicago COMP 330 — Software Engineering

**Authoritative Format:** Markdown

**Typical Repository Location:** `/docs/evidence/evidence-index.md`

---

# Purpose

The Evidence Index provides a high-level map of engineering evidence contained within a repository.

The purpose is not to duplicate existing artifacts.

The purpose is to help reviewers, instructors, future maintainers, and engineering teams quickly understand where important evidence exists and whether that evidence is complete.

As projects mature, engineering artifacts naturally accumulate.

The Evidence Index creates visibility into those artifacts.

It becomes a navigational layer for repository-centered engineering.

---

# Core Philosophy

The repository is the engineering memory system.

The Evidence Index is the table of contents for that memory.

This artifact helps answer questions such as:

* What evidence exists?
* What evidence is missing?
* What evidence supports release readiness?
* What evidence supports operational understanding?
* What evidence supports engineering decisions?
* What evidence remains incomplete?

The objective is engineering transparency.

---

# Engineering Lifecycle Coverage

The repository should gradually accumulate evidence throughout the engineering lifecycle.

```text
Intent
↓
Planning
↓
Architecture
↓
Implementation
↓
Testing
↓
Review
↓
Release
↓
Operations
↓
Learning
```

The Evidence Index helps teams understand where that evidence resides.

---

# Repository Information

| Field                   | Team Response              |
| ----------------------- | -------------------------- |
| Project Name            |                            |
| Team Number / Team Name |                            |
| Repository URL          |                            |
| Release Version / Cycle |                            |
| Last Updated            |                            |
| Primary Owner           | Operations & Evidence Lead |
| Backup Owner            |                            |

---

# Evidence Inventory

## Intent and Planning Evidence

| Artifact      | Repository Location | Status                               | Owner |
| ------------- | ------------------- | ------------------------------------ | ----- |
| Team Charter  |                     | Not Started / In Progress / Complete |       |
| Requirements  |                     |                                      |       |
| Role Matrix   |                     |                                      |       |
| Risk Register |                     |                                      |       |
| Meeting Notes |                     |                                      |       |

---

## Architecture Evidence

| Artifact                             | Repository Location | Status | Owner |
| ------------------------------------ | ------------------- | ------ | ----- |
| Architecture Overview                |                     |        |       |
| Architecture Decision Records (ADRs) |                     |        |       |
| Diagrams                             |                     |        |       |

---

## AI Engineering Evidence

| Artifact              | Repository Location | Status | Owner |
| --------------------- | ------------------- | ------ | ----- |
| AI Policy             |                     |        |       |
| AI Use Log            |                     |        |       |
| AI Verification Notes |                     |        |       |

---

## Testing and Quality Evidence

| Artifact      | Repository Location | Status | Owner |
| ------------- | ------------------- | ------ | ----- |
| Test Plan     |                     |        |       |
| Test Evidence |                     |        |       |
| CI Evidence   |                     |        |       |
| Defect Log    |                     |        |       |

---

## Release Evidence

| Artifact          | Repository Location | Status | Owner |
| ----------------- | ------------------- | ------ | ----- |
| Release Notes     |                     |        |       |
| Demo Script       |                     |        |       |
| Known Limitations |                     |        |       |

---

## Operational Evidence

| Artifact                | Repository Location | Status | Owner |
| ----------------------- | ------------------- | ------ | ----- |
| Runbook                 |                     |        |       |
| Observability Notes     |                     |        |       |
| Operational Assumptions |                     |        |       |

---

## Learning Evidence

| Artifact   | Repository Location | Status | Owner |
| ---------- | ------------------- | ------ | ----- |
| Postmortem |                     |        |       |
| Reflection |                     |        |       |

---

# Evidence Completeness Assessment

Rate the current repository.

| Category              | Assessment               |
| --------------------- | ------------------------ |
| Intent                | Strong / Adequate / Weak |
| Architecture          | Strong / Adequate / Weak |
| AI Governance         | Strong / Adequate / Weak |
| Testing               | Strong / Adequate / Weak |
| Release Readiness     | Strong / Adequate / Weak |
| Operational Readiness | Strong / Adequate / Weak |
| Learning              | Strong / Adequate / Weak |

---

# Missing Evidence

List evidence that should exist but does not yet exist.

| Missing Artifact | Why It Matters | Owner | Target Date |
| ---------------- | -------------- | ----- | ----------- |
|                  |                |       |             |

---

# Reviewer Questions

A reviewer should be able to answer:

* Can I understand what this system is trying to accomplish?
* Can I understand how it is built?
* Can I understand what AI was allowed to do?
* Can I understand what was tested?
* Can I understand what risks remain?
* Can I understand how to operate it?
* Can I understand what the team learned?

If not, additional evidence may be needed.

---

# Final Takeaway

The Evidence Index is not another document to maintain.

It is a navigational layer that helps transform repositories from collections of files into understandable engineering systems.

