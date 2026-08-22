---
hide:
  - toc
---

<div style="text-align:center; margin-bottom:1.5rem;">
  <img src="../../assets/etis-logo.svg"
       alt="ETIS"
       style="width:320px; max-width:60%; height:auto;">
</div>

# ETIS Repository Ecosystem

**Public source, reusable engineering assets, and repository-centered implementation**

ETIS is a repository-centered engineering ecosystem.

The public ETIS ecosystem is organized around two foundational repositories complemented by specialized educational, service, community, and organization repositories.

The Framework and Engineering Platform repositories form the knowledge-and-implementation foundation of ETIS. Specialized repositories support course implementations, educational services, community participation, organization-level resources, and other focused capabilities while preserving clear separation of responsibilities and release models.

- the **ETIS Framework Repository** defines, publishes, and preserves the ETIS body of knowledge;
- the **ETIS Engineering Platform Starter Kit Repository** operationalizes ETIS through stages, templates, examples, governance assets, and project workspaces.

This separation is deliberate.

The Framework repository defines and publishes the discipline.  
The Starter Kit repository demonstrates how to apply the discipline.

---

## Repository Map

| Repository | Public Site | Primary Responsibility |
|---|---|---|
| **ETIS Framework Repository** | [etisframework.org](https://etisframework.org) | Authoritative source for the Framework, Framework Reference Work, Books and Professional Computing Series materials, Publications Program, Educational Ecosystem, downloads, resources, roadmap, and public website. |
| **ETIS Engineering Platform Starter Kit Repository** | [platform.etisframework.org](https://platform.etisframework.org) | Practical implementation environment containing Engineering Stages ES-100 through ES-114, templates, LMU/COICP examples, governance assets, and Project Workspace materials. |
| **ETIS Engineering Studio Repository** | [Engineering Studio overview](../Educational_Ecosystem/Engineering_Studio.md) | Open-source reference implementation of the instructor-operated student-team environment for evidence-grounded developmental review and engineering-judgment formation. |

<div style="margin-top:.75rem;">

<a class="md-button md-button--primary"
   href="https://github.com/etis-framework/etis">
Browse Framework Repository
</a>

<a class="md-button"
   href="https://github.com/etis-framework/etis-starter-kit">
Browse Engineering Platform Starter Kit
</a>

</div>

For an introduction to the Platform and its relationship to the ETIS ecosystem, begin with the [Platform Overview](../Platform/Platform.md). The external Platform site is the working implementation environment.

---

## ETIS Framework Repository

**Repository:** [github.com/etis-framework/etis](https://github.com/etis-framework/etis)  
**Website:** [etisframework.org](https://etisframework.org)

The Framework repository contains the authoritative source for the ETIS public knowledge platform.

It includes:

- the complete *Engineering Trustworthy Intelligent Systems* Framework Reference Work;
- the ETIS Two-Volume Professional Edition;
- the ETIS Books architecture and Professional Computing Series materials;
- *From Data Structures to Engineering Judgment* website and companion-resource materials;
- the ETIS White Paper Series;
- the ETIS Executive Brief Series;
- the ETIS Education Paper Series;
- canonical publication webpages and publication PDF assets;
- appendices;
- educational ecosystem materials;
- educational-product references;
- downloads and resource guidance;
- public roadmap and governance files;
- MkDocs website source;
- visual, branding, and navigation assets.

This repository is the long-term authority for ETIS doctrine, the Framework Reference Work, ETIS Books, focused publications, and public framework content.

[Explore ETIS Books →](../Books/index.md)

[Explore ETIS Publications →](../publications/index.md)

---

## ETIS Engineering Platform Starter Kit Repository

**Repository:** [github.com/etis-framework/etis-starter-kit](https://github.com/etis-framework/etis-starter-kit)  
**Framework-site gateway:** [Platform Overview](../Platform/Platform.md)

**Website:** [platform.etisframework.org](https://platform.etisframework.org)

The Starter Kit repository contains the ETIS Engineering Platform.

It includes:

- Engineering Stages ES-100 through ES-114;
- stage guidance, activities, outputs, evidence expectations, readiness gates, and manifests;
- Template Library;
- completed LMU/COICP reference examples;
- Project Workspace;
- governance and evidence-centered engineering assets;
- GitHub workflows and collaboration templates;
- MkDocs-based platform site.

This repository is the practical application layer for ETIS.

---

## Ecosystem Architecture

```text
ETIS Framework Website and Repository
    Learn ETIS
    Read the Framework Reference Work
    Explore ETIS Books and the Professional Computing Series
    Explore focused publications
    Understand the doctrine
    Use education and framework resources
    Obtain curated downloads
    Inspect public framework source

ETIS Engineering Platform and Starter Kit Repository
    Apply ETIS
    Follow Engineering Stages ES-100 through ES-114
    Use reusable templates
    Study LMU/COICP examples
    Establish governance and evidence practices
    Create project-specific engineering records
```

The repositories complement each other without duplicating their primary responsibilities.

The Framework and Engineering Platform repositories remain the two foundational knowledge-and-implementation repositories. The public Engineering Studio repository adds an adoptable educational service implementation with a different operational responsibility and release model. Additional specialized repositories may support course tooling, instructor resources, student engineering workflows, and future professional capabilities while preserving clear separation of authority and provenance.

---

## Publications and Repository Authority

The Publications Program is published through the ETIS Framework repository.

For each publication:

- the canonical webpage provides discovery, metadata, citation, version history, related materials, and PDF access;
- the PDF is the authoritative publication edition;
- the repository preserves the Markdown source, publication assets, navigation, and versioned public record.

Readers should enter publications through the canonical landing pages rather than browse the repository directory directly.

[Explore the Publications Program →](../publications/index.md)

---

## LMU/COICP Reference Examples

ETIS uses Lakeside Metropolitan University (LMU) and the Campus Operations and Incident Coordination Platform (COICP) as a continuing enterprise example.

LMU/COICP examples are included inside the Engineering Platform Starter Kit. They are not presented as a separate public repository.

The examples show how ETIS artifacts connect across the lifecycle:

- vision and problem framing;
- requirements and constraints;
- planning and work breakdown;
- architecture;
- design decisions and ADRs;
- AI-assisted implementation controls;
- code review and integration evidence;
- testing and verification;
- release readiness;
- operational readiness;
- deployment and transition;
- operations and monitoring;
- post-release learning and stewardship.

The examples make the framework inspectable.

---

## Template Library

The Template Library provides reusable ETIS-aligned artifact structures.

Templates help teams start faster while preserving discipline. They support students, instructors, professional teams, review boards, and organizations adopting ETIS practices.

Templates do not replace engineering judgment. They create a consistent place to preserve it.

---

## Project Workspace

The Project Workspace gives adopters a controlled place to create project-specific evidence.

It is designed for:

- real projects;
- class projects;
- professional pilots;
- organizational demonstrations;
- reference implementations.

The workspace is where teams turn ETIS concepts into reviewable engineering evidence.

---

## Downloads and Repository Archives

The Downloads area may provide curated repository archives for local use, classroom use, institutional adoption, or project startup.

A repository archive is a packaged distribution of the working repository. It does not replace the public GitHub repository or the Engineering Platform website.

- [Download the ETIS Engineering Platform Starter Kit](download.md#engineering-platform-starter-kit)
- [Browse the Engineering Platform Starter Kit Repository](https://github.com/etis-framework/etis-starter-kit)
- [Explore the Platform Overview](../Platform/Platform.md)
- [Launch the Engineering Platform ↗](https://platform.etisframework.org)

---

## How to Use the Ecosystem

| Need | Start here |
|---|---|
| Learn what ETIS is | [What is ETIS?](../Framework/What_is_ETIS.md) |
| Understand why ETIS exists | [Why ETIS?](../Framework/Why_ETIS.md) |
| Read the complete Framework Reference Work | [Read Online](../Front_Matter/01_Title_Page.md) |
| Understand repository-centered engineering | [Repository-Centered Engineering](../Framework/ETIS_Repository_Centered_Engineering.md) |
| Understand the Platform and how to begin | [Platform Overview](../Platform/Platform.md) |
| Enter the working implementation environment | [Launch Engineering Platform ↗](https://platform.etisframework.org) |
| Use stages, templates, and examples | [Engineering Platform Starter Kit Repository](https://github.com/etis-framework/etis-starter-kit) |
| Download the Engineering Platform Starter Kit archive | [Starter Kit Download](download.md#engineering-platform-starter-kit) |
| Create a COMP 330 Fall 2026 team repository | [COMP 330 Course Starter Kit](https://github.com/etis-framework/comp330-f26-starter-kit) |
| Check COMP 330/474 phase-gate readiness | [ETIS Preflight](https://github.com/etis-framework/comp330-submission-preflight) |
| Participate in the ETIS community | [ETIS Community Discussions](https://github.com/orgs/etis-framework/discussions) |
| Explore ETIS Books and the Professional Computing Series | [ETIS Books](../Books/index.md) |
| Explore ETIS publications | [Publications](../publications/index.md) |
| Follow a publication reading path | [Reading Paths](../publications/reading-paths.md) |
| Download books or other ETIS resources | [Downloads](download.md) |
| Inspect the Framework source | [Framework Repository](https://github.com/etis-framework/etis) |

---

## Repository Governance Principles

The public repository ecosystem follows several principles:

1. **Clear authority** — each repository has a defined responsibility.
2. **Minimal duplication** — source and implementation materials have one primary home.
3. **Visible provenance** — important public artifacts remain connected to their source and version history.
4. **Repository-centered evidence** — requirements, decisions, reviews, AI use, verification, release, operations, and stewardship remain inspectable.
5. **Reusable structure** — templates and examples support adoption without replacing engineering judgment.
6. **Public maintainability** — navigation, source organization, and publication assets should remain understandable as the ecosystem grows.

---

## Specialized Repositories

In addition to the two primary ETIS repositories, specialized repositories support focused educational, community, and organization capabilities.

| Repository | Visibility | Role |
|---|---|---|
| **COMP 330 Fall 2026 Starter Kit** | Public template | Official Loyola University Chicago COMP 330 course repository template used by student teams to create their project repositories. It is distinct from the ETIS Engineering Platform Starter Kit. |
| **COMP 330 Submission Preflight** | Public | Reference implementation of **ETIS Preflight** for COMP 330/474. Student-facing, phase-gate-aware readiness tooling uses deterministic checks and analytical heuristics to evaluate whether expected repository evidence is present and has the basic shape required for formal review. It does not perform the formal phase-gate review or make the gate decision. |
| **ETIS Engineering Studio** | Public source / instructor-operated deployment | Open-source student-team learning environment for frozen-evidence review, controlled reviewer dialogue, engineering-judgment development, and links to relevant ETIS Platform guidance. Production use requires course and institutional configuration. |
| **ETIS Community** | Public | Organization-level home for GitHub Discussions and persistent dialogue about the Framework, books, publications, education, professional computing, trustworthy AI, and engineering practice. |
| **ETIS Organization Profile** | Public | GitHub organization profile and public organization-level configuration. |

Instructor-only formal review systems, rubrics, protected reviewer configuration, and other assessment logic may remain private when publication would weaken assessment integrity. The instructor-facing formal review environment is described publicly as the ETIS Engineering Review Center.

Specialized repositories allow individual capabilities to evolve independently while preserving clear responsibility, provenance, and alignment with ETIS engineering doctrine.

---

## Bottom Line

ETIS is intentionally organized as a framework, books, publication, and platform ecosystem.

The Framework Reference Work explains the discipline.
The Professional Computing Series develops durable professional capabilities aligned with ETIS.
Publications provide focused, citable guidance.
The Platform operationalizes the discipline.
The repositories preserve the source, reusable assets, and engineering evidence that make ETIS inspectable.
