# Karada Documentation

> The intelligent deployment and API integration platform built for the AI era.

## Why Karada Exists

AI agents need to interact with your data, but they cannot natively understand complex REST APIs. Karada solves this by automatically bridging the gap between traditional APIs and modern AI assistants. If your API has an OpenAPI or Swagger specification, Karada instantly generates a Model Context Protocol (MCP) server that acts as a secure proxy. No more writing custom wrapper code just to let AI interact with your systems.

## Quick Start

The fastest way to get your API talking to an AI agent is through the Auto-MCP quickstart.

1. Navigate to your **Dashboard** at [Karada.ai](https://karada.ai).
2. Create a new **Project** and select **Auto-MCP**.
3. Provide the URL to your API specification (OpenAPI or Swagger).
4. Click **Generate Server**.

[Follow the full quickstart guide →](https://docs.karada.ai/quickstart)

## Core Features

- **Auto-MCP Generation**: Instantly turn APIs into AI-ready tools.
- **Instant Deployments**: Deploy generated servers or custom applications with one click.
- **Project Management**: Organize your workspaces, monitor usage, and manage environments effortlessly.
- **Team Collaboration**: Manage granular access control and collaborate securely.
- **Integrations Marketplace**: Extend your projects with community-built plugins.

## Local Development

If you want to contribute to these docs or preview them locally, install the Mintlify CLI.

**Prerequisites**: Node.js 19+

```bash
npm i -g mint
```

Run the following command at the root of this documentation repository:

```bash
mint dev
```

View your local preview at `http://localhost:3000`.

## Need Help?

- **Email**: support@karada.ai
- **Discord**: [Join our community](https://discord.gg/karada)
- **GitHub Issues**: [karada-docs](https://github.com/shashtag-ventures/karada-docs/issues)
