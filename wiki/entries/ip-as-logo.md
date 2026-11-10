# ip-as-logo（极简 IP 吉祥物 Logo）

**Tags:** design, logo, mascot, image-gen, branding, skill
**Source:** [@laogeai](https://x.com/laogeai/status/2120030300403278044) · 2026-11-10
**Engagement:** 帖子互动低 · s1dashu/ip-as-logo-skill ~6.5k★ · MIT

## When to use
给产品做一个圆润、极简、在 32×32 也认得出的 IP 吉祥物 / Logo，而不想请设计师或在生图模型里反复抽卡。

## What it does
先读仓库 README / 产品文档推断定位（不够再问一轮）→ 提出三个方向（`主体 — 与产品的关联 — 轮廓特征`）→ 经同意后一次生成 6 张独立候选（A1–C2），可用子代理并行。严格的复杂度预算：4–7 个基本形、2 个 IP 色 + 1 个纯色背景、角色从左下角探出；要求顶级生图模型，禁止退回 SVG，也不做事后挑拣修图。

## Recipe / links
- Repo: https://github.com/s1dashu/ip-as-logo-skill （单个 `SKILL.md`）
- 用法：放进 agent 的 skills 目录，对 agent 说「给这个产品设计一个 IP logo」

## Why it made the cut
规则写得极具体（流程、配色、构图、批次、交付格式全有），场景清晰，社区信号强；是「把审美约束写成配方」的好范例。
