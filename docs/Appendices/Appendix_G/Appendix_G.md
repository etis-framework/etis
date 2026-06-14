# Appendix G<br><span class="chapter-title-main">AI Governance Framework

AI governance is the discipline of ensuring that intelligent capabilities remain subject to authority, accountability, oversight, evidence, and operational control. In trustworthy engineering, governance is not an after-the-fact compliance layer. It is part of system design.
Throughout Engineering Trustworthy Intelligent Systems (ETIS), AI is treated as useful, powerful, and limited. It can accelerate drafting, analysis, summarization, coding, testing, workflow support, and operational interpretation. It can also create fluent mistakes, hide assumptions, amplify poor context, blur responsibility, and make unsafe delegation look efficient.
This appendix consolidates the AI governance concepts developed throughout the book into a practical reference framework. It is intended for readers who need to decide what AI may do, what humans must verify, what evidence must be preserved, what authority must be bounded, and how intelligent capabilities should be operated and stewarded over time.

## G.1 Purpose of AI Governance in ETIS

AI governance exists because intelligent capabilities change the shape of engineering risk. The more a system can generate, recommend, summarize, classify, retrieve, route, call tools, or act on behalf of users, the more explicitly engineers must define authority, evidence, oversight, and accountability.

The purpose of AI governance is not to slow teams down with ritual. Its purpose is to keep speed from becoming unmanaged authority. AI can help teams move faster, but trustworthy engineering requires knowing what was proposed, what was accepted, what was rejected, what was verified, what risk remains, and who owns the result.

Effective AI governance connects architecture, repository evidence, review processes, operational readiness, observability, recoverability, human oversight, transparency, and stewardship. It is not a separate topic from software engineering; it is software engineering under intelligent-system conditions.

## G.2 Core AI Governance Principles

The following principles summarize the governance posture developed throughout the book. They are designed to be practical, reviewable, and usable by engineering teams.

| Principle | Meaning | Engineering Implication |
| --- | --- | --- |
| AI proposes; engineers verify | Generated or AI-assisted output is proposed material, not verified engineering truth. | Human review, testing, stakeholder validation, and traceable acceptance remain required. |
| The model is not the system | AI is one component inside a larger sociotechnical and operational system. | Architecture must include workflows, permissions, data, context, failure handling, operations, and accountability. |
| Context is control | AI behavior is shaped by the information, policies, examples, tools, and constraints it receives. | Context sources must be authoritative, current, permissioned, owned, versioned, and reviewable. |
| Governance is architecture | Authority, approval, audit, rollback, revocation, oversight, and monitoring are design concerns. | Governance must appear in architecture, repository artifacts, reviews, and operations, not only in policy prose. |
| Everything important leaves evidence | Consequential AI use should be reconstructable after the fact. | AI-use logs, delegation records, evaluation evidence, context registries, review decisions, and incident records matter. |
| Oversight requires control | Humans cannot be accountable for decisions they cannot inspect, influence, override, revoke, or recover from. | Oversight models must include authority, escalation, intervention, and evidence. |
| Trust depends on lifecycle maturity | AI cannot make an otherwise unreviewable, unobservable, unrecoverable, or ungoverned system trustworthy. | AI governance must connect to testing, release readiness, observability, incident response, and stewardship. |

## G.3 AI Use Zones

Not all AI use carries the same risk. This framework distinguishes between low-risk assistance, integrated engineering support, operational support, and state-changing or agentic behavior. Governance should be proportional to the consequence of failure and the degree of authority delegated.

| Use Zone | Examples | Minimum Governance Expectation |
| --- | --- | --- |
| Private learning and brainstorming | Explaining concepts, exploring alternatives, drafting questions, summarizing non-sensitive public material. | User judgment; no authoritative acceptance without verification. |
| Engineering drafting support | Drafting requirements, test ideas, ADR options, documentation, code sketches, or review checklists. | AI-use disclosure where relevant, human validation, repository evidence, and review. |
| Integrated implementation support | Code generation, refactoring suggestions, test generation, data transformation, configuration assistance. | Requirements traceability, architecture fit, tests, PR review, security review when relevant, and visible acceptance decisions. |
| Operational interpretation support | Log summarization, incident triage assistance, alert clustering, risk summaries, runbook suggestions. | Human confirmation, runtime evidence links, audit trails, limitations, escalation rules, and post-incident review. |
| Workflow recommendation | Routing suggestions, prioritization, classification, response drafting, stakeholder communication suggestions. | Evaluation evidence, context governance, human approval, monitoring, and feedback loops. |
| State-changing or agentic action | Creating tickets, sending messages, changing records, calling tools, approving actions, executing workflows. | Explicit authority boundaries, approval gates, action logs, rollback/revocation paths, monitoring, and accountable human owners. |

## G.4 Delegation and Authority Boundaries

The central governance question is not whether AI is used. The central question is what authority AI is allowed to exercise. A system that drafts a suggested message is different from a system that sends it. A system that recommends a routing path is different from a system that changes the assignment. A system that summarizes an incident is different from a system that closes it.

Authority should be defined in layers so teams can distinguish assistance from action.

| Authority Level | AI Role | Required Boundary |
| --- | --- | --- |
| Assist | Provides ideas, summaries, drafts, or alternatives. | Human decides whether anything becomes engineering work. |
| Recommend | Suggests classifications, priorities, routes, decisions, or actions. | Recommendation must be reviewable and rejectable. |
| Prepare | Creates a proposed artifact or action for approval. | Human approval required before consequence. |
| Execute with approval | Performs bounded actions after explicit human authorization. | Approval record, action log, and rollback/recovery path required. |
| Execute under policy | Performs low-risk bounded actions under preapproved rules. | Policy scope, monitoring, audit sampling, exception handling, and revocation required. |
| Autonomous consequential action | Acts without meaningful human approval in consequential contexts. | Generally unacceptable unless tightly bounded, observable, reversible, independently validated, and explicitly governed. |

## G.5 Verification Burden

Verification burden increases as AI influence becomes more consequential. A spelling suggestion may need little review. A generated requirement, routing recommendation, security configuration, medical summary, incident interpretation, or state-changing action needs much more.

Teams should not ask whether AI was helpful. They should ask what would happen if the AI were wrong, stale, biased, incomplete, overconfident, unauthorized, or misunderstood.

| Risk Factor | Governance Question | Evidence to Preserve |
| --- | --- | --- |
| Operational consequence | Could incorrect output affect users, operations, safety, trust, legal exposure, or institutional commitments? | Risk assessment, review record, approval decision, known limitations. |
| Integration depth | Is the output isolated, or does it affect architecture, data, workflows, security, or downstream systems? | Architecture links, ADRs, dependency notes, integration tests. |
| Authority scope | Can the AI recommend, prepare, approve, execute, or trigger state-changing behavior? | Delegation matrix, approval flow, action log, revocation plan. |
| Recoverability | Can errors be detected, contained, reversed, corrected, and learned from? | Rollback notes, runbooks, incident records, postmortems. |
| Observability | Can the team see what the AI did, why it mattered, and what happened afterward? | Audit logs, runtime evidence, monitoring notes, trace records. |
| Context dependence | Does the AI depend on current, authoritative, permissioned, and complete context? | Context source registry, freshness policy, lineage records, exception log. |
| Stakeholder impact | Could output shape communication, access, prioritization, fairness, or service quality? | Stakeholder review, transparency notes, appeal or escalation path. |

## G.6 Context Governance

Context governance is one of the most important AI-era engineering responsibilities. AI behavior depends heavily on what the system is allowed to see and use. Poor context creates poor behavior; stale context creates stale decisions; unauthorized context creates governance and privacy risk; undocumented context creates unreviewable systems.

Context should be treated as an engineering control surface.

| Context Governance Area | Required Practice | Representative Repository Evidence |
| --- | --- | --- |
| Source authority | Identify which sources are authoritative and which are advisory. | /docs/governance/context_engineering/context_source_registry.md |
| Freshness | Define how often context is refreshed and how stale material is detected. | /docs/governance/context_engineering/context_refresh_policy.md |
| Ownership | Assign owners for context sources, rules, examples, and policy material. | /docs/governance/context_engineering/context_ownership_matrix.md |
| Permission and privacy | Control what the AI may access and what must be excluded. | /docs/governance/context_engineering/context_access_policy.md |
| Lineage | Preserve enough provenance to know what informed consequential output. | /docs/governance/context_engineering/context_lineage_record.md |
| Reviewability | Make context choices inspectable by reviewers and operators. | /docs/governance/context_engineering/context_trust_model.md |
| Exception handling | Record and review cases where context is missing, conflicting, stale, or disputed. | /docs/governance/context_engineering/context_exception_log.md |

## G.7 Human Oversight

Human oversight is meaningful only when humans have enough information, authority, time, and control to influence outcomes. An approval button without understanding is oversight theater. Accountability without intervention authority is not real accountability.

Oversight should be designed as an operating model, not added as a checkbox.

| Oversight Requirement | Meaning | Evidence / Artifact |
| --- | --- | --- |
| Named accountability | Identify who owns the outcome, decision, exception, and escalation path. | Accountability matrix, review records, release approvals. |
| Decision visibility | Show humans what claim, evidence, risk, and recommendation they are approving. | Reviewer packet, evidence navigation guide, decision surface. |
| Intervention authority | Give humans the ability to pause, override, reject, escalate, revoke, or recover. | Intervention playbook, escalation matrix, revocation plan. |
| Risk proportionality | Match oversight depth to consequence, uncertainty, authority, and reversibility. | Risk register, delegation matrix, review criteria. |
| Auditability | Preserve what was proposed, accepted, rejected, changed, and approved. | AI-use log, action log, approval record. |
| Feedback and learning | Use oversight outcomes to improve policies, context, tests, prompts, workflows, and controls. | Postmortems, capability review log, stewardship records. |

## G.8 AI Governance Evidence Catalog

AI governance becomes durable when it leaves evidence. The following artifacts help teams reconstruct AI-related decisions and evaluate whether governance is actually operating.

| Artifact | Purpose | Representative Path |
| --- | --- | --- |
| AI-use log | Records consequential AI assistance, proposed outputs, human changes, acceptance or rejection, and verification notes. | /docs/governance/ai_governance/ai_use_log.md |
| Delegation matrix | Defines what AI may assist, recommend, prepare, execute, or never do. | /docs/governance/ai_governance/delegation_matrix.md |
| AI capability review log | Tracks capability changes, model/tool updates, observed limitations, evaluation outcomes, and governance updates. | /docs/governance/ai_governance/ai_capability_review_log.md |
| Evaluation record | Preserves test cases, scenario evaluations, adversarial cases, expected behavior, and failure analysis. | /docs/governance/ai_governance/evaluation_record.md |
| Known limitations record | Identifies where the AI is weak, uncertain, excluded, or restricted. | /docs/release_evidence/known_limitations.md |
| Agent authority matrix | Defines tool permissions, action boundaries, approval requirements, and prohibited actions. | /docs/governance/agentic_workflows/tool_authority_matrix.md |
| Agent action log | Records actions prepared or performed by AI-enabled workflows. | /docs/governance/agentic_workflows/agent_action_log.md |
| Revocation and rollback plan | Explains how delegated authority can be removed and erroneous actions recovered from. | /docs/governance/agentic_workflows/revocation_plan.md |
| Context source registry | Identifies source authority, ownership, freshness, and permissions for context used by AI. | /docs/governance/context_engineering/context_source_registry.md |
| Oversight review record | Shows that oversight is meaningful, evidence-based, and paired with authority. | /docs/governance/reviews/human_oversight_readiness_review.md |

## G.9 Review Questions for AI Governance

AI governance reviews should force confidence to meet evidence. The questions below can be used by teams, instructors, reviewers, or leaders when evaluating an AI-assisted or AI-enabled system.

| Review Area | Questions |
| --- | --- |
| Purpose and scope | What is the AI being used for? What is explicitly out of scope? What problem is it supposed to help solve? |
| Authority | Is the AI assisting, recommending, preparing, executing with approval, or acting under policy? What is it prohibited from doing? |
| Context | What sources inform AI behavior? Are they authoritative, current, permissioned, owned, and reviewable? |
| Verification | How was output evaluated? What tests, examples, adversarial cases, or stakeholder checks were used? |
| Oversight | Who reviews the AI output or action? Do they have enough visibility and authority to intervene? |
| Auditability | Can the team reconstruct what the AI proposed, what humans accepted, and what happened afterward? |
| Recoverability | If the AI causes or contributes to a failure, how will the team detect, contain, reverse, and learn from it? |
| Transparency | What limitations, uncertainties, AI involvement, or residual risks should stakeholders know? |
| Stewardship | How will the team revisit capability, context, policy, evaluation evidence, and authority over time? |

## G.10 AI Governance Across the Lifecycle

AI governance is not a single gate. It matures across the lifecycle as the system moves from idea to implementation, release, operations, agentic workflow, and stewardship.

| Lifecycle Stage | AI Governance Focus | Typical Evidence |
| --- | --- | --- |
| Worldview and launch | AI pressure, acceptable use, accountability, standards, disclosure expectations. | AI-use policy, launch standards, working agreements. |
| Requirements and planning | Generated requirements, stakeholder validation, ambiguity control, risk ownership. | Requirements review, AI-assisted requirements record, risk register. |
| Architecture and design | Model boundaries, context sources, authority, fallback, auditability, oversight. | Architecture overview, ADRs, context trust model, delegation matrix. |
| Implementation and review | Generated code, tests, configuration, documentation, PR evidence, AI disclosure. | AI-use log, PR review, test evidence, security review. |
| Testing and release | Scenario evaluation, adversarial cases, known limitations, readiness, rollback. | Evaluation record, release readiness record, known limitations, rollback notes. |
| Operations | Monitoring, audit logs, incident detection, runbooks, runtime behavior, postmortems. | Runtime evidence, incident records, runbooks, postmortems. |
| Agentic workflows | Tool authority, approval gates, action logs, revocation, recovery, human ownership. | Tool authority matrix, action approval flow, agent action log, revocation plan. |
| Stewardship | Capability drift, policy updates, context freshness, retirement, learning, portfolio evidence. | Capability review log, governance calendar, stewardship plan, professional portfolio. |

## G.11 AI Governance Anti-Patterns

AI governance also requires recognizing failure patterns. The following anti-patterns appear when teams treat AI capability as trustworthiness instead of treating AI as a governed engineering capability.

| Anti-Pattern | What It Looks Like | Correction |
| --- | --- | --- |
| Hidden AI use | AI materially shaped requirements, code, tests, documentation, or operations, but no evidence records it. | Use AI-use logs, PR disclosure, review notes, and verification evidence. |
| Fluent output acceptance | Polished generated text is accepted as correct because it sounds convincing. | Require source validation, stakeholder review, tests, and traceability. |
| Prompt as governance | The team assumes a carefully worded prompt replaces architecture, review, controls, or operations. | Use prompts only inside a broader governance system with evidence and oversight. |
| Context soup | AI is given uncontrolled, stale, conflicting, or unauthorized context. | Create context source registries, trust models, freshness policies, and exception handling. |
| Oversight theater | Humans approve outputs they cannot understand, challenge, override, or recover from. | Design decision surfaces, escalation paths, intervention authority, and audit records. |
| Silent authority | AI changes state, routes work, sends messages, or triggers actions without visible approval or audit. | Define authority boundaries, approval gates, logs, monitoring, and revocation. |
| Green evaluation fantasy | A small successful evaluation set is treated as proof of operational trustworthiness. | Use risk-based evaluation, adversarial cases, runtime monitoring, and known limitation disclosure. |
| Governance decay | Initial controls exist but are not reviewed as models, context, workflows, or risks change. | Use stewardship reviews, capability review logs, and governance update calendars. |

## G.12 AI Governance Maturity Reference

AI governance maturity is not measured by how much AI a team uses. It is measured by whether AI-related behavior is bounded, evidenced, reviewable, observable, recoverable, and owned.

| Maturity Level | Description | Evidence of Maturity |
| --- | --- | --- |
| Level 1 - Uncontrolled Assistance | AI use is individual, informal, and mostly invisible. | Little or no durable evidence. |
| Level 2 - Disclosed Assistance | AI use is acknowledged and reviewed when it affects engineering work. | AI-use notes, PR disclosure, human verification. |
| Level 3 - Reviewable AI Work | AI-assisted artifacts are traceable to requirements, architecture, tests, and review decisions. | AI-use log, review records, tests, stakeholder validation. |
| Level 4 - Governed Delegation | AI roles, authority, context, approval paths, and limitations are explicitly defined. | Delegation matrix, context registry, approval records, known limitations. |
| Level 5 - Operationally Controlled AI | AI-enabled behavior is observable, auditable, recoverable, monitored, and incident-ready. | Runtime evidence, action logs, runbooks, revocation plans, postmortems. |
| Level 6 - Stewardship-Ready AI | AI capability, context, governance, evaluation, and authority are reviewed over time. | Capability review log, stewardship plan, governance calendar, retirement/evolution records. |

## G.13 Relationship to Trustworthiness

AI governance supports trustworthiness only when it is connected to evidence and operations. It strengthens correctness by requiring verification. It strengthens traceability by preserving AI-use evidence. It strengthens reviewability by making AI influence inspectable. It strengthens governability by bounding authority. It strengthens recoverability by requiring rollback, revocation, and incident learning. It strengthens accountability by keeping humans responsible for consequential outcomes.

The absence of AI governance weakens trustworthiness even when the system appears to work. A fluent assistant, a successful demo, or a convenient automation does not prove that the system is correct, reviewable, observable, recoverable, or accountable.

## G.14 Final Reference Statement

AI governance in ETIS is not a rejection of AI. It is the professional discipline that makes AI usable inside trustworthy systems. Intelligent capabilities can help teams reason, draft, search, summarize, classify, recommend, and act. But when those capabilities affect engineering work, operational behavior, institutional decisions, or user trust, they must be bounded by context, evidence, review, oversight, recoverability, and accountable human judgment.

The final rule is direct: never give AI authority you cannot explain, control, audit, revoke, recover from, and own.
