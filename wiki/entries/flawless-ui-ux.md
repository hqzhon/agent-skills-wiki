# flawless-ui-ux（产品语境 UI/UX + 本地检查）

**Tags:** ui, ux, frontend, design, cli, skill
**Source:** [@GitTrend0x](https://x.com/GitTrend0x/status/2123016010366144917) · 2026-11-18
**Engagement:** 与 rust-anything 等一并出现在发现帖（约 4 赞 / 277 次展示）；仓库 [smokeeaasd/flawless-ui-ux](https://github.com/smokeeaasd/flawless-ui-ux) 现 248★，MIT（2026-11-03 建仓）

## When to use
要让编码 agent 为网页、原生手机或桌面界面做设计、改版或评审，并且希望它先弄清受众、内容和品牌，而不是套一层通用「高级感」。也适合对源码或已跑起来的页面做本地检查、验证修复。

## What it does
先通过对话初始化产品语境，再按产品做布局、字体、配色和交互。附带 27 份按需加载的参考（字体、表格、表单、动效、平台惯例等）和 10 个可对照的案例。CLI 可 `inspect` / `verify` 源码或浏览器界面（浏览器检查需 Playwright Chromium）。需要 Node 22.12+。Codex 用 `$flawless-ui-ux init`，带斜杠命令的宿主用 `/flawless-ui-ux init`。

## Recipe / links
- Repo: https://github.com/smokeeaasd/flawless-ui-ux（MIT，248★）
- 安装（项目目录下，会让你选作用域和宿主）：`npx flawless-ui-ux@latest install`（或 `pnpm dlx` / `bunx`）
- 也可：`npx skills add smokeeaasd/flawless-ui-ux --skill flawless-ui-ux`（这条只装 skill；检查 CLI 仍走上面的 npm 包）
- 更新已安装副本：`npx flawless-ui-ux@latest update --codex`；诊断：`npx flawless-ui-ux@latest doctor`
- Skill 路径：`skills/flawless-ui-ux/SKILL.md`

## Why it made the cut
技能与本地检查命令行配套，有明确产品语境流程和可核对照的案例，区分于只给设计词汇表的包。
