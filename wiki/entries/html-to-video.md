# html-to-video

**Tags:** video, html, canvas, ffmpeg, skill
**Source:** [@yaohongan2025](https://x.com/yaohongan2025/status/2114546206437502978) · 2026-10-26
**Engagement:** 1 like / 0 repost (discovery post; repo ~109★)

## When to use
When the user wants to **turn HTML/Canvas animations into MP4/GIF** without Remotion—product demos, data charts, title cards, timelines, vertical shorts—especially “AI wrote an HTML animation, make it a video.” Prefer this over Remotion when you do **not** want a React project; prefer Remotion for in-app editors / cloud render at scale.

## What it does
Deterministic HTML→video renderer: seek `frame(t)`, screenshot in headless Chromium, encode with ffmpeg. Ships `SKILL.md`, 11 templates, QA gate, multi-shot transitions, themes, alpha ProRes, SRT cues. Agents can edit CFG/story JSON and call `assets/render.sh`.

## Recipe / links
- Repo: https://github.com/wx4766/html-to-video (~109★, MIT)
- Skill file: `SKILL.md` at repo root
- Install deps: `npm install && npx playwright install chromium` (+ ffmpeg on PATH)
- Quick render: `bash assets/render.sh my.html --duration=6 --fps=60`
- WorkBuddy/Claude skill path: clone into skills dir, then `bash scripts/install-deps.sh`

## Why it made the cut
Real SKILL.md + runnable renderer + templates + QA, clear when-to-use vs Remotion, public MIT repo—not a promo GIF thread.
