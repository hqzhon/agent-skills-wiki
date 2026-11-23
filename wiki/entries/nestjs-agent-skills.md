# NestJS Agent Skills（官方：用当前 API 给 Nest 应用写代码）

**Tags:** official, nestjs, typescript, backend, skill-pack
**Source:** [@nestframework](https://x.com/nestframework/status/2123741121482489930) · 2026-11-20
**Engagement:** 官方发布帖 654 赞 / 72 转 / 244 收藏；仓库 [nestjs/agent-skills](https://github.com/nestjs/agent-skills) 145★，MIT。本窗新建（2026-11-20）。

## When to use
要用编码 agent **创建或扩展 NestJS 应用**，并希望它按**当前**官方 API、官方包和仍然能通过测试的常见坑来写，而不是凭过时训练数据瞎编时使用。覆盖从起项目、加接口、认证授权、持久化、测试到生产准备的完整路径。

## What it does
NestJS 官方 Agent Skills 包。每个技能是一个带 `SKILL.md` 的目录，另有 `references/` 长配方；官方写明每条配方都在已发布的包上跑过。六个技能按任务自动加载，不必手敲命令：

- `nestjs`：起项目、目录布局、模块系统、文档入口和常见错误
- `nestjs-feature`：增改端点、校验（Zod 的 `@Body({ schema })` 或 class-validator）、状态码、SSE 等
- `nestjs-auth`：`@nestjs/authentication` 与 `@nestjs/authorization`
- `nestjs-data`：`@nestjs/drizzle` / `@nestjs/typeorm`、迁移、分页、事务
- `nestjs-testing`：单测 / 服务测 / e2e，覆盖 provider 与全局 guard
- `nestjs-production`：配置、日志、NestJS Observe、健康检查、限流、OpenAPI、关停与部署

官方特别点出训练数据里没有的坑，例如登录接口泄漏邮箱是否存在、`@IsOptional()` 把 `null` 放进 500、限流看不到用户、事件流在密钥吊销后仍存活等。

## Recipe / links
- Repo：https://github.com/nestjs/agent-skills（MIT，145★）
- 官方安装（发布帖）：
  ```
  npx @nestjs/skills add
  ```
  也可 `npx skills add nestjs/agent-skills`。技能在仓库 `skills/` 目录；`nest new` 已内建。
- 适用于 Claude Code、Codex、Cursor 及其他符合 Agent Skills 格式的助手。

## Why it made the cut
框架官方包，场景清楚，六个可装技能都有配方和参考文档，专门补上模型过时记忆。本窗由 @nestframework 发布。
