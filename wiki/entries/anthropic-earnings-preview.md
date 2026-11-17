# earnings-preview（Anthropic 官方财报前瞻）

**Tags:** finance, equity-research, earnings, official, skill
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2122593312251224437) · 2026-11-17
**Engagement:** 发现帖互动很少；仓库 [anthropics/financial-services](https://github.com/anthropics/financial-services) 现 41,358★ / 5,759 forks，Apache-2.0

## When to use
财报**发布前**要为一只已覆盖（或即将见印）的股票准备一页前瞻：一致预期、重点观察指标、多空情景和可能决定股价反应的催化剂。不是财报后的季报更新备忘——那条走 [earnings-analysis](anthropic-earnings-analysis.md)。

## What it does
官方 `earnings-preview` 技能，位于 `plugins/vertical-plugins/equity-research/skills/`。流程是：搜集公司与季度、一致预期、发布时间以及上季电话会指引 → 按行业搭「what to watch」指标框架（财务 + 运营）→ 做牛/基/熊三档情景及对股价的含义 → 列出 3–5 个决定反应的催化剂 → 输出一页前瞻（预期表、指标排序、情景表、催化剂、近期走势与期权隐含波动）。技能提醒预期会变，需注明来源和日期，并可用历史业绩反应和隐含波动来校准。

## Recipe / links
- SKILL.md: https://github.com/anthropics/financial-services/blob/main/plugins/vertical-plugins/equity-research/skills/earnings-preview/SKILL.md
- 先审阅再装（GitHub CLI 带 skill 子命令的版本）：`gh skill preview anthropics/financial-services plugins/vertical-plugins/equity-research/skills/earnings-preview/SKILL.md`
- 读完 SKILL.md、LICENSE 与脚本，核对数据源、网络/文件权限后再 `gh skill install anthropics/financial-services plugins/vertical-plugins/equity-research/skills/earnings-preview/SKILL.md --agent codex --scope user`
- 用 `gh skill list --agent codex --scope user` 核对列表后，重开会话再调用
- 不要向技能提供非公开材料；模型额度、数据源和外部依赖仍可能收费
- `gh skill` 目前仍是公开预览功能，先确认本地 CLI 版本支持

## Why it made the cut
官方可加载技能，和已收录的 [earnings-analysis](anthropic-earnings-analysis.md) 分工清楚：一条是印前一页前瞻，一条是印后 8–12 页更新备忘。场景、步骤和输出格式都写在可核对的 `SKILL.md` 里。
