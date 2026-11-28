# OpenGame（把编码代理变成游戏工作室）

**Tags:** gamedev, html5, mcp, skill-pack, openmotion
**Source:** [@cutetoxicguy](https://x.com/cutetoxicguy/status/2126586905076597230) · 2026-11-28
**Engagement:** 本窗为第三方介绍帖（1 赞）；仓库 [nexu-io/opengame](https://github.com/nexu-io/opengame) 现 2,659★ / 411 forks，Apache-2.0，2026-11-25 建仓，本窗仍有推送。与已收录的同组织仓库 [OpenMotion](openmotion.md)（nexu-io/openmotion）不是同一条：OpenMotion 主打参考片重制成可编辑动效，OpenGame 主打可玩游戏的改版、测试和打包。

## When to use
不想让 agent 从空白项目凭空生成一整款游戏，而是要从可玩模板出发：改视觉和机制、测能不能玩、再打包到 itch.io、Telegram，或微信/抖音等小游戏渠道时用。它通过 Agent Skills 和 MCP 把 Claude Code、Codex、DeepSeek 等二十多种编码代理接到 Game Studio。只把技能说明拷进 agent **不会**带上本地 Studio 和 MCP，还要按文档做完本地安装。

## What it does
开源的「面向 agent 的游戏工作室」。介绍帖写明内置 25 个可玩的 HTML5 模板（竞速、平台、塔防、叙事分支、竖屏无尽跑等），每份都带可改源码。技能侧有入口技能 `opengame`，用于本地开通并把任务路由到 `openmotion-game` 以及玩法、动画、试玩广告和 QA 等参考手册。仓库文档还描述了与 OpenMotion 共享的技能分层（视频 / 游戏 / 设计 / 媒体）和 100+ 条可选风格配方；装游戏能力时以 `opengame` / `openmotion-game` 和官方安装说明为准，不必一次装下整个配方库。

Agent 可以改现成游戏的视觉识别、操作、角色和关卡，替换图形和音效，再走自动测试后打包。发布渠道和模板数量以仓库当前 README 为准（仓库简介写的是 100+ 可改游戏，可能比介绍帖里的 25 个样例更全）。

## Recipe / links
- Repo: https://github.com/nexu-io/opengame（2,659★，Apache-2.0）
- 安装入口技能：
  ```bash
  npx skills add https://github.com/nexu-io/opengame/tree/skills --skill opengame
  ```
  也可直接 `--skill openmotion-game`。
- 技能与 MCP 契约：https://github.com/nexu-io/opengame/blob/main/docs/skills.md
- 本地跑 Studio 与接通 MCP：按仓库 `docs/opengame-setup.md` / README 的安装节（需要 Git、Git LFS 等，以文档为准）

## Why it made the cut
同组织已有高星的 OpenMotion，这个新仓把「可玩游戏」做成可装技能和 MCP 工具，模板和安装路径都可以核对。本窗介绍帖互动很低，依据是仓库材料。条目里写清和 OpenMotion 的分工，避免当成重复收录。
