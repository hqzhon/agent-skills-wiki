# FlyAI（飞猪官方旅行搜索）

**Tags:** travel, fliggy, official, search, skill
**Source:** [@Lumizqj1](https://x.com/Lumizqj1/status/2119514290763727237) · 2026-11-09
**Engagement:** 0 likes / 0 reposts / 2 replies / 0 bookmarks · alibaba-flyai/flyai-skill · MIT · 1289★

## When to use
你已经在 Claude Code / OpenClaw 等 agent 里聊天，想用自然语言查机票、火车、酒店、景点、演唱会或签证信息，并拿到带预订链接的结构化结果，而不想另开浏览器或 App。

## What it does
阿里飞猪官方 Agent Skill：通过 `@fly-ai/flyai-cli` 调用飞猪 MCP，把旅行查询变成单行 JSON。八个命令：`keyword-search`、`ai-search`（语义搜索）、`search-flight`、`search-train`、`search-hotel`、`search-poi`，以及万豪酒店 / 套餐搜索。无需 API Key 即可起步，可选 `FLYAI_API_KEY` 增强结果。中英文都能问。

## Recipe / links
- Repo: https://github.com/alibaba-flyai/flyai-skill （MIT）
- 主页: https://open.fly.ai/
- OpenClaw：`clawhub install flyai` 或 `npx skills add alibaba-flyai/flyai-skill`
- Claude Code：把 `skills/flyai` 拷到 `~/.claude/skills/flyai`
- CLI：`npm i -g @fly-ai/flyai-cli`，然后 `flyai keyword-search --query "things to do in Tokyo"`
- 可选：`flyai config set FLYAI_API_KEY "your-key"`
- 每个命令的参数以 `skills/flyai/references/` 为准，不要猜测格式

## Why it made the cut
厂商官方 skill，有 CLI、SKILL.md 和可预订的实时库存，而不是又一个「帮我规划行程」的提示词；MIT，GitHub 约 1289★。
