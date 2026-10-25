# Microsoft Skill Recorder — Screen Recording → SKILL.md

**Tags:** skill-authoring, microsoft, screen-capture, automation, copilot
**Source:** [@realfxw](https://x.com/realfxw/status/2114211826493714625) · 2026-10-25
**Engagement:** 0 likes / 1 repost / 3 replies / 1 bookmark

## When to use
When you can **do a task once on screen** but do not want to hand-write a fragile prompt or UI-replay script — turn that demonstration into a reusable agent skill / automation.

## What it does
Records screen actions, window switches, browser paths, embedded terminal commands, and optional local Whisper narration. Copilot reverse-engineers the trace into structured intent + ordered steps, preferring native tools (CLI/API) over brittle click coordinates. Local capture; analysis only when you opt in. Targets macOS and Windows 11 (incl. ARM64). Outputs usable with Scout / Copilot Cowork / Copilot Studio.

## Recipe / links
- Repo: https://github.com/microsoft/skill-recorder
- Record the task once → analyze → review generated SKILL.md / automation
- Check for sensitive data before sending the event stream to Copilot

## Why it made the cut
Microsoft OSS with a clear record→skill recipe, privacy model, and multi-platform support — high reuse potential for skill authors.
