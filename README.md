# Jawahar Prasad

Coding agents for 1,300+ engineers at Tekion. I build the platform they run on (ORBIT) and the measurement that says whether it actually changed anything (CPI).

Bay Area · [jawaharprasad.com](https://jawaharprasad.com) · [LinkedIn](https://www.linkedin.com/in/jawaharprasad)

---

## Open source

**[tokendog](https://github.com/jawahar4k/tokendog)**: watchdog for Claude Code token spend. Prices every turn from authoritative usage, attributes cost by project / tool / model / context band, and tells you which sessions to close. Local-only, nothing leaves your machine.

Built it after measuring one developer's 255 transcripts (6.3B tokens): 62% of cost was cache reads, 29% cache writes, 9% output. Nine-tenths of the bill is context economics, not generation. Most token advice is about the last ninth.

Also: [argoproj-labs/mcp-for-argocd#116](https://github.com/argoproj-labs/mcp-for-argocd/pull/116), preserve subpath in `ARGOCD_BASE_URL` for ArgoCD behind an ingress.

## What I build

**ORBIT** is Tekion's internal AI engineering platform: the infrastructure that lets AI agents do real work across thousands of repositories (700+ microservices) for engineering, QA, and product. I architected it and run the team that builds it. The name means nothing outside Tekion, so here are the parts by the problem each one solves.

| Sub-system | The problem | What it is |
|---|---|---|
| **DeepContext** | An agent can't fix a bug if it can't find the ticket, the design doc, the PR that introduced it, and the three services it touches. Plain search finds documents; it doesn't find relationships. | Hybrid retrieval over Jira, Confluence, code, PRs, and commit history, exposed through one interface. The context layer every other sub-system reads from. |
| **Central** | Running an agent against one repo is easy. Running a code-review pass or a batch refactor across hundreds of repos needs isolation that no agent framework ships. | Agentic orchestration runtime. Headless agent workflows in sandboxed, ephemeral, network-policy-enforced environments. |
| **CPI** | "Is AI actually making us faster?" Most answers rely on surveys, tool-usage counts, or guessing which lines an AI wrote. All three are gameable. | Composite Productivity Index. Four outcome pillars (speed, effective throughput, rework, stability), each a z-score against a pre-AI baseline, with anti-gaming guardrails. Paper in development. |
| **Q** | Test coverage lags features, and at 700+ services nobody can hand-write the regression suite that a change actually needs. | Agentic QA pipelines: agents derive test plans from tickets and diffs, generate and run the tests, and triage failures before a human looks. In production. |
| **AIR** | On-call gets paged before anyone has looked at the root cause. | Adaptive Incident Intelligence and Remediation: detect, run RCA, and where confidence is sufficient, propose the fix as a PR. Early research preview. Auto-remediation is the part of AI engineering with the highest cost of being wrong, so this one moves slowly. |

ORBIT replaced **PDAF** (Persona-Driven AI Framework), the prompt-driven AI agent framework I shipped in 2025. PDAF produced the results Augment Code documented in their December 2025 customer feature: **60% reduction in merge time** (3 days to 1 day), **+21% MR volume** at same headcount.

## Public work

- [LeadDev: How Tekion enabled 1,300 employees to work with agents](https://leaddev.com/community/jawahar-prasad)
- [Augment Code customer feature (Dec 2025)](https://www.augmentcode.com/blog/introducing-augment-code-review)
- *CPI paper in development*
- More at [jawaharprasad.com](https://jawaharprasad.com)

## Background

~21 years engineering, ~16 of them in ML / search / shopping / AI. Yahoo!, Jabong, Flipkart (doubled ads revenue, Best People Manager 2018), Amazon (Recommendations and Personalization). Founding team of what became [Whatfix](https://whatfix.com) (2010, left after 13 months before product-market fit).

Currently at Tekion since 2020.
