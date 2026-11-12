# SwiftUI Pro（Paul Hudson / Hacking with Swift）

**Tags:** swift, swiftui, ios, code-review, accessibility, performance
**Source:** [@lovethelife2333](https://x.com/lovethelife2333/status/2120830896001400998) · 2026-11-12
**Engagement:** 帖子互动低 · twostraws/SwiftUI-Agent-Skill ~6.5k★ · MIT

## When to use
让 Claude Code / Codex / Gemini / Cursor 写或审 SwiftUI 代码时，模型老用废弃 API、按钮 VoiceOver 读不到、随手埋性能坑；想要一份针对「LLM 真实常犯错误」的 SwiftUI 审查清单。

## What it does
基于作者多年的 SwiftAgents AGENTS.md 整理成 Agent Skills 格式的 `swiftui-pro`：覆盖导航、布局、动画、状态管理、VoiceOver、废弃 API、性能与设计。可整体审查，也可带指令只查一项（如只查废弃 API 或无障碍）。目标 iOS 26+ / Swift 6.4+。同作者还有 SwiftData Pro、Swift Concurrency Pro、Swift Testing Pro 和 Swift-Agent-Skills 索引。

## Recipe / links
- 仓库：https://github.com/twostraws/SwiftUI-Agent-Skill
- 安装：`npx skills add https://github.com/twostraws/swiftui-agent-skill --skill swiftui-pro`
- Claude Code 插件：`/plugin marketplace add twostraws/SwiftUI-Agent-Skill` → `/plugin install swiftui-pro@swiftui-agent-skill`
- 调用：Claude Code `/swiftui-pro Check for deprecated API`；Codex `$swiftui-pro Focus on accessibility`

## Why it made the cut
知名 Swift 作者维护、MIT、安装与调用命令清晰、场景具体；和已收录的 [bama](bama.md)（21 个 Swift/SwiftUI 技能）互补，这个偏单点审查。
