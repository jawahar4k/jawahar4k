# Jawahar Prasad

Building AI dev productivity at scale, and the measurement framework that doesn't depend on AI lineage or surveys.

Bay Area · [jawaharprasad.com](https://jawaharprasad.com) · [LinkedIn](https://www.linkedin.com/in/jawaharprasad)

---

## Open source

**[tokendog](https://github.com/jawahar4k/tokendog)**: watchdog for Claude Code token spend. Prices every turn from authoritative usage, attributes cost by project / tool / model / context band, and tells you which sessions to close. Local-only, nothing leaves your machine.

Built it after measuring one developer's 255 transcripts (6.3B tokens): 62% of cost was cache reads, 29% cache writes, 9% output. Nine-tenths of the bill is context economics, not generation. Most token advice is about the last ninth.

Also: [argoproj-labs/mcp-for-argocd#116](https://github.com/argoproj-labs/mcp-for-argocd/pull/116), preserve subpath in `ARGOCD_BASE_URL` for ArgoCD behind an ingress.

## What I build

**ORBIT**: an agentic AI dev-productivity platform running across thousands of repositories (700+ microservices), used across engineering, QA, and product. Sub-systems:

- **DeepContext**: hybrid retrieval over Jira, Confluence, code, and PRs
- **Central**: agentic orchestration with sandboxed execution
- **CPI**: Composite Productivity Index, a measurement framework that doesn't depend on AI lineage or surveys
- **AIR**: incident-response research direction, currently in early preview

ORBIT replaced **PDAF** (Persona-Driven AI Framework), the prompt-driven AI agent framework I shipped in 2025. PDAF produced the results Augment Code documented in their December 2025 customer feature: **60% reduction in merge time** (3 days to 1 day), **+21% MR volume** at same headcount.

## Public work

- [LeadDev: How Tekion enabled 1,300 employees to work with agents](https://leaddev.com/community/jawahar-prasad)
- [Augment Code customer feature (Dec 2025)](https://www.augmentcode.com/blog/introducing-augment-code-review)
- *CPI paper in development*
- More at [jawaharprasad.com](https://jawaharprasad.com)

## Background

~21 years engineering, ~16 of them in ML / search / shopping / AI. Yahoo!, Jabong, Flipkart (doubled ads revenue, Best People Manager 2018), Amazon (Recommendations and Personalization). Founding team of what became [Whatfix](https://whatfix.com) (2010, left after 13 months before product-market fit).

Currently at Tekion since 2020.
