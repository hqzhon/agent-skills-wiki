# appsec-skills（Davide Imola / GoLab）

**Tags:** security, go, ci, fuzzing, skill-pack
**Source:** [@DavideImola](https://x.com/DavideImola/status/2115768150633709626) · 2026-10-29
**Engagement:** author talk promo; repo public MIT · Go pack first (TS next)

## When to use
When securing a **Go** repo for production: wire govulncheck / security CI, run an evidence-backed audit, or prove a suspected logic bug with a failing property/fuzz test before fixing—plain-language asks (“set up appsec-skills”, “audit this service”).

## What it does
Four Agent Skills (`appsec-setup`, `appsec-ci`, `appsec-audit`, `appsec-prove`) from Davide Imola’s GoLab 2026 talk. Skills write canonical assets that the repo’s own CI tests against real fixtures; every action pinned to full commit SHAs. Open Agent Skills format (Claude Code, Codex, Cursor, Copilot, Gemini CLI, …).

## Recipe / links
- Repo: https://github.com/davideimola/appsec-skills (MIT; formerly go-security-skills)
- Install: `npx skills add davideimola/appsec-skills`
- Start with `appsec-setup`; docs under `docs/agents/`
- Site overview: https://www.davideimola.dev/skills

## Why it made the cut
Concrete SKILL.md pack tied to a real talk checklist, install CLI, and CI-tested outputs—even with early star count—beats generic “secure your Go app” advice.
