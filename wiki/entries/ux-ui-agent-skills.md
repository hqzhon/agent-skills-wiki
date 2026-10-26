# UX/UI Agent Skills（XIAS / plugin87）

**Tags:** design, ui-ux, accessibility, design-system, skill-pack, gates
**Source:** [@thanhmam](https://x.com/thanhmam/status/2114711263309926414) · 2026-10-26
**Engagement:** discovery post (low) · repo ~3.0K★ · MIT

## When to use
When agents ship screens that look slightly different each time and treat accessibility as a guess — load a design-system doctrine pack with tokens, components, and **objective gates** (many browser-based) that fail the build instead of rubber-stamping “looks fine.”

## What it does
aka **XIAS**: DTCG tokens, component specs, large design-system library, 26 runnable skills, and ~50+ gates targeting WCAG 2.2 AA→AAA (contrast, axe, keyboard, target size, overflow, tokens-by-intent, …). Works across frameworks; Claude Code plugin + Homebrew + npx paths. Distinct from lighter UI taste packs (e.g. ui-ux-pro-max) because of measurable gates.

## Recipe / links
- Repo: https://github.com/plugin87/ux-ui-agent-skills
- Live demo: https://plugin87.github.io/ux-ui-agent-skills/
- Claude Code: `/plugin marketplace add plugin87/ux-ui-agent-skills` then `/plugin install ux-ui-agent-skills@ux-ui-agent-skills`
- Homebrew: `brew install plugin87/tap/ux-ui-agent-skills`
- Browser gates need Chrome / `npx playwright install chrome`

## Why it made the cut
Concrete skill pack + verifiable repo + clear a11y/design-system when-to-use; gates make “success” checkable rather than vibes-only.
