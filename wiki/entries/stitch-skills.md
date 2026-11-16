# Stitch Skills（Google Labs 官方设计 / 出码技能包）

**Tags:** official, design, frontend, stitch, skill-pack, google
**Source:** [@GitTrend0x](https://x.com/GitTrend0x/status/2122125019241230486) · 2026-11-16
**Engagement:** 发现帖 12 赞（热榜综述之一）· 仓库 [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) 现 9,447★ / 1,163 forks，Apache-2.0；同窗口多帖复读

## When to use
要让编码 agent 配合 [Google Stitch](https://stitch.withgoogle.com) MCP 做界面：从文字或图片生成屏幕、改设计稿、维护设计系统，再把设计转成 React / React Native / shadcn 等代码。需要先完成 [Stitch MCP 设置](https://stitch.withgoogle.com/docs/mcp/setup)。没有 Stitch 账号或只想要纯本地前端规范时，应改用 [Modern Web Guidance](modern-web-guidance.md)、[design.how](design-how.md) 等不依赖该 MCP 的技能。

## What it does
Google Labs 按 Agent Skills 开放标准发布的三组插件，共 16 个 `SKILL.md`：

- **stitch-design**：`generate-design`（文/图生界面，先做提示词增强，颜色和主题交给设计系统）、`code-to-design`、`upload-to-stitch`、`extract-design-md`、`extract-static-html`、`manage-design-system`
- **stitch-build**：`react-components`、`react-vite-dashboard`、`react-native`、`shadcn-ui`、`remotion`
- **stitch-utilities**：`site-md`、`design-md`、`stitch-loop`、`taste-design`、`enhance-prompt`

兼容 Codex、Claude Code、Cursor、Gemini CLI、Antigravity；OpenCode 需手动拷贝技能目录并自行配置远程 MCP。注意：仓库最近一次推送停留在 2026-08-17，技能内容可能落后于当前 Stitch 产品，装前对照官方文档。

## Recipe / links
- Repo: https://github.com/google-labs-code/stitch-skills（Apache-2.0，9,447★）
- MCP 设置：https://stitch.withgoogle.com/docs/mcp/setup
- Claude Code（当前项目）：`npx plugins add google-labs-code/stitch-skills --scope project --target claude-code`
- Cursor（当前工作区）：`npx plugins add google-labs-code/stitch-skills --scope workspace --target cursor`
- Codex 可先把该仓加为 plugin marketplace，再按需安装 `stitch-design` / `stitch-build` / `stitch-utilities`
- OpenCode：把需要的 `plugins/*/skills/<name>` 拷到 `.opencode/skills/`，并按官方说明填写远程 Stitch MCP URL；部分技能的 `name` 使用 `stitch::…` 形式，OpenCode 可能要求改成与目录一致的 kebab-case

## Why it made the cut
大厂官方技能包，16 份可加载 `SKILL.md`，安装路径清楚，使用场景就是「Stitch 出设计再出码」。星标和 forks 都很高，本窗口多次出现在 GitHub 热榜综述里。必须先接 Stitch MCP，且上游仓已约三个月未推送，当作官方起点而不是保证与最新 UI 完全同步的活文档。
