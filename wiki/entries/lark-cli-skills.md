# 飞书 / Lark 官方 CLI Agent Skills

**Tags:** official, feishu, lark, cli, skill-pack, productivity
**Source:** [@xiaoanlab](https://x.com/xiaoanlab/status/2121250481632637253) · 2026-11-14
**Engagement:** 发现帖热度一般；上游 [larksuite/cli](https://github.com/larksuite/cli) 约 18.1k★，MIT，飞书官方维护

## When to use
要在终端或编码 agent 里操作飞书（消息、文档、多维表格、日历、邮箱、任务、会议、审批等），不想在网页和 App 之间来回切，或希望改动前先 dry-run、拿到结构化 JSON 再往下走。

## What it does
官方 `lark-cli`：200+ 命令覆盖 18 个业务域，仓库 `skills/` 下带 26 个 Agent Skills（README 现写 26；帖子说 20 多个）。`lark-shared` 负责应用配置、登录、身份切换、权限和安全规则，其他 skill 会自动加载它。领域 skill 包括 `lark-im`、`lark-doc`、`lark-sheets`、`lark-base`、`lark-calendar`、`lark-mail`、`lark-task`、`lark-meeting`、`lark-slides`、`lark-approval` 等，另有会议纪要、站会报告两条工作流 skill，以及 `lark-skill-maker` 用于自定义 skill。命令分三层：快捷命令、与平台同步的 API 命令、通用调用；支持 JSON 输出和改前 dry-run。凭证走操作系统密钥链。

## Recipe / links
- Repo: https://github.com/larksuite/cli
- Skills 目录：https://github.com/larksuite/cli/tree/main/skills
- 中文说明：https://github.com/larksuite/cli/blob/main/README.zh.md
- 安装 CLI Skill（官方文档）：`npx skills add larksuite/cli -y -g`
- 使用前先完成飞书应用创建与交互式登录授权

## Why it made the cut
厂商官方 CLI + 可安装 SKILL.md，场景和 Google Workspace CLI Skills 对位，仓库可核对，适合把飞书办公交给 agent。
