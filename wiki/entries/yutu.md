# yutu（YouTube API CLI / MCP / Skill）

**Tags:** youtube, cli, mcp, publishing, skill
**Source:** [@Manojkumar2257](https://x.com/Manojkumar2257/status/2115302418447749166) · 2026-10-28
**Engagement:** ~708★ · Apache-2.0 · Go CLI + MCP + skill

## When to use
When the agent must **talk to the YouTube Data API** for real—upload, retitle, thumbnails, playlists, comments, captions—rather than only draft scripts/hooks offline (see also existing `youtube-agent-skill` content pack).

## What it does
`yutu` is a Go **CLI + MCP server + Agent Skill**. The `youtube` skill teaches when/how to call MCP tools (read/write/destructive tiers with confirm-before-delete). Needs Google OAuth (`client_secret.json` + token cache).

## Recipe / links
- Repo: https://github.com/eat-pray-ai/yutu (~708★, Apache-2.0)
- Skill: `npx skills add eat-pray-ai/yutu --skill youtube`
- SKILL.md: https://github.com/eat-pray-ai/yutu/blob/main/skills/youtube/SKILL.md
- MCP: `yutu mcp` (stdio/HTTP) after OAuth setup

## Why it made the cut
Executable API surface with a real SKILL.md and MCP bridge—complements (does not duplicate) the content/hooks-focused youtube-agent-skill pack.
