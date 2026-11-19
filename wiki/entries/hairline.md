# hairline（等距单线插画技能）

**Tags:** illustration, isometric, svg, frontend, skill-pack
**Source:** [@joshuiuxdesign](https://x.com/joshuiuxdesign/status/2123373180308070612) · 2026-11-19
**Engagement:** 展示帖（约 1 赞 / 1 转）；仓库 [lucasmarkes/hairline](https://github.com/lucasmarkes/hairline) 4,015★，MIT。

## When to use
想让 coding agent **按一个想法画出 Hairline 风格的等距单线插画**，或把已有 SVG（图标、Logo、插画）**领养成**可交互的 Hairline 图形，并交出一个打开即用、无需安装的 HTML 文件时使用。

## What it does
两个可加载技能，共用同一套引擎和十条造型规则：

- `hairline-create`：给出想法（或 `/hairline-create [idea]`），先给两三个概念，再按规则画出单线等距体，做成自包含 `hairline-<name>.html`（含强度滑杆、主题切换、指针巡游播放）。
- `hairline-adopt`：提供 `.svg`，读取对象与部件比例后交给 create 流程，并建议指针手势；不描摹、不直接给 SVG 加动画。

构建后用自带脚本在浏览器里对照规则做检查，通过才交文件。

## Recipe / links
- Repo: https://github.com/lucasmarkes/hairline（MIT，4,015★）
- 安装：`npx skills add lucasmarkes/hairline`（一次装上两个技能）
- 用法：`/hairline-create a sales funnel` 或 `/hairline-adopt icons/deploy.svg`
- 技能页与样张：https://hairline.lucasmarkes.com/skills
- SKILL.md：[`skills/hairline-create/SKILL.md`](https://github.com/lucasmarkes/hairline/blob/main/skills/hairline-create/SKILL.md)、[`skills/hairline-adopt/SKILL.md`](https://github.com/lucasmarkes/hairline/blob/main/skills/hairline-adopt/SKILL.md)

## Why it made the cut
官方作者技能，规则、引擎和验收脚本齐全，安装路径清楚；仓库星标高，且本窗有独立成片展示，不只是「画一张插画」的提示词。
