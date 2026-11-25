# Oxylabs Web API Skills（官方：实时搜索 / 读网页）

**Tags:** official, oxylabs, web-search, scraping, mcp, skill-pack
**Source:** [@Sophia_Ai0](https://x.com/Sophia_Ai0/status/2125251160173093204) · 2026-11-24
**Engagement:** 介绍帖 57 赞 / 12 转发 / 15 收藏；仓库 [oxylabs/web-api-skills](https://github.com/oxylabs/web-api-skills) 现 14★，MIT，2026-11-23 仍在推送

## When to use
编码 agent 需要**当前**网页或搜索结果时用：查最新文档与新闻、读会被普通 HTTP 拦截的页面、做竞品或公司资料调研。不要用它读写本地文件、git、包管理或改代码。这是 Oxylabs 官方技能，走他们的 Web API（需单独申请该产品的 key，其它 Oxylabs 产品的 key 不能用）。

## What it does
官方技能包，当前三个技能：
- `oxylabs-web-api`：经 MCP 或 HTTP 搜索/读页，结果可按目标国家排序，走反爬通道；
- `oxylabs-web-research`：多源网页调研；
- `migrate-to-oxylabs`：从 Tavily / Exa / Firecrawl / Perplexity / Brave / Linkup 迁过来。
技能要求优先用它而不是模型记忆或内置搜索。Claude Code / Cursor 插件可一并接上 Oxylabs 托管 MCP。

## Recipe / links
- Repo: https://github.com/oxylabs/web-api-skills（14★，MIT）
- 通用安装：`npx skills add oxylabs/web-api-skills`
- Claude Code 插件（技能 + 托管 MCP）：
```
/plugin marketplace add oxylabs/web-api-skills
/plugin install oxylabs-web-api@oxylabs-web-api
```
  启用时会要 Web API key，存在系统钥匙串；之后可用 `/plugin configure oxylabs-web-api@oxylabs-web-api` 更换。
- Cursor：Marketplace 安装 **Oxylabs Web API**，在 Plugins → Configure 里设置 `OXYLABS_WEB_API_KEY`。
- 也可 `git clone` 后跑 `./install.sh`，或把 `skills/*` 拷进 `~/.claude/skills/`。
- 注意：必须在 [Oxylabs dashboard](https://dashboard.oxylabs.io) 创建 **Web API** 实例再生成 key。这是商业 API，用量与计费以官方为准。

## Why it made the cut
厂商官方包，三个可加载 SKILL.md、安装和鉴权路径清楚，使用边界写得很硬。本窗有 57 赞的专门介绍。和已收录的 You.com 等搜索技能互补，但这边依赖 Oxylabs 付费/账号体系，条目里必须写明。
