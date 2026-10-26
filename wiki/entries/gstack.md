# gstack（Garry Tan / YC）

**Tags:** skill-pack, claude-code, review, qa, shipping, ycombinator
**Source:** [@benou_irl](https://x.com/benou_irl/status/2114719570632060952) · 2026-10-26
**Engagement:** discovery listicle · repo ~138K★ · MIT

## When to use
When you want Claude Code (or other agents) to act like a small eng team — CEO pushback, architecture lock, design anti-slop, production review, real-browser QA, security audit, and release/ship — via slash-command skills instead of one giant prompt.

## What it does
Garry Tan’s open “software factory”: opinionated Markdown skills/roles (`/office-hours`, `/review`, `/qa`, `/autoplan`, `/cso`, `/ship`, browse helpers, design reviews, etc.). Root `SKILL.md` + many skill folders; `./setup` installs for Claude Code and optionally other hosts (`--host auto` / codex). Team mode can require gstack for AI-assisted work in a repo.

## Recipe / links
- Repo: https://github.com/garrytan/gstack
- Install (Claude Code paste / clone): `git clone --single-branch --depth 1 https://github.com/garrytan/gstack.git ~/.claude/skills/gstack && cd ~/.claude/skills/gstack && ./setup`
- Multi-agent: clone to `~/gstack` then `./setup --host auto`
- Needs Bun (and Node on Windows); browser skills prefer Aside on macOS

## Why it made the cut
Named SKILL.md recipes with clear roles, one-command setup, huge community signal, and concrete “when” for shipping/review/QA loops — not empty hype.
