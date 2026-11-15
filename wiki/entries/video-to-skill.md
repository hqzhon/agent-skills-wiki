# video-to-skill（教程视频变成可验证 skill）

**Tags:** skill-authoring, video, whisper, local, meta, skill
**Source:** [@Vladic_ETH](https://x.com/Vladic_ETH/status/2121668506752061630) · 2026-11-15
**Engagement:** 发现帖 10 赞 / 3 回复；仓库 [brenoepics/video-to-skill](https://github.com/brenoepics/video-to-skill) 约 155★ / 21 forks，MIT；站点 [v2s.dev](https://v2s.dev)

## When to use
要把一小时的 Blender、剪辑或命令行教程变成 agent 以后能照着做的 skill，而不只是一份「视频摘要」。适合 YouTube 链接或本地视频；口播理论课、没有操作步骤的 vlog 不该硬生成步骤。

## What it does
本地 Rust 抽取器 `vts-extract` 在本机做下载、转写、分镜和关键帧（视频不离开机器，只有你选中的帧进入模型上下文）。agent 读时间线、对照画面里的命令和操作，写出有证据的步骤，再尝试在隔离环境里跑一遍：能验证的写进 skill，不能验证的标出来，而不是编造步骤。默认模式 `generate` 会编译、校验并装成可安装 skill；也可只要分析报告，或把新视频折进已有 skill。

## Recipe / links
- Repo: https://github.com/brenoepics/video-to-skill（~155★，MIT）
- 站点 / 文档：https://v2s.dev
- 安装：`npx skills@latest add brenoepics/video-to-skill`，然后按装上的 `SKILL.md` 设置 `vts-extract`（macOS / Windows 10+ / Linux）
- 用法：把 YouTube URL 或本地 `.mp4/.mkv/.webm/.mov` 交给 agent，说「把这个教程做成 skill」或触发词 video to skill / watch this video
- 边界：非流程型视频只出分析报告并说明为何不生成 skill；安装前应先看计划再确认写入

## Why it made the cut
配方具体（解说 + 画面 + 沙箱验证），使用场景清楚，有可验证的 MIT 仓库、本地抽取器和 SKILL.md。与 [book-to-skill](book-to-skill.md) 同属「材料 → skill」的元技能，但针对教程视频而不是书/文档。
