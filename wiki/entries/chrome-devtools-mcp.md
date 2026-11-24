# Chrome DevTools MCP（官方：实况 Chrome 调试 + 8 个 Agent Skills）

**Tags:** official, chrome, devtools, mcp, debugging, performance, a11y, skill-pack
**Source:** [@hsianghui](https://x.com/hsianghui/status/2124900166507585833) · 2026-11-23
**Engagement:** 本窗介绍帖 7 赞 / 7 收藏 · 仓库 [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) 现 59,020★，Apache-2.0，Google Chrome DevTools 官方维护

## When to use
要让编码 agent 在**真实 Chrome** 里调试、做性能分析、查无障碍或修内存泄漏，而不是只看静态代码；需要 DevTools 的性能追踪、网络请求、控制台和截图。

## What it does
官方包同时提供 MCP 服务器、CLI，以及 8 个教 agent 怎么用这套工具的 `SKILL.md`：

- `chrome-devtools`：用 MCP 工具调试和自动化页面
- `chrome-devtools-cli`：用 CLI 写 shell 脚本（需先全局安装 CLI）
- `a11y-debugging`：无障碍审计与修复
- `cookie-debugging`：Cookie / 会话 / 鉴权
- `debug-optimize-lcp`：排查并改善 Largest Contentful Paint
- `memory-leak-debugging`：找内存泄漏
- `troubleshooting`：修 MCP 与 Chrome 的连接问题
- `inspect-in-devtools`：在 DevTools 里检查页面

技能描述的是特定版本的工具，升级 MCP/CLI 后应同步更新 skill，以免参数过时。

默认会向 Google 收集用量统计（调用成功率、延迟、环境信息）；可用 `--no-usage-statistics`，或设置 `CHROME_DEVTOOLS_MCP_NO_USAGE_STATISTICS` / `CI` 关闭。这与 Chrome 浏览器自己的用量统计是分开的。

## Recipe / links
- Repo: https://github.com/ChromeDevTools/chrome-devtools-mcp（59,020★，Apache-2.0）
- 以插件同时装 MCP + 全部 skill（Claude Code）：
  ```
  /plugin marketplace add ChromeDevTools/chrome-devtools-mcp
  /plugin install chrome-devtools-mcp@chrome-devtools-plugins
  ```
- 手动安装单个 skill（先 `npm i chrome-devtools-mcp@latest -g`）：
  ```bash
  mkdir -p ~/.claude/skills
  cp -R "$(npm root -g)/chrome-devtools-mcp/skills/chrome-devtools-cli" ~/.claude/skills/
  ```
- MCP 启动关闭用量统计示例：`"args": ["-y", "chrome-devtools-mcp@latest", "--no-usage-statistics"]`

## Why it made the cut
Chrome 官方出品，59k★，既有可调用的 MCP/CLI，也有 8 份可加载 `SKILL.md`，场景具体（LCP、无障碍、Cookie、内存泄漏）。本窗介绍帖互动一般，按高星漏收补上。和已收录的 [Modern Web Guidance](modern-web-guidance.md)（教 agent 用现代 Web API）互补：一个管「怎么写」，一个管「在真浏览器里怎么查」。
