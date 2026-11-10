# Webcrawl Anything（本地网页 / 文档抓取技能包）

**Tags:** scraping, crawl, skill-pack, cli, mcp, research
**Source:** [@ai_fengshou](https://x.com/ai_fengshou/status/2119722160604529060) · 2026-11-09
**Engagement:** 发现帖 · brainfish-ai/webcrawl-anything · MIT · 早期星标 · 8 个 SKILL.md

## When to use
要让 coding agent **本地、免 Key** 地搜/扒/地图爬站点、PDF、YouTube 字幕、GitHub 仓、CVE 等，写成 Markdown；或挂 MCP / CLI 做监控与专题研究——尤其不想绑 Firecrawl 一类云 API。

## What it does
CLI `webcrawl` + 可选 `@webcrawl/mcp`，并自带 8 个 Agent Skills（crawl、deal-watch、jobs-leads、learn-topic、protected-sites、real-estate、research-corpus、ticket-watch 等），每个有独立 `SKILL.md` 与 references。发现帖实测：scrape GitHub 仓页很快；search 质量仍弱，以 scrape/map 为主。

## Recipe / links
- Repo: https://github.com/brainfish-ai/webcrawl-anything （MIT）
- 安装技能：`npx skills add brainfish-ai/webcrawl-anything`（可加 `--skill webcrawl-deal-watch`）
- MCP：`npx webcrawl setup` · CLI：`npx webcrawl scrape <url>`
- 技能目录：`.agents/skills/*/SKILL.md` · 站点 https://webcrawl.app

## Why it made the cut
八份可安装 SKILL.md + CLI/MCP 可验证；场景清楚（agent 读网页/文档），与「只会喊 scraping」的帖不同。收录时注明 search 仍糙、以 scrape 为准。
