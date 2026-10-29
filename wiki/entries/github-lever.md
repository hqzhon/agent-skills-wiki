# github/lever（Copilot 反馈环技能包）

**Tags:** skill-pack, github, copilot, feedback-loops, automation
**Source:** [@_Evan_Boyle](https://x.com/_Evan_Boyle/status/2115518284590420317) · 2026-10-29
**Engagement:** ~66★ · MIT · github org Copilot plugin

## When to use
When you want **feedback loops, safe delegation, and turning chores into Copilot automations**—Loop Cards, autonomy dials, PR shepherding—instead of babysitting the agent.

## What it does
Copilot plugin/skills mined from GitHub eng sessions. One `/lever` entrypoint routes to verbs: `loop` (Loop Card), `brief`, `automate`, `review`, `shepherd`, `refactor`, autonomy L0–L5, `steer`, `mirror`, etc. Skills that only read can auto-load; anything that pushes/files waits for an explicit `/lever` ask.

## Recipe / links
- Repo: https://github.com/github/lever (~66★, MIT)
- Install: `copilot plugin marketplace add github/lever` then `copilot plugin install lever@lever`
- Skills dir: https://github.com/github/lever/tree/main/skills
- Try: `/lever loop our test suite feels slow. just the card, don't change anything`

## Why it made the cut
Official github-org pack with clear when-to-use verbs, autonomy dials, and installable Copilot plugin—not empty hype.
