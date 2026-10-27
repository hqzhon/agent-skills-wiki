# z-video-downloader

**Tags:** video, download, yt-dlp, local, skill
**Source:** [@0x8888](https://x.com/0x8888/status/2115008350035284383) · 2026-10-27
**Engagement:** discovery post (low) · pack `tjxj/z-skills` ~575★

## When to use
When the user pastes a **video URL / URL list / media inventory** and wants it saved locally (YouTube, Bilibili, X, TikTok, 抖音, Instagram, Facebook, 微信视频号, common direct links) with optional subtitles, cover, resume, and a download report.

## What it does
Agent skill under `tjxj/z-skills`: wraps `yt-dlp` + scripts for batch/resume/archive, cookies retry, WeChat Channels via online resolver, optional Invidious fallback for YouTube bot checks. Writes under `Video/Downloads/` with `download-report.md`.

## Recipe / links
- Skill path: https://github.com/tjxj/z-skills/tree/main/z-video-downloader
- Pack: https://github.com/tjxj/z-skills (~575★)
- Caveat: SKILL.md hardcodes author local paths (`miniconda3`/`yt-dlp`); adapt interpreter paths before first run

## Why it made the cut
Concrete SKILL.md + scripts + evals, clear download workflow, verifiable pack with solid stars — not a “use yt-dlp” tip alone.
