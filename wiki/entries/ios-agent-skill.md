# iOS Agent Skill（本机参考 + 模拟器里构建验收）

**Tags:** ios, swift, swiftui, xcode, simulator, mcp, skill
**Source:** [@Nagarjuna2997](https://x.com/Nagarjuna2997/status/2125728412014694711) · 2026-11-26
**Engagement:** 本窗为作者介绍帖（1 赞）；仓库 [Nagarjuna2997/ios-agent-skill](https://github.com/Nagarjuna2997/ios-agent-skill) 现 42★ / 2 forks，MIT，带测试与文档一致性 CI

## When to use
要让编码 agent 写、审或重构 Swift / SwiftUI / UIKit / SwiftData，或从一句话搭出可在 Xcode Simulator 里构建、运行并截图的 iOS 应用时用。它提供本机 Apple 参考检索、能力模块和模拟器工具，用来减少「能生成代码、却没在模拟器里跑过」的情况。需要 macOS 与 Xcode；账号登录、付费能力等仍要你自己配置。若主要是拦 LLM 写废弃 SwiftUI API，可与已收录的 [SwiftUI Pro](swiftui-pro.md) 一起用。

## What it does
根目录 `SKILL.md`（标明 v3.9.1，对齐 Swift 6.4 / Xcode 27，部署下限 Swift 5.9 / iOS 17）要求 agent 先查仓库里的本地参考和 `samples/`，再写带显式错误处理与预览数据的实现。配套 npm 包 `ios-agent-mcp` 提供参考检索、脚手架和模拟器构建/测试/截图。`/ios-build "<一句话>"` 会做计划、写 SwiftUI 与 Xcode 工程、按能力模块（登录、存储、支付、地图等）装配，再在模拟器里构建运行，并报告还需要你账号或付费才能完成的部分。文档站写明已在 Xcode 27.0 上验证过若干示例，也列出尚未完成的能力。仓库另有 `capabilities/`、`checklists/`、`templates/` 和可选的 `install.sh`（只装源码指导，不代替 MCP）。

## Recipe / links
- Repo: https://github.com/Nagarjuna2997/ios-agent-skill（42★，MIT）
- SKILL.md：https://github.com/Nagarjuna2997/ios-agent-skill/blob/main/SKILL.md
- 文档与客户端安装：https://nagarjuna2997.github.io/ios-agent-skill/install.html
- 常用（Claude Code，需 Node 20+）：
  ```bash
  claude mcp add ios-agent -- npx -y ios-agent-mcp@latest
  npx -y ios-agent-mcp@latest install-command --global
  ```
- 从 brief 建工程：`npx -y ios-agent-mcp@latest new MyApp --brief "A reading list with local storage" --xcodegen`
- 只装本地技能指导：克隆后 `bash install.sh --help`

## Why it made the cut
有可加载 SKILL.md、MCP、模拟器验收路径和文档站，场景明确（把 iOS 开发从「生成代码」收到「能构建并截图」）。42★、MIT，作者帖互动很低，按完整可验证材料收录。它是工具包而不是「保证上架」的一键工厂，付费接口和账号配置仍要人来做。
