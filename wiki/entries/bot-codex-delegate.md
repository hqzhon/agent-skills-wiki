# bot-codex-delegate（Grok Bot → Codex app-server）

**Tags:** grok-bot, codex, delegation, session, skill
**Source:** [@realTaki42](https://x.com/realTaki42/status/2115543314183422342) · 2026-10-29
**Engagement:** 0★ · MIT · installable SKILL.md + scripts

## When to use
When a **Grok Bot** should run local Codex like a cloud agent: dispatch work, stay awake via waiter, wake on completion, steer/interrupt, reuse named sessions—without babysitting every turn.

## What it does
Resident `codex app-server` (ws localhost) + low-effort waiter subagent that foreground-blocks (~13 min Shell/AwaitShell) so the bot computer stays awake while Codex works. Skills cover setup, `codex-turn` / `codex_ws.py` (start/turn/steer/interrupt), session naming/reuse, safe defaults (`workspace-write` + on-request; full access opt-in only).

## Recipe / links
- Repo: https://github.com/realTaki/bot-codex-delegate (0★, MIT)
- SKILL.md: https://github.com/realTaki/bot-codex-delegate/blob/main/skills/bot-codex-delegate/SKILL.md
- Install: send SKILL.md link to Grok Bot; then `bash scripts/install-codex-app-server.sh`
- Note: root `SKILL.md` 404; real path is `skills/bot-codex-delegate/SKILL.md`

## Why it made the cut
Real installable skill + scripts solving a concrete Grok Bot↔Codex babysitting problem with clear safety defaults.
