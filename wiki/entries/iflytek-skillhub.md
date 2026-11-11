# SkillHub（科大讯飞，企业级 skill 注册中心）

**Tags:** registry, enterprise, self-hosted, versioning, skill-infra
**Source:** [@xiaoanlab](https://x.com/xiaoanlab/status/2120178360240496940) · 2026-11-10
**Engagement:** iflytek/skillhub ~5.4k★ · Apache-2.0

## When to use
团队里 skill 越写越多、到处复制粘贴，出现版本对不上、谁改了不知道的问题时；需要在防火墙内私有部署、统一发布和安装 skill。

## What it does
自托管的 agent skill 注册中心：skill 包按命名空间发布并做版本管理，RBAC 权限和审计日志治理，CLI 一条命令安装；支持 Docker / Kubernetes 本地部署。

## Recipe / links
- Repo: https://github.com/iflytek/skillhub（[中文 README](https://github.com/iflytek/skillhub/blob/HEAD/README_zh.md)）
- 文档: https://zread.ai/iflytek/skillhub
- 同类：[claude-code-templates](claude-code-templates.md)（公共组件注册表 + CLI）

## Why it made the cut
不是单个配方，而是 skill 的分发与治理基础设施；有完整仓库、文档和明确的团队场景，适合想把 skill 规模化的人。
