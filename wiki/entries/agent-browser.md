# agent-browser（Vercel Labs：给 Agent 用的浏览器 CLI）

**Tags:** official, vercel, browser, cli, automation, testing, skill-pack
**Source:** [@alanversefir](https://x.com/alanversefir/status/2125228884824342824) · 2026-11-24
**Engagement:** 本窗介绍帖互动很低（0 赞）；仓库 [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) 现 53,798★，Apache-2.0，2026-11-24 仍在推送

## When to use
编码 agent 需要**操作网页**时用：打开页面、点按钮、填表、截图、抽数据、做 QA / 探路，或自动化 Electron 应用。技能写明优先用它，而不是内置浏览器工具。不要把它理解成「再包装一层 Playwright 教程」——它是给 agent 用的 CLI，页面以无障碍树形式读出。

## What it does
Vercel Labs 的浏览器自动化 CLI（Rust）。安装后用 `agent-browser` 打开页面、快照、按引用点击。仓库提供与 CLI 版本对齐的技能：`skills/agent-browser/SKILL.md` 以及 `skill-data/core`、`slack`、`electron`、`vercel-sandbox` 等专项技能。也可用 `agent-browser skills get core` 拉取当前版本的技能正文。

## Recipe / links
- Repo: https://github.com/vercel-labs/agent-browser（53,798★，Apache-2.0）
- 安装 CLI：
```bash
npm install -g agent-browser
agent-browser install           # 首次下载 Chrome for Testing
```
  也可用 `brew install agent-browser`，然后 `agent-browser install`。Linux 可用 `agent-browser install --with-deps`。临时试用：`npx agent-browser open example.com`。
- 安装技能：`npx skills add vercel-labs/agent-browser`（本窗介绍帖给出的路径）；或 `agent-browser skills get core` / `skills list`。
- 主技能：[skills/agent-browser/SKILL.md](https://github.com/vercel-labs/agent-browser/blob/main/skills/agent-browser/SKILL.md)
- 文档：https://agent-browser.dev/installation

## Why it made the cut
高星漏收：Vercel Labs 官方工具，可加载 SKILL.md 和明确使用场景，53,798★、Apache-2.0。本窗互动为 0，按仓库信号补上。和 Chrome DevTools MCP（偏调试实时 Chrome）互补：这边是 agent 可脚本化的浏览/操作 CLI。
