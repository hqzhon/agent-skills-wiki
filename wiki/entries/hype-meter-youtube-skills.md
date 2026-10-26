# Hype Meter — 3 YouTube Claude Skills

**Tags:** youtube, research, critique, news-digest, skill-pack
**Source:** [@tinycrewgo](https://x.com/tinycrewgo/status/2114268820806521204) · 2026-10-25 (promo in this hour)
**Engagement:** article post low; free GitHub pack, no email gate

## When to use
When you run a channel mostly alone and need help with **niche topic research**, **pre-publish critique**, or a **signed-in X news digest**—without pasting secrets into chat.

## What it does
Three free Claude skills under `lf03-claude-skills/`:
- **Trend Scout** — finds YouTube outliers vs a channel’s usual views (needs free YouTube Data API key in env)
- **Fresh Critic** — new-session SHIP/FIX review with ≤5 problems; optional paste-block for a second model
- **Daily Digest** — Claude-in-Chrome reads your X For You/Following (read-only) into one brief

## Recipe / links
- Repo: https://github.com/HypeMeter/hype-meter-templates → folder `lf03-claude-skills`
- Copy each skill folder into `~/.claude/skills/` (Claude Code / desktop Code tab)
- Triggers: “scout my niche”, “fresh critic this”, digest-style asks
- Keep API keys in env, not chat; keep X tab foreground while digest scrapes

## Why it made the cut
Concrete SKILL.md trio with install path, failure notes from real runs, and verifiable GitHub material—usable recipes, not growth-hack fluff.
