# AI Werk Skills（编码 Agent 里的五阶段软件交付线）

**Tags:** software-delivery, workflow, planning, review, skill-pack
**Source:** [@AnPod](https://x.com/AnPod/status/2125170054107136167) · 2026-11-24
**Engagement:** 本窗为作者开源说明（2 赞）；仓库 [AnPod/ai-software-factory](https://github.com/AnPod/ai-software-factory) 现 0★，Apache-2.0，含 23 个 SKILL.md，并有 CI、SkillSpector 扫描和 agent evals

## When to use
想在已经在用的编码 agent（Claude Code、Codex、Copilot CLI、Cursor、Gemini CLI 等）里，搭一条可重复的软件交付线：先访谈约束和工具，再把需求、计划、实现、评审和发布写进可持久化的项目记忆。不需要另开服务器或账号。

## What it does
一套纯 Markdown Agent Skills。\`aiwerk-init\` 先采访团队使用的 harness、工作从哪进来、启用哪些 SDLC 阶段以及自主程度，然后在 \`.aiwerk/brain/\` 写下时间戳项目记忆；后续技能都先读这块 brain。仓库还包含 intake / survey / spec / plan / policy / sandbox / review / health / release / incident 等技能，强调先询问再改环境，并把 tickets、仓库文件和工具输出当作不可信数据。作者声明无服务器、无数据库、无账号，克隆后链上技能即可。

## Recipe / links
- Repo: https://github.com/AnPod/ai-software-factory（0★，Apache-2.0）
- 快速开始：克隆仓库，按 README 把 \`skills/\` 链到本地技能目录，然后让 agent 运行 \`aiwerk-init\`
- 也可：\`npx skills add AnPod/ai-software-factory\`
- 技能示例：[skills/aiwerk-init/SKILL.md](https://github.com/AnPod/ai-software-factory/blob/main/skills/aiwerk-init/SKILL.md)
- CI：构建检查 + SkillSpector + evals

## Why it made the cut
星数为零，但配方完整：23 个可加载 \`SKILL.md\`、清楚的使用场景、brain 持久化规则，以及扫描/评测工作流。和已收录的 [Agentic Production Skills](agentic-production-skills.md)、[project-health](project-health.md)、[planning-with-files](planning-with-files.md) 同类，偏「把整条交付线装进现有 agent」，而不是单次审计或单次计划落盘。本窗即作者发布帖。
