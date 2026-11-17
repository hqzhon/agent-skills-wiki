# thesis-tracker（Anthropic 官方投资论点跟踪）

**Tags:** finance, equity-research, portfolio, official, skill
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2122502730321367294) · 2026-11-17（安装说明见[后续帖](https://x.com/huangcheng943/status/2122502788949344631)）
**Engagement:** 发现帖 1 赞；仓库 [anthropics/financial-services](https://github.com/anthropics/financial-services) 约 41.4k★，Apache-2.0

## When to use
维护或更新组合持仓、观察名单的投资论点：写入新信息、检查论点是否仍成立、追加数据点或回顾持仓理由。触发示例："update thesis for [company]"、"is my thesis still intact"、"thesis check"。不是下单或给出投资建议的工具。

## What it does
官方 `thesis-tracker` 技能：新建论点时记录公司/代码、多空、1–2 句核心论点、支柱、否决风险、催化剂、目标估值与止损触发；更新时对照新信息检查支柱是否仍成立。位于 equity-research 插件中，与已收录的 [initiating-coverage](anthropic-initiating-coverage.md) 等研究类技能同仓。

## Recipe / links
- SKILL.md: https://github.com/anthropics/financial-services/blob/main/plugins/vertical-plugins/equity-research/skills/thesis-tracker/SKILL.md
- 先审第三方 Skill：读完整 SKILL.md、附带文件与 LICENSE，检查脚本涉及的文件/网络权限
- 预览：`gh skill preview anthropics/financial-services plugins/vertical-plugins/equity-research/skills/thesis-tracker/SKILL.md`
- 安装到 Codex 用户目录（`gh skill` 仍为 preview）：`gh skill install anthropics/financial-services plugins/vertical-plugins/equity-research/skills/thesis-tracker/SKILL.md --agent codex --scope user`
- 用 `gh skill list --agent codex --scope user` 确认；装完重开会话再显式调用

## Why it made the cut
官方维护的完整 SKILL.md，适用场景和字段结构清楚，可在大仓库里直接核对；与同系列已收录的股权研究技能互补。
