# ja-zh-subtitles（日语视频 → 简体中文 ASS）

**Tags:** subtitles, japanese, chinese, whisper, video, skill
**Source:** [@jiamu_x](https://x.com/jiamu_x/status/2114631318944542743) · 2026-10-26
**Engagement:** discovery post (low); author install follow-up; MIT repo with SKILL.md + scripts/tests

## When to use
When you have one local Japanese MP4/MKV (film, TV episode, or anime episode) and need a quick Simplified Chinese `.zh.ass` sidecar for viewing—not a line-by-line coverage audit.

## What it does
Agent skill driven by whisper.cpp `large-v3` (no VAD on main pass) plus contextual translation into ASS. Pipeline: `init` → `transcribe` → translate with decision ledger (`direct`/`inferred`/`unclear`/`omit`) → `assemble`/`build`/`publish`. Does not modify the source video; translation may send transcript context to the active AI service (skill discloses this).

## Recipe / links
- Repo: https://github.com/jiamu-git/ja-zh-subtitles (MIT)
- Skill: `SKILL.md` + `references/workflow.md` + `scripts/`
- Codex/DSH install: ask the agent to install from that GitHub repo per README, configure deps/models/fonts, and check SKILL.md + CLI before overwriting an existing same-named skill

## Why it made the cut
Full SKILL.md with executable steps and scripts; clear single-file scope; verifiable OSS. Niche but reproducible.
