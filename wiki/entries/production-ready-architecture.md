# production-ready-architecture（带出处的生产级架构评审）

**Tags:** architecture, review, security, payments, cicd, skill
**Source:** [@n_bukhtiyarova](https://x.com/n_bukhtiyarova/status/2124830631712493825) · 2026-11-23
**Engagement:** 发现帖当时近乎 0 互动；仓库 [natdexterra/production-ready-architecture](https://github.com/natdexterra/production-ready-architecture) 本窗新建，0★ / MIT。材料本身完整：SKILL.md + 7 份 references + 会过期事实表。

## When to use
要给 web/移动应用做架构评审或选型，而不是让模型凭记忆拍板：单体还是微服务、会话/Cookie/JWT/OAuth 与 token 存放、支付幂等与 webhook 对账、环境/CI/预览发布/数据库迁移、密钥与移动端 token、或评估外包方案是否「能上生产」。用户没说「架构」但在问「token 放哪」「这份说明能上线吗」时也应触发。不做视觉设计或文案。

## What it does
按风险级别给默认方案，并写明何时改默认（例如在独立发布被证实之前先用模块化单体，访问模式不匹配之前先用 PostgreSQL）。每条建议标明出处（OWASP、IETF RFC、MDN、web.dev、Stripe、Fowler/DORA 等），并给出处分级。会过期的事实（草案状态、标准版本、套餐限额等）标 ⏳，在 `references/sources.md` 里给出权威 URL 和技能所写的值，引用前应对页复核。附带认证、移动、交付、支付、安全隐私、可靠性/可观测性参考，以及开发前 / PR / 发布清单和 ADR 模板。不是渗透测试，也不是法律或合规意见。

## Recipe / links
- Repo: https://github.com/natdexterra/production-ready-architecture（MIT）
- 安装：把仓库（含 `SKILL.md` 与 `references/`）拷到 agent 的 skills 目录，例如 `git clone https://github.com/natdexterra/production-ready-architecture ~/.claude/skills/production-ready-architecture`
- 入口是 `SKILL.md`；易变事实见 `references/sources.md`，核对记录在 `CHANGELOG.md`

## Why it made the cut
星数还是 0，但配方不是空喊「先做架构」：有默认值、改默认的条件、分级出处和过期事实对照表，参考文件分域可查。适合检查 agent 搭出来的应用能不能上线，而不是再要一份空泛的架构图。
