# ECMWF Weather Skills（官方：预报 / ERA5 / Destination Earth）

**Tags:** official, ecmwf, weather, climate, era5, mcp, skill-pack
**Source:** [@AKapur36490](https://x.com/AKapur36490/status/2126194503816040519) · 2026-11-27
**Engagement:** 发现帖 0 赞 / 账号几乎无粉丝，正文短链未展开；经核对，官方仓库为 [ecmwf/ecmwf-weather-skills](https://github.com/ecmwf/ecmwf-weather-skills)，现 23★，Apache-2.0。ECMWF（欧洲中期天气预报中心）官方技能包，项目自标为 Emerging。仓最近推送到 2026-11-20。

## When to use
要让编码 agent **查找、申请、解码、绘图并正确引用** ECMWF 天气数据时用：实时 IFS / AIFS 预报、ERA5 再分析、CAMS 空气质量、MARS 档案、站点观测、Polytope 特征提取、Destination Earth 数字孪生，以及 ecCharts / OpenCharts 地图服务。不要靠模型记忆或网页搜索来「编」历史气温和预报场。

## What it does
一套遵循 Agent Skills 标准的官方技能（也可作为 Claude Code / Codex 插件安装），告诉 agent 该走哪条服务、如何组请求、如何用 [earthkit](https://github.com/ecmwf/earthkit) 解 GRIB，以及如何署名。本窗核对到的技能包括：`ecmwf-open-data`、`ecmwf-earthkit`、`ecmwf-opencharts-wms`、`ecmwf-polytope`、`ecmwf-cds-ads`、`ecmwf-mars`、`ecmwf-destine`、`ecmwf-observations`、`ecmwf-weather-feedback`。

无密钥也可先用：免费 ECMWF Open Data、公开地图服务，以及无需 key 的 ERA5 点序列。若配置了 CDS / ADS / MARS / Polytope，技能会改走更快或更完整的路径，并说明密钥能补上什么。仓库把远程 MCP 服务器 `https://mcp.ecmwf.int` 打进 Claude Code 和 Codex 插件（无需账户），用于图表、meteogram 和 Destination Earth 目录；当前该 MCP **没有**预报或 ERA5 工具，那些仍走技能脚本，所以不连 MCP 也能用。脚本用 `uv run` 按 PEP 723 按需安装 earthkit 组件。需要 Linux 或 macOS（Windows 请用 WSL），脚本侧建议 Python ≥ 3.12。

## Recipe / links
- Repo: https://github.com/ecmwf/ecmwf-weather-skills（23★，Apache-2.0）
- 技能文档：https://github.com/ecmwf/ecmwf-weather-skills/blob/main/docs/skills.md
- Claude Code：
  ```
  /plugin marketplace add ecmwf/ecmwf-weather-skills
  /plugin install ecmwf-weather@ecmwf
  /reload-plugins
  ```
- Codex：
  ```
  codex plugin marketplace add ecmwf/ecmwf-weather-skills
  codex plugin add ecmwf-weather@ecmwf
  ```
- 其他兼容客户端：`npx skills add ecmwf/ecmwf-weather-skills`
- 可选 MCP：`https://mcp.ecmwf.int`（可在 Claude Code `/mcp` 或 Codex 插件配置里关闭）

## Why it made the cut
气象领域权威机构的官方可加载技能包，使用场景清楚，有 SKILL.md、安装路径、测试和许可。发现帖本身几乎没有互动，也没给出仓库链接，但官方材料可独立核实。项目仍标 Emerging，数据引用和许可条款以 ECMWF / Copernicus 原文为准。
