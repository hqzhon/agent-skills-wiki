# financial-statements（Anthropic 官方三张表 + 差异分析）

**Tags:** finance, financial-statements, variance-analysis, official, skill
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2121823503448260896) · 2026-11-15
**Engagement:** 发现帖热度一般；技能位于官方仓 [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) 约 35.9k★，Apache-2.0

## When to use
手里有美股公司 10-Q，或已经核验过的期间数据，想按月 / 季 / 年 / YTD 把利润表、资产负债表和现金流量表对齐，并标出需要对问的差异。不要实时行情，也不要投资结论。

## What it does
官方 `financial-statements` skill。按用户给的期间数据整理三张表、期间对比和异常项。工作流：先采集当期与对比期数据（若已接 ERP / 数仓则拉取，否则粘贴、上传或提供底稿），再按多列格式生成利润表，并附资产负债表、现金流量表的列报参考、GAAP 要点（ASC 220/210/230）和常见期末调整。调用形态如 `$financial-statements quarterly`（也可 `monthly` / `annual` / `ytd`，并带上期间）。明确声明不提供投资建议，财务结论需回到原始 10-Q 或底稿核对。

## Recipe / links
- SKILL.md: https://github.com/anthropics/knowledge-work-plugins/blob/main/finance/skills/financial-statements/SKILL.md
- 同仓角色插件总述见 [Knowledge Work Plugins](knowledge-work-plugins.md)
- 预览（只读）：`gh skill preview anthropics/knowledge-work-plugins finance/skills/financial-statements/SKILL.md`
- 安装到 Codex 用户级（`gh skill` 仍为 preview）：`gh skill install anthropics/knowledge-work-plugins finance/skills/financial-statements/SKILL.md --agent codex --scope user`
- 重开会话后调用：`$financial-statements quarterly`
- 装前读完 SKILL.md、LICENSE、关联文件和权限；模型额度、数据连接和外部依赖仍可能收费

## Why it made the cut
官方可执行配方，场景清楚（期间三张表 + 差异分析，不编行情、不下投资结论），与已收录的 audit-xls / DCF / 研报 skill 配套。
