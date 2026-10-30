# next-bundle-optimizer（Next.js 官方捆包优化 Skill）

**Tags:** nextjs, vercel, bundle, performance, turbopack, skill, official
**Source:** [@poseidanai](https://x.com/poseidanai/status/2115957875994464644) · 2026-10-30
**Engagement:** tipster post; material = Next.js 16.4 official blog

## When to use
When a **Next.js 16.4+ (Turbopack)** app 的客户端 JS 膨胀，你想让 coding agent 顺着模块图找「该懒加载却被静态 import 拖进来」的边界，而不是盲砍依赖。

## What it does
Official agent skill shipping with Next.js: exports Turbopack module/chunk graph via `next analyze`, finds large connected groups, proposes minimum-cut import boundaries, and can also surface RSC moves, duplicate heavy deps, and failed tree-shaking. Default reports issues; `/next-bundle-optimizer fix` applies changes, re-analyzes, and diffs snapshots. Vercel reports ~2 MB compressed JS cut across v0 + vercel.com with agent-opened PRs.

## Recipe / links
- Blog: https://nextjs.org/blog/ship-less-javascript-with-ai
- Requires Next.js **16.4+** and Turbopack
- Install: `npx skills add vercel/next.js --skill next-bundle-optimizer`
- Run: `/next-bundle-optimizer` · apply: `/next-bundle-optimizer fix`
- Human analyzer: `next analyze` · export: `next analyze export`

## Why it made the cut
First-party Next.js skill with install command, concrete graph-driven recipe, and published production savings—watchlisted as next-bundle-optimizer and now verifiably public.
