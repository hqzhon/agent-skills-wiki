# mockship（ui-to-mock → mock-to-ui）

**Tags:** ui, prototyping, feature-flags, frontend, skill-pack
**Source:** [@marcellefter](https://x.com/marcellefter/status/2115223124858007921) · 2026-10-28
**Engagement:** new author post (low) · repo MIT · full SKILL.md pair

## When to use
When you need a **clickable mock inside an existing app** (real routes/theme, fake data, flag off by default) for product sign-off, then promote that approved mock to production code with APIs, i18n and tests—without the mock drifting into half-finished prod.

## What it does
Two Agent Skills: `ui-to-mock` builds a flag-gated mock in one feature folder with a `MOCK.md` hand-off; `mock-to-ui` turns an approved mock into production code, stopping if required API ops are missing. Stack-agnostic; follows project `AGENTS.md` / conventions.

## Recipe / links
- Repo: https://github.com/marcellefter/mockship (MIT)
- Install: `npx skills add marcellefter/mockship` or Claude plugin marketplace `marcellefter/mockship`
- Skills: `skills/ui-to-mock/SKILL.md`, `skills/mock-to-ui/SKILL.md`

## Why it made the cut
Concrete two-phase recipe with clear mock-vs-prod boundary, installable SKILL.md pair, and a verifiable open-source repo—not just a design rant.
