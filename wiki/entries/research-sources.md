# research-sources（rsrc：补上搜索引擎看不到的 X / Reddit / HN）

**Tags:** research, cli, x, reddit, hacker-news, youtube, skill
**Source:** [@ai_researchad](https://x.com/ai_researchad/status/2126559388840464591) · 2026-11-28
**Engagement:** 本窗两条介绍帖互动都很低（0 赞）；仓库 [SamuelZ12/research-sources](https://github.com/SamuelZ12/research-sources) 现 244★ / 11 forks，MIT，2026-11-20 建仓。@AlphaByPablo 的跟帖补了只读边界和非官方接口的提醒。

## When to use
已经有网页搜索，但还想按各站自己的结果读 X、Reddit、Hacker News、YouTube、公开 LinkedIn 帖或 App Store 列表/评论，并且希望输出是同一种 JSON 时用。它是只读 CLI + 可加载技能，不写报告、不排序、不缓存。若要一份写好的近 30 天综述，用已收录的 [last30days](last30days-skill.md)；中文平台（小红书/B 站/知乎）用 [last30days-cn](last30days-skill-cn.md)。给 Muse 补只读 X 搜索则是 [muse-grok-x-search](muse-grok-x-search.md)。仓库自己也把这三条边界写在 README 里。

## What it does
命令行工具 `rsrc`（Python 3.11+，用 uv 安装，除标准库外无其它 Python 依赖）按来源提供 `read` / `search` 等子命令，成功、空结果和失败都走同一套 JSON 与退出码。可加载技能 `skills/research-sources/SKILL.md` 告诉 agent 什么问题用哪条命令、以及登录墙、验证码、限流时该怎么处理。

| 来源 | 额外准备 |
| --- | --- |
| X（读帖/串/回复/时间线；搜索需会话） | 仅搜索需要你自己的 X 会话 |
| Reddit | 搜索和直播帖需 Ego Lite；否则 `reddit read` 走公开 Arctic Shift 归档 |
| Hacker News | 无 |
| YouTube（含字幕） | `yt-dlp`，读详情还需 `deno` |
| LinkedIn（公开帖和评论） | 无 |
| App Store（列表和评论） | 无 |

**限制（装前必看）：** 只读，不发帖、不点赞、不关注。X、Reddit、YouTube、LinkedIn 和 App Store 走的是非官方途径，站点条款可能限制自动访问，路由也可能随时失效；X / Reddit 搜索用的是你自己的会话，不要高频打。维护者写明目前主要在 macOS 上测过，项目仍早。

## Recipe / links
- Repo: https://github.com/SamuelZ12/research-sources（244★，MIT）
- 安装 CLI：
  ```bash
  uv tool install git+https://github.com/SamuelZ12/research-sources
  rsrc check hn appstore
  ```
- 安装技能：`npx skills add SamuelZ12/research-sources`，或把 `skills/research-sources` 拷进 agent 的 skills 目录
- 技能正文：https://github.com/SamuelZ12/research-sources/blob/main/skills/research-sources/SKILL.md
- X 会话说明：https://github.com/SamuelZ12/research-sources/blob/main/docs/x-session.md

## Why it made the cut
有可安装 CLI、技能和分源参考，使用边界写得很清楚，并主动对照 已收录的 last30days。244★、MIT。本窗帖子没有互动，依据是仓库材料；条目里保留非官方接口和会话风险说明。
