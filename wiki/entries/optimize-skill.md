# /optimize（31 项性能体检）

**Tags:** performance, frontend, database, audit, grok-bot, skill
**Source:** [@sebbsssss](https://x.com/sebbsssss/status/2119358044060762414) · 2026-11-08
**Engagement:** 23 likes / 2 reposts / 6 replies / 13 bookmarks · sebbsssss/optimize-skill · MIT

## When to use
你要检查并改进 Web 应用的速度（N+1 查询、重复读取、串行 API、过重前端、阻塞任务、AI 整段响应等），而且希望先测量、只做安全修复、再对比前后数字。

## What it does
可移植的 31 项体检 skill：先摸清技术栈并跑同一套基线脚本，覆盖感知速度、资源、渲染、网络、后端/数据库和可观测性六组。每项给出 Pass / Fixed / Recommend / Needs decision / N/A，并要求代码或测量证据。安全、可逆的修复打在新分支上，然后重跑同一脚本，写出带前后对比的 `OPTIMIZE_REPORT.md`。不会擅自安装 Redis/队列/CDN、跑生产迁移、改 API 响应、commit/push 或部署；这些只作为建议或等你拍板。作者称在一个内部应用上修掉重复页面加载和重复读数后，从选角色到看到总览的重复访问时间降了 32–40%。

## Recipe / links
- Repo: https://github.com/sebbsssss/optimize-skill （MIT）
- Claude Code: 把文件夹拷到 `~/.claude/skills/optimize/` 或项目内 `.claude/skills/optimize/`，需要时会自动加载，也可打 `/optimize` 或 `/optimize audit only`
- Cursor: `.cursor/skills/optimize/`、`.agents/skills/optimize/` 或 `~/.cursor/skills/optimize/`（也能读 `.claude/skills/`）
- Grok Bot: 把 raw `SKILL.md` 贴给 bot，让它存成名为 `optimize` 的 skill，再说 run the optimize audit
- 31 项清单和安全规则见仓库 README

## Why it made the cut
作者公开了完整配方：先测后改、单独分支、证据门和付费基建禁区都写进 skill，适用 Claude Code / Cursor / Grok Bot，不是空喊「让 AI 优化性能」。
