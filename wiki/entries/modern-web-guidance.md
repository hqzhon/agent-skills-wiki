# Modern Web Guidance（Chrome / Edge / Firefox / MDN 官方）

**Tags:** web, frontend, official, browser-compat, skill-pack, cli
**Source:** [@usuperman2017](https://x.com/usuperman2017/status/2120387385963995566) · 2026-11-11（另见 [@echo_vic](https://x.com/echo_vic/status/2120359259624137021)、[@AndrewSignalZ](https://x.com/AndrewSignalZ/status/2120323883324916125)）
**Engagement:** 帖子互动低 · GoogleChrome/modern-web-guidance ~3.5k★ · Apache-2.0 · 1.0 版

## When to use
让 Claude Code、Codex、Cursor 等编码 agent 写前端（弹窗、暗色模式、表单、动画等）时，避免它默认堆 div + JS 的老写法，改用原生 Web 平台能力并顾及兼容性；或要扫一个老项目找可现代化的旧写法。

## What it does
200 多篇人工编写的指南（约 1.7MB），带 Baseline 兼容数据和降级方案。agent 先用 CLI 本地检索相关指南、取回具体条目再写代码，不需要 MCP 或 API key。`legacy-scan` 可扫描代码库列出可替换的旧模式。由 Chrome、Edge、Firefox、MDN 团队共同维护，附公开评测看板。

## Recipe / links
- Repo: https://github.com/GoogleChrome/modern-web-guidance （源码 https://github.com/GoogleChrome/modern-web-guidance-src）
- 文档: https://developer.chrome.com/docs/modern-web-guidance
- 安装：`npx modern-web-guidance@latest install`
- 试用：`npx modern-web-guidance@latest search "animate a dialog modal backdrop"`、`retrieve <id>`、`legacy-scan .`

## Why it made the cut
上轮近失线索（当时无仓库），本轮 1.0 发布并定位到官方仓库。浏览器厂商联合维护、内容人工编写、可本地检索且有评测，场景明确，属于高信号官方技能。
