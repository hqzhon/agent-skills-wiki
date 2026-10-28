# coding-agent-skills（证据驱动审计包）

**Tags:** engineering, audit, safety, evidence-pack, skill-pack
**Source:** [@JohnWOE15](https://x.com/JohnWOE15/status/2115411585954943355) · 2026-10-28
**Engagement:** MIT · evidence-pack contract · audit-only default

## When to use
When a coding agent should **inspect before acting**—repo map, routes, env/secret names (no values), API contracts, migrations, deploy preflight, build-verify—and keep audit results separate from application validation.

## What it does
Shared pilot pack with an evidence-pack completion standard: `repo-map`, `route-trace`, `env-audit`, `secret-audit`, `api-contract-audit`, `migration-review`, `github-handoff`, `deployment-preflight`, `build-verify`, `git-preflight`, `runtime-truth`, `llm-drift-control`, plus `validate-pack` for the installed workflows (not the app).

## Recipe / links
- Repo: https://github.com/AyobamiH/coding-agent-skills (MIT)
- Docs: architecture / safety / authoring under `docs/`

## Why it made the cut
Clear audit-vs-action split, concrete skill list, and an explicit evidence contract—installable engineering hygiene, not another “agent marketplace” pitch.
