# Changelog

All notable changes to the Engineering Trustworthy Intelligent Systems (ETIS) ecosystem are documented in this file.

The format is inspired by *Keep a Changelog* and adapted for framework, publication, educational, platform, website, and ecosystem releases.

---

## [Unreleased] - August 2026

### Engineering Education Suite Integration

This update expands the ETIS Educational Ecosystem with a coordinated, phase-gate-aware Engineering Education Suite for student readiness, engineering-judgment development, and instructor-led formal review.

### Added

#### Engineering Education Suite

- ETIS Engineering Education Suite overview and cross-site integration
- ETIS Preflight as the student/team phase-gate readiness capability
- ETIS Engineering Studio as the instructor-operated student-team engineering-judgment environment
- ETIS Engineering Review Center as the instructor-facing formal phase-gate review environment
- Dedicated public pages for the Suite, Preflight, Engineering Studio, and Engineering Review Center
- Education navigation for the three coordinated but modular capabilities
- Institutional-adoption guidance for instructor- and university-operated deployment

#### Engineering Studio

- Phase-gate-aware developmental review
- Frozen evidence snapshots initiated by student teams throughout a phase
- Shared team evidence snapshots with independent student-reviewer conversations
- Controlled multidisciplinary engineering review board behavior
- Evidence-grounded mentoring, challenge, questioning, and developmental mini-reviews
- Prior phase-gate awareness and longitudinal engineering context
- Links to relevant Engineering Platform stages, Starter Kit guidance, templates, and LMU/COICP examples
- Public documentation of the Azure production reference deployment and its reliability, availability, serviceability, recoverability, observability, identity, database, backup, and deployment architecture

#### Formal Phase-Gate Review

- Formal evidence boundary based on the designated phase-gate Git tag
- Rubric-aligned evidence analysis
- Confidence assessments
- Review summaries and findings
- Evidence lineage and traceability to repository artifacts
- Longitudinal context from prior formal phase-gate analysis
- Explicit preservation of instructor academic authority

#### Educational Model

- Two-cycle COMP 330/474 flagship delivery model documented
- First five phase gates positioned from project launch through initial release
- Sixth phase gate positioned as an operational enhancement cycle
- Educational relationship to the broader ETIS lifecycle and the transition into Volume II operational, governance, resilience, oversight, and stewardship concerns
- Clarification that a semester selectively adapts the broader ETIS lifecycle rather than attempting to cover every ETIS topic

### Changed

- Repositioned educational tooling as the **ETIS Engineering Education Suite** rather than a collection of unrelated utilities.
- Replaced the public-facing **Instructor Engineering Workbench** terminology with **ETIS Engineering Review Center** where the current capability is being described.
- Repositioned **Student Submission Preflight** as **ETIS Preflight** in current public-facing product language while preserving historical repository and release terminology where appropriate.
- Clarified the distinct roles of Preflight, Engineering Studio, and Engineering Review Center.
- Clarified that all three capabilities are phase-gate aware and informed by prior phase-gate analysis.
- Clarified that Preflight evaluates phase-gate readiness but does not conduct the formal engineering review.
- Clarified that Engineering Studio reviewers coach, mentor, question, and challenge rather than provide engineering answers.
- Clarified that Studio developmental review and formal phase-gate review remain intentionally separate.
- Clarified that Studio conversations do not silently become evidence in the formal phase-gate review.
- Clarified that the formal phase-gate evidence submitted at the designated Git tag must stand on its own.
- Clarified that evidence, findings, confidence assessments, summaries, and rubric-aligned analysis support instructor decision-making rather than autonomous grading.
- Updated Educational Ecosystem, Educational Products, Instructor Resources, Student Resources, Flagship Implementation, Institutional Adoption, Resources, Repository Ecosystem, Downloads, ETIS Library, About, What's New, Framework references, and repository-level documentation.
- Updated the main landing page with a single text-only ecosystem description change; no homepage layout or CSS changes were introduced.
- Updated `README.md` and `ROADMAP.md` to reflect the Engineering Education Suite and current ecosystem architecture.

### Validation

- MkDocs strict clean build completed successfully.
- New and modified Education pages reviewed in the local site.
- Navigation and internal links reviewed.
- Homepage CSS and layout intentionally left unchanged.

### Release Note

These changes are currently recorded as **Unreleased**.

The latest tagged repository release remains **v1.4.0** until the next formal release is created.

---

## [1.4.0] - August 2026

### Books and Professional Computing Series Release

This release established the mature ETIS long-form publishing architecture while preserving *Engineering Trustworthy Intelligent Systems* as the foundational ETIS Framework Reference Work.

### Added

- ETIS Books landing architecture
- ETIS Framework Reference Work publishing page
- ETIS Professional Computing Series
- *From Data Structures to Engineering Judgment: Professional Computing in the AI Era* as the inaugural Professional Computing Series title
- Book companion-resources and updates/errata structure
- Framework and Professional Computing book-cover integration
- Cross-site Books discovery from Publications, Education, About, Resources, and supporting pages

### Changed

- Clarified *Engineering Trustworthy Intelligent Systems* as the **ETIS Framework Reference Work**.
- Clarified the **ETIS Two-Volume Professional Edition** as the two-volume publishing form of one integrated Framework Reference Work rather than a separate book series.
- Distinguished the **ETIS Professional Computing Series** from the focused ETIS Publications Program.
- Updated Downloads, Publications, Educational Ecosystem, Engineering Platform, About, Author, First Edition, Legal, and homepage terminology to reflect the expanded publishing architecture.
- Preserved Publications as a separate program for White Papers, Executive Briefs, and Education Papers.
- Preserved the Engineering Platform as the practical implementation environment for the ETIS Framework.
- Updated repository-level documentation to reflect the Books architecture.

### Fixed

- Corrected and normalized internal MkDocs link handling where needed.
- Corrected malformed or inconsistent internal links discovered during the publishing-architecture review.
- Clarified ambiguous “Complete Book” homepage language as “Full Framework.”

### Milestone

This release established the current ETIS publishing architecture:

- ETIS Framework Reference Work
- ETIS Two-Volume Professional Edition
- ETIS Professional Computing Series
- *From Data Structures to Engineering Judgment*
- ETIS Publications Program
- Educational Ecosystem
- Engineering Platform
- integrated resource, repository, and navigation architecture

---

## [1.3.0] - August 2026

### Educational Ecosystem and Platform Integration Release

This release expanded ETIS education into a coherent public teaching and institutional-adoption architecture and aligned educational practice with the Engineering Platform.

### Added

- ETIS Educational Ecosystem architecture
- Instructor Resources
- Student Resources
- Educational Products
- COMP 330/474 Flagship Implementation
- Institutional Adoption guidance
- ETIS Educational Ecosystem Guide
- ETIS Instructor Course Package
- ETIS Classroom Facilitation Guide
- ETIS Instructor Handbook
- ETIS Student Professional Engineering Guide
- ETIS COMP 330 Flagship Implementation Guide
- Engineering Platform course-use guidance

### Changed

- Positioned ETIS education as professional formation rather than course content alone.
- Integrated repository-centered engineering, evidence-centered engineering, responsible AI use, professional teamwork, review and release defense, operational thinking, stewardship, and professional portfolio development into the educational model.
- Aligned the Educational Ecosystem with the Engineering Platform as the practical project environment for ETIS course work.
- Expanded public navigation, resource discovery, and institutional-adoption guidance for educational users.
- Updated Framework, Resources, About, and supporting website pages to reflect the mature educational architecture.

### Milestone

This release established the educational foundation later extended by the Engineering Education Suite.

---

## [1.2.0] - July 2026

### Publications and Platform Integration Release

This release transforms ETIS from a book-centered publication site into a complete professional engineering ecosystem.

### Added

#### Publications Program

- ETIS Publications landing page
- White Paper Series (12 papers)
- Executive Brief Series (5 briefs)
- Education Paper Series (5 papers)
- Canonical publication landing pages
- Publication metadata, citation guidance, and version history
- Role-based reading paths
- Publication PDF integration

#### Engineering Platform

- Platform gateway on the ETIS Framework website
- Companion Engineering Platform integration
- Starter Kit repository integration
- Explore / Launch / Browse navigation model
- Starter Kit download integration

#### Website

- Homepage integration of Publications and Platform
- Platform overview section
- Updated Resource Center
- Updated ETIS Library
- Updated About pages
- Updated Framework pages
- Updated Educational Ecosystem pages
- Updated Appendices landing page
- Updated navigation architecture
- Publications integrated throughout the website

#### Repository

- Repository documentation modernized
- README updated to reflect the complete ETIS ecosystem
- Roadmap updated to reflect completed ecosystem architecture
- License updated to reflect the expanded ETIS intellectual property portfolio and AI training restrictions
- Release documentation aligned with the v1.2.0 architecture

### Changed

- Clarified the distinction between Publications and Downloads.
- Established the Platform gateway as the canonical entry point to the companion Engineering Platform.
- Standardized external navigation using the Explore / Launch ↗ / Browse Repository ↗ convention.
- Updated ecosystem terminology throughout the public website.

### Fixed

- Corrected Platform download links.
- Corrected publication cross-links.
- Corrected MkDocs relative-link issues.
- Improved navigation consistency across the site.

### Milestone

This release establishes the mature ETIS public ecosystem consisting of:

- ETIS Framework
- ETIS Framework Reference Work and Two-Volume Professional Edition
- Publications Program
- Educational Ecosystem
- Engineering Platform
- Framework Repository
- Starter Kit Repository
- Resource Center
- Downloads
- Appendices

---

## [1.1.0] - July 2026

### Ecosystem Expansion Release

### Added

- Two-Volume Edition landing pages
- Volume reading guidance
- Expanded downloads architecture
- Resource Center enhancements
- Educational Ecosystem integration
- Initial Platform references
- Improved website navigation and branding
- Repository governance improvements
- GitHub release and versioning model
- Expanded framework documentation

### Changed

- Reorganized website architecture around the Two-Volume Edition.
- Improved navigation consistency and discoverability.
- Expanded educational and framework resources.
- Strengthened repository documentation and release management.

### Milestone

This release evolved ETIS beyond the initial publication into a broader framework and educational ecosystem, establishing the foundation for the Publications Program and Engineering Platform introduced in v1.2.0.

---

## [1.0.0] - July 2026

### First Edition Release

Initial public release of the ETIS framework and publication ecosystem.

### Added

#### Publication

- Engineering Trustworthy Intelligent Systems (ETIS) — First Edition
- Complete four-part framework
- Front matter and back matter publication package
- Appendix collection
- Resource and reference materials

#### Framework

- Repository-Centered Engineering doctrine
- Evidence-Centered Engineering doctrine
- AI Proposes; Engineers Verify doctrine
- Governance is Architecture doctrine
- Context is Control doctrine
- Operational Trust doctrine
- Trustworthy Intelligent Systems doctrine

#### Website

- MkDocs Material publication platform
- ETIS publication website
- Custom ETIS branding system
- ETIS logo integration
- Favicon and browser identity system
- Landing Page Freeze V1 architecture
- Framework navigation architecture
- Repository-Centered Engineering presentation
- Resource Center architecture
- Download Center architecture

#### Visual Governance

- ETIS visual governance system
- Figure governance architecture
- Publication branding architecture
- Website visual governance architecture
- Typography governance standards
- Color-palette governance standards

#### Repository Architecture

- Repository-centered publication architecture
- Markdown source publication workflow
- GitHub Pages publication preparation
- Publication continuity architecture
- Constitutional governance registers
- Freeze-boundary registers
- Recovery and continuity packages

### Publication Baseline

This release establishes the constitutional baseline for:

- The ETIS Framework
- The First Edition manuscript
- The ETIS publication website
- Publication governance
- Visual governance
- Repository governance
- Supporting ecosystem artifacts

### Notes

Version 1.0.0 represents the initial publication baseline of the Engineering Trustworthy Intelligent Systems ecosystem and serves as the foundation for future editions, updates, companion materials, educational resources, and supporting publication assets.
