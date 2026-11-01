# Teachable Figures（可操作的交互教学图解）

**Tags:** education, interactive, explainer, svg, 3d, skill, chinese
**Source:** [@MirrortekUK](https://x.com/MirrortekUK/status/2116690985614721340) · 2026-11-01
**Engagement:** 新仓库 ywEdAi/teachable-figures ~200★（2026-10-27 创建），中文圈有讨论

## When to use
要把课文、文章或技术概念里的**一个结论**做成学习者能动手操作的图解：先预测、改一个条件、观察结果、再解释新情境。适合机制模拟、等距 SVG 物件、机械剖视 / 爆炸图、需要转动的真 3D 模型。不适合纯数据图表、Dashboard、幻灯片、静态插画或整门课程。

## What it does
`SKILL.md` 默认先做一轮最多 5 个问题的引导访谈（学习者、要理解的结论与要推翻的误解、目标形态、保真度、交互深度），每题带推荐默认值；用户说「直接生成」则跳过并在交付说明里列出假设。之后：找出可教的机制（因 → 果、误解、真值模型，区分有来源的事实与示意参数）→ 分开选「教什么」和「用什么渲染」→ 产出独立离线 HTML，或适配已有应用的课程结构，并保留无障碍要求。附渲染套件、审过的示例和浏览器检查脚本。

## Recipe / links
- Repo: https://github.com/ywEdAi/teachable-figures （`SKILL.md`、`references/`、`examples/`、`scripts/`、`tests/`）
- 中文说明：仓库内 `README.zh-CN.md`

## Why it made the cut
场景清晰、边界写得很明确（什么时候拒绝），配方完整到「访谈 → 机制 → 渲染选择 → 校验」，还带测试和浏览器检查；把「预测 → 调参 → 解释」固化进流程，比滑块玩具式课件更有教学价值。和 teardown / anatomy 这类 3D 讲解 skill 互补。
