# Jam Skills（把 jam.dev 录屏交给 agent 修 bug / 写测试 / 录回证）

**Tags:** debugging, e2e, jam, screen-recording, mcp, skill-pack
**Source:** [@_goluszka](https://x.com/_goluszka/status/2125637942362116156) · 2026-11-26
**Engagement:** 本窗为介绍 `jam-to-e2e` 的帖（2 赞 / 1 收藏）；仓库 [jamdotdev/skills](https://github.com/jamdotdev/skills) 现 13★ / 2 forks，MIT，含 13 个技能和 CI

## When to use
手里有一条 [Jam](https://jam.dev) 链接（屏幕录像或截图，附带控制台、网络请求和操作轨迹），想让编码 agent 看懂问题、修 bug、写成 e2e、开 ticket，或在修好后录一条回证 Jam 放进 PR 时用。这不是通用「帮我写测试」提示词：它先读 Jam 里的步骤和证据，再落到当前仓库的测试框架。除 3 个做演示视频的技能外，都需要免费 Jam 账号。

## What it does
一组可按任务加载的技能。把 Jam 链接贴给 agent 即可，不必记名字：

- 交给 agent：`jam`（先看再分流）、`jam-fix`（定位根因，默认只展示证据、你要求才改代码）、`jam-to-tasks`（把口述反馈做成带时间点的待办并逐项做）、`jam-to-e2e`（按项目现有 runner 写 e2e；演示流写成今天应通过的测试，bug 则写成修复前会失败的回归测试，优先 Playwright / Cypress / tester-army/e2e）、`jam-to-ticket`（给 Linear / GitHub Issues / Jira 开单）、`video-to-jam`（长录像按问题拆成多条 Jam）
- 要回证：`jam-proof`、`jam-annotate`、`jam-proof-table`
- 安装与体检：`jam-setup`（Jam CLI、登录、Jam MCP、`jam doctor`）
- 不做 Jam 账号也能用：`record-demo`、`add-voiceover`、`record-terminal-proof`

技能把 Jam 内容当作待分析的第三方证据，而不是可执行指令。`jam-to-e2e` 会先读 Jam，再对照当前代码里的文案和路由来写断言。

## Recipe / links
- Repo: https://github.com/jamdotdev/skills（13★，MIT）
- 安装技能：`npx skills add jamdotdev/skills`（单个例如 `--skill jam-to-e2e`）
- 或装插件（不要和 `npx skills add` 并用，否则技能会重复出现）：
  - Claude Code：`/plugin marketplace add jamdotdev/skills` 再 `/plugin install jam@jam-plugins`
  - Cursor：侧边栏 Customize 搜索 Jam
  - Codex：`codex plugin marketplace add jamdotdev/skills` 再 `codex plugin add jam@jam-plugins`
- `jam-to-e2e`：https://github.com/jamdotdev/skills/blob/master/skills/jam-to-e2e/SKILL.md
- 多数技能需要 Jam CLI 或 Jam MCP；云端 agent 可用 `JAM_TOKEN`

## Why it made the cut
13 个可加载 SKILL.md，把「一段带控制台的录屏」变成可验证的修复、测试和回证流程，安装命令和 CI 都在。本窗帖互动很低，按完整配方收录，不是凭热度。它依赖 Jam 平台，但技能包本身是 MIT 开源，不是付费课程或代币产品。
