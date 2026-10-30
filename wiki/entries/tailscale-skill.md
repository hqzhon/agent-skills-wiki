# Tailscale Skill（官方）

**Tags:** tailscale, networking, devops, tsnet, kubernetes, official, skill
**Source:** [@honglong0420](https://x.com/honglong0420/status/2116029695485710746) · 2026-10-30
**Engagement:** tipster post (~7 likes / 3 bookmarks); material = Tailscale official repo (~44★, BSD-3-Clause, Alpha)

## When to use
When a coding agent needs **可信的 Tailscale 产品知识**——家用 exit node、Aperture LLM API 治理、Kubernetes operator、`tsnet` 应用开发——而不是每次手动贴文档碎片。

## What it does
Official Tailscale agent skill (public Alpha): packs platform knowledge + references so Claude Code / Cursor / Codex / OpenCode / Pi 等兼容 Agent Skills 标准的工具，在碰到 Tailscale 任务时自己去翻技能内参考资料。文档语法会演进，技能会链到官方 docs 作为权威源；输出应视为起点而非终稿。

## Recipe / links
- Repo: https://github.com/tailscale/tailscale-skill
- Install: `npx skills add https://github.com/tailscale/tailscale-skill`
- Skill path: `skills/tailscale/SKILL.md` + `references/`
- Docs: https://tailscale.com/docs · release stages note Alpha = unsupported

## Why it made the cut
First-party vendor skill with clear install path, scoped networking/devops use cases, and verifiable `SKILL.md` tree—even as Alpha, better than pasting Tailscale docs into every chat.
