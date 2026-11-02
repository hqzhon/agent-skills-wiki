# GenOffice CLI + Agent Skill

**Tags:** office, docx, xlsx, pptx, documents, cli
**Source:** [@OnchainOffDuty](https://x.com/OnchainOffDuty/status/2116850335226691720) · 2026-11-01
**Engagement:** genspark-ai/genoffice ~11.5k★，Apache-2.0

## When to use
要让 Claude Code / Codex / Cursor 在本地直接生成或修改**真实格式**的 `.docx` / `.xlsx` / `.pptx`：带活公式的表格、带母版排版的幻灯片、可审阅的文档改动，而不是导出一份纯文本或截图。

## What it does
GenOffice 是开源 AI Office 套件（Docs / Sheets / Slides / PDF / Markdown / HTML 编辑器），附 `genoffice` CLI、MCP 和 agent skill。Skill 让本地 Agent 通过 CLI 读写 Office 文件：只重写被改动部分、其余字节保留；表格写入公式而非粘贴数值；改动以修订 / diff 呈现。PDF→Word/Excel/PPT 等转换在本机完成。

## Recipe / links
- Repo: https://github.com/genspark-ai/genoffice
- 安装 skill：`npx skills add genspark-ai/genoffice`

## Why it made the cut
填补「Agent 产出真 Office 文件」这一高频需求，有官方仓库、CLI 与 skill 三件套。注意：应用内的「隐藏敏感片段」只对软件内置 AI 生效，走 CLI / MCP 时 Agent 能读到原文。
