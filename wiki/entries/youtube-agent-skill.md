# YouTube Agent Skill pack

**Tags:** youtube, content, hooks, retention, skill-pack
**Source:** [@Manojkumar2257](https://x.com/Manojkumar2257/status/2114592269961707987) · 2026-10-26
**Engagement:** listed in video-skills roundup; repo ~3.0k★

## When to use
When running a **YouTube channel with Claude**—scripts/hooks, title+thumbnail pairing, retention cliffs, Shorts extraction, SEO/chapters, comment triage—without auto-publishing (skills write; human uploads).

## What it does
**Eleven** Claude skills (`yt-script`, `yt-package`, `yt-edit`, `yt-comment`, `yt-plan`, `yt-viral`, `yt-retention`, `yt-shorts`, `yt-seo`, `yt-chapters`, `yt-audit`) plus six dependency-free Python helpers (hookscore, title linter, deadair EDL, chapters, retention, viral swipe). Shared `voice.md` for channel voice. MIT, no API key required.

## Recipe / links
- Repo: https://github.com/Jakeschincariol/youtube-agent-skill (~3.0k★, MIT)
- Claude Code: `cp -r skills/yt-* ~/.claude/skills/` or plugin marketplace `Jakeschincariol/youtube-agent-skill` → install `youtube-agent`
- Paste-to-chat: any single `SKILL.md` as a mode (loses the Python tools)

## Why it made the cut
Concrete multi-skill pack with scored hooks, retention tooling, and install paths—overlaps Hype Meter thematically but is a different, channel-ops-focused open pack.
