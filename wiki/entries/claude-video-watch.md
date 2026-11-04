# /watch（claude-video：让 agent 看视频）

**Tags:** video, transcription, multimodal, research, skill
**Source:** [@0xForce_](https://x.com/0xForce_/status/2117937493135761708) · 2026-11-04
**Engagement:** 仓库 bradautomates/claude-video，~19.8k★，MIT，2026-04 创建；已有多个 fork（mlx-whisper 本地版、西语版、Gemini 画面版）

## When to use
要让 agent 理解一段 YouTube / X / Vimeo / 本地视频：拆解爆款视频结构、从教程里提炼步骤、核对视频里说了什么和画面里出现了什么。

## What it does
`/watch <URL 或文件>` 先下载视频，抽取带时间戳的关键帧，再拿转录：优先用原生字幕，没有字幕时可选本地 WhisperX 或 Groq/OpenAI 转写；帧和转录一起交给 agent 分析。原帖的玩法是再接一段「distill」提示，把画面和台词合成一条节拍时间线，提炼出带时间戳的要点，沉淀成新的 skill。

## Recipe / links
- Repo: https://github.com/bradautomates/claude-video
- Claude Code 插件：`/plugin install watch@claude-video`（或在 Claude Desktop 的 Code 会话里通过 Customize → Plugins 添加该仓库）
- 其他 agent（Cursor、Copilot、Codex 等）：用 Skills CLI 安装，见 README
- 注意：不支持 Claude Chat / Cowork，需要能跑本地命令的 Code 会话

## Why it made the cut
场景清晰、安装路径完整、社区信号很强（近 2 万星且被多次 fork），补上 wiki 里「视频输入 / 视频理解」这一块，和已收录的各类视频生成 skill 互补。
