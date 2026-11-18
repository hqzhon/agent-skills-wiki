# QuadMotion（终端 Unicode 像素吉祥物）

**Tags:** terminal, animation, pixel-art, tui, skill
**Source:** [@Liquid__Ring](https://x.com/Liquid__Ring/status/2122871577914306996) · 2026-11-18
**Engagement:** 作者自荐帖互动很低（0 赞 / 62 次展示）；仓库 [LiquidRing/quadmotion](https://github.com/LiquidRing/quadmotion) 现 0★，MIT（2026-11-17 建仓）。早期条目。

## When to use
要在终端里做不闪烁的像素吉祥物或短动画（CLI 吉祥物、状态小部件、庆祝动效），或让 coding agent 按同样的规格画出并导出自己的角色。每个终端单元格只有前景/背景两色，直接让模型「画 ASCII」往往会对不齐。

## What it does
在 2×2 子像素网格上画画，再编译成 Unicode 象限字符（`▘▝▀▖▌▞▛…`），可输出 ANSI、Ink 组件、Claude Code mod 或 SVG。技能名是 `quadrant-pixel-animator`：自包含，只需 Node 20+，不用再 `npm install`。仓库带 evals、rig 格式说明、编译/播放脚本和演示角色 Pip。

## Recipe / links
- Repo: https://github.com/LiquidRing/quadmotion（MIT，0★）
- 任意兼容宿主：`npx skills add LiquidRing/quadmotion`（或加 `-a claude-code -a codex -a cursor`，`-g` 装到用户级）
- Claude Code 插件：`/plugin install quadmotion --marketplace LiquidRing/quadmotion`
- 也可把 `skills/quadrant-pixel-animator` 拷进对应宿主的 skills 目录
- 源码演示：`git clone https://github.com/LiquidRing/quadmotion && cd quadmotion && npm run demo`

## Why it made the cut
有明确的终端动效场景、完整 SKILL.md / 脚本 / evals，不是一条提示词。社区信号仍为零，属于早期条目，安装前需自审。
