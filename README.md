# Vet — Claude Code plugin marketplace

[![Vet Security Report](https://getvet.ai/badge/mcp-ai-getvet-vet.svg)](https://getvet.ai/skill/mcp-ai-getvet-vet)

Security verification for MCP servers and AI tools, from [getvet.ai](https://getvet.ai).

The **vet** plugin bundles the [`@getvetai/mcp`](https://www.npmjs.com/package/@getvetai/mcp)
MCP server — so Claude Code can search and security-vet 200K+ MCP servers and AI tools
(trust scores, L0–L3 verification, permission mapping, tool schemas) right from your session.

## Install

```
/plugin marketplace add getvetai/claude-plugins
/plugin install vet@getvet
```

Then `/reload-plugins`. The `vet` MCP server starts automatically.

## Optional API key

Search and discovery work with no setup. To get full tool input/output schemas, set a free
API key (from [getvet.ai/dashboard](https://getvet.ai/dashboard)):

```json
{ "mcpServers": { "vet": { "command": "npx", "args": ["-y", "@getvetai/mcp"],
  "env": { "VET_API_KEY": "your-key" } } } }
```

## Links

- Web: https://getvet.ai
- npm: https://www.npmjs.com/package/@getvetai/mcp
- MCP Registry: `ai.getvet/vet`
- Contact: juanpalacor@getvet.ai
