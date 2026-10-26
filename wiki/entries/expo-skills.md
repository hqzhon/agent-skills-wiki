# Expo Skills（官方）

**Tags:** expo, react-native, eas, skill-pack, official
**Source:** [@n7wb1l](https://x.com/n7wb1l/status/2114714122206183645) · 2026-10-26
**Engagement:** discovery post (low) · repo ~3.0K★ · Expo official

## When to use
When coding agents guess outdated Expo Router / EAS / React Native APIs — install the official Expo skill pack so the agent follows current Expo + EAS workflows (structure, router, animation, upgrades, updates, App Store submit).

## What it does
Official Agent Skills from the Expo team. Start with `expo-overview`, then route into framework skills (`expo-router`, `expo-animation`, `expo-native-ui`, `expo-design-system`, `expo-upgrade`, …) and paid-services skills (`eas-workflows`, `eas-update`, `eas-app-stores`, `eas-observe`, …). Docs/CLI remain source of truth; skills teach agents how to apply them. Optional Expo MCP for live docs/builds.

## Recipe / links
- Repo: https://github.com/expo/skills
- Docs: https://docs.expo.dev/skills/
- Skills CLI: `npx skills@latest add expo/skills --skill '*'`
- Claude Code: `claude plugin install expo@claude-plugins-official`
- Codex: `codex plugin add expo@openai-curated`

## Why it made the cut
Vendor-official SKILL.md pack with clear when-to-use table, one-command install across agents, and verifiable GitHub + docs — high reuse for any Expo/RN project.
