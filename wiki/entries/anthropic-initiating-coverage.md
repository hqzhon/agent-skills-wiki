# initiating-coverage（Anthropic 官方，卖方研报首次覆盖）

**Tags:** finance, equity-research, report, excel, docx, official
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2121188878199701962) · 2026-11-13
**Engagement:** discovery post (low engagement); repo anthropics/financial-services ~41k★

## When to use
需要为一家公司写机构级的首次覆盖（initiation）研报：公司研究、财务建模、估值、图表，最后汇成 DOCX 报告。

## What it does
把首次覆盖拆成 5 个独立任务：① 公司研究 ② 财务建模（Excel）③ 估值（DCF + 可比公司）④ 生成 25–35 张图表 ⑤ 报告组装。强制单任务模式：用户说「把整份报告做了」时先问从哪一步开始，每一步执行前检查前置产物是否存在，3–5 步依赖前面的交付物；默认 Times New Roman，按大行研报格式产出。

## Recipe / links
- SKILL.md: https://github.com/anthropics/financial-services/blob/main/plugins/vertical-plugins/equity-research/skills/initiating-coverage/SKILL.md
- 预览/安装（GitHub CLI 带 skill 子命令的版本）：`gh skill preview anthropics/financial-services plugins/vertical-plugins/equity-research/skills/initiating-coverage/SKILL.md`，读完 SKILL.md、references/、scripts/ 并核对权限与依赖后再 `gh skill install`
- 可配套：[lbo-model](anthropic-lbo-model.md)、[comps-analysis](anthropic-comps-analysis.md)、[idea-generation](anthropic-idea-generation.md)

## Why it made the cut
官方维护、步骤和依赖写得很清楚；「一次只做一个任务、先验前置条件」的设计是长链路文档类 skill 的好样板，可防止 agent 一口气跑完整条流水线而出错。
