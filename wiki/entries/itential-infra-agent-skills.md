# Itential Infrastructure Agent Skills（官方基础设施技能库）

**Tags:** official, infrastructure, networking, devops, skill-pack
**Source:** [@Itential](https://x.com/Itential/status/2122695045585248299) · 2026-11-17
**Engagement:** 发现帖几乎无互动（1 转帖 / 1 收藏 / 26 次展示）；官方公告同步见 [Itential 新闻稿](https://www.itential.com/news/itential-introduces-open-source-infrastructure-agent-skills/)；仓库 [itential/infra-agent-skills](https://github.com/itential/infra-agent-skills) 现 1★ / 2 forks，Apache-2.0

## When to use
要让 agent 做网络/基础设施操作（DNS 记录、证书、防火墙、变更单、软件升级、IPAM、VPN、容器部署等），并且希望按「一种能力、下面挂各厂商步骤」来加载，而不是每个厂商单独写一套 skill，或临时从厂商 API 文档现场推演。

## What it does
官方开源库，发布时含 40 个按能力组织的 skill、153 份厂商参考。每个能力目录是自包含的 `SKILL.md` + `references/`（索引和分厂商的 procedure / endpoints）。遵循 Agent Skills 规范，可与 Itential FlowAI 或其他兼容宿主一起用；只拷需要的能力目录即可。覆盖从计算开通、容器工作负载到证书、事件和网络变更等操作。技能提供操作指导，执行与权限仍由宿主、提示词和已连接系统约束。

## Recipe / links
- Repo: https://github.com/itential/infra-agent-skills（Apache-2.0，1★）
- 克隆后把需要的 `skills/<capability>/` 拷到或软链到宿主的 skills 目录，例如 Claude Code：
  ```bash
  git clone https://github.com/itential/infra-agent-skills.git
  mkdir -p .claude/skills
  ln -s ../../infra-agent-skills/skills/dns-record-management .claude/skills/dns-record-management
  ```
- 只取一个能力也可用 sparse checkout（见仓库 README）。无需编译或 pip 安装。

## Why it made the cut
厂商官方发布、Apache-2.0、能力清单和厂商参考都在可验证仓库里，场景清楚。星标还很少（新闻稿当日刚公开推广），装前仍要按自己的变更窗口和权限模型使用，它给的是步骤而不是替你执行变更。
