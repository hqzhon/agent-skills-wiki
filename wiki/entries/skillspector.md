# SkillSpector — Pre-Install Agent Skill Security Scanner

**Tags:** security, skill-safety, nvidia, scanning, install-hygiene
**Source:** [@guangGitHub](https://x.com/guangGitHub/status/2112204122833183182) · 2026-10-19
**Engagement:** 0 likes / 0 reposts / 0 replies / 1 bookmark

## When to use
**Before installing** a third-party Agent Skill (repo, zip, directory, or single file) — especially when you maintain a team skill library or pull skills from GitHub without reading every file.

## What it does
NVIDIA-open-sourced scanner that looks for prompt injection, data exfiltration, dangerous code, and permission-related risks. Runs static analysis first; optional LLM pass for semantic judgment. Emits risk levels, locations, and remediation suggestions.

## Recipe / links
- Repo: https://github.com/nvidia/skillspector
- Point it at a skill repo / archive / folder / file
- Review the report (severity + optional LLM findings) before you install
- Treat findings as clues; still read the SKILL.md and scripts yourself

## Why it made the cut
Clear when-to-use (pre-install), concrete OSS recipe from NVIDIA, and actionable security workflow — not hype.
