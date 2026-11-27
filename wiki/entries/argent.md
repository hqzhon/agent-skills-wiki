# Argent（Software Mansion：用 MCP / 技能驱动模拟器、真机、电视和 Mac 应用）

**Tags:** official, software-mansion, mcp, ios, android, tv, macos, e2e, profiling, skill-pack
**Source:** [@hsianghui](https://x.com/hsianghui/status/2126142899197035002) · 2026-11-27
**Engagement:** 介绍帖 3 赞 / 3 收藏；仓库 [software-mansion/argent](https://github.com/software-mansion/argent) 现 3,257★，源码 Apache-2.0（含专有二进制，见下）。Software Mansion 官方工具，仓仍在更新（最近推送到 2026-11-26）。

## When to use
要让编码 agent（Claude Code、Codex、Cursor 等）直接操作 **iOS 模拟器 / 真机、Android 模拟器 / 设备、Apple TV / Android TV / Fire TV、Electron 或原生 Mac 应用**：点击、输入、复现路径、对截图做视觉回归、或做渲染/CPU 性能分析，而不想离开终端时用。和已收录的 [iOS Agent Skill](ios-agent-skill.md)（本机参考与模拟器构建验收）、[Mobile Agent Skills](mobile-agent-skills.md)（工程规范）不是同一条路：Argent 是驱动设备的 MCP + 技能包。

## What it does
MCP 服务器 + CLI + 约 19 个 Agent Skill（如 `argent-ios-simulator-setup`、`argent-device-interact`、`argent-qa-e2e`、`argent-screenshot-diff`、`argent-native-profiler`、`argent-macos-app-interact`、`argent-tv-interact` 等）。可以点按/滑动/打字、把录过的路径重放成 e2e、对基线截图做 OCR/字体感知的 diff，以及接 Hermes、React DevTools、Xcode Instruments、Perfetto 做性能分析。React Native 工作流有专门技能。安装向导：`npx @swmansion/argent@latest init`。遥测默认开启，可用 `argent telemetry disable` 关闭。

源码是 Apache-2.0，但各平台的 `simulator-server`、`ax-service` 以及部分 `.dylib` 是 Software Mansion 的专有二进制，只允许在本项目内使用，不能反编译或单独再分发。

## Recipe / links
- Repo: https://github.com/software-mansion/argent（3,257★；源码 Apache-2.0 + 专有二进制）
- 文档：https://docs.swmansion.com/argent/docs/fundamentals/installation
- 站点：https://argent.swmansion.com
- 安装（项目根目录）：
  ```bash
  npx @swmansion/argent@latest init
  ```
  向导会探测编辑器并写入 MCP 配置。也可以 `npm install -g @swmansion/argent` 后把 `argent mcp` 加进 MCP 配置。
- 技能目录：`packages/skills/skills/*/SKILL.md`

## Why it made the cut
厂商官方的可加载技能包，使用场景清楚（让 agent 真正驱动模拟器和桌面应用），有文档、安装命令和约 19 份 SKILL.md。本窗由盘点账号介绍；星标和持续推送都够格单列。许可是混合的，收录时写明专有二进制和遥测默认开启。
