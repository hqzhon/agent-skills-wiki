# seo-canon（Google 官方搜索文档离线技能）

**Tags:** seo, google, documentation, schema, audit, skill
**Source:** [@abhayofc](https://x.com/abhayofc/status/2123046486216933575) · 2026-11-18
**Engagement:** 作者本人介绍帖（约 7 赞）；仓库 [Abhaysoft-inc/seo-canon](https://github.com/Abhaysoft-inc/seo-canon) 现 0★，MIT（2026-11-12 建仓，文档快照 2026-11-13；早期条目）

## When to use
要查「Google 对搜索怎么说、要求、支持或建议什么」，或要写/审查 JSON-LD、robots.txt、canonical、hreflang、sitemap、重定向，或对页面做 Google SEO 合规审计——即使对方没提官方文档。不要靠模型记忆里的旧要求作答。

## What it does
把 Google Search Central 与 crawler 文档（185 页）做成离线 Markdown，按页引用后回答、审计或生成合规输出（JSON-LD、robots 规则、hreflang、meta robots 等），并区分强制项与建议项，避免编造字段。可在线浏览打包后的文档：https://abhaysoft-inc.github.io/seo-canon/ 。作为 Claude Code 插件发布，也是单插件 marketplace。

## Recipe / links
- Repo: https://github.com/Abhaysoft-inc/seo-canon（MIT，0★）
- Claude Code 插件：`claude plugin install seo-canon --marketplace Abhaysoft-inc/seo-canon`（会话内也可用 `/plugin install seo-canon --marketplace Abhaysoft-inc/seo-canon`）
- 其他宿主：把 `skills/seo-canon/` 指给 agent；入口是 `SKILL.md`
- 浏览快照：https://abhaysoft-inc.github.io/seo-canon/

## Why it made the cut
和已有的 [SEO Prompt Master](seo-prompt-master.md) 等审计技能不同：这条把 Google 官方文档做成可引用的离线包，适合「不要凭记忆写 schema / robots」。仓仍新、星数为零，属早期收录；用前先看快照日期是否够新。
