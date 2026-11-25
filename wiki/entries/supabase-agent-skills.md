# Supabase Agent Skills（官方）

**Tags:** official, supabase, postgres, auth, skill-pack
**Source:** [@Astrodevil_](https://x.com/Astrodevil_/status/2125446900103209152) · 2026-11-25
**Engagement:** 本窗官方盘点帖（0 赞）；仓库 [supabase/agent-skills](https://github.com/supabase/agent-skills) 现 3,136★，MIT，2026-11-12 仍有推送

## When to use
编码 agent 要做 Supabase 开发时用：Database / Auth / Edge Functions / Realtime / Storage、RLS、迁移，或 supabase-js / SSR 在 Next.js、SvelteKit、Astro 等框架里的集成。不要把它当成通用 Postgres 教程——这边按 Supabase 产品与当前客户端 API 来写。

## What it does
官方两个技能：
- `supabase`：覆盖各产品、客户端库、CLI / MCP、schema 与安全审计；
- `supabase-postgres-best-practices`：Postgres 侧最佳实践。
文档称兼容 18+ 种编码 agent。

## Recipe / links
- Repo: https://github.com/supabase/agent-skills（3,136★，MIT）
- 文档：https://supabase.com/docs/guides/getting-started/ai-skills
- 安装全部：`npx skills add supabase/agent-skills`
- 只装一个：`npx skills add supabase/agent-skills --skill supabase` 或 `--skill supabase-postgres-best-practices`
- Claude Code：`claude plugin marketplace add supabase/agent-skills`，再 `claude plugin install supabase@supabase-agent-skills`

## Why it made the cut
Supabase 官方包，两个技能分工清楚，有官方文档和标准安装命令。3,136★、MIT。本窗盘点帖互动低，按官方仓库补收。
