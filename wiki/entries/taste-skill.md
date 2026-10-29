# Taste Skill（design-taste-frontend）

**Tags:** design, frontend, anti-slop, art-direction, skill
**Source:** [@KeyoAPI](https://x.com/KeyoAPI/status/2115679485488148832) · 2026-10-29
**Engagement:** ~105k★ · MIT · art direction + real images + browser self-check

## When to use
When coding agents keep shipping **generic AI landing pages** and you need art direction, credited open-archive photography, and a real-browser anti-slop check before ship—including dashboards/app screens (v2.1).

## What it does
Single installable skill `design-taste-frontend`: reads the brief, deals researched art directions, builds with real public-domain/CC images, then inspects the page in Chrome/Edge/Chromium at multiple widths and iterates on top failures. App/dashboard path uses product-screen styles and quiet-panel rules. Needs Node 22+ and a local Chromium; no API keys for core loop (network only to fetch images).

## Recipe / links
- Repo: https://github.com/Leonxlnx/taste-skill (~105k★, MIT)
- Install: `npx skills add https://github.com/Leonxlnx/taste-skill --skill "design-taste-frontend"`
- Claude Code: `/plugin marketplace add Leonxlnx/taste-skill` then `/plugin install taste-skill@taste-skill`
- Classics / imagegen spin-offs: `Leonxlnx/taste-skill-classics`, `Leonxlnx/imagegen-skills`

## Why it made the cut
Executable multi-step SKILL.md with browser QA scripts, explicit when-to-use, and a massive verifiable open-source footprint.
