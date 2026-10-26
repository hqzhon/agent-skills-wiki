# jianshuo/claude-skills（视频本地化 & 内容生产）

**Tags:** video, localization, dubbing, subtitles, skill-pack, wechat
**Source:** [@Manojkumar2257](https://x.com/Manojkumar2257/status/2114622862141391004) · 2026-10-26
**Engagement:** low on discovery tweet; repo ~137★

## When to use
When you need end-to-end **transcribe → translate → dub → burn subs** on a video in one agent run, or related WeChat/short-form video production skills (segment, reframe, multicam).

## What it does
MIT skill pack for Claude Code / Codex / Cursor. Orchestrator `wjs-localizing-video` chains Whisper ASR, punctuated SRT translation, time-aligned TTS dub (edge-tts / 豆包), and final burn/mix. Bonus: segmenting, reframing 16:9→9:16, WeChat publishing, multicam sync.

## Recipe / links
- Repo: https://github.com/jianshuo/claude-skills (MIT, ~137★)
- Install: `git clone https://github.com/jianshuo/claude-skills ~/.claude/skills/wjs`
- Or marketplace: `claude plugin marketplace add jianshuo/claude-skills`
- Key skills: `wjs-localizing-video`, `wjs-transcribing-audio`, `wjs-translating-subtitles`, `wjs-dubbing-video`, `wjs-burning-subtitles`

## Why it made the cut
Concrete multi-skill video pipeline with install paths; clear creator use case; verifiable SKILL.md folders (README notes Codex CLI too).
