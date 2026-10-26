# LinkedIn Creator Radar

**Tags:** linkedin, research, scraping, apify, claude-skill
**Source:** [@alexey_chernyak](https://x.com/alexey_chernyak/status/2114680230669340748) · 2026-10-26
**Engagement:** discovery post (low); brand-new repo with SKILL.md + scripts

## When to use
When you want to find which LinkedIn creators in a niche punch above their follower count, what formats they use, and which hooks win—without logging into LinkedIn yourself.

## What it does
Claude skill that takes LinkedIn profile URLs, pulls ~3 months of posts via Apify (no LinkedIn login/cookies), scores each author against their own median engagement, compares formats (text / image / video / document / link), and writes CSVs plus a one-page report. Treats scraped text as data only (ignores prompt-injection-style About text).

## Recipe / links
- Repo: https://github.com/blackyak/linkedin-creator-radar
- SKILL.md: https://github.com/blackyak/linkedin-creator-radar/blob/main/SKILL.md
- Install: copy into your Claude skills dir, or tell the agent to read `SKILL.md` and run the scripts (needs Apify)

## Why it made the cut
Concrete SKILL.md + scripts; clear competitor-research use case; verifiable GitHub package with install path.
