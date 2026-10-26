# hithink-finance（同花顺金融数据 Agent Skill）

**Tags:** finance, a-share, market-data, skill, mcp, api
**Source:** [@ruyi3699](https://x.com/ruyi3699/status/2114573484403892639) · 2026-10-26
**Engagement:** discovery post (~2 likes / 4 replies); official Tonghuashun / HiThink tooling

## When to use
When an agent needs **A-share quotes, K-lines, financials, limit-up / dragon-tiger / hot lists, indices, funds**, or to choose among REST / MCP / CLI / Python for that data—in Chinese or English natural language.

## What it does
Official unified Agent Skill (`hithink-finance`) for 同花顺金融数据服务: intent routing, symbol disambiguation, credential checks, then API / MCP / CLI / Python / local DuckDB. Large results go to disk; outputs should cite source and time (not investment advice).

## Recipe / links
- Docs (Agent Skill quickstart): https://fuyao.aicubes.cn/docs/developer-tools/agent-skill/
- SkillHub: https://www.skillhub.cn/skills/hithink-finance
- Install: `npx skills add HiThink-Tech/Financial-API --skill hithink-finance -g --yes`
- Set `HITHINK_FINANCE_API_KEY` (user-level); keep full `skills/hithink-finance/` including `references/`
- Note: GitHub repo page may 404 from some networks; use docs/SkillHub or the npx installer when available

## Why it made the cut
Clear when-to-use, official installable Skill with multi-path data access, and public docs/SkillHub—not a screenshot-only tip.
