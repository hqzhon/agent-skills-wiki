# HITC NetSuite Agent Skills

**Tags:** netsuite, erp, suitecommerce, performance, skill-pack, mit
**Source:** [@HITCforNetSuite](https://x.com/HITCforNetSuite/status/2118648374413201599) · 2026-11-06
**Engagement:** headintheclouddev/hitc-netsuite-agent-skills · MIT · 补齐 Oracle SuiteCloud Agent Skills 未覆盖的实操面

## When to use
在 NetSuite / SuiteCommerce 上做 **性能诊断** 或 **主题与扩展开发**，希望 Ask Oracle / Claude / Codex / Cline 按可追溯的 Oracle 文档走，而不是空口建议。

## What it does
两个技能：
1. `hitc-netsuite-performance` — 慢页面 / 保存 / 搜索 / 任务：走 Performance Details、APM SuiteApp、Scripted Records，再给修复与开发 brief。
2. `hitc-suitecommerce-development` — SuiteCommerce / MyAccount / SCA 2020.2+ 主题扩展：devtools、Extensibility API（含 Cart）、沙箱重建后的站点、调试笔记。

原则写死：事实溯源到 `references/`、先测量再猜、默认只读、供应商相关建议单独标注。

## Recipe / links
- Repo: https://github.com/headintheclouddev/hitc-netsuite-agent-skills (MIT)
- Install: `npx skills add headintheclouddev/hitc-netsuite-agent-skills`
- 单技能: `npx skills add headintheclouddev/hitc-netsuite-agent-skills --skill hitc-netsuite-performance`
- Ask Oracle: 用 Releases 里的单技能 zip（不要整仓 Download ZIP）
- Oracle 官方对照: https://github.com/oracle/netsuite-suitecloud-sdk/tree/master/packages/agent-skills

## Why it made the cut
垂直 ERP 场景清晰、SKILL.md + references 可核、MIT；星数尚低但配方完整，补 Catalog 的 NetSuite 缺口。
