# deed-page（一键发布静态页）

**Tags:** publishing, hosting, static-site, mcp, skill
**Source:** [@Avatar8Ops](https://x.com/Avatar8Ops/status/2114857354625708350) · 2026-10-26
**Engagement:** launch post (low) · MIT skill + hosted MCP

## When to use
When the agent generated HTML/docs/a prototype and you need a permanent public URL ("put this on the web") without signing up, API keys, or email confirmation — including unattended runs.

## What it does
One `SKILL.md` (+ optional remote MCP at `https://deed.page/mcp`) that publishes a file or folder to `https://<slug>.deed.page/` with a single `curl`. No account to start; first publish mints an owner token for later update/delete. Works in Claude Code, Codex, Cursor, Gemini CLI, Grok Bot, Hermes. Static files only — do not publish secrets.

## Recipe / links
- Repo: https://github.com/f-o-x11/deed-page-skill
- Skill path: `skills/deed-page/SKILL.md`
- Install: `npx skills add f-o-x11/deed-page-skill`
- MCP: `https://deed.page/mcp` · docs https://deed.page/docs
- Site: https://deed.page

## Why it made the cut
Concrete installable SKILL.md with a crisp publish scenario, verifiable repo + MCP, and cross-agent packaging — fills the "share the artifact" gap many skill packs skip.
