# Day Trader Skill pack

**Tags:** finance, trading, skill-pack, paper-trading
**Source:** [@yvshpvtil](https://x.com/yvshpvtil/status/2114567539841810657) · 2026-10-26
**Engagement:** discovery thread; repo ~1.7K★ (+~521/24h)

## When to use
When the user wants a coding agent to help with **day-trading research on free public data**—scan charts, watch news, time entries/exits, simulate outcomes—without auto-placing real orders.

## What it does
Eleven Claude skills (`trader-scanner`, `trader-news`, `trader-entry`, `trader-exit`, `trader-timemachine`, `trader-risk`, `trader-budget`, `trader-broker`, `trader-alerts`, `trader-analyst`, `trader-pelosi`) chained via a project `trader/` folder. Time Machine replays sessions; broker defaults to paper and requires explicit yes. Python tools use Yahoo Finance, Nasdaq lists, SEC EDGAR / House Clerk—no paid API required.

## Recipe / links
- Repo: https://github.com/Jakeschincariol/day-trader-skill (~1.7K★, MIT)
- Claude Code: `/plugin marketplace add Jakeschincariol/day-trader-skill` then `/plugin install day-trader-skill@day-trader-skill`
- Or copy `trader-*` folders into `~/.claude/skills/`
- Related long-horizon pack: https://github.com/Jakeschincariol/trader-skill

## Why it made the cut
Eleven real SKILL.md files, clear install, paper-first safety, and public tools—not a single “trade better” tip.
