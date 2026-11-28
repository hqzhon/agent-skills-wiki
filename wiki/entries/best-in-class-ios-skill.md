# Best-in-Class iOS Skill（按任务审/做 SwiftUI 与 UIKit）

**Tags:** ios, swiftui, uikit, accessibility, design, skill
**Source:** [@SahilSatralkar](https://x.com/SahilSatralkar/status/2126594790653600084) · 2026-11-28
**Engagement:** 作者介绍帖 1 赞 / 1 书签；仓库 [sahilsatralkar/best-in-class-ios-skill](https://github.com/sahilsatralkar/best-in-class-ios-skill) 现 0★，MIT，2026-11-28 建仓。灵感来自 Jordan Morgan 免费公开的 *A Best-in-Class iOS App*（[bestinclassiosapp.com](https://www.bestinclassiosapp.com/)）。

## When to use
要设计、实现或审查 iOS / iPadOS 上的 SwiftUI 或 UIKit 流程：导航、无障碍、自适应布局、小组件、分享、同步等系统集成，并希望判断标准落在「用户打开应用要完成的那件事」上时用。它不提供模拟器 MCP，也不从一句话搭完整 Xcode 工程——那是已收录的 [iOS Agent Skill](ios-agent-skill.md)。若主要是拦过时 SwiftUI API，可与 [SwiftUI Pro](swiftui-pro.md) 一起用。

## What it does
可加载技能 `skills/best-in-class-ios-skill/SKILL.md` 要求 agent 先找到真实路径（相关视图/控制器、模型和动作处理），再按任务类型分路：做设计决策、做审查，或从现有入口改实现。七份参考按问题路由：

- 产品范围、首次启动、标签与层级、自适应布局 → `references/design.md`
- VoiceOver 焦点、可达性、读屏宣布 → `accessibility.md`
- 引导、搜索、编辑与撤销、本地化、键盘/指针、内购 → `interaction.md`
- 启动慢、滚动卡、异步加载、过期结果 → `responsiveness.md`
- 小组件、分享扩展、App Clip、快捷指令、通知 → `integrations.md`
- CloudKit / 权限 / 相机 / 地图等设备能力 → `data-and-device.md`
- 模拟器证据、内存、scheme 行为 → `verification.md`

审查要锚定到屏幕、符号或配置，先写会挡住任务或弄丢草稿的问题。部署目标以宿主工程为准，新 API 要给旧系统留一条能走的路。

## Recipe / links
- Repo: https://github.com/sahilsatralkar/best-in-class-ios-skill（0★，MIT）
- 安装：克隆后把整个 `skills/best-in-class-ios-skill` 文件夹拷进 Claude Code 的 `~/.claude/skills/`，或 Codex / Gemini CLI / Copilot CLI 的 `~/.agents/skills/`。团队项目则可放进仓库的 `.claude/skills/` 或 `.agents/skills/` 并提交。
- 技能正文：https://github.com/sahilsatralkar/best-in-class-ios-skill/blob/main/skills/best-in-class-ios-skill/SKILL.md
- 原书与示例工程（免费）：https://www.bestinclassiosapp.com/#downloads

## Why it made the cut
有完整 SKILL.md 和七份可核对的参考，使用边界清楚，和本机参考/模拟器验收的 iOS Agent Skill 不是同一条。0★、当天新建，社区信号弱，按可验证材料收录。技能声明受 Jordan Morgan 一书启发，但仓库是独立实现，不是该书官方包。
