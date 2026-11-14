# dcf-model（Anthropic 官方 DCF 估值建模）

**Tags:** finance, equity-research, dcf, excel, official
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2121415796924862488) · 2026-11-14
**Engagement:** 发现帖 1 赞；仓库 [anthropics/financial-services](https://github.com/anthropics/financial-services) 约 41k★，Apache-2.0

## When to use
要用现金流折现做股权估值、写内在价值分析，或按投行习惯出带敏感性分析的专业 Excel DCF 模型时。与已收录的 [lbo-model](anthropic-lbo-model.md)（杠杆收购）不是同一条。

## What it does
官方 `dcf-model` skill：从 SEC 文件和卖方/分析师材料取数，搭建现金流预测、WACC 与终值，并输出带敏感性分析和执行摘要的 Excel 模型。计算必须写成 Excel 公式而非硬编码；区分 Office JS（Excel 内直接写公式）和 openpyxl（独立 `.xlsx`，交付前跑 `recalc.py`）两种环境。SKILL 很长、约束很细，适合当「按投行标准建 DCF」的可重复配方，而不是一次性让模型自由发挥。

## Recipe / links
- SKILL.md: https://github.com/anthropics/financial-services/blob/main/plugins/agent-plugins/model-builder/skills/dcf-model/SKILL.md
- 同目录还有 lbo-model、3-statement-model、comps-analysis 等；审计用 [audit-xls](anthropic-audit-xls.md)
- 先审阅再装：`gh skill preview anthropics/financial-services plugins/agent-plugins/model-builder/skills/dcf-model/SKILL.md`
- 安装到 Codex 用户范围：`gh skill install anthropics/financial-services plugins/agent-plugins/model-builder/skills/dcf-model/SKILL.md --agent codex --scope user`，新对话用 `$dcf-model`
- 该 skill 还依赖 xlsx 相关 skill；Excel 公式须重算并检查错误。装前读完 SKILL.md、LICENSE、scripts/references
- 仓库声明：输出需由具备资格的人士审阅，不构成投资建议

## Why it made the cut
官方维护的完整 DCF 配方，数据来源、公式约束和交付环境都写清楚了；补上了已有 LBO / comps / 研报条目之外的核心估值模型。
