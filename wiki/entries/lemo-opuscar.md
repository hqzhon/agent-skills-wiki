# Lemo-Opuscar（影片风格 Skill 工具箱）

**Tags:** video, film-style, claude-code, skill-pack, code-render
**Source:** [@no_morenicotine](https://x.com/no_morenicotine/status/2114674148652024156) · 2026-10-26
**Engagement:** discovery post (low); repo ~7.8k★ / ~870 forks · 59 styles

## When to use
When you want a short film (≈30–60s) directed by a coding agent in a named visual style—whiteboard, watercolor, motion graphics, evidence/documentary, etc.—built entirely from code (canvas/Three.js + TTS + procedural audio + FFmpeg), not from a video-generation model.

## What it does
Open-source Claude Code skill / plugin packing 59 film styles. Each style ships a reusable `STYLE.md` prompt plus a code-made demo film. The agent follows DIRECTOR/TECHNIQUE guides: storyboard optional, then frame-by-frame render, voice, music, foley, subtitles, loudnorm mix. You can remix a library style or author a new one and keep it.

## Recipe / links
- Repo: https://github.com/lemomo-ai/lemo-opuscar (~7.8k★)
- Install (Claude Code):
  ```sh
  claude plugin marketplace add lemomo-ai/lemo-opuscar
  claude plugin install lemo-opuscar@lemolab
  ```
- Other agents: copy `plugin/skills/lemo-opuscar/` into the skills folder
- Site: https://lemomo-ai.github.io/lemo-opuscar/

## Why it made the cut
Concrete plugin/SKILL.md install path; clear film-from-code use case; large verifiable repo with 59 style recipes and technique docs.
