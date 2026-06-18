# Appendix C<br><span class="chapter-title-main">Repository-Centered Engineering Artifact Catalog

Repository-centered engineering is one of the central concepts developed throughout this book. Repository artifacts serve not merely as documentation but as evidence supporting requirements, decisions, implementation, testing, governance, operations, learning, stewardship, and professional accountability.

This appendix catalogs the major artifact families discussed throughout the book and explains their purpose, ownership, evidence role, review relationships, and contribution to trustworthiness.

The goal is not to prescribe a specific toolchain or repository structure. Instead, the appendix provides a practical reference for understanding how artifacts support engineering decisions and create durable organizational memory.

## C.1 Introduction to Repository-Centered Engineering

Repository-centered engineering is one of the central concepts developed throughout this book. The repository is not merely a code host, storage location, or collaboration platform. It serves as the system of record for engineering evidence. It preserves what was intended, what was decided, what changed, what was reviewed, what was tested, what failed, what was learned, what AI proposed, what humans accepted or rejected, who owned the result, and how the system will be operated and stewarded over time.

Together with the trustworthiness framework and review-board catalog, the artifact catalog provides the evidence perspective that connects engineering claims to durable proof. It explains how engineering claims become durable, reviewable, and professionally defensible through repository artifacts.

The repository examples used throughout this appendix are illustrative rather than prescriptive. Organizations should adapt structures and naming conventions to their own environments while preserving evidence quality, ownership, reviewability, and traceability.

Everything important leaves evidence. Repository artifacts matter because they allow future engineers, reviewers, operators, auditors, and stakeholders to understand what happened, why decisions were made, what risks were accepted, and how responsibility was exercised throughout the lifecycle.

## C.2 Repository-Centered Engineering Principle

The repository is the engineering witness. It should allow a reviewer, maintainer, operator, stakeholder, instructor, auditor, or future engineer to reconstruct the meaningful engineering story of the system. That story includes intent, requirements, assumptions, decisions, implementation, review, verification, release, operation, incidents, recovery, AI governance, context governance, oversight, stewardship, and professional accountability.

A trustworthy repository is not measured by folder count. It is measured by whether important claims can be traced to evidence, challenged by humans, connected to risk, maintained over time, and used during real operational decisions.

## C.3 Canonical Artifact Catalog

The following catalog lists the primary repository artifact domains described throughout this book. Teams may adapt file names and folder structure, but they should preserve artifact purpose, ownership, reviewability, evidence quality, and lifecycle meaning.

| **Artifact Domain**                       | **Purpose**                                                                                                                         | **Evidence Role**                                                                                           | **Representative Path Examples**                                                                                                           |
|-------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| Project governance                        | Establishes project intent, roles, standards, lifecycle posture, risk ownership, and AI-use expectations.                           | Creates the baseline against which later claims, reviews, and releases are judged.                          | /docs/governance/project_charter.md; /docs/governance/team_working_agreement.md; /docs/governance/risk_register.md                         |
| Requirements and ambiguity control        | Preserves stakeholder intent, system scope, acceptance criteria, assumptions, constraints, and unresolved ambiguity.                | Supports correctness, traceability, stakeholder validation, planning, testing, and release defense.         | /docs/requirements/requirements.md; /docs/requirements/use_cases.md; /docs/requirements/ambiguity_log.md                                   |
| Planning, estimation, and risk            | Records scope decomposition, estimates, commitments, dependencies, RACI/ownership, and risk tradeoffs.                              | Makes commitments reviewable and prevents planning from becoming private optimism.                          | /docs/planning/wbs.md; /docs/planning/estimate_record.md; /docs/planning/risk_tradeoff_log.md                                              |
| Architecture                              | Documents system boundaries, responsibilities, dependencies, data authority, integration surfaces, and control points.              | Supports reviewability, governability, understandability, change control, and AI-system boundary reasoning. | /docs/architecture/architecture_overview.md; /docs/architecture/component_responsibility_map.md; /docs/architecture/dependency_register.md |
| Architecture decisions                    | Preserves consequential decisions, options considered, rejected alternatives, rationale, owners, and consequences.                  | Prevents decision amnesia and enables future review, incident learning, and stewardship.                    | /docs/architecture/adrs/adr-0001-record-architecture-decision.md                                                                           |
| Implement\-ation change evidence            | Links issues, branches, commits, pull requests, reviews, tests, and merge decisions.                                                | Makes change inspectable and ties implementation to intent, risk, and verification.                         | Issues, branches, commits, PRs, review records, CI results; summarized under /docs/release_evidence/ when needed                           |
| Testing and verification                  | Defines test strategy, risk-based test coverage, acceptance tests, regression evidence, evaluation sets, and known gaps.            | Supports correctness, reviewability, release readiness, AI behavior evaluation, and defect reduction.       | /docs/testing/test_strategy.md; /docs/testing/test_evidence.md; /docs/testing/evaluation_sets.md                                           |
| Release evidence                          | Collects readiness claims, test status, defect status, known limitations, risk acceptance, rollback notes, and approval records.    | Turns release from confidence into evidence-backed judgment.                                                | /docs/release_evidence/release_readiness_record.md; /docs/release_evidence/known_limitations.md; /docs/release_evidence/release_notes.md   |
| Operations and runbooks                   | Records operating procedures, support ownership, escalation paths, fallback, rollback, degradation, and communication procedures.   | Makes the system operable, recoverable, and supportable beyond the demo path.                               | /docs/operations/runbooks/; /docs/operations/operational_readiness_record.md                                                               |
| Observ\-ability and runtime evidence        | Preserves logs, metrics, traces, request IDs, dashboard interpretation, audit evidence, and diagnostic paths.                       | Allows runtime behavior and failure to be understood, challenged, and improved.                             | /docs/operations/observability/observability_plan.md; /docs/operations/runtime_evidence/                                                   |
| Incidents and postmortems                 | Captures incident timelines, containment, recovery, evidence, root-cause reasoning, lessons, and corrective actions.                | Converts operational failure into durable learning without blame theater.                                   | /docs/operations/incidents/; /docs/operations/postmortems/coicp_pilot_postmortem_001.md                                                    |
| Security and privacy governance           | Documents threat reasoning, access control, data handling, dependency review, auditability, and privacy-sensitive context rules.    | Protects systems, data, integrations, workflows, and trust relationships.                                   | /docs/governance/security/; /docs/governance/privacy/; /docs/governance/security_governance_review.md                                      |
| AI governance                             | Records AI use, delegation boundaries, evaluation evidence, limitations, accepted/rejected output, and human verification.          | Makes AI use visible, bounded, auditable, and human-owned.                                                  | /docs/governance/ai_governance/ai_use_log.md; /docs/governance/ai_governance/delegation_matrix.md                                          |
| Agentic workflow governance               | Documents tool authority, action approval, agent logs, rollback, revocation, monitoring, and exception handling.                    | Prevents silent state-changing authority and makes agentic behavior governable.                             | /docs/governance/agentic_workflows/tool_authority_matrix.md; /docs/governance/agentic_workflows/agent_action_log.md                        |
| Context engineering governance            | Records authoritative context sources, freshness, ownership, lineage, permissions, trust assumptions, and exception handling.       | Treats context as a control surface rather than prompt decoration.                                          | /docs/governance/context_engineering/context_source_registry.md; /docs/governance/context_engineering/context_trust_model.md               |
| Human oversight governance                | Documents oversight policy, accountability matrix, escalation authority, intervention playbook, audit sampling, and review records. | Makes oversight meaningful, scalable, auditable, and paired with authority.                                 | /docs/governance/human_oversight/human_oversight_policy.md; /docs/governance/human_oversight/intervention_playbook.md                      |
| Review-board records                      | Preserves claims, evidence, questions, risks, decisions, conditions, owners, and next actions from lifecycle reviews.               | Turns review boards into durable engineering challenge evidence.                                            | /docs/governance/reviews/review_index.md; /docs/governance/reviews/release_readiness_review.md                                             |
| Understand\-ability and evidence navigation | Documents complexity maps, role-based decision surfaces, reviewer context packets, evidence indexes, and navigation guidance.       | Reduces cognitive load so humans can govern, operate, review, and recover the system.                       | /docs/governance/evidence_navigation/evidence_navigation_guide.md; /docs/architecture/understandability/complexity_map.md                  |
| Repository stewardship                    | Tracks evidence inventory, artifact freshness, repository health, retention, ownership, and continuity.                             | Prevents archive rot and keeps repository memory trustworthy over time.                                     | /docs/governance/repository_stewardship/evidence_inventory.md; /docs/governance/repository_stewardship/repository_health_dashboard.md      |
| Long-term stewardship                     | Records stewardship plan, governance cadence, capability reviews, retirement/evolution decisions, and institutional learning.       | Keeps trustworthy systems trustworthy after release and after team turnover.                                | /docs/stewardship/stewardship_plan.md; /docs/stewardship/capability_review_log.md                                                          |
| Professional portfolio                    | Collects evidence of judgment, governance, AI responsibility, release defense, operations, and stewardship.                         | Converts repository evidence into professional identity proof.                                              | /docs/professional_portfolio/evidence_portfolio.md; /docs/professional_portfolio/final_defense_packet.md                                   |

## C.4 Lifecycle Evidence Map

Repository evidence matures across the book. Early evidence establishes standards and accountability. Construction evidence makes work reviewable. Operational evidence makes runtime reality inspectable. Stewardship evidence keeps trustworthiness alive after release and after team turnover.

| **Lifecycle Stage**                | **Primary Repository Evidence**                                                                                                              | **Repository-Centered Meaning**                                                                            |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|
| Part I - Worldview                 | Project standards, risk register, early repository expectations, AI-use expectations                                                         | Make trust, evidence, review, accountability, and AI verification visible before construction begins.      |
| Part II - Responsible construction | Requirements, planning, architecture, ADRs, PRs, reviews, tests, release evidence                                                            | Convert intent and construction work into reviewable engineering evidence.                                 |
| Part III - Operational trust       | Runbooks, observability evidence, incidents, postmortems, security records, release-governance records                                       | Move from release confidence to runtime evidence, recovery, learning, and operational accountability.      |
| Part IV - AI-era stewardship       | Agentic workflow records, context registries, oversight records, understandability artifacts, repository stewardship, professional portfolio | Convert operational trust into governed intelligent-system stewardship and professional identity evidence. |
| Appendices and publication         | Catalogs, templates, reference maps, figure assets, glossary, publication artifacts                                                          | Support reuse and teaching without reopening doctrine or replacing engineering judgment with templates.    |

## C.5 Trustworthiness-to-Repository Mapping

Each trustworthiness pillar requires evidence. The repository does not make the system trustworthy by itself, but it makes trustworthiness claims reviewable, challengeable, recoverable, and maintainable.

| **Trustworthiness Pillar**                  | **Representative Evidence**                                                                     | **Typical Repository Locations**                                                                    |
|---------------------------------------------|-------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| Correctness                                 | requirements, acceptance criteria, tests, evaluation sets, defect records                       | /docs/requirements/, /docs/testing/, /docs/release_evidence/                                        |
| Traceability                                | issues, commits, PRs, ADRs, release notes, incident links                                       | /docs/architecture/adrs/, /docs/release_evidence/, issue/PR records                                 |
| Reviewability                               | PR comments, review-board records, reviewer packets, evidence indexes                           | /docs/governance/reviews/, /docs/governance/evidence_navigation/                                    |
| Observability                               | logs, metrics, traces, request IDs, dashboards, runtime evidence                                | /docs/operations/observability/, /docs/operations/runtime_evidence/                                 |
| Governability                               | role rules, approval records, delegation matrices, authority boundaries, audit expectations     | /docs/governance/, /docs/governance/ai_governance/, /docs/governance/agentic_workflows/             |
| Recoverability                              | runbooks, rollback plans, revocation plans, incident records, postmortems                       | /docs/operations/runbooks/, /docs/operations/incidents/, /docs/operations/postmortems/              |
| Security and privacy                        | access reviews, data handling rules, dependency reviews, context permissions, audit records     | /docs/governance/security/, /docs/governance/privacy/, /docs/governance/context_engineering/        |
| Accountability                              | owners, RACI, approval history, stewardship ownership, portfolio claims                         | /docs/governance/, /docs/stewardship/, /docs/professional_portfolio/                                |
| Operational visibility                      | release notes, runtime dashboards, health evidence, risk registers, operational summaries       | /docs/release_evidence/, /docs/operations/, /docs/governance/risk_register.md                       |
| Human oversight                             | oversight policies, escalation matrices, intervention playbooks, audit samples                  | /docs/governance/human_oversight/, /docs/governance/reviews/                                        |
| Transparency and organizational confidence  | known limitations, trust evidence maps, stakeholder communication records, governance summaries | /docs/release_evidence/known_limitations.md, /docs/governance/, /docs/professional_portfolio/       |
| Understandability and stewardship readiness | complexity maps, evidence navigation, repository health, stewardship plans                      | /docs/architecture/understandability/, /docs/governance/repository_stewardship/, /docs/stewardship/ |

## C.6 Ownership, Review Use, and Freshness Expectations

Artifacts decay when ownership is unclear. Appendix C therefore treats every important artifact as having an owner, a review purpose, and a freshness expectation. A stale artifact can be worse than no artifact because it creates false confidence.

| **Artifact / Record**                              | **Typical Owner**                                          | **Review Use**                                                            | **Freshness Expectation**                                                                |
|----------------------------------------------------|------------------------------------------------------------|---------------------------------------------------------------------------|------------------------------------------------------------------------------------------|
| Project charter and standards                      | Team lead / engineering lead                               | Launch review; standards review; final defense                            | At launch and whenever scope or governance changes materially                            |
| Requirements and acceptance criteria               | Product owner / requirements owner with engineering review | Requirements readiness review; testing review; release readiness          | Whenever stakeholder intent, assumptions, or acceptance criteria change                  |
| Architecture overview and ADRs                     | Architecture owner / technical lead                        | Architecture review; ADR review; incident learning; stewardship review    | At every consequential design decision and after material incidents                      |
| PRs, review comments, and CI evidence              | Change owner with reviewers                                | Change acceptance review; release readiness                               | Every meaningful change                                                                  |
| Test strategy and test evidence                    | QA/test owner with team participation                      | Testing review; intelligent-system testing review; release readiness      | Every release cycle and after defect-pattern changes                                     |
| Release readiness record                           | Release owner / approval authority                         | Release readiness review; release defense; operational release governance | Every release or operational exposure decision                                           |
| Runbooks and operational readiness records         | Operations owner / support owner                           | Operational readiness review; incident response review                    | Before release and after operational learning                                            |
| Incident and postmortem records                    | Incident owner / postmortem facilitator                    | Postmortem learning review; stabilization review; stewardship review      | Every significant incident or near miss                                                  |
| AI-use logs and delegation matrix                  | AI governance owner / engineering lead                     | AI delegation governance review; agentic workflow review; final defense   | Every AI capability change, delegated authority change, or material AI-assisted decision |
| Context source registry and trust model            | Context owner / data owner / architecture owner            | Context engineering review; security/privacy review; stewardship review   | Whenever context source, freshness, permissions, or ownership changes                    |
| Human oversight policy and intervention playbook   | Oversight owner / accountable operational authority        | Human oversight readiness review; incident response; final defense        | Before consequential AI workflow use and after oversight failures                        |
| Repository evidence inventory and health dashboard | Repository steward                                         | Operational repository review; stewardship review                         | At least once per cycle and during major handoff, audit, or stewardship transition            |
| Professional portfolio and evidence map            | Individual engineer / student                              | Final Trustworthy Engineer Review / Portfolio Defense                     | At capstone, promotion, handoff, or professional review milestones                       |

## C.7 Review-Board Evidence Inputs

Review boards are only as strong as the evidence they inspect. The following table summarizes common repository inputs for major review families. Appendix B owns the review-board catalog; Appendix C owns the artifact evidence side of the relationship.

| **Review Family**                                     | **Primary Evidence Question**                                              | **Typical Repository Inputs**                                                             |
|-------------------------------------------------------|----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|
| Project Launch / Standards Review                     | Project governance, standards, role definitions, AI-use expectations       | Project charter; working agreement; risk register; AI-use policy                          |
| Repository Evidence Review                            | Repository front door, artifact locations, evidence chain expectations     | README/front door; evidence index; artifact ownership map                                 |
| Requirements Readiness / Ambiguity Review             | Stakeholder intent, acceptance criteria, ambiguity, assumptions            | Requirements; use cases; acceptance criteria; ambiguity log                               |
| Architecture Readiness / ADR Review                   | Boundaries, decisions, responsibility, dependencies, consequences          | Architecture overview; component map; ADRs; dependency register                           |
| AI-Assisted Implementation / Generated-System Review  | AI-originated material, tests, assumptions, hidden authority, verification | AI-use log; PR disclosure; test evidence; review comments                                 |
| Testing / Intelligent-System Testing Review           | Behavior evidence, AI evaluation, adversarial cases, limitations           | Test strategy; test evidence; evaluation sets; limitation records                         |
| Release Readiness / Release Defense                   | Integrated release claims, defects, risk, rollback, known limits, approval | Release readiness record; release notes; known limitations; risk acceptance               |
| Operational Readiness / Observability Review          | Support, escalation, runbooks, diagnostic evidence, runtime visibility     | Runbooks; observability plan; runtime evidence examples; escalation matrix                |
| Security Governance / AI Delegation Governance Review | Authority, access, privacy, AI delegation, audit, revocation, recovery     | Security records; delegation matrix; AI capability review; audit expectations             |
| Incident Response / Postmortem Learning Review        | Incident evidence, containment, recovery, learning, corrective action      | Incident timeline; postmortem; corrective action log; follow-up issues                    |
| Agentic Workflow / Context Engineering Review         | Tool authority, action approval, context trust, freshness, ownership       | Tool authority matrix; agent action log; context source registry; context trust model     |
| Human Oversight / Understandability Review            | Meaningful control, escalation, cognitive load, evidence navigation        | Oversight policy; intervention playbook; complexity map; reviewer context packet          |
| Repository Stewardship / Final Portfolio Defense      | Repository health, stewardship evidence, professional evidence map         | Evidence inventory; repository health dashboard; stewardship plan; professional portfolio |

## C.8 Repository Evidence Quality Criteria

Repository artifacts should be evaluated by quality, not merely presence. A file exists is not a sufficient claim. The relevant question is whether the artifact helps a competent reviewer make a better engineering decision.

- Clear purpose: the artifact says what engineering question it answers.

- Named ownership: someone is accountable for accuracy, updates, and use.

- Traceability: the artifact links to related requirements, decisions, changes, tests, reviews, releases, incidents, or stewardship records.

- Reviewability: a human can inspect the artifact without reconstructing the whole project from memory.

- Freshness: the artifact indicates when it was last updated or what event should trigger revision.

- Risk relevance: the artifact clarifies risk, limitation, uncertainty, assumption, or consequence.

- Operational usefulness: the artifact can help during release, incident response, recovery, audit, handoff, or stewardship.

- AI transparency: where AI materially contributed, the artifact records what was proposed, modified, accepted, rejected, and verified.

## C.9 Minimal Repository Reference Architecture

The following structure is a compact reference architecture for repository-centered engineering environments. It is not a mandatory folder tree. It is a practical starting point for preserving evidence without drowning the team in documentation.

| **Representative Path**                              | **Primary Purpose**                                                                    |
|------------------------------------------------------|----------------------------------------------------------------------------------------|
| /docs/governance/project_charter.md                  | Project intent, scope, roles, standards, evidence expectations                         |
| /docs/governance/risk_register.md                    | Project, operational, AI, governance, security, and release risks                      |
| /docs/requirements/requirements.md                   | Functional, nonfunctional, governance, operational, and AI-relevant requirements       |
| /docs/requirements/ambiguity_log.md                  | Open questions, assumptions, stakeholder conflicts, resolution history                 |
| /docs/planning/wbs.md                                | Work breakdown, dependencies, ownership, milestones, and commitments                   |
| /docs/architecture/architecture_overview.md          | Boundaries, responsibilities, integrations, systems of record, control surfaces        |
| /docs/architecture/adrs/                             | Decision records with options, rationale, consequences, owners                         |
| /docs/testing/test_strategy.md                       | Test approach, risk-based depth, acceptance, regression, AI evaluation                 |
| /docs/release_evidence/release_readiness_record.md   | Release claims, evidence, limits, risks, rollback, approvals                           |
| /docs/release_evidence/known_limitations.md          | Honest limitations, deferred work, residual risk, ownership                            |
| /docs/operations/runbooks/                           | Procedures for operation, escalation, fallback, rollback, recovery                     |
| /docs/operations/observability/observability_plan.md | Logs, metrics, traces, dashboards, audit events, diagnostic questions                  |
| /docs/operations/incidents/                          | Incident records, timelines, containment, recovery, communication                      |
| /docs/operations/postmortems/                        | Blameless learning records and corrective actions                                      |
| /docs/governance/security/                           | Security governance, access review, data and dependency considerations                 |
| /docs/governance/ai_governance/ai_use_log.md         | AI assistance, accepted/rejected output, verification, responsible owner               |
| /docs/governance/ai_governance/delegation_matrix.md  | AI authority levels, approval rules, monitoring, revocation, recovery                  |
| /docs/governance/agentic_workflows/                  | Tool authority, action logs, approval flows, rollback, revocation                      |
| /docs/governance/context_engineering/                | Source registry, trust model, freshness, lineage, ownership, permissions               |
| /docs/governance/human_oversight/                    | Oversight policy, accountability, escalation, intervention, audit sampling             |
| /docs/governance/evidence_navigation/                | Evidence index, reviewer packet, role-based decision surfaces                          |
| /docs/governance/repository_stewardship/             | Evidence inventory, repository health, freshness, retention, continuity                |
| /docs/stewardship/                                   | Stewardship plan, governance calendar, capability review, retirement/evolution records |
| /docs/professional_portfolio/                        | Evidence portfolio, trustworthiness map, final defense packet                          |

## C.10 Artifact Anti-Patterns and Corrective Controls

Repository-centered engineering can fail when teams mistake file accumulation for evidence. The following anti-patterns should be challenged during review and corrected before they become institutional habits.

| **Anti-Pattern**          | **What It Looks Like**                                                                                           | **Corrective Control**                                                                                            |
|---------------------------|------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
| Folder theater            | A repository has many folders but no reliable evidence chain.                                                    | Require artifact purpose, owner, freshness expectation, and review use for important files.                       |
| Evidence dump             | Teams upload documents after the fact without linking them to decisions, reviews, tests, releases, or incidents. | Tie evidence to claims, decisions, risks, owners, and next actions.                                               |
| Green check fallacy       | CI passes are treated as sufficient release evidence.                                                            | State what CI checks and does not check; require review, testing depth, risk, and operational readiness evidence. |
| Hidden AI use             | AI-generated artifacts appear polished but are not disclosed, reviewed, or verified.                             | Use AI-use logs, PR disclosure, verification notes, and review-board challenge.                                   |
| ADR amnesia               | Architecture choices are made in meetings or chats but not preserved as durable decision memory.                 | Record consequential decisions in ADRs with options, rationale, consequences, and owners.                         |
| Release evidence scramble | Evidence is assembled at the end to justify a decision already made.                                             | Build release evidence continuously from requirements, tests, PRs, defects, risks, and operational readiness.     |
| Runbook shelfware         | Runbooks exist but are stale, untested, ownerless, or unavailable during incidents.                              | Assign owners, test runbooks, update after incidents, and connect them to operational readiness review.           |
| Context soup              | AI systems consume unclear, stale, unauthorized, or ownerless context.                                           | Maintain source registry, trust model, refresh policy, lineage, and exception records.                            |
| Oversight theater         | Humans are nominally accountable but lack time, information, authority, or intervention paths.                   | Document meaningful oversight policy, escalation, audit samples, intervention playbooks, and control authority.   |
| Archive rot               | Repository evidence becomes stale, fragmented, duplicated, or impossible to navigate.                            | Use evidence inventory, repository health dashboard, retention rules, stewardship reviews, and freshness checks.  |

## C.11 AI-Era Repository Evidence

AI changes the repository because AI can produce plausible artifacts faster than teams can verify them. AI output should be treated as proposed engineering material. The repository must therefore preserve not only the final artifact, but also enough evidence to understand what was generated, what context was used where consequential, what humans changed, what was accepted or rejected, and how the result was verified.

- AI-use logs should record material AI assistance, especially requirements, architecture, code, tests, release language, governance summaries, and operational documents.

- Delegation matrices should define what AI may recommend, prepare, execute, or never do without explicit human approval.

- Context registries should identify source authority, freshness, ownership, permissions, and trust assumptions.

- Agent action logs should preserve state-changing behavior, approval history, exception handling, rollback, and revocation evidence.

- Oversight records should show meaningful human control, not merely nominal signoff.

- Professional portfolios should make AI use visible as part of judgment, verification, and accountability.

## C.12 Adaptation and Reuse

The artifact families described in this appendix are intended as reference patterns rather than rigid prescriptions. Different organizations, teams, industries, and technology environments will naturally adopt different repository structures, naming conventions, tools, and governance approaches.

The enduring value of repository-centered engineering is not a specific folder hierarchy or documentation format. Its value lies in preserving evidence that allows important engineering decisions to be understood, challenged, reviewed, operated, recovered, governed, and stewarded over time.

Organizations may adapt these artifact categories to support software development, systems engineering, operational governance, intelligent systems oversight, security programs, compliance initiatives, technology modernization efforts, or educational environments. The specific implementation may vary, but the underlying principles remain consistent:

- Important decisions leave durable evidence.
- Significant risks have visible ownership.
- Reviews inspect evidence rather than assumptions.
- Releases are supported by defensible readiness evidence.
- Operational learning is preserved for future teams.
- AI-assisted work remains reviewable, accountable, and verifiable.
- Stewardship extends beyond initial deployment.

The objective is not repository uniformity. The objective is maintaining a trustworthy engineering record that helps future engineers understand what was built, why it was built, how it was governed, what risks were accepted, what lessons were learned, and how responsibility was exercised throughout the system lifecycle.

## C.13 Final Repository-Centered Engineering Statement

The repository is not the system, but it is the durable witness of the system. It records the evidence by which trustworthiness can be challenged, defended, operated, recovered, governed, and stewarded. A repository that cannot support review, release judgment, operational learning, AI governance, context control, oversight, stewardship, and professional defense is not yet an engineering system of record. It is only storage.
