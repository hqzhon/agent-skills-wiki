# Transitions.dev（UI 动效 skill + 「agent 正在生成 UI」效果）

**Tags:** frontend, css, motion, ui, design, skill
**Source:** [@usual_member](https://x.com/usual_member/status/2117390086962925651) · 2026-11-03
**Engagement:** 仓库 Jakubantalik/transitions.dev ~5.6k★（作者另有 thinking-orbs ~3.8k★）

## When to use
在 Web 项目里要加交互动效（下拉、弹窗、面板滑入、页面切换、数字跳动、图标切换、骨架屏、tooltip、tabs 滑块、手风琴等），或想让 agent 把散落的硬编码 duration 统一成 motion token；也适合想做「AI 正在生成界面」的点阵线框揭示效果。

## What it does
- `transitions-dev`：20+ 个可移植 CSS 过渡，每个用 `t-*` 选择器和语义化 CSS 变量，附 HTML 挂钩说明和 `prefers-reduced-motion` 兜底；SKILL.md 带速查表和逐个过渡的参考文件，还支持 reveal / review / apply / refine 几种指令（扫描并替换 ad-hoc 过渡）。
- `transitions-ui-generation`：从元素自身结构画出点阵线框再揭示真实 UI，有 `skeleton` / `skeleton-texts` 模式和 `text`、`image`、`auto` 等变体，零依赖运行时。

## Recipe / links
- Repo: https://github.com/Jakubantalik/transitions.dev · 入口 `skills/transitions-dev/SKILL.md`、`skills/transitions-ui-generation/`
- 安装：`npx skills add Jakubantalik/transitions.dev`（Cursor / Claude Code / Codex 等）
- 注意：X 上有人反馈 `transitions-ui-generation` 的 SKILL.md frontmatter 里 description 含未加引号的 `: `，导致 `npx skills add` 跳过它；手动给 description 加双引号即可（[原帖](https://x.com/usual_member/status/2117390227987644631)）

## Why it made the cut
有完整 SKILL.md + 逐项参考文件，场景具体（前端动效落地），仓库星数高且 skill 由展示站自动生成、与演示保持一致；补足 wiki 中「UI 动效」类。
