# Effective HTML（自包含 HTML 产物技能包）

**Tags:** frontend, html, wireframe, prototype, diagrams, skill-pack
**Source:** [@tom_doerr](https://x.com/tom_doerr/status/2122324126064935034) · 2026-11-16
**Engagement:** 发现帖 59 赞 / 65 书签；仓库 [plannotator/effective-html](https://github.com/plannotator/effective-html) 现 4,194★ / 288 forks，MIT。指南站点 [effectivehtml.com](https://www.effectivehtml.com/)。最近推送 2026-10-31。

## When to use
要用编码 agent 产出自包含的 HTML 产物：低保真线框、可交互原型、一页纸说明、架构/流程/时序图、计划与路线图，或把复杂信息做成「大图少字」的讲解页。提示词可以指向这些产物，而不写一堵文字墙。只想要设计系统或去 AI 味视觉方向，应走 [Impeccable](impeccable.md) / [Taste Skill](taste-skill.md)；要滚动叙事落地页见 [scroll-craft](scroll-craft.md) 或 [scroll-world](scroll-world.md)。

## What it does
8 个可选、可单独安装的 agent skill，既可当参考手册，也可装进 Claude Code / Codex 等：

- `html`：总入口，混合产物、报告、讲解、落地页，并路由到专项技能
- `html-wireframe`：低保真布局，测内容层级、导航、流程和响应式结构
- `html-prototype`：带真实状态、交互、键盘支持和响应式的可运行原型
- `html-plan`：计划、路线图、实施顺序，保留来源承诺
- `html-diagram`：架构、时序、流程与状态图
- `one-pager` / `big-pics-little-words`：大图少字的一页纸或讲解页（源自 backnotprop/bro）
- `design-artifact`：针对当前主题的创意方向，不强制一套可复用的品牌样式

仓库说明：可以先不安装，只把本仓库当参考。

## Recipe / links
- Repo: https://github.com/plannotator/effective-html（MIT，4,194★）
- 指南：https://www.effectivehtml.com/
- 安装整包：`npx skills add plannotator/effective-html`
- 单项：`npx skills add plannotator/effective-html --skill html-prototype`（`--list` 可列出全部）
- Claude Code：`/plugin marketplace add plannotator/effective-html` 后 `/plugin install plannotator-effective-html@effective-html`
- Codex：`codex plugin marketplace add plannotator/effective-html` 后 `codex plugin add plannotator-effective-html@effective-html`

## Why it made the cut
8 份 SKILL.md 场景清楚、安装路径明确，MIT，星标过 4k，本窗口有高互动推荐。和已有的设计词汇表 / 滚动落地页技能互补，专攻「自包含 HTML 产物」这条工作流。
