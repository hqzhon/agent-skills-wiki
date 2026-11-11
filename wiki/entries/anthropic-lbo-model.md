# lbo-model（Anthropic 官方 LBO 杠杆收购建模）

**Tags:** finance, private-equity, excel, spreadsheet, official
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2120465417500287166) · 2026-11-11
**Engagement:** discovery post (low engagement); repo anthropics/financial-services ~41k★

## When to use
为私募交易、交易材料或投委会填 LBO 模型模板（Sources & Uses、经营模型、债务表、回报分析）时。

## What it does
优先用你给的模板，没有就问，再退回自带 `examples/LBO_Model.xlsx`。所有计算必须写成 Excel 公式而不是硬编码数值；区分 Office JS（Excel 内）和 openpyxl（独立文件，交付前跑 `recalc.py`）两种环境；按蓝/黑/紫/绿颜色约定标注输入、计算、同表链接、跨表链接；逐个板块完成并让用户确认后再做下一块，避免后面整体返工。

## Recipe / links
- SKILL.md: https://github.com/anthropics/financial-services/blob/main/plugins/agent-plugins/model-builder/skills/lbo-model/SKILL.md
- 同目录还有 3-statement-model、dcf-model、comps-analysis、audit-xls、xlsx-author
- 预览/安装（GitHub CLI ≥2.102）：`gh skill preview anthropics/financial-services plugins/agent-plugins/model-builder/skills/lbo-model/SKILL.md`，审阅后 `gh skill install ... --agent codex --scope user`
- 安装前读完 SKILL.md、示例 xlsx 和脚本权限

## Why it made the cut
官方维护的完整配方，带模板文件和重算脚本；「公式而非硬编码」「分块确认」这类约束正是金融建模里 agent 最容易出错的地方；可与已收录的 comps-analysis 配套使用。
