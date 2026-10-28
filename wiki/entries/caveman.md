# caveman（省 Token 简答模式）

**Tags:** token-budget, writing, brevity, meta, skill
**Source:** [@ReignSwords](https://x.com/ReignSwords/status/2115318020092666115) · 2026-10-28
**Engagement:** ~115.6k★ · Apache-2.0 · measured token cuts in field reviews

## When to use
When coding-agent chat is **bloated with ceremony** (“Sure! I’d be happy to help…”) and you pay per token—want terse answers that keep code, paths, numbers, and negations intact.

## What it does
Skill `/caveman` switches the agent into a persistent **terse voice**: answer-first, kill filler, optional articles, payload (code/commands/errors) verbatim. Stays on until `stop caveman` / `normal mode`. Sibling compress skill for memory files (`/caveman-compress`). Also ships a proxy/CLI for broader harnesses.

## Recipe / links
- Repo: https://github.com/JuliusBrussee/caveman (~115.6k★, Apache-2.0)
- Docs: https://docs.caveman.so/caveman
- Skill: https://github.com/JuliusBrussee/caveman/blob/main/skills/caveman/SKILL.md
- Install: `npx @caveman-ai/cli@latest` (multi-agent) or copy skills folder

## Why it made the cut
Full SKILL.md with explicit safety exceptions (irreversible actions, security warnings), clear cost/use case, and a large verifiable project—not a meme-only prompt.
