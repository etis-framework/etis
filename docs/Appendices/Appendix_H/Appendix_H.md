# Appendix H<br><span class="chapter-title-main">Terminology and Definitions

This book introduces a common vocabulary for discussing software engineering, trustworthiness, governance, operations, stewardship, and intelligent systems. Precise language matters because engineering decisions depend on what teams mean by evidence, authority, review, risk, oversight, readiness, and trust.

This appendix provides concise definitions for the most important terms used throughout the book. It is intended as a practical reference for readers, teams, instructors, reviewers, and organizations that want to apply trustworthy engineering concepts consistently in project work, professional practice, operational environments, and governance activities.

The definitions emphasize how terms are used throughout this book rather than how they might appear in every possible technical, organizational, or academic context. The goal is not to create a dictionary for all of software engineering. The goal is to preserve the shared professional vocabulary needed to build, review, operate, govern, and steward trustworthy intelligent systems.

## H.1 Purpose of this Appendix

This book uses a deliberately consistent vocabulary because trustworthy engineering depends on shared meaning. Words such as evidence, governance, oversight, context, trust, review, release, and stewardship carry professional consequences. If teams use those words loosely, they can appear aligned while making very different assumptions about risk, authority, accountability, and proof.

This appendix provides concise definitions for the most important terms used throughout the book. It is designed as a reader-facing reference rather than an instructional chapter. The definitions are intentionally practical: each term is defined in the way it is used throughout the book and connected to the engineering responsibilities that make the term operationally meaningful.

Readers can use this appendix when reviewing chapters, preparing project artifacts, conducting reviews, evaluating AI-assisted work, designing governance processes, supporting operational decision-making, or adapting the book's concepts to a course project, research effort, or professional engineering environment.

## H.2 Core Terms

The following terms form the core vocabulary used throughout this book. They appear across chapters, appendices, reviews, governance activities, operational records, and repository artifacts, and should be interpreted consistently wherever they appear. Consistent terminology supports consistent engineering judgment, review, governance, and stewardship.

| Term | Definition | Related Concepts |
| --- | --- | --- |
| Accountability | The explicit assignment of ownership for decisions, actions, evidence, risks, and outcomes. | Owners, approval, review, stewardship |
| AI-assisted work | Engineering work supported by AI-generated suggestions, drafts, analysis, code, tests, summaries, or recommendations. | AI proposes; engineers verify |
| AI delegation | The decision to allow an AI-enabled capability or agent to perform a bounded role, recommend an action, prepare an action, or execute an approved action. | Authority, oversight, audit, revocation |
| AI governance | The discipline of ensuring that AI-assisted and AI-enabled behavior remains bounded, evidence-backed, reviewable, auditable, recoverable where appropriate, and human-owned. | Delegation, context, oversight |
| AI-use log | A durable record of consequential AI assistance, including what was requested, what was produced, what was accepted, what was changed, and how it was verified. | Repository evidence, reviewability |
| Architecture | The structure of responsibilities, boundaries, dependencies, data ownership, authority, interfaces, and change surfaces that shape how a system behaves and evolves. | ADRs, reviews, governability |
| Architecture Decision Record (ADR) | A concise record of a consequential design decision, including context, options considered, decision, rationale, consequences, ownership, and links to evidence. | Decision memory, traceability |
| Authority | The power to approve, reject, change, execute, release, revoke, escalate, or accept risk. | Governance, human oversight |
| Automation | A system capability that performs a task according to designed rules, workflows, or learned behavior. | Control, observability, accountability |
| Black-box tolerance | The degree to which a team can responsibly accept behavior that is not fully explainable internally. Tolerance decreases as risk, authority, irreversibility, and operational impact increase. | AI governance, risk |
| COICP | Campus Operations and Incident Coordination Platform; the recurring LMU initiative used throughout ETIS to illustrate trustworthy engineering across the lifecycle. | LMU, enterprise reference |
| Context | The requirements, policies, repository evidence, source-of-truth data, examples, constraints, history, and operational facts that shape human and AI behavior. | Context is control |
| Context engineering | The design, selection, governance, freshness, ownership, permissioning, and review of context used by intelligent systems and engineering teams. | Source authority, AI governance |
| Correctness | The degree to which system behavior matches validated intent, requirements, constraints, and acceptance criteria. | Testing, validation |
| Defect | A gap between expected and actual behavior, including functional faults, documentation errors, configuration issues, governance gaps, or operational weaknesses. | Testing, stabilization |
| Demo | A demonstration of a working path. In ETIS, a demo is useful communication but not operational proof. | Release defense, evidence |
| Evidence | Durable, inspectable information that supports or challenges an engineering claim. | Repository-centered engineering |
| Evidence chain | A connected path from intent to decision, implementation, review, test, release, operation, incident, learning, or stewardship record. | Traceability |
| Governability | The ability to control authority, permissions, approvals, auditability, rollback, revocation, release, and stewardship decisions. | Governance is architecture |
| Governance | The designed system of authority, review, control, evidence, escalation, approval, audit, and accountability. | Architecture, accountability |
| Human oversight | Meaningful human review and control over consequential work, including authority to challenge, approve, override, intervene, escalate, or stop action. | Accountability, AI governance |
| Intelligent system | A software-intensive system that uses AI, machine learning, rules, automation, or agentic behavior to support decisions, workflows, interpretation, or action. | AI governance, trustworthiness |
| LMU | Lakeside Metropolitan University; the fictional enterprise environment used throughout ETIS. | COICP, enterprise reference |
| Operational trust | Confidence grounded in runtime evidence, observability, recovery, governance, transparency, ownership, and learning—not merely in construction or release claims. | Part III, operations |
| Repository-centered engineering | The practice of treating the repository as the system of record for engineering truth, including requirements, decisions, code, tests, reviews, release evidence, operations, governance, AI use, and stewardship. | Everything important leaves evidence |
| Reviewability | The degree to which humans can inspect, challenge, understand, and validate work, decisions, evidence, behavior, and risk. | Review boards, PRs |
| Stewardship | Long-term responsibility for keeping systems understandable, governed, observable, recoverable, updated, and trustworthy as conditions change. | Part IV, professional identity |
| Traceability | The ability to reconstruct why work was done, how it changed, what evidence supports it, who reviewed it, and what consequences remain. | Evidence chain |
| Trustworthiness | Trustworthiness | The lifecycle property by which a system can be responsibly understood, verified, reviewed, governed, operated, recovered, stewarded, evolved, and defended. | ETIS framework |

## H.3 Trustworthiness Terms

This book treats trustworthiness as cumulative lifecycle maturity. Trust is not established through a single activity, artifact, review, or control. It emerges from the combined effects of engineering discipline, governance, evidence, accountability, operational learning, and stewardship. The following terms describe the major trustworthiness concerns that recur throughout the book.

| Term |  Meaning |
| --- | --- |
| Accountability | Ownership is explicit and consequences are not hidden behind process, tools, AI, or teams. |
| Correctness | Behavior is validated against intent, requirements, constraints, and acceptance criteria. |
| Governability | Authority and action can be controlled, approved, audited, revoked, or constrained. |
| Human oversight | Humans retain meaningful control over consequential decisions and actions. |
| Observability | Runtime behavior, failure, health, and operational state can be understood from evidence. |
| Operational visibility | Stakeholders can see the health, risk, limits, dependencies, and impact of a system. |
| Recoverability | Failures can be detected, contained, rolled back, recovered from, and learned from. |
| Reviewability | Work and claims can be inspected and challenged by qualified humans. |
| Security and privacy | Systems, data, identities, workflows, integrations, and context are protected appropriately. |
| Stewardship readiness | The system can be maintained, governed, understood, reviewed, and evolved over time. |
| Traceability | Claims, decisions, changes, tests, releases, incidents, and learning can be reconstructed. |
| Transparency | The organization can honestly explain what is known, limited, monitored, governed, and owned. |
| Understandability | Humans can understand enough of the system to review, operate, govern, recover, and improve it. |

## H.4 Review and Governance Terms

Review and governance language throughout this book is intentionally action-oriented. Reviews exist to challenge claims, test evidence, expose assumptions, and improve judgment. Governance exists to design authority, accountability, intervention capability, and responsibility into systems rather than adding controls after the fact. Both disciplines exist to support trustworthy engineering, trustworthy operations, and trustworthy decisions.

| Term | Definition |
| --- | --- |
| Challenge mechanism | A structured way to test a claim against evidence, assumptions, risk, ownership, and next action. |
| Evidence expectation | The type and quality of evidence a review requires before a claim can be accepted. |
| Readiness question | A question used to determine whether a team is prepared to proceed responsibly. |
| Release defense | A professional explanation of readiness grounded in claims, evidence, limitations, risk, and ownership. |
| Review board | An evidence-aware challenge mechanism used at consequential lifecycle moments. |
| Review decision | The outcome of a review, such as approve, approve with conditions, defer, reject, escalate, or request more evidence. |
| Residual risk | Risk that remains after mitigation, review, testing, governance, or operational controls have been applied. |
| Risk owner | The person or role accountable for monitoring, mitigating, accepting, or escalating a risk. |
| Signoff theater | Approval behavior that appears official but does not challenge evidence, assumptions, risk, or ownership. |
| Trust claim | A statement that the system, team, artifact, or decision can be trusted for a specific purpose under stated conditions. |

## H.5 Repository and Evidence Terms

Repository and evidence terminology is important because this book treats the repository as engineering memory rather than merely a storage location. Requirements, architecture decisions, reviews, tests, releases, incidents, governance records, operational learning, and stewardship activities all leave evidence that must remain understandable, reviewable, and traceable over time. The following definitions support the repository practices, artifact catalogs, evidence relationships, and trustworthiness expectations used throughout the book.

| Term | Definition |
| --- | --- |
| Artifact | A durable work product that records intent, decision, evidence, behavior, review, risk, or learning. |
| Artifact freshness | The degree to which an artifact remains current, accurate, owned, and useful for decisions. |
| Evidence index | A navigational aid that helps reviewers locate the artifacts needed to evaluate a claim. |
| Issue | A repository record that connects work, intent, acceptance criteria, discussion, risk, or follow-up action. |
| Known limitations record | A visible record of what the system does not yet do, where confidence is limited, and what risks remain. |
| Operational memory | Repository evidence that preserves incidents, postmortems, runbooks, observability records, and recovery learning. |
| Pull request | A proposed change packaged with evidence, review, discussion, test results, and links to related work. |
| Release readiness record | A repository artifact that summarizes evidence, risks, defects, limitations, approvals, and rollback or recovery expectations for a release. |
| Repository health | The condition of a repository as an evidence system: current, navigable, owned, reviewable, and trustworthy. |
| Repository memory | The repository’s accumulated record of engineering intent, decisions, changes, reviews, operations, governance, and stewardship. |
| Runbook | An operational guide for diagnosing, responding to, recovering from, or escalating known situations. |
| Stewardship record | Evidence that long-term ownership, governance cadence, capability review, retirement, and learning have been preserved. |

## H.6 AI Governance Terms

AI governance terminology throughout this book emphasizes authority, accountability, control, oversight, evidence, and recovery. Intelligent systems may assist, recommend, summarize, retrieve, or act within governed workflows, but capability is not authority and automation does not eliminate responsibility. The following definitions support the governance, context engineering, human oversight, and stewardship practices required for trustworthy intelligent systems.

| Term | Definition |
| --- | --- |
| Agentic system | A system component or workflow participant that can pursue goals, select actions, use tools, or coordinate steps under bounded authority. |
| AI capability review | A recurring assessment of whether an AI-enabled capability remains useful, safe, governed, evaluated, and appropriate for its current role. |
| AI-generated artifact | An artifact drafted, proposed, summarized, analyzed, or modified with AI assistance. |
| Audit trail | A durable record of actions, approvals, inputs, outputs, decisions, and responsible parties. |
| Context source registry | A record of approved context sources, ownership, freshness, authority, permissions, and intended use. |
| Context trust model | A description of which sources can be trusted for which purposes and under what constraints. |
| Delegation matrix | A record that defines what an AI capability may suggest, prepare, execute, escalate, or never do. |
| Evaluation set | A set of cases, scenarios, examples, or tests used to evaluate AI-assisted or intelligent behavior. |
| Human-in-the-loop | A control pattern in which a human participates in review or approval; meaningful only when the human has enough context and authority to act. |
| Override | A human or system action that interrupts, reverses, blocks, or changes an automated or AI-enabled action. |
| Revocation | The removal or reduction of authority, access, capability, or permission granted to an AI-enabled function or agent. |
| Silent authority | Unclear or hidden authority given to automation or AI, especially when state changes, decisions, or consequences occur without visible control. |
| Tool authority | The permission for an agent or system component to use a tool, call an API, change state, retrieve data, or initiate workflow action. |
| Verification burden | The obligation to review, test, challenge, and evidence AI-assisted work before accepting it as engineering truth. |

## H.7 Operational Terms

Operational terminology becomes increasingly important as systems move from implementation into real-world operation. Trustworthy systems must do more than satisfy requirements and pass tests. They must survive incidents, support recovery, enable learning, preserve evidence, and sustain confidence under changing conditions. The following definitions support the operational engineering concepts used throughout the book.

| Term | Definition |
| --- | --- |
| Degradation | A reduced operating mode that preserves essential capability or safety when full service is unavailable. |
| Incident | An operational event that disrupts, threatens, or reveals weakness in service, trust, security, reliability, governance, or user impact. |
| Incident timeline | A chronological record of detection, triage, decisions, actions, communication, containment, recovery, and follow-up. |
| Observability | The ability to understand runtime behavior from outputs such as logs, metrics, traces, request IDs, events, and audit records. |
| Postmortem | A learning record that examines what happened, why it happened, what was missed, what changed, and who owns follow-up. |
| Reliability | The ability of a system to perform acceptably under expected conditions, stresses, dependency failures, and change. |
| Rollback | A controlled return to a prior known state or behavior after a release, configuration, workflow, or AI capability causes unacceptable risk. |
| Runtime evidence | Evidence collected from actual system behavior in operation. |
| Service owner | The person or role accountable for the operation, health, support, and evolution of a service. |
| Stabilization | Work aimed at reducing defects, recurrence, volatility, uncertainty, and operational risk. |
| Transparency record | A record that communicates known behavior, limitations, risks, governance status, and ownership to appropriate stakeholders. |

## H.8 Engineering Judgment Terms

Engineering judgment terminology describes the professional responsibilities that cannot be delegated entirely to tools, processes, or intelligent systems. These terms help explain how engineers evaluate evidence, manage uncertainty, balance tradeoffs, exercise accountability, and make defensible decisions. They form a core part of the professional identity developed throughout this book and remain essential to trustworthy engineering in the AI era.

| Term | Definition |
| --- | --- |
| Assumption | A belief treated as true for planning, design, testing, release, or operation until it is validated or replaced. |
| Decision surface | The information, evidence, constraints, and tradeoffs visible to a person making a decision. |
| Engineering judgment | The disciplined professional capability to interpret evidence, weigh risk, reason under uncertainty, communicate tradeoffs, and own consequences. |
| Evidence sufficiency | The degree to which available evidence is strong enough for the decision being made. |
| Limitation disclosure | An honest statement of what is unknown, unsupported, weak, incomplete, risky, or deferred. |
| Professional defense | A structured explanation of a decision, release, system, or portfolio using evidence, tradeoffs, limitations, and ownership. |
| Tradeoff | A decision that favors one value, constraint, or outcome while accepting cost, risk, delay, limitation, or complexity elsewhere. |
| Uncertainty | A condition in which evidence, requirements, behavior, risk, or impact is incomplete, changing, or contested. |
| Ownership | The explicit responsibility for maintaining evidence, making decisions, accepting risk, correcting failure, or stewarding outcomes. |
| Steward | An engineer who preserves trustworthiness over time through evidence, governance, operations, learning, and responsible evolution. |

## H.9 Common Anti-Pattern Terms

Common anti-pattern terminology identifies recurring ways teams confuse activity with trustworthiness. These terms are intentionally blunt because vague language can hide weak evidence, weak governance, weak accountability, and weak engineering judgment. Naming anti-patterns helps organizations recognize trustworthiness failures before they become incidents, governance failures, or operational risk.

| Term | Definition |
| --- | --- |
| Archive rot | The decay of repository evidence until artifacts exist but are stale, misleading, unowned, or unusable. |
| Checklist theater | The appearance of control created by completed checklists that do not reflect actual evidence, review, operation, or risk. |
| Context soup | A poorly governed mixture of stale, unauthorized, irrelevant, conflicting, or unowned context used by people or AI systems. |
| Demo theater | The treatment of a successful demonstration as proof of readiness, trustworthiness, or operational maturity. |
| Evidence fragmentation | A condition in which evidence exists but is scattered, disconnected, inaccessible, or impossible to reconstruct. |
| Green-CI fallacy | The belief that passing automated checks proves system safety, quality, readiness, or trustworthiness. |
| Governance theater | A performance of approval, review, or compliance that does not control authority, risk, evidence, or accountability. |
| Hidden AI usage | Consequential AI assistance that is not visible to reviewers, maintainers, release authorities, or future stewards. |
| Magic agent | An agentic capability treated as capable, safe, or authoritative without explicit boundaries, audit, oversight, recovery, and ownership. |
| Oversight theater | A human approval step that appears responsible but lacks time, context, competence, authority, or willingness to challenge. |
| Replacement mythology | The belief that AI eliminates the need for engineering judgment, accountability, governance, or operational responsibility. |
| Ship-and-forget | A release posture that treats deployment as the end of responsibility rather than the beginning of operational learning and stewardship. |
| Tool worship | The replacement of engineering judgment with enthusiasm for a platform, vendor, process, or automation tool. |

## H.10 Acronyms and Short Forms

The following acronyms and short forms appear throughout this book. Some are widely used industry terms, while others have specialized meanings within the trustworthiness concepts presented here. Where a term requires additional context or interpretation, the relevant definition appears in the earlier sections of this appendix.

| Acronym | Meaning |
| --- | --- |
| ADR | Architecture Decision Record |
| AI | Artificial Intelligence |
| CI/CD | Continuous Integration / Continuous Delivery or Deployment |
| COICP | Campus Operations and Incident Coordination Platform |
| ETIS | Engineering Trustworthy Intelligent Systems: Software Engineering, Governance, and Operational Trust in the AI Era |
| LLM | Large Language Model |
| LMU | Lakeside Metropolitan University |
| PR | Pull Request |
| RACI | Responsible, Accountable, Consulted, Informed |
| RAG | Retrieval-Augmented Generation |
| SLA | Service Level Agreement |
| SLO | Service Level Objective |

## H.11 Usage Notes for Readers

Many of the terms used throughout this book are familiar words that take on specialized engineering meaning within this framework. Terms such as trust, evidence, governance, oversight, readiness, ownership, transparency, and stewardship are common in everyday conversation, but within the context of trustworthy engineering they describe specific responsibilities, expectations, decisions, and behaviors.

For example, trust is not treated as confidence, optimism, or belief. It is a conclusion supported by evidence, reviewability, governance, operational visibility, accountability, and stewardship. Similarly, governance is not viewed as paperwork or compliance activity. It is the practical design of authority, accountability, oversight, auditability, escalation, and control within a system and the organization that operates it.

Readers may encounter definitions that differ slightly from how the same terms are used in other disciplines, standards, organizations, or publications. This is intentional. The definitions in this appendix reflect the meaning required to support the engineering, operation, governance, and stewardship of software-intensive and intelligent systems.

When applying the concepts presented in this book to a project, organization, educational environment, or professional practice, focus on preserving the meaning behind the terminology rather than reproducing exact wording. Shared vocabulary is valuable because it helps teams reason consistently about evidence, risk, governance, operations, intelligent systems, accountability, and long-term stewardship.

The purpose of this appendix is not vocabulary standardization for its own sake. Its purpose is to support clear communication, consistent decision-making, effective review, and responsible engineering practice across the full lifecycle of trustworthy intelligent systems.

## H.12 Final Reference Statement

Terminology is not cosmetic. In trustworthy engineering, language shapes decisions. Teams that use precise language can make risk visible, assign ownership, challenge weak evidence, expose uncertainty, and communicate limitations honestly. Teams that use vague language can hide uncertainty, overstate readiness, weaken accountability, and create misunderstanding about responsibility and authority.

The vocabulary presented throughout this appendix is intended to support professional clarity. These terms help engineers, reviewers, operators, managers, governance bodies, educators, and students describe the responsibilities that remain after software works, after AI produces output, after tests pass, after a release ships, and after an organization begins depending on a system.

Trustworthy intelligent systems require more than technical capability. They require shared language for evidence, judgment, governance, operation, learning, accountability, and stewardship. Consistent terminology helps organizations preserve understanding, improve decisions, strengthen reviews, and sustain trust over time.

The definitions in this appendix are therefore not merely reference material. They are part of the professional foundation needed to build, operate, govern, and steward trustworthy intelligent systems.

