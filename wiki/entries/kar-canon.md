# kar-canon（JSON 规范化等价证明）

**Tags:** json, canonicalization, diff, deterministic, skill
**Source:** [@ainativesol](https://x.com/ainativesol/status/2121524252394537111) · 2026-11-14
**Engagement:** 发现帖互动低；仓库 [sjgant80-hub/kar-canon](https://github.com/sjgant80-hub/kar-canon) 0★，MIT；有可在浏览器里跑的演示页

## When to use
要判断两份 JSON（API 响应、工具调用参数、缓存快照、配置）是不是同一份数据，而不是看文本像不像。也适用于找出大 JSON 里真正改动的路径，并给复核人一个可重算的哈希收据。不负责 schema 校验。

## What it does
按 RFC 8785 思路做确定性规范化（各层对象键按 code unit 排序、数组保序、数字最短往返形式、最小转义），再对规范字节做 SHA-256：哈希相同则数据相同，否则列出每个改动/新增/删除/类型变化的路径。全程无 LLM 裁判、无网络。浏览器页、`scripts/kar-canon.mjs` 和 skill 脚本共享同一份 KERNEL，CI 会检查三者是否一致。诚实限制：数组顺序算数据、数值精度跟 JS 双精度、尚未跑完整 RFC 8785 套件。

## Recipe / links
- Repo: https://github.com/sjgant80-hub/kar-canon
- SKILL.md: https://github.com/sjgant80-hub/kar-canon/blob/main/SKILL.md
- Live demo（纯前端，不上传）：https://sjgant80-hub.github.io/kar-canon/
- 本地：`node scripts/kar-canon.mjs examples/tamper.json`（Node 20+，无依赖）
- 技能市场包：`node make-zip.mjs` 生成 `dist/kar-canon.zip`

## Why it made the cut
场景清楚（「看起来一样」不够，要可重算的等价证明），有 SKILL.md、无依赖脚本和可点开的演示；星标虽无，材料可验证，适合给 agent 核对工具调用或日志快照。
