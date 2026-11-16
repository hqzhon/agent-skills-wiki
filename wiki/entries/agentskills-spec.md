# Agent Skills 开放标准（agentskills / skills-ref）

**Tags:** meta, specification, validation, official, skill-infra
**Source:** [@KaiyuanDesk](https://x.com/KaiyuanDesk/status/2122134059774070973) · 2026-11-16
**Engagement:** 发现帖互动很少 · 仓库 [agentskills/agentskills](https://github.com/agentskills/agentskills) 现 27,330★ / 2,036 forks，Apache-2.0

## When to use
要按开放标准编写、校验或接入 Agent Skill（`SKILL.md` 目录：至少含 `name` / `description` 与步骤说明，可选 scripts / references / assets），或给自己的 agent 生成 `<available_skills>` 提示块。不要把它当成一条可加载的业务技能，也不要把参考实现 `skills-ref` 直接当生产依赖。

## What it does
[agentskills.io](https://agentskills.io) 背后的规范与文档仓库：约定技能就是带 `SKILL.md` 的文件夹，以及元数据、资源目录的组织方式。同仓 `skills-ref/` 是 Python 参考工具，可校验目录、读取属性，并把技能列表转成给模型看的 XML。README 写明该库**仅供演示，不用于生产**。

## Recipe / links
- Repo: https://github.com/agentskills/agentskills（Apache-2.0，27,330★）
- 规范站点：https://agentskills.io
- 参考 CLI（在克隆仓库的 `skills-ref/` 目录里，先建虚拟环境再装）：
  ```bash
  cd skills-ref
  python -m venv .venv && source .venv/bin/activate
  pip install -e .
  skills-ref validate ./my-skill
  skills-ref read-properties ./my-skill
  skills-ref to-prompt ./skill-a ./skill-b
  ```
  也可用 `uv sync` 代替 pip。本轮发现帖是文档核验，未实测命令。

## Why it made the cut
这是 Agent Skills 开放标准的权威副本，也是本 wiki 大多数条目所遵循的格式来源。有可验证仓库、明确的「何时用」（写技能 / 做规范校验），以及具体的校验命令。同主题的评测/卫生工具见 [SkillEvaluator](nvidia-skillevaluator.md)、[agnix](agnix.md)、[skill-guard](skill-guard.md)；本条管的是规范本身，不是某条业务配方。
