---
hide:
  - toc
---

# Companion Resources

**For _Engineering Agentic AI Systems_**

The authoritative manuscript and runnable implementation live in the public [Engineering Agentic AI Systems repository](https://github.com/etis-framework/etis-agentic-ai-book). The ETIS website points to those resources without duplicating maintained source or implying that demonstrations prove production guarantees.

## Reference Implementation: Builds 0–5

[Explore the Python Reference System ↗](https://github.com/etis-framework/etis-agentic-ai-book/tree/main/examples/refund-reference-system){ .md-button .md-button--primary }
[Browse the Full Book Repository ↗](https://github.com/etis-framework/etis-agentic-ai-book){ .md-button }

The progressive **CASE-204 $500 refund** implementation introduces the architecture's controls, trust boundaries, identity and context handling, bounded advisory behavior, approvals, provider reconciliation, and integrated checks. Read each build's README, architecture figure, test instructions, and stated limitations before using or adapting its code.

The reference architecture is mapped to **E1–E9 responsibilities** and **C01–C09 contracts**. MCP clients can reside in the agent application; the MCP server and independent authorization must enforce trusted boundaries before effects. Neither MCP nor A2A grants authority by itself.

## Suggested Learning Path

The companion is designed for working software engineers and advanced students. **Basic Python, software engineering, APIs, and testing** are useful starting points; prior experience building AI agents is not required. The examples use the Python standard library and simulated services, so readers do not need paid AI APIs or payment-provider credentials.

1. **Orient yourself.** Read the [getting-started guide](https://github.com/etis-framework/etis-agentic-ai-book/blob/main/docs/GETTING_STARTED.md) and the [chapter-to-code map](https://github.com/etis-framework/etis-agentic-ai-book/blob/main/docs/CHAPTER_MAP.md).
2. **Understand the boundaries.** Compare the book's E1–E9 responsibilities and C01–C09 contracts with the [reference architecture](https://github.com/etis-framework/etis-agentic-ai-book/blob/main/examples/refund-reference-system/ARCHITECTURE.md).
3. **Run Builds 0–5 in order.** Use the [guided learning path](https://github.com/etis-framework/etis-agentic-ai-book/blob/main/examples/refund-reference-system/LEARNING_PATH.md), following each build's README, source-module diagram, tests, and limitations.
4. **Test failure and recovery.** Continue into the repository's [security](https://github.com/etis-framework/etis-agentic-ai-book/tree/main/examples/refund-reference-system/security), [reliability](https://github.com/etis-framework/etis-agentic-ai-book/tree/main/examples/refund-reference-system/reliability), [operations](https://github.com/etis-framework/etis-agentic-ai-book/tree/main/examples/refund-reference-system/operations), and [assurance](https://github.com/etis-framework/etis-agentic-ai-book/tree/main/examples/refund-reference-system/assurance) exercises.

These builds are educational reference implementations, **not production-certified systems**. Reproduce and inspect their evidence before drawing conclusions about security or operational guarantees. For a stable first-edition snapshot, use the repository's [release guidance](https://github.com/etis-framework/etis-agentic-ai-book/blob/main/RELEASE.md) rather than assuming `main` remains unchanged.

## For Readers, Educators, and Engineering Teams

- **Readers:** work through the six builds in order, inspect tests and failure cases, and compare observed behavior with claimed guarantees.
- **Educators:** use architecture and trust-boundary reviews, adversarial tests, implementation inspections, and evidence-based engineering defenses as assignments.
- **Engineering teams:** apply the reference contracts, observability, recovery, approval, and verification concepts to your own environment, with controls tested independently.

## PDF and Edition Information

**First Edition publication date:** November 26, 2026. The First Edition PDF is available as a [free ETIS website download](../../downloads/books/Engineering_Agentic_AI_Systems_First_Edition_2026.pdf). The public Markdown manuscript can also be read in the [source repository](https://github.com/etis-framework/etis-agentic-ai-book).

[Book Overview →](index.md) · [Updates & Errata →](updates-and-errata.md)
