# Zep Agent Skills（从已验证轨迹自动编译 SKILL.md）

**Tags:** skill-infra, procedural-memory, trace-to-skill, distillation, mcp
**Source:** [@yibie](https://x.com/yibie/status/2121154006978621742) · 2026-11-13（另见 [@sonuv_dev](https://x.com/sonuv_dev/status/2121126511600177613)）
**Engagement:** 原帖热度中等；有官方博客、文档与 arXiv 论文（2611.01386）可核

## When to use
生产环境里的 agent 反复遇到同类任务，你想把大模型（teacher）跑通的步骤沉淀成可复用流程，让更便宜的小模型照着做，而不想做微调；或者想让 agent 的「经验」在多次运行之间保留下来。

## What it does
- 记录每次任务尝试为 Trace（有序事件 + 结果 + 验证强度），也可从 Braintrust / LangSmith 导入
- 只用被工具或评测确认成功的运行做证据；编译器分 Reflector（提案）与 Curator（对证据核查）两个角色，生成或修改按任务族归类的 Skill
- 每个字段须引用对应运行事件；实例数据替换为占位符；来自工具输出的指令会被拒收
- 每个版本可回滚，渲染成标准 Agent Skills 格式的 SKILL.md，agent 通过 MCP 或 SDK 检索使用
- 官方数据：用 Opus 5.5 轨迹编译的 Skills 让三个小模型在 τ³-bench banking / AppWorld / EnterpriseOps-Gym 上通过率提升 4.5–18.8 点，长任务 token 最多降约 45%

## Recipe / links
- 公告：https://www.getzep.com/blog/introducing-zep-agent-skills/
- 快速开始：https://help.getzep.com/agent-skills/quickstart（示例把 `compilation_mode` 设为 `on_close`，关闭一条 Trace 即编译；默认是 `scheduled`）
- 采集 Trace：https://help.getzep.com/agent-skills/capture-traces.md
- 论文：https://arxiv.org/html/2611.01386
- 用法思路：新任务先用前沿模型跑 → 确认成功的 Trace 关闭并标注验证强度 → 编译出 Skill → 小模型执行时检索并读取当前版本

## Why it made the cut
不是单个技能，而是「技能从哪来」的生产化方案：只认已验证结果、逐条引证、可版本回滚，补齐了本目录里手写技能（[agent-skill-builder](agent-skill-builder.md)）和评测技能（[SkillEvaluator](nvidia-skillevaluator.md)）之间的一环。注意是 Zep 的托管服务，非纯开源仓库。
