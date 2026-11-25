# Cloudflare Skills（官方）

**Tags:** official, cloudflare, workers, agents-sdk, skill-pack
**Source:** [@Astrodevil_](https://x.com/Astrodevil_/status/2125446900103209152) · 2026-11-25
**Engagement:** 本窗官方盘点帖（0 赞）；仓库 [cloudflare/skills](https://github.com/cloudflare/skills) 现 3,450★，Apache-2.0，2026-11-24 仍有推送

## When to use
要用编码 agent 开发 Cloudflare Workers、Agents SDK、Wrangler，或把 Next.js / 其他框架部署到 Cloudflare 开发者平台时用。Claude Code / Codex 的插件还会一并带上 Cloudflare MCP 服务器。

## What it does
官方约 24 个技能，覆盖 Workers 开发与最佳实践、性能剖析、Wrangler、Durable Objects、Agents SDK、Email Service、Cloudflare One、Turnstile、Sandbox、网关 Workers 等。原生插件路径会同时装技能和 MCP；只支持 Agent Skills 标准的宿主可以只装技能。

## Recipe / links
- Repo: https://github.com/cloudflare/skills（3,450★，Apache-2.0）
- `npx skills add https://github.com/cloudflare/skills`
- Claude Code：`/plugin marketplace add cloudflare/skills` → `/plugin install cloudflare@cloudflare`
- Codex：`codex plugin marketplace add cloudflare/skills` 然后 `codex plugin add cloudflare@cloudflare`（装完需新开会话）

## Why it made the cut
Cloudflare 官方技能包，安装路径清楚，技能覆盖 Workers / Agents 主线，3,450★、Apache-2.0。与已有的 [cloudflare-security-audit-skill](cloudflare-security-audit-skill.md)（安全审计向）互补。
