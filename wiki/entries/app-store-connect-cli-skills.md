# App Store Connect CLI Skills（asc）

**Tags:** ios, macos, app-store, testflight, cli, skill-pack, release
**Source:** [@hsianghui](https://x.com/hsianghui/status/2121367504605806919) · 2026-11-14
**Engagement:** 发现帖热度一般；CLI [rorkai/App-Store-Connect-CLI](https://github.com/rorkai/App-Store-Connect-CLI) 约 8.3k★，技能仓 [app-store-connect-cli-skills](https://github.com/rorkai/app-store-connect-cli-skills) 约 1.1k★，均为 MIT

## When to use
要用脚本或编码 agent 跑 App Store Connect 流程：上传构建、加 TestFlight 组、提交审核、拉崩溃日志、同步元数据与截图、签名与公证，而不想在 App Store Connect 网页上点。

## What it does
`asc` 是 App Store Connect API 的 Go CLI（MIT）。`asc install-skills` 只通过 git 安装技能仓里钉死的审阅提交（文档写 25 个；当前 `skills/` 下可见 `asc-release-flow`、`asc-testflight-orchestration`、`asc-metadata-sync`、`asc-signing-setup`、`asc-crash-triage`、`asc-aso-audit`、`asc-screenshot-resize`、`asc-whats-new-writer`、`asc-apple-ads` 等，约 26 个目录），覆盖构建生命周期、提交流程、本地化、订阅定价、公证和 Xcode 构建。CLI 本体另有一组维护用 skill（审 PR、发版等），与给使用者装的这包不是同一套。

## Recipe / links
- CLI: https://github.com/rorkai/App-Store-Connect-CLI
- Skills 仓库：https://github.com/rorkai/app-store-connect-cli-skills
- 安装技能（需已安装 `asc`）：`asc install-skills`
- 技能从钉选 commit 拉取，不跑 npm / npx；详见 CLI README 的「asc skills」一节

## Why it made the cut
可执行 SKILL.md + 明确的 iOS/macOS 发版场景，CLI 与技能仓都能核对；`asc install-skills` 把安装路径写死，适合 agent 直接调用。
