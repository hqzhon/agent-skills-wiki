# Kubai Icons（统一画风动态图标）

**Tags:** design, icons, svg, animation, skill
**Source:** [@xqliu](https://x.com/xqliu/status/2119757644214997252) · 2026-11-09
**Engagement:** 发现帖 · kubai087/kubai-icons · 图标 MIT · skill 源码可得 · ~476★

## When to use
做产品 / demo 页需要**一整套风格统一的功能图标**，还想要悬停动效（文件夹打开、信封拆封、齿轮转动）或可交付的静态 SVG；不想东拼西凑图标库，也不想每次重写画法。

## What it does
可安装 agent skill：硬性规则在 `PROMPT.md`，引擎在 `src/engine.js`（主色推导、外描边、分层、悬停关键帧），范例与自检/导出脚本齐全。给功能清单或产品代码，按同一几何与配色体系画新图标；也可只用仓库里 2600+ 已开源图标（React / Vue / Web Components / 纯 SVG）。配套站点可搜图标、改色、导出，并复制 prompt 贴给 agent。

## Recipe / links
- Repo: https://github.com/kubai087/kubai-icons （图标包 MIT；skill 本体为 Kubai Icons License，可商用安装运行）
- 入口：根目录 [`SKILL.md`](https://github.com/kubai087/kubai-icons/blob/master/SKILL.md) · [`PROMPT.md`](https://github.com/kubai087/kubai-icons/blob/master/PROMPT.md)
- 安装：把 README 安装说明发给 Claude Code / Codex（skills 目录分别为 `~/.claude/skills`、`~/.agents/skills`），重启后可用
- 自检 / 导出：`node scripts/check.mjs` · `node scripts/export.mjs`；浏览站 [icons.kubai.design](https://icons.kubai.design/)

## Why it made the cut
真实 SKILL.md + 可跑引擎/自检，场景清晰（统一画风图标 + 动效），材料可验证；与通用设计包互补，专做图标交付。
