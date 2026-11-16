# 3-statement-model（Anthropic 官方三张表模板填报）

**Tags:** finance, financial-model, excel, official, skill
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2122141869199229232) · 2026-11-16
**Engagement:** 发现帖热度一般；仓库 [anthropics/financial-services](https://github.com/anthropics/financial-services) 现 41,329★ / 5,759 forks，Apache-2.0

## When to use
手里已有三张表（利润表 / 资产负债表 / 现金流量表）的 Excel 模板或半成品框架，需要按勾稽关系把历史数和预测公式填进去、把三张表打通。不要从零生成一套报表排版（那是 [financial-statements](anthropic-financial-statements.md)），也不要把它当成估值结论或自动出投资建议。

## What it does
官方 `3-statement-model` skill，位于 `plugins/agent-plugins/model-builder/skills/`。核心家规是：**预测、结转、勾稽和小计必须写 Excel 公式，不能把 Python 算好的数字写进单元格**；只有历史实际数和 Assumptions 页的驱动假设可以硬编码。环境分两种：在 Excel 加载项 / Office JS 里用 `range.formulas` 写入；导出独立 `.xlsx` 时用 openpyxl 写公式字符串，再跑 `recalc.py`。流程要求分步和用户确认：先汇报识别到的页签，再核对历史块，再确认预测利润表，然后做资产负债和现金流的链接。同目录还有 [dcf-model](anthropic-dcf-model.md)、[lbo-model](anthropic-lbo-model.md)、[audit-xls](anthropic-audit-xls.md)。

## Recipe / links
- SKILL.md: https://github.com/anthropics/financial-services/blob/main/plugins/agent-plugins/model-builder/skills/3-statement-model/SKILL.md
- 先审阅再装（`gh skill` 仍为 Preview）：`gh skill preview anthropics/financial-services plugins/agent-plugins/model-builder/skills/3-statement-model/SKILL.md`
- 安装到 Codex 用户级：`gh skill install anthropics/financial-services plugins/agent-plugins/model-builder/skills/3-statement-model/SKILL.md --agent codex --scope user`
- 重开 Codex 会话后用 `$3-statement-model` 显式调用；未识别时检查 `~/.agents/skills/3-statement-model/SKILL.md`
- 装前读完 SKILL.md、`references/`、LICENSE 及脚本；只提供完成任务所需的模板和公开数据

## Why it made the cut
官方可加载技能，使用场景和「公式优先、分步确认」的约束都很清楚，与已收录的 DCF / LBO / 三张表整理技能互补：本条专管**在已有模板里把三张表填通**。仓库星标高、许可明确。
