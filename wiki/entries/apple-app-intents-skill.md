# Apple App Intents Skill（给 iOS 应用加 Siri / Shortcuts / App Intents）

**Tags:** ios, siri, shortcuts, app-intents, apple-intelligence, skill
**Source:** [@Sdefendre](https://x.com/Sdefendre/status/2125032562812682413) · 2026-11-24
**Engagement:** 本窗 5 赞 / 9 书签 / 3 回复 · 仓库 [Sdefendre/apple-app-intents-skill](https://github.com/Sdefendre/apple-app-intents-skill) 现 9★，MIT，有 CI，2026-11-24 仍在推送

## When to use
给现有 iOS 应用补 App Intents、App Entities、App Shortcuts、App Schemas，或让能力出现在 Siri、快捷指令、控制中心、桌面小组件、Focus filters 里时用。需要对照当前 SDK / 系统版本实现，而不是让模型凭记忆写一套过时 API。

## What it does
一份可加载的 Agent Skill（`skills/apple-app-intents/SKILL.md`，v0.2.0），面向 Claude Code、Cursor、Codex、OpenClaw 等能读 Markdown 的 agent。先盘点工程与已安装的 Xcode/SDK，再按自定义 Intent 与 Schema 合规动作分流，并带 Swift/SwiftUI 示例、测试流程，以及以 2026-09-10 / WWDC26 为基线、来自 Apple 文档和 WWDC 记录的研究材料。可选 `scripts/doctor.py` 做库存盘点（不是合规结论）。不实现替代系统的语音助手。

## Recipe / links
- Repo: https://github.com/Sdefendre/apple-app-intents-skill（9★，MIT）
- 站点 / 下载: https://sdefendre.github.io/apple-app-intents-skill/
- 安装（需 Git；可选安装器需 Python 3.10+）：
  ```bash
  git clone https://github.com/Sdefendre/apple-app-intents-skill.git
  cd apple-app-intents-skill
  python3 scripts/install.py --agent claude    # 或 cursor / codex / openclaw
  ```
  安装器只做本地复制，不覆盖已有安装，也不下载或执行远程代码。真机/模拟器构建仍需要 macOS 与完整 Xcode。
- 无 API key、无订阅、无遥测。Apple 开发者账号与系统服务仍按苹果自己的要求。

## Why it made the cut
场景清楚、有 `SKILL.md`、安装器、CI 和示例，MIT 可商用。星数不高，但材料完整，且和已收录的 [Apple Human Interface Skills](apple-human-interface-skills.md)、[cleared-for-takeoff](cleared-for-takeoff.md)、[app-store-compliance](app-store-compliance.md) 不重复：那些管界面规范和上架预检，这一条专做系统级调用入口。
