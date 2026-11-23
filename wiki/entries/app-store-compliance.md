# app-store-compliance（App Store / Play 拒审预检）

**Tags:** ios, android, app-store, google-play, compliance, skill
**Source:** [@forgetsen](https://x.com/forgetsen/status/2124684491994087498) · 2026-11-23（合集帖中的一条，称当日 +621★）
**Engagement:** 仓库 [mjmirza/app-store-compliance](https://github.com/mjmirza/app-store-compliance) 4,170★ / 252 forks；许可证为 OpenRoots Agent License 2.3（不是 MIT/Apache，使用前请先读许可）

## When to use
iOS 或 Android 应用即将提交 App Store / Google Play、刚被拒需要改法和申诉路径，或要在每次上传前加一道自动预检。扫描能证明的和仍需人工核对的，仓库会分开写；它不保证过审。

## What it does
预提交合规审查 + 按严重程度给出修复计划：124 种已文档化的拒审模式与修法、隐私清单 / Data safety、以及一批跟踪中的法定期限（EU AI Act、DSA、COPPA、年龄相关法律等）。可先只跑扫描（不改你的工程），也可装成各编码 agent 的 hook/skill，在 `upload` / 提交类命令前拦截 `[CRITICAL]` 风险。结论行包括 `BLOCKED.` / `CLEAR.` / `Rule pack STALE.`（规则包超过 60 天要 `git pull`）。托管 Expo 应用无原生目录时仍会读 `app.json` / `app.config`。

## Recipe / links
- Repo: https://github.com/mjmirza/app-store-compliance（4,170★，OpenRoots ORA 2.3）
- 站点：https://mjmirza.github.io/app-store-compliance
- Skill 路径：`agent-os/skill/SKILL.md`
- 只扫描、不安装：
  ```bash
  git clone https://github.com/mjmirza/app-store-compliance ~/repositories/app-store-compliance
  bash ~/repositories/app-store-compliance/agent-os/hooks/app-store-compliance-guard.sh "/path/to/your/app"
  ```
- 装进编码工具（需 git / bash；除 Claude Code 外还需 python3）：
  ```bash
  git clone https://github.com/mjmirza/app-store-compliance ~/repositories/app-store-compliance
  bash ~/repositories/app-store-compliance/scripts/install.sh --tool all
  ```
  也可把 `--tool all` 换成 `cursor`、`codex`、`gemini` 等单个工具。

## Why it made the cut
材料厚、可验证、场景清楚，星数远高于本目录里较早的 [cleared-for-takeoff](cleared-for-takeoff.md)（偏 iOS / Flutter / RN 预检，当时为新建 0★ 仓）。两者可并存；本包覆盖 iOS + Play，并带 hook。许可偏少见，条目里标明，装前请自行阅读。本窗出处是合集帖，按高星漏收补上。
