# Video Compression Agent Skill（agent 批量压视频）

**Tags:** video, ffmpeg, hevc, macos, media, skill
**Source:** [@twannl](https://x.com/twannl/status/2116662004890964202) · 2026-11-01（Antoine van der Lee）
**Engagement:** author post; material = AvdLee/Video-Compression-Agent-Skill（新仓库，星少）

## When to use
一堆录屏、素材视频占空间，想让 Claude Code / Cursor / Codex 直接帮你压成 HEVC 或 H.264，又不想原文件被动。

## What it does
先探测本机能力（ffmpeg 或 macOS `avconvert`），判断哪些文件值得压（已高效的跳过），编码后逐个校验输出，绝不改原片。单个 Python 3 文件、零依赖、默认不联网。预设与作者的 iOS App 同一套逻辑。

## Recipe / links
- Repo: https://github.com/AvdLee/Video-Compression-Agent-Skill
- 任何读 `SKILL.md` 的 agent 可用；README 有安装说明（含 App 推广，可忽略）

## Why it made the cut
配方具体、安全默认（先判断、后校验、不碰原件），作者是知名 Swift 开发者；比 ffmpeg-skill 更聚焦「压缩」这一件事。
