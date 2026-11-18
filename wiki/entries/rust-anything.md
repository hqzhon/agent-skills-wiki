# rust-anything（逐步迁到 Rust，行为对照）

**Tags:** rust, migration, performance, testing, skill
**Source:** [@GitTrend0x](https://x.com/GitTrend0x/status/2123016010366144917) · 2026-11-18
**Engagement:** 发现帖约 4 赞 / 277 次展示；仓库 [erkamyaman/rust-anything](https://github.com/erkamyaman/rust-anything) 现 2,386★，MIT（2026-11-16 建仓，仍在频繁推送）

## When to use
要把 TypeScript / JavaScript、Python、C、Go、Ruby 或 Java 的一段热路径、一个库甚至整个应用迁到 Rust，并且要求每一步都对照原程序的真实行为，而不是「先重写再看能不能跑」。也适用于先规划迁移，或用 Rust 加速现有代码。

## What it does
先用 CLI / MCP 给原程序录像（生成边沿用例，也可挂上原有测试套件），再一块一块桥接到 Rust（napi-rs / wasm、PyO3、C ABI、cgo、magnus、JNI 等），用 `diff`、`bench`、`shadow` 对照，只有 `gate` 通过才算这块完成。整应用重写走独立的 whole-app 流程：先问清决策、录下整应用、在原程序前加 Rust 前门，再逐单元抬升成纯 Rust 二进制或 crate。PHP / C# 目前只支持部分预览步骤。README 称有数万条录制用例回放。

## Recipe / links
- Repo: https://github.com/erkamyaman/rust-anything（MIT，2,386★）
- 安装 CLI：`cargo install rust-anything`，然后 `rust-anything setup`（会给已检测到的 Claude Code / Codex / Cursor / Gemini CLI 注册 MCP 并写入 skill）。没有 Rust 工具链时可从 [GitHub Releases](https://github.com/erkamyaman/rust-anything/releases) 下预编译包，或在 JS 项目里 `npm install -g rust-anything`
- Claude Code 插件（CLI 需在 `PATH`）：`/plugin install rust-anything --marketplace erkamyaman/rust-anything`
- Skill 路径：`skills/rust-anything/SKILL.md`

## Why it made the cut
有明确迁移场景、完整 SKILL.md / CLI / MCP，以及「先录像再对照」的可验证闭环，不是一份空喊重写的清单。仓库很新但星数和文档都已足够核对。
