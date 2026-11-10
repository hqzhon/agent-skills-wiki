# cinecode（用代码拍短片）

**Tags:** video, film, rendering, motion, skill
**Source:** [@CreativeAiNinja](https://x.com/CreativeAiNinja/status/2119871501331579179) · 2026-11-09
**Engagement:** 发现帖 · sarpstar/cinecode · MIT · ~1.9k★

## When to use
想让编码 agent（Claude Code / Cursor / Codex）从一句创意直接产出**可播放的 MP4**：短片、长 YouTube 视频、广告、讲解片或 MV，而不是只拿到脚本或分镜。

## What it does
根目录 `SKILL.md` + `AGENTS.md` 定义流程：agent 先写剧本，再用代码逐帧构建画面（附 `starter/`、`templates/`、`styles/` 风格预设与 `references/`），最后用 `scripts/` 渲染合成成片。README 有土耳其语、英语、日语、简中多版本。

## Recipe / links
- Repo: https://github.com/sarpstar/cinecode （MIT）
- 入口：[`SKILL.md`](https://github.com/sarpstar/cinecode/blob/main/SKILL.md) · [README.zh-CN](https://github.com/sarpstar/cinecode/blob/main/README.zh-CN.md)
- 用法：把仓库放进 agent 的 skills 目录（或在仓库里直接开 agent），描述想要的片子，按 SKILL.md 走「剧本 → 逐帧代码 → 渲染」

## Why it made the cut
真实 SKILL.md + 模板/脚本/测试齐全，场景清晰（代码生成视频成片），近 2k 星可验证；与 huashu-motion 等发布片 skill 互补，覆盖叙事短片。
