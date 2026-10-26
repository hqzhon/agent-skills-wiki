# Answer me with HTML

**Tags:** output-format, html, diagrams, explainer, skill-pack
**Source:** [@fernandoabishai](https://x.com/fernandoabishai/status/2114522497076850964) · 2026-10-26
**Engagement:** 0 likes / 0 repost / 0 replies (discovery post)

## When to use
When a coding agent should answer **hard / multi-part questions as one offline HTML page** (diagrams, tables, comparisons, timelines) instead of a wall of Markdown—or when the user asks to “explain in HTML” / wants explainer-video style pages.

## What it does
Model writes a short Markdown draft; bundled CLI (`am`) lays out panels, themes, sequence/flow/ER/tree/timeline charts (~8× fewer output tokens vs hand-written HTML per their bench). Optional always-on mode, ASD-STE100 writing checks, and 3b1b-style explainer videos. Works across Claude Code / Cursor / Codex / 70+ agents via `npx skills add`.

## Recipe / links
- Repo: https://github.com/QingYunA/answer-me-with-html (MIT)
- Skill folder: `skills/answer-me-with-html/` (+ INSTALL.md for agent-led install)
- Install: `npx skills add QingYunA/answer-me-with-html` or paste INSTALL.md to the agent; needs Node ≥20

## Why it made the cut
Full Agent Skill layout with install docs, bench numbers, and a reusable output recipe—not news or a concept list.
