# Karada Documentation

> The official developer documentation for **Karada.ai**, the complete AI tool infrastructure platform to auto-generate, productionize, host, and distribute Model Context Protocol (MCP) servers from APIs.

## The 4 Platform Layers

1. **Build & CI/CD Sync**: Auto-compiles APIs (OpenAPI & Postman) into MCP servers. Keeps tools in sync with CI/CD on every API deploy and spec drift.
2. **Production Middleware**: Bolt on 1-click composable plugins (Sentry error tracing, GA4 telemetry, Slack alert webhooks, rate limits, AI firewalls) without modifying server code.
3. **Managed High-Throughput Hosting**: Deploy stateless Streamable HTTP runtimes in Go with sub-5ms latency and 10,000+ concurrent stream support.
4. **Unified Gateway**: Dual-audience gateway—configure tools once across Cursor, Claude Code, and Windsurf while enforcing org standards across the company; publish to our registry to distribute tools directly to active agent fleets.

## Quick Start

The fastest way to get your API talking to an AI agent is through the Auto-MCP quickstart:

1. Navigate to your **Dashboard** at [Karada.ai](https://karada.ai).
2. Create a new **Project** and select your API specification.
3. Attach composable plugins and click **Deploy Server**.

[Follow the full quickstart guide →](https://docs.karada.ai/quickstart)

## Local Development

If you want to contribute to these docs or preview them locally, install the Mintlify CLI.

**Prerequisites**: Node.js 19+

```bash
npm i -g mint
mint dev
```

View your local preview at `http://localhost:3000`.

## Need Help?

- **Email**: support@karada.ai
- **Discord**: [Join our community](https://discord.gg/karada)
- **GitHub Issues**: [karada-docs](https://github.com/shashtag-ventures/karada-docs/issues)
