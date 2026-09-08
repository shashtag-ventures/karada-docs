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
2. **Plugins (Non-Negotiable)**:
   - Always use **Plugins** / **Plugins Marketplace** (NEVER use "integrations").
3. **Core Engine & Architecture**:
   - **Auto-MCP**: Karada's automated pipeline converting OpenAPI v3 and Swagger v2 specifications into Model Context Protocol (MCP) servers.
   - **Proprietary Go Engine**: Karada is a proprietary language-agnostic platform powered by a high-performance Go translation engine (NEVER refer to Karada as open-source or OSS).
   - **Unified MCP Gateway**: Multiplexing proxy aggregating multiple upstream MCP servers into a single Streamable HTTP / SSE endpoint.
   - **Zero Fabricated Claims**: Never invent benchmark multipliers or fake memory numbers.
   - **No Demo Videos**: Do not reference demo videos or link to video walkthroughs.

---

## SEO, AEO & Agentic Discoverability Standards

- **Frontmatter Requirements**:
  Every `.mdx` file must define an explicit `title` (clean without `| Karada.ai` suffix, as Mintlify handles site branding automatically), a concise `sidebarTitle` for the navigation table of contents, and an action-oriented `description` (120–160 characters).
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
  Always provide complete, copyable configuration JSON blocks for Claude Desktop (`claude_desktop_config.json`) and Cursor IDE settings.
