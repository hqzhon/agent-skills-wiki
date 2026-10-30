# Microsoft SkillOpt（训练 Skill.md，不动模型权重）

**Tags:** skill-authoring, evaluation, microsoft, optimization, skill-pack, official
**Source:** [@_vmlops](https://x.com/_vmlops/status/2115854336094073184) · [@ruyi3699](https://x.com/ruyi3699/status/2115821208151244935) · 2026-10-29
**Engagement:** tipster posts; repo ~18.8k★ · MIT · aka.ms/skillopt

## When to use
When a hand-written `SKILL.md` 已经能跑，但你想用 **轨迹反馈 + 留出验证** 系统迭代它——像训网络一样训 skill 文档，而不是改模型权重或无限手搓 Prompt。

## What it does
Treats the skill document as the trainable state of a frozen agent. An optimizer model proposes bounded add/delete/replace edits from scored rollouts; default path accepts a candidate only when held-out validation strictly improves. Deployable artifact is a compact `best_skill.md` (often 300–2k tokens) with **zero extra model calls at inference**. Paper-style results claim best/tied-best across evaluated cells; GPT-5.5 lifts reported on direct chat / Codex / Claude Code harnesses. **SkillOpt-Sleep** plugins mine recurring tasks from local sessions and stage gated skill updates for Cursor, Claude Code, Codex, Copilot, Devin, etc.

## Recipe / links
- Repo: https://github.com/microsoft/SkillOpt (~18.8k★, MIT)
- Docs / project: https://aka.ms/skillopt · https://microsoft.github.io/SkillOpt/
- Install core: `pip install skillopt`（Python ≥ 3.10）
- Agent plugins under `plugins/`（Cursor / Claude Code / Codex install scripts in README）
- Sleep loop: harvest sessions → mine tasks → replay → propose edits → validate → you adopt

## Why it made the cut
Official Microsoft OSS with a clear train-the-skill recipe, validation gate, multi-harness plugins, and strong star signal—meta tooling for skill authors, not another prompt dump.
