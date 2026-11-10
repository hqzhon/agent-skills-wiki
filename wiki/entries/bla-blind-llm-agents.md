# BLA / Blind LLM Agents（Counter-REA 加固技能）

**Tags:** security, anti-reverse-engineering, mcp, hardening, skill
**Source:** [@zg0820](https://x.com/zg0820/status/2119625103361380462) · 2026-11-09
**Engagement:** 发现帖 · qybaihe/bla · MIT · 3918★

## When to use
你要保护**自己的**发布产物（Electron/ASAR、JS bundle、Python、WASM、原生二进制等）对抗 AI 逆向 agent（如 `morluto/rea` 一类自主反编译/侦察流水线）：审计暴露面、一键加固、或让 coding agent 按剧本做语义级 decoy 编织。明确**防御自有软件**；拒绝破解第三方。

## What it does
仓库带 Agent Skills 规范技能 `blind-llm-agents`：主机 coding agent 负责读业务语义、按 `bla_lint` / `bla_weave_plan` 的 surgical workorder 改源码；`bla-agents` MCP/CLI 负责确定性 Counter-REA 耗尽盾与验证。口号 Poison → Exhaust → Hallucinate；宣称 25+ MCP 防御工具、19+ 产物格式、14 目标基准与运行时等价验证。默认动词 `bla_harden`。

## Recipe / links
- Repo: https://github.com/qybaihe/bla （MIT，约 3918★）
- CLI：`npx bla-agents harden .` · npm：`bla-agents`
- Skill：`.agents/skills/blind-llm-agents/SKILL.md`
- 官网 / CrackMe：https://bla.tools/

## Why it made the cut
真实 SKILL.md 四阶段加固剧本 + MCP/CLI 可验证材料，星标与文档完整；蓝队方向与已收录的 REA/逆向攻击侧技能形成对照。
