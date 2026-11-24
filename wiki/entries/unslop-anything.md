# unslop-anything（先查真用户痛点，再修 AI 味 UI/UX）

**Tags:** design, ui, ux, frontend, mobile, anti-slop, skill
**Source:** [@fngly343149](https://x.com/fngly343149/status/2125108987104522520) · 2026-11-24
**Engagement:** 本窗介绍帖互动很低（1 赞）；仓库 [erkamyaman/unslop-anything](https://github.com/erkamyaman/unslop-anything) 现 358★，MIT，零运行时依赖，有测试 CI

## When to use
网页或移动应用看起来像「生成出来的」：套模板、不像自己的产品，或手机应用用起来像套了壳的网站。若只想按编号清掉文案/图表里的 AI 痕迹，用已收录的 [unslop-ui](unslop-ui.md)；若要把已有页面逐轮改出视觉性格，用 [unslop](unslop.md)（heydamir/unslop）。

## What it does
可加载技能 \`skills/unslop-anything/SKILL.md\`（自称 Dr. Unslopovich）。作者称规则来自约 500 万条应用评论研究，先查真正让人离开的问题（慢列表、移动的按钮、任务中弹出的窗、布局跳动、空洞的 Oops），再看界面是否还长得像所有生成应用。支持 Web（React/Next/Vue/Svelte/HTML 等）和移动（SwiftUI、Jetpack Compose、React Native、Flutter 等）。命令包括 \`review\`、\`treat\`、\`scan\`、\`chart\`、\`follow-up\`。

## Recipe / links
- Repo: https://github.com/erkamyaman/unslop-anything（358★，MIT）
- 安装：\`npx skills add erkamyaman/unslop-anything\`（也提供 npm 包 \`unslop-anything\`，宣称覆盖 6 类 agent）
- Skill: [skills/unslop-anything/SKILL.md](https://github.com/erkamyaman/unslop-anything/blob/main/skills/unslop-anything/SKILL.md)
- 研究方法说明在仓库 \`research/\`

## Why it made the cut
和已收录的两个 unslop 不是同一仓库：这边把移动端和「真实差评里的 UX 故障」放在视觉套装之前，有独立规则、测试和明确命令。358★、MIT、零依赖，配方可核对。本窗互动低，按仓库信号补上，并在条目里写清和 [unslop](unslop.md) / [unslop-ui](unslop-ui.md) 的分工。
