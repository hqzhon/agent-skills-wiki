# Mobile Agent Skills（Android / iOS / Flutter 工程规范包）

**Tags:** mobile, android, ios, swiftui, flutter, compose, security, skill-pack
**Source:** [@liyunpe75402444](https://x.com/liyunpe75402444/status/2125916341949583515) · 2026-11-26
**Engagement:** 介绍帖 0 赞；仓库 [leotyndale/mobile-agent-skills](https://github.com/leotyndale/mobile-agent-skills) 现 0★，MIT，带 CI。本窗由作者开源，仓于 2026-11-26 新建。与已收录的 [iOS Agent Skill](ios-agent-skill.md)（本机参考 / 模拟器验收）和 [Compose Skill](compose-skill.md) 不是同一仓库。

## When to use
让编码 agent 写或改 **Android（Compose）、iOS（SwiftUI）、Flutter** 或移动端架构时用——避免把移动代码写成阻塞主线程、泄漏 `Activity`/`ViewModel`、引发重建风暴、忽略 ROM 碎片或端侧 AI 内存预算的「后端脚本」。也可用于崩溃排查、性能审计、MASVS 取向的安全审查、PR 审查和发版门禁。

## What it does
10 条可安装 playbook，并带一键安装脚本，可写入 Claude Code、Cursor（`.mdc`）、Codex、Antigravity、Gemini CLI（或一次装到全部路径）：

- 架构与 UI：`android-compose-architect`、`ios-swiftui-architect`、`flutter-architecture-audit`、`mobile-ddd-modularization`
- 可靠性与端侧 AI：`android-performance-audit`、`android-crash-triage`、`mobile-ondevice-ai`
- 安全与发版：`mobile-security-review`、`mobile-pr-review`、`mobile-release-readiness`

## Recipe / links
- Repo: https://github.com/leotyndale/mobile-agent-skills（0★，MIT）
- 安装到某个移动项目（把路径换成你的仓库）：
  ```bash
  git clone https://github.com/leotyndale/mobile-agent-skills.git /tmp/mobile-agent-skills
  bash /tmp/mobile-agent-skills/scripts/install.sh --target claude --dest /path/to/your-mobile-app
  # 或一次写入全部支持的 agent：
  bash /tmp/mobile-agent-skills/scripts/install.sh --target all --dest /path/to/your-mobile-app
  ```
- 全局安装：`bash /tmp/mobile-agent-skills/scripts/install.sh --target claude --scope global`
- 中文文档：仓库内 `README_ZH.md`

## Why it made the cut
10 个带 `SKILL.md` 的可执行规范 + 多 agent 安装脚本和 CI，使用场景具体，和已有的 iOS/Compose 条目互补。星标和介绍帖都还是零，按完整技能包收录，后续需再观察是否持续维护。
