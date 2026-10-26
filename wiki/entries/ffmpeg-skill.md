# ffmpeg-skill

**Tags:** video, ffmpeg, mcp, editing, skill, local
**Source:** [@Manojkumar2257](https://x.com/Manojkumar2257/status/2114592269961707987) · 2026-10-26
**Engagement:** roundup post (~1 like); also [@Nexo_Xing](https://x.com/Nexo_Xing/status/2114595943714824450); repo ~2.9k★

## When to use
When a coding agent should **edit local video/audio with FFmpeg**—cut, join, silence removal, 9:16 reframe, captions/karaoke, loudness, overlays, platform exports—**offline, no API keys**, and verify the file it just made.

## What it does
Agent Skill + MCP server: fixed workflow (probe → edit → check → verify) and **42 local FFmpeg tools** (core 12 advertised by default). Machine-readable contract derived from argparse (SPEC). Works with Claude Code, Cursor, Codex, and any MCP client. `npx ffmpeg-skill` if ffmpeg + python3 are on PATH.

## Recipe / links
- Repo: https://github.com/kajisho5/ffmpeg-skill (~2.9k★, MIT)
- npm: `npx ffmpeg-skill` · https://www.npmjs.com/package/ffmpeg-skill
- Demos: repo `docs/demos.md` (before/after GIFs + exact commands)
- Related ecosystem (optional): `video-production-agent`, `remotion-ffmpeg-skill`, etc. under the same author

## Why it made the cut
Concrete installable skill with SKILL.md, MCP, self-checks, and a large local tool surface—not a “prompt to edit video” tip.
