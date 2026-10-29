# Anthropic Knowledge Work Plugins

**Tags:** skill-pack, cowork, anthropic, sales, finance, productivity, official
**Source:** [@KeyoAPI](https://x.com/KeyoAPI/status/2115679485488148832) · 2026-10-29
**Engagement:** ~33.7k★ · Apache-2.0 · role plugins with skills + MCP connectors

## When to use
When you want Claude Cowork / Claude Code to act like a **role specialist** (sales, support, PM, marketing, legal, finance, data, enterprise search, bio-research, productivity) with packaged skills, slash commands, and MCP connector stubs—then customize for your company’s tools.

## What it does
Open marketplace of 11+ plugins. Each plugin is markdown/JSON: `skills/` (auto-loaded domain playbooks), `commands/` (explicit slash actions), `.mcp.json` (tool connections). Examples: `/sales:call-prep`, `/data:write-query`, `/finance:reconciliation`. Also includes `cowork-plugin-management` for authoring/customizing plugins.

## Recipe / links
- Repo: https://github.com/anthropics/knowledge-work-plugins (~33.7k★, Apache-2.0)
- Cowork: https://claude.com/plugins/
- Claude Code: `claude plugin marketplace add anthropics/knowledge-work-plugins` then `claude plugin install sales@knowledge-work-plugins` (swap plugin name)

## Why it made the cut
Vendor-official, file-based skill/command packs with clear role scenarios and a public Apache-2.0 repo—portable beyond a single blog post.
