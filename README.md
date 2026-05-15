# Ceramic Claude Code Plugins

Claude Code plugins for [Ceramic AI](https://docs.ceramic.ai). Install once, use across every project.

## Plugins

| Plugin | Description |
|--------|-------------|
| `ceramic-search` | High quality web search for AI agents using Ceramic |

## Installation

### Step 1 — Register the marketplace

```bash
claude plugin marketplace add CeramicTeam/ceramic-claude-code-plugin
```

This clones the repo and makes the plugins discoverable in Claude Code. The plugins are not installed yet.

### Step 2 — Install the plugin

```bash
claude plugin install ceramic-search@ceramic-ai
```

Or from within a Claude Code session:

```
/plugin install ceramic-search@ceramic-ai
```

### Step 3 — Authenticate with Ceramic

Open a **new terminal outside of any Claude Code session** and run:

```bash
claude mcp login ceramic-search
```

Open the printed authorization URL in your browser and complete the **WorkOS OAuth** flow — sign in or create an account. The browser will show "Authentication complete. You may close this window." and your terminal will confirm `Successfully logged in to MCP server 'ceramic-search'`.

> **Important:** do not run `claude mcp login` as a command inside a Claude Code session. The OAuth callback server requires binding to a local port that may be blocked in certain environments.

Sessions last a maximum of **7 days**, with a **2-day inactivity timeout**. When your session expires, re-run `claude mcp login ceramic-search` from a terminal outside of Claude Code.

### Step 4 — Start a new Claude Code session and use it

The `search` skill is now active in every Claude Code session. You can invoke it manually:

```
/ceramic-search:search
```

Or Claude will call it automatically whenever it needs current information from the web.

## Links

- [Ceramic documentation](https://docs.ceramic.ai)
- [Ceramic API reference](https://docs.ceramic.ai/api-reference/search)
- [Ceramic MCP server](https://docs.ceramic.ai/mcp/ceramic-mcp)
