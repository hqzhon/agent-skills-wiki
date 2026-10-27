# yaya-skills（X Space 蒸馏笔记）

**Tags:** x-twitter, transcription, notes, local, skill-pack
**Source:** [@eatmoreduck98](https://x.com/eatmoreduck98/status/2114961845207621698) · 2026-10-27
**Engagement:** author announce (low) · repo ~8★ · MIT · Apple Silicon focus

## When to use
When you need an agent/pipeline to turn an **X Space** recording into speaker-attributed Chinese notes + a shareable card — locally (audio stays on device) — plus newer helpers like draft→local TTS with bilingual subs.

## What it does
Writer-oriented skill pack (`eatmoreduck/yaya-skills`). Flagship `yaya-xspace`: download → local ASR with speakers → LLM distill → `distilled.md` + share image (Swiss / other card styles). Atomic download/transcribe/diarize skills underneath. Recent update adds local English-draft grammar fix → MP3 + ZH/EN subs without uploading the manuscript.

## Recipe / links
- Repo: https://github.com/eatmoreduck/yaya-skills (~8★, MIT)
- Install: `npx skills add eatmoreduck/yaya-skills`
- Quick Space run: `bash skills/yaya-xspace/run.sh "https://x.com/i/spaces/<id>"`
- Platform note: README targets M-series Mac / local models

## Why it made the cut
Concrete SKILL pack + scripts, clear Space→notes use case, local-privacy story, and verifiable demo outputs — not a marketing farm.
