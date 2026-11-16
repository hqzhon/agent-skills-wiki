# earnings-analysis（Anthropic 官方季报更新备忘）

**Tags:** finance, equity-research, earnings, official, skill
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2122186405980078174) · 2026-11-16
**Engagement:** 发现帖互动很少；仓库 [anthropics/financial-services](https://github.com/anthropics/financial-services) 现 41,329★ / 5,759 forks，Apache-2.0

## When to use
要对**已覆盖**的公司写一份季报更新（earnings update / quarterly update / Q1–Q4 results），强调超预期或不及预期、关键指标、估计上修和论点变化，而不是发起覆盖或一份完整启动报告。公司尚未覆盖应走 [initiating-coverage](anthropic-initiating-coverage.md)；闪讯/一页快评也不是这条的格式。

## What it does
官方 `earnings-analysis` skill，位于 `plugins/agent-plugins/earnings-reviewer/skills/`。目标输出是机构风格的 8–12 页、约 3,000–5,000 字更新备忘（1–3 张汇总表、8–12 张图），在财报后 24–48 小时内聚焦「什么是新的」：beat/miss 及原因、更新后的估计、对投资论点的影响。强制要求图表和表格带可点击的具体来源链接（10-Q、业绩稿等），不要只写裸 URL。同插件里还有 earnings-preview、morning-note、model-update 等，本条只收录这条被点名安装的分析技能。依赖最新财报、10-Q、电话会稿和一致预期来源，以及 Python 绘图和 DOCX 技能。

## Recipe / links
- SKILL.md: https://github.com/anthropics/financial-services/blob/main/plugins/agent-plugins/earnings-reviewer/skills/earnings-analysis/SKILL.md
- 先审阅再装：`gh skill preview anthropics/financial-services plugins/agent-plugins/earnings-reviewer/skills/earnings-analysis/SKILL.md`
- 读完 SKILL.md、`references/`、许可证和脚本，核对依赖、网络/文件权限后再决定是否安装
- 不要向技能提供非公开材料；模型额度、数据源和外部依赖仍可能收费
- `gh skill` 目前仍是公开预览功能，先确认本地 CLI 版本支持

## Why it made the cut
官方可加载技能，场景边界清楚（已覆盖公司的季报更新，不是启动报告），对引用和篇幅有可执行约束。与 [initiating-coverage](anthropic-initiating-coverage.md)、[financial-statements](anthropic-financial-statements.md) 互补。
