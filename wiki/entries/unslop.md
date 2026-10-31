# unslop（去 AI 味 UI）

**Tags:** design, ui, frontend, anti-slop, redline-review, skill
**Source:** [@GreatCreations_](https://x.com/GreatCreations_/status/2116343100214071596) · 2026-10-31（另见 [@TypingMindApp](https://x.com/TypingMindApp/status/2116397867929858484)）
**Engagement:** 帖子信号低；材料 = heydamir/unslop ~1.6k★（发布约 2 天），CC BY 4.0

## When to use
vibecoding 出来的页面一眼 AI 味（紫色渐变、发光、emoji 标签、喊叫式文案、间距不齐），想让 Claude Code 像设计师做 redline review 一样把仪表盘 / App / 落地页改出自己的性格；只有线上链接也能用。

## What it does
1. **Audit**：逐条列出 slop 迹象及其位置；若页面已经不错，只给小改建议。
2. **Direction**：先从产品本身提炼性格、世界观、1–2 个承载颜色的时刻和一个签名细节，改代码前先征求确认。
3. **Passes**：按 间距 → 颜色 → 图标 → 文案 → 字体 → 布局 → 细节 → 视觉 → 动效 的顺序逐轮修。
4. 可选：通过 fal / Replicate / OpenAI images 等生成 hero 视觉（每次付费生成前询问）；用 Playwright + ffmpeg 产出 <10 秒的「自我去 slop」方形短视频。

## Recipe / links
- Repo: https://github.com/heydamir/unslop （`skills/unslop/` 为技能目录，`examples/` 有两个 vibecoded 示例页）
- 安装：`git clone https://github.com/heydamir/unslop && mkdir -p ~/.claude/skills && cp -r unslop/skills/unslop ~/.claude/skills/`（单项目则放 `.claude/skills/`）
- 用法：`/unslop this dashboard`、`/unslop the hero of https://example.com`
- 技术栈无关：Next.js / React / Vue / Svelte / Tailwind / 纯 HTML+CSS

## Why it made the cut
步骤明确（审计 → 方向 → 分轮修）、先确认再改、仓库带示例可验证，两天内 1.5k+★ 且多个独立账号推荐。和 [impeccable](impeccable.md)（设计审美规则）、[stop-slop](stop-slop.md)（写作去 AI 味）互补，专攻已有 UI 的逐轮重设计。注意许可证是 CC BY 4.0（需署名）。
