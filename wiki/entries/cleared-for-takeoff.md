# cleared-for-takeoff（App Store 提交前预检）

**Tags:** ios, app-store, qa, flutter, react-native, skill
**Source:** [@pavleos](https://x.com/pavleos/status/2123099078804295809) · 2026-11-19
**Engagement:** 作者本人介绍帖（约 1 赞）；仓库 [Paul-Sizon/cleared-for-takeoff](https://github.com/Paul-Sizon/cleared-for-takeoff) 为 2026-11-18 新建、0★，MIT（早期条目）

## When to use
iOS / iPadOS 应用（Swift/ObjC、React Native、Expo 或 Flutter）即将提交 App Store 或 TestFlight 外部审核，或已被拒、需要对照审核指南 / ITMS-9xxxx / PrivacyInfo.xcprivacy / 用途字符串做预检。

## What it does
确定性扫描器（`preflight.py`，零依赖）先给出 file:line 证据：隐私清单、用途字符串、entitlements、图标、IAP、ATT、AI 同意、密钥等；再由 skill 对照当时的 App Review Guidelines 做扫描器做不到的人工判断（元数据是否属实、4.2/4.3、隐藏功能 2.5.19、UGC 1.2 等），输出带置信度和修复建议的就绪结论，以及可检索的 HTML 报告。也可对 `.ipa` / `.xcarchive` 或 CI `--strict` 运行。指南核验日期写在 skill 元数据里（当前为 2026-11-18）。

## Recipe / links
- Repo: https://github.com/Paul-Sizon/cleared-for-takeoff（MIT，0★）
- 插件：`/plugin marketplace add Paul-Sizon/cleared-for-takeoff` 后 `/plugin install cleared-for-takeoff@cleared-for-takeoff`
- 或：`npx skills add Paul-Sizon/cleared-for-takeoff`
- 只跑扫描器：`python3 skills/cleared-for-takeoff/scripts/preflight.py /path/to/app --html report.html`
- Skill 路径：`skills/cleared-for-takeoff/SKILL.md`

## Why it made the cut
和已有的 [mobile-app-audit](mobile-app-audit.md)、[App Store Connect CLI Skills](app-store-connect-cli-skills.md) 互补：前者偏通用移动 QA，后者偏发版 CLI；这条把确定性扫描和对照现行指南的判断写进同一个可加载 skill，有报告格式和 CI 用法。仓很新、星数为零，属早期收录。
