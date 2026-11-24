# Claude for Legal（Anthropic 官方法律工作流插件包）

**Tags:** official, legal, anthropic, skill-pack, cowork
**Source:** [@r3ktFM](https://x.com/r3ktFM/status/2125079629467910255) · 2026-11-24
**Engagement:** 本窗为安装说明转述，互动很低 · 仓库 [anthropics/claude-for-legal](https://github.com/anthropics/claude-for-legal) 现 10,078★，Apache-2.0，2026-11-21 仍在推送

## When to use
要让 Claude Cowork / Claude Code 按律师工作流起草材料时用：隐私/DPO、商事合同、公司与并购、劳动、产品法务、知识产权、诉讼、监管合规、AI 治理，以及法学院诊所和法学学生学习。所有输出都是供律师复核的草稿，不是法律意见，也不能代替律师。

## What it does
Anthropic 官方的法律插件套件：同一套系统提示和技能，既可以当 Cowork / Claude Code 插件安装，也可以经 Claude Managed Agents API 部署。公开仓里能搜到约 157 个 `SKILL.md`，按业务域分成 12 个插件（如 `privacy-legal`、`commercial-legal`、`ip-legal`、`litigation-legal`、`ai-governance-legal`、`legal-clinic`、`law-student`、`legal-builder-hub` 等）。默认强调引用来源、保守处理特权和管辖假设，在对外发送、提交或依赖结论前设有明确门禁。

## Recipe / links
- Repo: https://github.com/anthropics/claude-for-legal（10,078★，Apache-2.0）
- 快速开始: [QUICKSTART.md](https://github.com/anthropics/claude-for-legal/blob/main/QUICKSTART.md)
- Claude Code 安装市场后按角色装插件，例如：
  ```text
  /plugin marketplace add anthropics/claude-for-legal
  /plugin install privacy-legal@claude-for-legal
  ```
  装完需重启 Claude Code，再跑该插件的 cold-start / 首条命令。官方建议装到 user scope，以便读取你明确指定的项目外文件。
- 引用若要标成已核实，需连接调研工具（如 CourtListener）。插件不代表 Anthropic 的法律立场。

## Why it made the cut
厂商官方、Apache-2.0、可加载的角色插件 + 大量 `SKILL.md`，使用场景和护栏写得很清楚。本窗介绍帖本身没有热度，但仓库有 1 万星，属于高信号漏收，值得作为法律域的官方入口。与已收录的 [Knowledge Work Plugins](knowledge-work-plugins.md) 互补：后者是多角色通用包，本仓专做法务工作流。
