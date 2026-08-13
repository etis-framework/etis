---
hide:
  - toc
---

<div style="text-align:center; margin-bottom:1.5rem;">
  <img src="../../assets/etis-logo.svg"
       alt="ETIS"
       style="width:320px; max-width:60%; height:auto;">
</div>

# ETIS Repository-Centered Engineering

## From Framework Doctrine to Platform Practice

Repository-Centered Engineering is one of the central ideas of ETIS.

A trustworthy intelligent system is not defined only by the code it runs, the model it calls, or the demo it presents. It is defined by the evidence that shows what the system is intended to do, how it was designed, what risks were identified, what decisions were made, how AI assistance was used, how behavior was verified, who reviewed the work, what was released, what happened in operation, and how the system will be stewarded over time.

Within ETIS, the repository is the engineering memory system.

It is where trust becomes reviewable.

---

## The Public ETIS Repository Model

The public ETIS ecosystem is anchored by two primary repositories, complemented by specialized educational, community, and organization repositories.

These two repositories form the primary Framework-and-Platform architecture. Specialized repositories support focused capabilities such as course implementations, student-facing engineering tooling, community participation, and organization-level resources.

| Repository | Public Site | Primary Role |
|---|---|---|
| **ETIS Framework Repository** | [etisframework.org](https://etisframework.org) | Defines and publishes the ETIS discipline: book, Publications Program, framework, education, downloads, resources, and roadmap. |
| **ETIS Engineering Platform Starter Kit Repository** | [platform.etisframework.org](https://platform.etisframework.org) | Demonstrates how to apply ETIS through Engineering Stages ES-100 through ES-114, templates, LMU/COICP examples, governance assets, and a Project Workspace. |

For an introduction to the Platform, its audiences, capabilities, and relationship to the broader ETIS ecosystem, begin with the [Platform Overview](../Platform/Platform.md). The external Platform site is the working implementation environment.

The relationship is intentional.

```text
Framework Repository
    Defines the discipline
    Publishes the Two-Volume Edition
    Publishes white papers, executive briefs, and education papers
    Maintains education, downloads, and ecosystem guidance

Engineering Platform Repository
    Operationalizes the discipline
    Provides stages, templates, examples, and workspaces
    Helps teams practice ETIS in real project repositories
```

The Framework repository is the authority.  
The Platform repository is the application environment.

---

## Why the Repository Matters

Modern AI-assisted engineering can generate artifacts quickly. That speed is useful, but it also makes verification, accountability, context, and continuity more important.

Repository-Centered Engineering answers a practical question:

> When the work accelerates, where does engineering truth live?

In ETIS, the answer is the repository.

A trustworthy repository preserves:

- stakeholder intent;
- requirements and constraints;
- assumptions and risks;
- architecture decisions;
- AI-use logs and verification notes;
- design decisions;
- implementation records;
- pull requests and reviews;
- test evidence;
- release-readiness evidence;
- operational-readiness evidence;
- deployment and transition records;
- incidents and postmortems;
- governance decisions;
- stewardship reviews.

The repository is not bureaucracy. It is the evidence system that allows engineers, reviewers, operators, instructors, auditors, leaders, and future maintainers to understand what happened and why.

---

## The ETIS Engineering Platform

The ETIS Engineering Platform is the practical implementation layer of the ETIS Framework.

It includes:

- **Engineering Stages ES-100 through ES-114** — lifecycle guidance from project start through post-release learning and stewardship;
- **Template Library** — reusable artifacts for requirements, architecture, reviews, release readiness, governance, operations, and stewardship;
- **LMU/COICP reference examples** — completed examples showing how ETIS artifacts look in a realistic institutional system;
- **Project Workspace** — a reusable environment where adopters create project-specific engineering evidence;
- **Governance and evidence assets** — practical controls that make AI use, review, release, and operations visible;
- **GitHub and MkDocs structure** — a publication and collaboration model suitable for teaching, practice, and professional adoption.

The Platform is not a replacement for the Framework or the book. It is the bridge from understanding ETIS to practicing ETIS.

[Explore the Platform Overview →](../Platform/Platform.md)

[Launch the ETIS Engineering Platform ↗](https://platform.etisframework.org)

---

## Engineering Stages ES-100 through ES-114

The Engineering Platform organizes practice through a staged lifecycle.

```text
ES-100 — Start Here
ES-101 — Vision and Problem Definition
ES-102 — Requirements and Constraints
ES-103 — Planning and Work Breakdown
ES-104 — Architecture
ES-105 — Design and Technical Decisions
ES-106 — Implementation Readiness
ES-107 — AI-Assisted Implementation
ES-108 — Code Review and Integration
ES-109 — Testing and Verification
ES-110 — Release Readiness
ES-111 — Operational Readiness
ES-112 — Deployment and Transition
ES-113 — Operations and Monitoring
ES-114 — Post-Release Learning and Stewardship
```

Each stage gives teams a practical operating model:

- engineering context;
- activities;
- expected evidence;
- outputs;
- readiness gate;
- stage manifest.

This matters because ETIS is not only a set of ideas. It is a disciplined way to move work through the lifecycle.

---

## LMU/COICP as Reference Examples

ETIS uses Lakeside Metropolitan University (LMU) and the Campus Operations and Incident Coordination Platform (COICP) as the continuing enterprise example.

LMU/COICP is represented through completed reference examples inside the Engineering Platform Starter Kit. It should not be described as a separate planned public repository unless a separate repository is intentionally created later.

The examples show how ETIS evidence accumulates across a lifecycle:

- requirements become reviewable commitments;
- constraints shape architecture;
- architecture decisions preserve judgment;
- AI use is disclosed and verified;
- reviews challenge claims before release;
- test evidence supports readiness;
- operational records create learning;
- postmortems drive improvement;
- stewardship preserves trust over time.

The examples are not meant to be copied blindly. They are meant to calibrate judgment.

---

## Starter Kit, Examples, and Project Workspace

The Engineering Platform contains four practical modes of use.

| Platform Area | Purpose | Question Answered |
|---|---|---|
| **Engineering Stages** | Guide teams through the ETIS lifecycle | “What should we do next?” |
| **Template Library** | Provide reusable artifact structures | “What should this artifact contain?” |
| **LMU/COICP Examples** | Show completed reference examples | “What does this look like when done well?” |
| **Project Workspace** | Give adopters a place to create evidence | “Where do we put our project work?” |

Together, these areas create a practical loop.

```text
Learn the doctrine in the Framework
        ↓
Use Publications for focused guidance
        ↓
Use the Platform stages to guide the work
        ↓
Use templates to create evidence
        ↓
Study LMU/COICP examples to calibrate quality
        ↓
Preserve project-specific evidence in the workspace
        ↓
Review, release, operate, learn, and steward
```

That loop is Repository-Centered Engineering in practice.

---

## Publications and Repository-Centered Engineering

The ETIS Publications Program extends repository-centered engineering in two important ways.

First, the Framework repository preserves the source, metadata, version history, canonical landing page, and authoritative PDF for each publication.

Second, several publications provide focused guidance on the repository-centered model itself, including:

- [WP-002 — Repository-Centered Engineering](../publications/white-papers/wp-002.md)
- [WP-003 — Engineering Evidence](../publications/white-papers/wp-003.md)
- [WP-007 — Engineering Review and Readiness](../publications/white-papers/wp-007.md)
- [WP-009 — Context Engineering](../publications/white-papers/wp-009.md)
- [EB-004 — Building an AI Engineering Platform](../publications/executive-briefs/eb-004.md)

Readers should enter through the canonical publication webpages, not through repository directories or direct PDF links.

---

## How Instructors Can Use It

For instructors, Repository-Centered Engineering gives students an environment where professional behavior becomes visible.

Students can use the Engineering Platform as a professional reference and implementation environment to:

- understand staged engineering work;
- study reusable artifact structures;
- examine requirements, planning, architecture, review, verification, release, and operational evidence patterns;
- understand how AI assistance should be disclosed and verified;
- compare engineering approaches against LMU/COICP reference examples;
- and strengthen the quality of evidence preserved in their project repositories.

When a course defines a course-specific team repository, that repository remains the authoritative location for project-specific engineering evidence. The Engineering Platform provides the lifecycle guidance, examples, templates, and professional reference model that help students produce stronger engineering work.

The Framework teaches the professional doctrine.  
The Education Papers reinforce professional formation.  
The Platform demonstrates how the discipline is applied.  
The course repository preserves what the team actually did.

[Explore the ETIS Education Papers →](../publications/education-papers/index.md)

---

## How Professionals Can Use It

For professional teams, the Engineering Platform provides a practical starting point for applying ETIS without inventing every artifact from scratch.

Teams can use it to:

- establish a project evidence structure;
- standardize lifecycle stages;
- align governance with engineering work;
- make AI use visible and reviewable;
- create release and operational-readiness evidence;
- train review boards and technical leaders;
- adapt ETIS practices to organizational standards.

The Platform is not a rigid compliance template. It is a disciplined starting architecture for trustworthy engineering work.

---

## What Repository-Centered Engineering Changes

Repository-Centered Engineering changes the center of gravity for AI-era software engineering.

It moves trust from assertion to evidence.

It moves governance from policy slides into architecture, workflows, reviews, release gates, and operational records.

It moves AI assistance from hidden productivity to visible, verified contribution.

It moves learning from memory and meetings into durable postmortems, decisions, and stewardship records.

It moves professional accountability into the place where the work actually happens.

---

## Bottom Line

ETIS is not only a framework to read. It is a discipline to practice.

The Framework defines the discipline.  
Publications provide focused guidance.  
The Engineering Platform operationalizes the discipline.  
The repository preserves the evidence.

In the AI era, the repository is no longer just where the code lives.

It is where engineering truth lives.

[Explore the Platform Overview →](../Platform/Platform.md)

[Launch the ETIS Engineering Platform ↗](https://platform.etisframework.org)

[Browse the ETIS Engineering Platform Starter Kit Repository ↗](https://github.com/etis-framework/etis-starter-kit)
