# Mapbox Agent Skills（官方：Web / iOS / Android / Flutter 地图开发）

**Tags:** official, mapbox, maps, mobile, web, skill-pack
**Source:** [@gitrepos](https://x.com/gitrepos/status/2124624047530975256) · 2026-11-23
**Engagement:** 本窗为开源雷达转述（0 赞）；仓库 [mapbox/mapbox-agent-skills](https://github.com/mapbox/mapbox-agent-skills) 87★，MIT。Mapbox 官方维护，本窗仍有推送。

## When to use
要让编码 agent 做 **Mapbox** 应用（Web、iOS、Android、Flutter），并希望它按官方在性能、地图设计、框架集成、平台迁移、搜索、地理空间、导航和安全上的现行做法来写时使用。

## What it does
官方 Agent Skills + 插件包，教助手如何做出快、好看、安全的 Mapbox 应用。仓库符合 Open Plugins 规范，也可作为 Claude Code / Codex 插件安装；安装插件时会带上 `mapbox`、`mapbox-devkit`、`mapbox-docs` 三个 MCP。技能源目录在 `skills/`。

## Recipe / links
- Repo：https://github.com/mapbox/mapbox-agent-skills（MIT，87★）
- Skills CLI：
  ```
  npx skills add mapbox/mapbox-agent-skills
  ```
- 插件（Cursor / Codex / Copilot / Claude Code）：
  ```
  /plugin marketplace add mapbox/mapbox-agent-skills
  /plugin install mapbox
  ```
- 部分技能会通过 MCP 访问 Mapbox 服务，装前准备好自己的 token，并先看权限范围。

## Why it made the cut
厂商官方技能包，平台覆盖完整，有 SKILL.md、插件清单和 MCP 接线，可验证材料充足。本窗由开源聚合账号带出仓库，按官方仓收录。
