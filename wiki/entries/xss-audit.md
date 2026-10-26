# xss-audit

**Tags:** security, xss, react, typescript, static-analysis
**Source:** [@Z3nlyte](https://x.com/Z3nlyte/status/2114496111851315573) · 2026-10-26
**Engagement:** 1 like / 0 repost / 0 replies / 0 bookmarks

## When to use
When you want an agent to run a **deep static XSS audit** on a React/TS/JS codebase (mXSS, sanitizer bypass, Trusted Types, JSON-in-script, URL/protocol pitfalls) and write findings to a report—without modifying code.

## What it does
Single `SKILL.md` playbook with **14 search layers** (DOM sinks, attribute/event injection, URL/navigation anti-patterns, JS execution sinks, SVG/MathML/CSS, markdown pipelines, postMessage, etc.). Requires data-flow + context-correct sanitization checks; outputs `xss-audit-report.md`.

## Recipe / links
- Repo: https://github.com/songjianyang/xss-audit (~397★)
- Root `SKILL.md` is the skill; see `examples/` and `SECURITY.md`
- Combine with CSP/Trusted Types and dynamic testing; static checklist alone is not a guarantee

## Why it made the cut
Executable SKILL.md with explicit layers, sinks, and anti-patterns—verifiable security recipe, not hype.
