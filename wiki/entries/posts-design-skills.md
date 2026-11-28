# posts.design Skills（按真实品牌发布作参考做海报 / OG / 头图）

**Tags:** design, social, launch, og-image, mcp, skill-pack
**Source:** [@KOF97AI](https://x.com/KOF97AI/status/2126582886107328900) · 2026-11-28
**Engagement:** 本窗中文介绍帖 3 赞；仓库 [posts-design/mcp](https://github.com/posts-design/mcp) 现 74★ / 6 forks，MIT。11-28 上午仍在观察名单（当时只有站点、未解析到仓库），本窗给出可核的 GitHub 组织仓和安装命令，故单列。

## When to use
做产品发布海报、页面 OG 图、X 头图或发布短片时，希望先看真实品牌怎么排，而不是再生成一套「AI 味」模板时用。技能会去 posts.design 的人工精选图库里找参考，再在你的项目里出方向或成片。它依赖托管 MCP（`https://posts.design/mcp`），需要 posts.design 账号；免费档每月 100 MCP credits，Pro 为 1,000，部分成片/逐镜拆解在免费档受限。不要把它当成无需登录的纯本地设计技能。

## What it does
仓库同时提供托管 MCP 和一组可加载技能（`skills/` 与 Claude Directory 副本）。本轮核到的技能包括：

- `launch-references` / `competitor-audit` / `launch-brief` / `launch-copy` / `launch-video-direction`：找相近的真实发布帖、看某品牌怎么发、从一句话写出简报和文案、按真实发布片排 30 秒镜序
- `og-image` / `x-header`：按真实 OG 图和 X 头图的方向，在你的项目里做图
- `remake` / `rebuild`：按参考片在本机重做，带上你的文案、Logo、颜色和字体
- `sound-breakdown` / `layered-sound`：把参考片放到时间线上拆声音和镜头

Claude Code 可用插件一次装上 MCP 和技能；其他 agent 用 `npx skills add posts-design/mcp`，并把 MCP 服务加进配置后登录。技能用服务器取参考，所以只拷技能文件夹、不接通 MCP，核心检索会不可用。

## Recipe / links
- Repo: https://github.com/posts-design/mcp（74★，MIT）
- 站点：https://posts.design/
- Claude Code：
  ```text
  /plugin marketplace add posts-design/mcp
  /plugin install posts-design@posts-design
  ```
  然后 `/mcp` 里登录 posts.design。
- 其他 agent：`npx skills add posts-design/mcp`（可用 `--skill remake` 只装一个），并添加 MCP `https://posts.design/mcp`
- 技能目录：https://github.com/posts-design/mcp/tree/main/skills

## Why it made the cut
观察名单补上了可核仓库：MIT、11 个技能、安装路径清楚。它是带免费额度的托管 MCP 产品旁边的开源技能包，条目里写明登录和 credits 限制。本窗介绍帖互动一般，依据是仓库材料。
