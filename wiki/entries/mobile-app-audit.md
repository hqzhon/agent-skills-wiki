# mobile-app-audit（移动应用证据式 QA）

**Tags:** mobile, qa, ios, android, flutter, react-native, skill
**Source:** [@ronaldmaco_](https://x.com/ronaldmaco_/status/2122828999722459175) · 2026-11-18
**Engagement:** 发现帖互动很低（16 次展示）；仓库 [ronaldmaco/mobile-app-audit](https://github.com/ronaldmaco/mobile-app-audit) 现 1★，MIT，版本 2.6.1（2026-11-06 建仓）

## When to use
要让编码 agent 在 iOS / Android / Flutter / React Native 上查证用户报的 bug、确认修复是否真的到了用户会安装的构建，或在发版前做针对性/完整审计、应用商店就绪检查，而不是只看「好像能跑」。

## What it does
按最小够用的模式工作：bug 查证、修复查证、局部审计、完整审计、商店就绪、线上复盘、未来风险。每条缺陷走同一闭环：接报 → 在真实构建和状态下复现（界面与 API 对照）→ 根因与影响面 → 修复+测试 → 在发版构建上复核。仓库带 `evals/`、案例和 changelog；文档称在 Claude Code 上做过触发与带/不带 skill 的对照评测。作者说明其他宿主尚未充分测试。

## Recipe / links
- Repo: https://github.com/ronaldmaco/mobile-app-audit（MIT，1★）
- Claude Code：`/plugin marketplace add ronaldmaco/mobile-app-audit` → `/plugin install mobile-app-audit@mobile-app-audit`
- 其他 Agent Skills 宿主：`npx skills add ronaldmaco/mobile-app-audit`，或 `git clone https://github.com/ronaldmaco/mobile-app-audit.git && mobile-app-audit/scripts/install.sh`
- 安装细节与「同名技能不要装两份」：仓库 `docs/INSTALL.md`

## Why it made the cut
有明确使用场景、完整 SKILL.md / 插件格式、评测和案例，不是一份静态清单。社区信号仍弱，属于早期条目，安装前需自审。
