# story-to-handdrawn-video（手绘日记动画）

**Tags:** video, remotion, handdrawn, chinese, storytelling, skill
**Source:** [@GitHub_Daily](https://x.com/GitHub_Daily/status/2116130539522683388) · 2026-10-30
**Engagement:** tipster; material = gnipbao/story-to-handdrawn-video ~2319★ MIT

## When to use
把**中文故事文案**或一组排好顺序的本地图片，做成 **3:4 竖屏静音手绘动画**（后期再配音/BGM），而不是一张张文生图再手工拼片、人物还对不上。

## What it does
Agent Skill + Remotion 渲染工程：Agent 规划分镜与角色 → 生图工具出「手写中文 + 插画」母图 → 本地脚本统一素材处理 → Remotion 导出 H.264。两种动效：**逐层绘制**（文字→黑白→彩色）与**右下角翻书**。内置约 327 项风格/配色资产，可用参考图收藏私有画风。

## Recipe / links
- Repo: https://github.com/gnipbao/story-to-handdrawn-video (~2319★, MIT)
- Install renderer: `git clone` → `npm ci` → `npm run check`（Node 20+ / Python 3.10+ / FFmpeg）
- Install skill: copy `skill-package/story-to-handdrawn-video` → `~/.claude/skills/` / `~/.codex/skills/` / `~/.agents/skills/`
- Optional: `export STORY_VIDEO_PROJECT=/abs/path/to/repo`
- Style library: https://story-handdrawn-style-library.vercel.app
- SKILL.md: `skill-package/story-to-handdrawn-video/SKILL.md`

## Why it made the cut
Clear Chinese bedtime/story use case, verifiable Remotion + SKILL.md package, strong stars and a concrete install path amplified by GitHubDaily—not a tipster-only pitch.
