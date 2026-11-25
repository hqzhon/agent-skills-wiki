# HashiCorp Agent Skills（官方）

**Tags:** official, hashicorp, terraform, packer, skill-pack
**Source:** [@Astrodevil_](https://x.com/Astrodevil_/status/2125446900103209152) · 2026-11-25
**Engagement:** 本窗官方盘点帖（0 赞）；仓库 [hashicorp/agent-skills](https://github.com/hashicorp/agent-skills) 现 939★，MPL-2.0，2026-11-04 仍有推送

## When to use
要用编码 agent 写或重构 Terraform 模块 / Provider、跑测试与策略，或用 Packer 做 AWS AMI、Azure 镜像、Windows 构建并推送到 registry 时用。

## What it does
官方 20 个技能，按产品插件组织：Terraform 16 个（风格、测试、Stacks、策略、模块重构、Provider 开发与迁移等），Packer 4 个。旧的插件 ID（如 `terraform-code-generation`）已迁移到 `terraform@hashicorp` / `packer@hashicorp`，路径改为 `plugins/<product>/skills/<skill-name>`。完整清单与生命周期状态见仓库 `SKILLS.md`。

## Recipe / links
- Repo: https://github.com/hashicorp/agent-skills（939★，MPL-2.0）
- 列出并安装：`npx skills add hashicorp/agent-skills`
- 单个技能示例：`npx skills add hashicorp/agent-skills/plugins/terraform/skills/terraform-style-guide`
- 产品包请按 README 使用 `terraform@hashicorp` 或 `packer@hashicorp`，不要再用已废弃的插件 ID
- 许可是 MPL-2.0；第三方 MCP/LLM 的条款由对应提供方负责

## Why it made the cut
HashiCorp 官方 Terraform / Packer 技能包，20 个可加载 SKILL.md、安装路径和迁移说明都写清楚。939★、MPL-2.0。本窗按官方盘点补收。
