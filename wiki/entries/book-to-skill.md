# book-to-skill（书本 → Agent Skill）

**Tags:** skill-authoring, books, knowledge-base, meta
**Source:** [@itsharmanjot](https://x.com/itsharmanjot/status/2114619397293957396) · 2026-10-26
**Engagement:** 4 likes · 5 bookmarks · 2 RTs · ~220 impressions; repo ~36k★

## When to use
When a technical book, brand guide, RFC set, or docs folder keeps getting re-opened—you want it distilled into an on-demand agent skill instead of dumping the whole PDF into context.

## What it does
Points at PDF/EPUB/DOCX/HTML/RTF/Kindle (etc.), builds `SKILL.md` + per-chapter files + glossary/patterns/cheatsheet. Chapters load only when asked (~24–51× fewer tokens than dumping the book). Cross-agent install via skills CLI.

## Recipe / links
- Repo: https://github.com/virgiliojr94/book-to-skill (MIT, ~36k★)
- Install: `npx skills add virgiliojr94/book-to-skill`
- Usage: `/book-to-skill ./my-book.pdf` then `/my-book <topic>`

## Why it made the cut
Concrete recipe + clear meta use case; large verifiable OSS; measured token savings and multi-host support.
