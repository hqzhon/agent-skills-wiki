# Music Video Generator（TheMarco）

**Tags:** video, music, claude-code, plugin, ffmpeg
**Source:** [@AIandDesign](https://x.com/AIandDesign/status/2114421153909596522) · 2026-10-25 (shared again in this hour)
**Engagement:** ~20 likes / 2 reposts / 13 replies / 7 bookmarks; repo ~1★

## When to use
When you want Claude Code to **autonomously cut a music video to the beat**—archive.org or your own footage, optional AI performer clips via any video MCP, then local GPU composite with per-video overlays.

## What it does
Claude Code plugin/skill: beat-grid + section analysis, footage gather, optional MCP video gens (Hedra/Runway/etc.), cut to beat, render 16:9 / 9:16 / square with original audio. Supports “edit 0:43–0:56…” feedback after a first render. History file avoids repeating earlier looks.

## Recipe / links
- Repo: https://github.com/TheMarco/claude-music-video
- Install: `claude plugin marketplace add TheMarco/claude-music-video` then `claude plugin install music-video-generator@music-video`
- Or copy `plugins/music-video-generator/skills/music-video/` → `~/.claude/skills/music-video/`
- Needs: Claude Code, Python 3.10–3.13, ffmpeg, GPU with OpenGL 3.3; start with `/music-video` or ask in plain language

## Why it made the cut
End-to-end recipe with install commands, clear trigger, and a public plugin repo—not a demo-only clip dump.
