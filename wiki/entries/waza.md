# waza（Microsoft Agent Skills 评测 CLI）

**Tags:** evaluation, skill-authoring, cli, microsoft, skill-pack
**Source:** [@aidevnewss](https://x.com/aidevnewss/status/2115583693372952638) · 2026-10-29
**Engagement:** ~1485★ · MIT · Go CLI + docs + dashboard

## When to use
When you are **authoring or shipping agent skills** and need graded trials (YAML evals, fixtures, graders, CI gates) instead of vibes.

## What it does
Microsoft’s Go CLI/framework to create, test, grade, and improve agent skills (`SKILL.md`). Supports YAML eval suites, fixtures, built-in/remote graders, offline preflight, adversarial packs, result dashboard (`waza serve`), and GitHub Actions CI. Docs at microsoft.github.io/waza.

## Recipe / links
- Repo: https://github.com/microsoft/waza (~1485★, MIT)
- Docs: https://microsoft.github.io/waza/
- Install: `curl -fsSL https://raw.githubusercontent.com/microsoft/waza/main/install.sh | bash`
- Typical: `waza init my-project --no-skill` → `waza new skill my-skill` → `waza run my-skill`

## Why it made the cut
First-party Microsoft tooling for skill quality with real graders, evidence, and CI—not a prompt dump.
