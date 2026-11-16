# ib-check-deck（Anthropic 官方投行路演材料质检）

**Tags:** finance, investment-banking, presentation, qa, official, skill
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2122277961516904951) · 2026-11-16
**Engagement:** 发现帖 1 赞 / 51 次展示；仓库 [anthropics/financial-services](https://github.com/anthropics/financial-services) 现 41,339★ / 5,758 forks，Apache-2.0

## When to use
要对路演 / 投资者 / 客户演示稿做交付前质检：跨页数字是否一致、图表是否支撑结论、语言是否符合投行语域、版式和来源是否完整。它只出报告，不改稿，也不判断投资价值。写模型或估值应走 [dcf-model](anthropic-dcf-model.md)、[3-statement-model](anthropic-3-statement-model.md) 等；审计 Excel 模型走 [audit-xls](anthropic-audit-xls.md)。

## What it does
官方 ib-check-deck skill，位于 plugins/vertical-plugins/financial-analysis/skills/。可在 PowerPoint 加载项（读当前打开的演示稿）或聊天里上传 .pptx 使用，工作流相同。四件事：

1. 抽取每页文本，用 scripts/extract_numbers.py 做数字口径与冲突检查（单位归一、同类指标打架、合计与增速）
2. 核对叙事与数据是否同向（趋势、份额、市场地位是否站得住）
3. 按投行语域扫口语、缩写、感叹号和含混量化
4. 视觉 / 版式：缺来源、缺轴标签、数字格式漂移、对比度与溢出等

输出按 Critical / Important / Minor 分级，带页码；没有致命问题也要写明「未发现数字不一致」。

## Recipe / links
- SKILL.md: https://github.com/anthropics/financial-services/blob/main/plugins/vertical-plugins/financial-analysis/skills/ib-check-deck/SKILL.md
- 先审阅再装：`gh skill preview anthropics/financial-services plugins/vertical-plugins/financial-analysis/skills/ib-check-deck/SKILL.md`
- 安装（Codex 用户级示例）：`gh skill install anthropics/financial-services plugins/vertical-plugins/financial-analysis/skills/ib-check-deck/SKILL.md --agent codex --scope user`
- 调用示例：`$ib-check-deck`。请逐页检查这份[公司]投资者/路演 PPT：列出跨页数字冲突、单位与期间不一致、叙事和图表矛盾、缺失来源/轴标签；按 Critical/Important/Minor 标注页码与理由。只报告，不修改文件。
- 读完 SKILL.md、references/、scripts/ 和 LICENSE，核对文件/网络权限后再决定是否安装
- 不要向技能提供非公开材料；模型调用与 Office 插件按各自计划计费
- gh skill 目前仍是 GitHub CLI 的公开预览功能，先确认本地版本支持

## Why it made the cut
官方可加载技能，场景边界清楚（只读质检，不改稿、不做投资结论），有抽取脚本和分级报告格式。与同仓的财务建模 / 研报技能互补。
