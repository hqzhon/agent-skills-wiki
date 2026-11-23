# formant-voice（Klatt 式共振峰合成语音 + 频谱视频）

**Tags:** audio, speech-synthesis, formant, video, ffmpeg, skill
**Source:** [@NyxYujin](https://x.com/NyxYujin/status/2124830587508707433) · 2026-11-23（v1.1 更新；首发帖 [2124670759217803627](https://x.com/NyxYujin/status/2124670759217803627)）
**Engagement:** 本窗更新帖信号低；首发帖 6 赞 / 1 转发 / 约 1.8 万浏览。材料为作者站点可下载的 zip（MIT），内含 SKILL.md、Klatt 合成脚本与日英 README，无 GitHub 仓库。

## When to use
要让 agent 用「纯数学」做出复古/机器感语音（DECtalk 那一路），不要录音、也不要 TTS 模型；同时需要频谱图视频（横屏 YouTube/X，或 TikTok/Shorts/Reels 竖屏，或两者都要）并做合成自检。

## What it does
用 Klatt 式共振峰合成：声门脉冲与噪声经过级联共振滤波器，模仿声道。agent 先写音标，再渲染，并对照目标共振峰和频谱自检。每段文本可得到：
- `.wav` 语音（22050 Hz）
- 横屏 16:9 频谱视频（词对齐标签 + 播放头），可选竖屏 9:16（大字幕跟随当前词）
- 缩略图 `.png`；多段可合并为 `joined.wav` / `joined.mp4`（竖屏另有 `joined_vertical.mp4`）

v1.1 新增 `--layout wide | vertical | both`：提到 TikTok / Shorts / Reels /「竖屏」时走竖屏，多平台分发时两者都出，并抽竖屏中间帧核对字幕与播放头是否对齐。

## Recipe / links
- 项目页：https://nyxyujin.com/skills/formant-voice
- 下载：https://nyxyujin.com/downloads/formant-voice-skill.zip（MIT，Copyright 2026 NyxYujin）
- 安装：解压后把含 `SKILL.md` 的 `formant-voice/` 文件夹拷到 `~/.claude/skills/`（Claude Code）或 `~/.agents/skills/`（Codex），重启后用 `/formant-voice` 或直接下指令
- 依赖：Python 3.10+（numpy / scipy / matplotlib，agent 可建本地 venv）、出视频需要 ffmpeg

## Why it made the cut
不是套一层商业 TTS：合成器、音标、频谱自检和出片脚本都在 zip 里，步骤可验证。首发帖因没写「SKILL.md / agent skill」短语漏出搜索窗，本窗 v1.1 更新把它补上。和 ElevenLabs 等云端语音 skill 路线完全不同，适合要复古声线或可离线复现的场景。
