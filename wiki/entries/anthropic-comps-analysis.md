# comps-analysis（Anthropic 官方同业可比估值）

**Tags:** finance, valuation, spreadsheet, official
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2118244486736380354) · 2026-11-05
**Engagement:** discovery post (low engagement); repo anthropics/financial-services ~41k★

## When to use
做上市公司可比公司分析（M&A、投资分析、IPO/融资定价、同业对标、找估值离群值）时；不适合无可比上市同业的私企、多元化集团、困境公司和 pre-revenue 初创。

## What it does
按研究问题挑经营指标和估值倍数，要求记录数据来源与假设、统一期间口径，用中位数/四分位数做统计对标，输出结构化 Excel。明确数据源优先级：先用 S&P Kensho / FactSet / Daloopa 等 MCP，其次 SEC EDGAR 等机构源，不把网页搜索当主数据源。不提供实时行情，也不替你下投资结论。

## Recipe / links
- SKILL.md: https://github.com/anthropics/financial-services/blob/main/plugins/vertical-plugins/financial-analysis/skills/comps-analysis/SKILL.md
- 同仓库还有 `/comps` 命令和 market-researcher / model-builder / pitch-agent 插件里的同名 skill
- 安装前完整读一遍 SKILL.md

## Why it made the cut
官方维护的完整 SKILL.md；适用/不适用场景写得很清楚；可直接在大仓库里核对；数据口径约束是金融分析里最容易出错的点。
