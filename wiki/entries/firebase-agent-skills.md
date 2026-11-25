# Firebase Agent Skills（官方）

**Tags:** official, firebase, google, analytics, firestore, skill-pack
**Source:** [@Astrodevil_](https://x.com/Astrodevil_/status/2125446900103209152) · 2026-11-25
**Engagement:** 本窗官方盘点帖（0 赞）；仓库 [firebase/agent-skills](https://github.com/firebase/agent-skills) 现 529★，Apache-2.0，2026-11-09 仍有推送。此前多轮 Watch「Google Analytics for Firebase 官方技能」。

## When to use
编码 agent 要接入或排查 Firebase 时用：Auth、Firestore、Hosting / App Hosting、Crashlytics、Remote Config、Analytics、Security Rules，或 Xcode 工程设置。不要期待它覆盖所有 Google Cloud 服务——那是 [google/skills](google-cloud-skills.md) 的范围。

## What it does
官方约 14 个技能，包括 `firebase-basics`、Auth / Firestore / Hosting / App Hosting / Analytics / Crashlytics / Remote Config / Data Connect 入门，以及 Security Rules 审计、规则创建、Extensions 迁到 Functions 等。可按 Agent Skills CLI、Gemini CLI 扩展或 Claude / Codex / Kimi 插件安装。

## Recipe / links
- Repo: https://github.com/firebase/agent-skills（529★，Apache-2.0；`firebase/skills` 会重定向到此仓）
- `npx skills add firebase/skills`（README 推荐写法）或 `npx skills add firebase/agent-skills`
- Gemini CLI：`gemini extensions install https://github.com/firebase/skills`
- Claude：`claude plugin marketplace add firebase/skills` → `claude plugin install firebase@firebase`
- Codex：`codex plugin marketplace add firebase/skills` → `codex plugin add firebase@firebase`

## Why it made the cut
Firebase 官方技能包，SKILL.md 与多种安装路径已可复核，补上此前 Watch。529★、Apache-2.0。本窗另有 Google AdMob 工具博文，未见独立 AdMob 技能仓，暂不单列。
