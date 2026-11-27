# Meta VR Agentic Tools（官方：Quest / Horizon OS 开发技能）

**Tags:** official, meta, vr, quest, horizon-os, mcp, skill-pack
**Source:** [@Dilmerv](https://x.com/Dilmerv/status/2126013737739911372) · 2026-11-27
**Engagement:** 介绍帖 24 赞 / 19 收藏 / 5 转；仓库 [meta-quest/agentic-tools](https://github.com/meta-quest/agentic-tools) 现 255★，Apache-2.0。Meta 官方技能包，文档站有完整技能目录；仓最近推送到 2026-09-24。

## When to use
在用 AI 编码 agent 做 Meta Quest / Horizon OS 开发（Unity、Unreal、Android / Spatial SDK、WebXR、React Native、性能分析或上架检查），希望 agent 按官方步骤和 metavr CLI / MCP 工作，而不是凭训练数据猜测时用。设备相关技能需要已开开发者模式的 Meta VR 设备。

## What it does
官方 Agent Skills 包，每个技能一份 SKILL.md，覆盖项目脚手架、Meta XR Core / Platform SDK、Unity / Android / WebXR / RN 常见任务、Perfetto / simpleperf 性能分析、舒适度与无障碍审阅，以及上架相关流程。技能由 **metavr** CLI 驱动（设备与应用管理、文档搜索），也可作为 MCP 服务器。文档：[Browse agent skills](https://developers.meta.com/vr/essentials/agent-skills/)。最快的安装方式是 `metavr init`，按本机已装的 agent 配置技能和 MCP；帖中也提到 `metavr skills install --all`。

## Recipe / links
- Repo: https://github.com/meta-quest/agentic-tools（255★，Apache-2.0）
- 文档：https://developers.meta.com/vr/essentials/agent-skills/
- 安装 metavr CLI（macOS / Linux）：
  ```bash
  curl -fsSL https://developers.meta.com/horizon/install-cli/ | sh
  metavr init
  ```
  或 `npx -y metavr --version` 后同样运行 `metavr init`。
- Claude Code：`/plugin marketplace add meta-quest/agentic-tools`，再 `/plugin install meta-vr@meta-vr`
- 也可用 `npx skills add meta-quest/agentic-tools` 或 `gh skill install meta-quest/agentic-tools`（仓库 README 有 Cursor / Codex / Copilot / Muse 的对应命令）。

## Why it made the cut
厂商官方技能包，有可验证仓库、文档站和明确的安装路径；场景就是「别让 agent 猜 Quest 工作流」。星标不算顶格，按官方材料和完整配方收录。仓最近推送停在 2026-09-24，装前看文档是否仍与当前 SDK 一致。
