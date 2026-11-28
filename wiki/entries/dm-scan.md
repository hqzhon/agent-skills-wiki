# dm-scan（排查 Solana Direct Mapping 升级会不会把程序打崩）

**Tags:** solana, security, audit, rust, web3, skill
**Source:** [@AshrafSyed](https://x.com/AshrafSyed/status/2126383752695968060) · 2026-11-27
**Engagement:** 作者第一方介绍帖 5 赞；仓库 [ItsAshrafSyed/solana-direct-mapping-scanner](https://github.com/ItsAshrafSyed/solana-direct-mapping-scanner) 当天公开，现 0★，Apache-2.0 / MIT 双许可。

## When to use
要检查 Solana / Anchor / Pinocchio 程序在 Account Data Direct Mapping（SIMD-0460 等）开通之后会不会出 `AccountDataTooSmall`、`InvalidRealloc`、`ReadonlyDataModified`、跨区访问或静默栈布局问题，并希望有 CLI / MCP 扫描和 CI（含 SARIF）时用。不要只靠扫描结果宣称「程序是安全的」——技能要求最后必须给出测试计划。

## What it does
可加载技能 `direct-mapping-audit` 搭配 Rust 扫描器 `dm-scan`。流程包括：确认扫描器可用（或 `cargo install --path crates/dm-scan`）、查询主网/开发网特性开关、扫描源码（`dm-scan scan <program-dir> --format json`）、必要时扫描已部署程序、逐条判定真阳性/假阳性、给出最小修复（例如 `resize` 替代 `realloc`、升级 Anchor 到 1.2.2）、复扫，并以测试网和 `solana-test-validator` 方案收尾。也提供 MCP 工具（`scan_source`、`check_program`、`explain_rule` 等）。

## Recipe / links
- Repo: https://github.com/ItsAshrafSyed/solana-direct-mapping-scanner（0★，Apache-2.0 / MIT）
- 技能路径：`skills/direct-mapping-audit/SKILL.md`
- 安装扫描器与技能：
  ```bash
  cargo install --path crates/dm-scan
  npx skills add ItsAshrafSyed/solana-direct-mapping-scanner
  ```
- 规则说明以 https://solana.com/upgrades/direct-mapping 为准，不要编造升级规则。

## Why it made the cut
第一方发布，场景很具体（一次链上运行时变更引发的程序审计），有 SKILL.md、双许可、CLI/MCP 和明确的验收/测试要求。星标还是零，但配方可执行，值得收录；扫描不能代替测试，条目里已写明。
