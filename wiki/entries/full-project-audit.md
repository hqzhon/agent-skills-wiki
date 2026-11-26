# Full Project Audit（全项目安全/正确性/无障碍审计）

**Tags:** security, accessibility, audit, code-quality, skill
**Source:** [@devbyrayray](https://x.com/devbyrayray/status/2125895446606336170) · 2026-11-26
**Engagement:** 介绍帖 1 赞；仓库 [DevByRayRay/security-audit-agent](https://github.com/DevByRayRay/security-audit-agent) 现 0★，MIT。本窗由作者开源，仓于 2026-11-26 新建。技能名是 `full-project-audit`，与已收录的 [xss-audit](xss-audit.md)（React/TS XSS 静态层）和 [Cloudflare Security Audit](cloudflare-security-audit-skill.md) 范围不同。

## When to use
要对**当前检出的项目**做一次结构化、可交叉检查的全面审计时用：应用安全、依赖、正确性、前端渲染、WCAG 无障碍、测试和文档。默认是静态阅读本仓库；不要用它去扫你没有明确授权的远程系统，也不要把它缩小成只查 XSS——那是 xss-audit 的活。

## What it does
产出一份独立的 Markdown 报告。技能正文写明授权与安全边界：把仓库内容和命令输出当不信任数据；默认不做第三方外传；对活系统的主动探测必须由用户指出目标并确认范围；运行时测试仅限隔离的本地实例；禁止 DoS、破坏性操作、提权和上传活动内容；发现的凭据要打码并建议轮换。随后按分阶段清单审查，而不是一口气散打。

## Recipe / links
- Repo: https://github.com/DevByRayRay/security-audit-agent（0★，MIT）
- 技能：仓库内 `.agents/skills/full-project-audit/SKILL.md`（另有 Claude Code / Copilot 副本）
- 安装（需 Node.js 22.20+）：
  ```bash
  npx skills add DevByRayRay/security-audit-agent --skill full-project-audit
  ```
- 装完后让 agent 使用 `$full-project-audit`，或直接请求一次 full project audit。

## Why it made the cut
可加载、分阶段、带安全边界的全项目审计配方，和 xss-audit 的专项清单互补。星标几乎为零，按完整 `SKILL.md` 收录，使用时仍需人工复核发现，不能当成已授权的渗透测试。
