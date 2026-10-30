# CodexQA（本地优先验证技能包）

**Tags:** qa, testing, code-review, local-first, skill-pack, chinese
**Source:** [@argusiccom](https://x.com/argusiccom/status/2116002266284965970) · 2026-10-30
**Engagement:** tipster (~52 impressions); material = openqa-cn/codexqa ~236★ Apache-2.0

## When to use
After AI coding, when you need to **合入前验证质量**：变更影响面、逻辑缺陷、需求符合度、用例/测试数据、浏览器回放证据、根因分析——而不是只靠“看起来能跑”。

## What it does
11 local-first Agent Skills for Cursor / Claude Code / Codex / OpenClaw：10 个专项验证技能 + 1 个 router（`codexqa-skill-router`）。覆盖 defect scan、code review、change analysis、requirement analyzer、testcase/testdata generation、browser replay、RCA 等；强调本地可装、可复现。

## Recipe / links
- Repo: https://github.com/openqa-cn/codexqa
- Skills index: `skills.json` · `skills/`
- Example installs:
  - `npx skills add openqa-cn/codexqa --skill codexqa-skill-router`
  - `npx skills add openqa-cn/codexqa --skill codexqa-defect-analyzer`
  - `npx skills add openqa-cn/codexqa --skill codexqa-code-reviewer`
- Also: README.zh-CN.md · benchmarks/ · schemas/

## Why it made the cut
Verified multi-skill QA pack with explicit install commands and a clear post-codegen verification use case—complements shipping skills rather than duplicating them.
