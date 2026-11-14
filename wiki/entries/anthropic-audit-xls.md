# audit-xls（Anthropic 官方表格 / 模型审计）

**Tags:** finance, excel, spreadsheet, audit, official
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2121461015972093983) · 2026-11-14
**Engagement:** 发现帖 1 赞 / 1 收藏；仓库 [anthropics/financial-services](https://github.com/anthropics/financial-services) 约 41k★，Apache-2.0

## When to use
要把 Excel 工作簿或财务模型交给 agent 做公式质检、查错或「模型不平」排查时：从当前选区的快速检查，到整本模型的资产负债平衡、现金勾稽和逻辑健全性审计。

## What it does
官方 `audit-xls` skill。先确定范围（选区 / 单表 / 整本模型），再跑一套公式级检查：`#REF!` 等错误、公式里的硬编码、行列不一致、漏行、粘贴覆盖、循环引用、断掉的跨表链接、单位混用、隐藏行/表。选「整本模型」时还会按 DCF / LBO / 三表 / 并购 / comps 等类型做结构与勾稽检查（例如每期资产负债是否平衡、输入与计算是否分离、颜色约定是否一致）。SKILL 强调先报告发现，未经请求不改工作簿。

## Recipe / links
- SKILL.md: https://github.com/anthropics/financial-services/blob/main/plugins/agent-plugins/statement-auditor/skills/audit-xls/SKILL.md
- 同仓还有 [dcf-model](anthropic-dcf-model.md)、[lbo-model](anthropic-lbo-model.md)、[comps-analysis](anthropic-comps-analysis.md) 等建模 skill
- 先审阅再装（GitHub CLI ≥2.102）：`gh skill preview anthropics/financial-services plugins/agent-plugins/statement-auditor/skills/audit-xls/SKILL.md`
- 安装到 Codex 用户范围：`gh skill install anthropics/financial-services plugins/agent-plugins/statement-auditor/skills/audit-xls/SKILL.md --agent codex --scope user`
- 装前读完 SKILL.md、LICENSE 和附带资料，检查文件读写与工具权限

## Why it made the cut
官方可执行配方，把「查公式」和「查模型是否自洽」分成明确范围；与已收录的 LBO / comps / 研报 skill 配套，且约束 agent 先报告、不擅自改表。
