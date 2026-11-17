# SEO Prompt Master（技术 SEO / GEO 审计）

**Tags:** seo, geo, audit, cli, skill
**Source:** [@DanKornas](https://x.com/DanKornas/status/2122795905602740651) · 2026-11-18
**Engagement:** 发现帖 6 赞 / 6 收藏 / 720 次展示；仓库 [umutxyp/Seo-Promt-Master](https://github.com/umutxyp/Seo-Promt-Master) 现 591★ / 318 forks，MIT

## When to use
要检查站点能不能被搜索引擎和 AI 爬虫真正抓到、索引：robots.txt、sitemap、canonical、hreflang、结构化数据、软 404、AI 爬虫放行等，并且希望 agent 按引用过的官方规则去修，而不是凭记忆给过时建议。

## What it does
四件套：引用 Google Search Central / web.dev / Bing / Yandex / Apple 等公开文档的知识库（`docs/01`–`docs/18`）、可安装的 `seo-audit` skill、47 条分类提示词，以及零依赖的 `tools/seo-audit.mjs`（Node 18+）。工具对照「代码里打算怎样」和「线上实际返回什么」，输出 SEO / GEO 分数、爬虫放行矩阵和分级发现；P1 未关闭时退出码为 1，可做发布门禁。也可以只跑 CLI：`npx github:umutxyp/Seo-Promt-Master --url https://your-site.com --md seo-report.md`。作者写明它不评估内容质量、站外权威和来自 CrUX 的真实 CWV。

## Recipe / links
- Repo: https://github.com/umutxyp/Seo-Promt-Master（MIT，591★；仓库名里的 Promt 是原项目拼写）
- 只出报告：`npx github:umutxyp/Seo-Promt-Master --url https://your-site.com --md seo-report.md`
- 给当前项目装 skill：
  ```bash
  git clone https://github.com/umutxyp/Seo-Promt-Master.git
  cd /path/to/your-project
  bash /path/to/Seo-Promt-Master/install.sh
  ```
  随后对 agent 说 `run the SEO audit`。安装脚本会写入 `.claude/skills/seo-audit/SKILL.md`、`AGENTS.md`、Cursor rules、`GEMINI.md` 和 Copilot instructions。

## Why it made the cut
场景清楚，有可运行的零依赖审计工具、带出处的知识库和标准 SKILL.md，星标也够看。与已收录的文案/SEO 技能包不同，它偏技术面与 AI 搜索可见性，并要求用工具验证而不是口头保证。
