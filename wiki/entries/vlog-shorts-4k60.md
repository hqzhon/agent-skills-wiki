# vlog-shorts-4k60（实拍短视频或墨线漫画：画面与字幕分层）

**Tags:** video, shorts, subtitles, ffmpeg, playwright, chinese, skill
**Source:** [@YiFuBai](https://x.com/YiFuBai/status/2125110945131479048) · 2026-11-24
**Engagement:** 本窗为作者发布帖（互动接近于零），仓库链接在回复中；仓库 [lovemage/vlog-shorts-4k60](https://github.com/lovemage/vlog-shorts-4k60) 现 2★，MIT，有多语 README

## When to use
要做竖屏短视频（TikTok / YouTube Shorts / Reels），并且不想把底片送进浏览器渲染、也不想让 AI 视频模型直接「画字」时用。一条铁则：底片（手机实拍或 AI 2D 画面）不走浏览器；浏览器（HyperFrames / Playwright）只渲染透明的字幕/HUD 层，再用 ffmpeg 叠到高码率画面上。

## What it does
v2 双模式可加载技能（根目录 \`SKILL.md\`）：
- Mode A：把手机 vlog 片段切成 4K 60fps 竖屏短片，带多语言字幕、信息标签、可选克隆配音；
- Mode B：把脚本做成 2D 墨线 POV 互动漫画短片（约 70–95 秒），字幕和 HUD 用 Playwright 透明层叠加，可用 \`--lang th|en\` 做零额外 GPU 的双语分发。
作者强调同一套画面可以出泰/英等版本，而不必把底片再渲染一遍。

## Recipe / links
- Repo: https://github.com/lovemage/vlog-shorts-4k60（2★，MIT）
- 安装：\`npx skills add lovemage/vlog-shorts-4k60\`，或按多语 README 把技能目录拷到 Claude Code / Codex / Cursor 等
- Skill: 仓库根目录 [SKILL.md](https://github.com/lovemage/vlog-shorts-4k60/blob/main/SKILL.md)
- Mode A 模板在 \`template/\`，Mode B 相关材料在 \`template_pov_comic/\` 与 \`docs/\`
- 成片流程依赖 ffmpeg 等本地工具；若用到克隆配音或外部视频模型，需另行准备并注意各段素材许可。

## Why it made the cut
星数很低，但铁则和双模式配方写得很清楚，有可加载 \`SKILL.md\` 和多语文档，和已收录的 [stickman-video-director](stickman-video-director.md)、[subtitle-skills](subtitle-skills.md)、[boring-video-studio](boring-video-studio.md) 互补：这边抓的是「底片不进浏览器、字不让模型画」。本窗即作者开源说明。
