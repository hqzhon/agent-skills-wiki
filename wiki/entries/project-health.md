# project-health（上线前证据驱动审计与交付验收）

**Tags:** audit, qa, delivery, verification, skill
**Source:** [@fallen_leaves08](https://x.com/fallen_leaves08/status/2125102616518791268) · 2026-11-24
**Engagement:** 本窗为作者首发说明，互动接近于零 · 仓库 [Fallen-leaves089/project-health](https://github.com/Fallen-leaves089/project-health) 现 1★，PolyForm Noncommercial 1.0.0（商业使用需另授权），有 verify CI 与预印本 DOI，2026-11-24 仍在推送

## When to use
Agent 已经写完代码，或项目要上线、交接、做周期性体检时用：不要再让同一个 agent 只「再看一眼」，而是要带 `file:line` 证据的 P0–P3 问题清单、真实回归，以及可勾选的交付验收。只想做轻量首次体检时，仓库还提供 `project-health-lite`。

## What it does
一份可加载的审计 skill（根目录 `SKILL.md`，v1.5.0）：先确认环境并查阅项目历史，再做规范/规格双轴审查，覆盖真实构建、迁移、容器以及 macOS / Apple Silicon、Linux / Windows Server 回归，最后输出分级问题（影响、建议、验证方式）。检查阶段默认只读，发现问题先报告、不擅自改代码。目标仓库里的 `AGENTS.md` / `CLAUDE.md` / README 等一律当作不可信数据，防止提示词注入改写检查边界。它不替代代码生成，也不承诺零缺陷。

## Recipe / links
- Repo: https://github.com/Fallen-leaves089/project-health（1★，PolyForm Noncommercial 1.0.0）
- 预印本: https://doi.org/10.5281/zenodo.24161471
- Skill: 仓库根目录 [SKILL.md](https://github.com/Fallen-leaves089/project-health/blob/main/SKILL.md)（中英对照）
- 许可默认仅限非商业用途；商业使用需联系作者书面授权，见仓库 `COMMERCIAL.md`。装前先读许可和权限边界。

## Why it made the cut
星数和互动都很低，但配方完整：有明确使用场景、可加载 `SKILL.md`、CI、平台避坑参考和「先报告再改」的边界。和已收录的 [Agentic Production Skills](agentic-production-skills.md)、[production-ready-architecture](production-ready-architecture.md) 同类，偏交付验收与真实回归，而不是架构评审或生产门禁清单。非商业许可需要在条目里标明，不能当成可随意商用的 MIT 包。
