# Karada Documentation Guidelines & Agent Rules

## About This Project

- This is the official documentation site for **Karada.ai**, built on [Mintlify](https://mintlify.com).
- Content is written in MDX files with YAML frontmatter.
- Global navigation, SEO, and structured data configuration live in `docs.json`.
- Preview locally with `mint dev` or check links with `mint broken-links`.

---

## Canonical Terminology & Brand Guardrails

1. **Brand Entity Scope**:
   - In all public documentation titles, OpenGraph metadata, structured schemas, and outreach copy, always write **Karada.ai** (to differentiate from karada.com and establish entity clarity).
   - Within internal UI text and headings, "Karada" may be used normally.
2. **The 4 Infrastructure Layers**:
   - **Layer 1: Build & CI/CD Sync**: Auto-compile APIs (OpenAPI & Postman) into MCP servers. Keep tools in sync with CI/CD on every API deploy and spec drift.
   - **Layer 2: Production Middleware**: 1-Click composable plugins (Sentry error tracing, GA4 telemetry, Slack alert webhooks, rate limits, AI firewalls) with zero code modifications.
   - **Layer 3: Managed Hosting**: High-throughput stateless Streamable HTTP runtimes in Go with sub-5ms latency and 10,000+ concurrent stream support.
   - **Layer 4: Unified Gateway**: Dual-audience gateway—configure once across harnesses (Cursor, Claude Code, Windsurf) and enforce org standards across the company; direct distribution for MCP creators by publishing to our registry to work everywhere across active agent fleets.
3. **Core Engine & Architecture**:
   - **Proprietary Platform**: Karada is a proprietary language-agnostic platform and Go engine (NEVER refer to Karada as open-source or OSS).
   - **Zero Fabricated Claims**: Never invent benchmark multipliers or fake memory numbers.
   - **No Demo Videos**: Do not reference demo videos or link to video walkthroughs.
   - **Protocol Standard**: Stateless Streamable HTTP (`POST /mcp` + `stdio`, protocol `2026-07-28`).

---

## SEO, AEO & Agentic Discoverability Standards

- **Frontmatter Requirements**:
  Every `.mdx` file must define an explicit `title` (clean without `| Karada.ai` suffix), a concise `sidebarTitle` for the navigation table of contents, and an action-oriented `description` (120–160 characters).
- **AEO Definition Snippets**:
  High-value conceptual pages must begin with a clear blockquote definition (`> **What is [Feature]?**`) to facilitate answer engine extraction by Perplexity, ChatGPT Search, Claude, and Gemini.
- **Diátaxis Information Architecture**:
  - **Tutorials**: `quickstart.mdx` (learning-oriented).
  - **How-To / Playbooks**: `playbooks/*.mdx` (goal-oriented developer recipes for specific APIs like GitHub or Stripe).
  - **Explanation**: `features/*.mdx` (architecture-oriented deep dives).
  - **Reference**: `troubleshooting/error-codes.mdx` (information-oriented diagnostics).
- **Token Budgeting**:
  Keep individual documentation pages under 15,000 tokens so coding agents (Cursor, Claude Code, Antigravity) can ingest complete files without lossy summarization.
- **Copy-Ready Configs**:
  Always provide complete, copyable configuration JSON blocks for Cursor IDE and Claude Code.
