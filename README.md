# Ceramic Claude Code Plugins

> [!IMPORTANT]
> This plugin has moved to [CeramicTeam/agent-skills](https://github.com/CeramicTeam/agent-skills). New installs should use that repo. See the [Agent Skill docs](https://docs.ceramic.ai/api/search/agent-skill) for all install options.
>
> Already installed from this repo? Point the `ceramic-ai` marketplace to the new repo and update the plugin, then restart Claude Code:
>
> ```bash
> claude plugin marketplace add CeramicTeam/agent-skills
> claude plugin update ceramic-search@ceramic-ai
> ```

Claude Code plugins for [Ceramic AI](https://docs.ceramic.ai).

## Plugins

| Plugin | Description |
|--------|-------------|
| `ceramic-search` | High quality web search for AI agents using Ceramic |

## Installation

### Step 1 — Register the marketplace

```bash
claude plugin marketplace add CeramicTeam/ceramic-claude-code-plugins
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

### Step 3 — Start a new Claude Code session and authenticate

Claude will call the skill automatically whenever it needs current information from the web. On first use, Claude Code will detect that authentication is required and open a browser window to complete the **WorkOS OAuth** flow. Sign in or create an account, then return to Claude Code — authentication is handled automatically.


## Links

- [Ceramic documentation](https://docs.ceramic.ai)
- [Ceramic API reference](https://docs.ceramic.ai/api-reference/search)
- [Ceramic MCP server](https://docs.ceramic.ai/mcp/ceramic-mcp)
