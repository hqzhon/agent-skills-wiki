# Beautiful Rust

**Tags:** rust, best-practices, review, clippy, skill-pack
**Source:** [@Z3nlyte](https://x.com/Z3nlyte/status/2114496111851319608) · 2026-10-26
**Engagement:** 2 likes / 0 repost / 0 replies / 1 bookmark

## When to use
When a coding agent should **write or review idiomatic Rust** with explicit rule citations, not just “make it compile.”

## What it does
Two Agent Skills plus a drop-in Clippy config: `rust-best-practices` steers generation toward robust APIs/docs; `rust-review` produces a prioritized report citing the broken rule and the fix. Guidance is distilled from Google, rust-lang API Guidelines, Effective Rust, Rust Design Patterns, and Microsoft’s pragmatic guidelines—when sources disagree, the skill picks a side and explains why. Works with Claude Code, Codex, Cursor, Copilot, Gemini CLI.

## Recipe / links
- Repo: https://github.com/morganlinton/BeautifulRust (~705★)
- Skills live under `skills/` (`rust-best-practices`, `rust-review`); Clippy rules under `lints/`
- Install via the repo’s Agent Skills / Claude plugin layout; pin a commit before CI use

## Why it made the cut
Concrete dual-skill + lint package with named sources, installable SKILL folders, and a clear write/review split.
