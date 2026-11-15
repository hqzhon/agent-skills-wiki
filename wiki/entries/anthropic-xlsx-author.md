# xlsx-author（Anthropic 官方 headless 出 Excel）

**Tags:** finance, excel, spreadsheet, official, skill
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2121778388830756874) · 2026-11-15
**Engagement:** 发现帖热度一般；仓库 [anthropics/financial-services](https://github.com/anthropics/financial-services) 约 41.3k★，Apache-2.0

## When to use
要用已核验的财务数据（例如美股 CSV）在没有打开 Excel 窗口的 headless / 托管 agent 会话里，生成一份可交付、可复核的 `.xlsx`。不适合拉行情，也不适合去改用户正在编辑的工作簿。

## What it does
官方 `xlsx-author` skill。用 Python / `openpyxl` 在磁盘上写出工作簿，约定输出到 `./out/<name>.xlsx`，并在最终回复里给出相对路径以便编排层回收。约定与 [audit-xls](anthropic-audit-xls.md) 对齐：Inputs 表放硬编码输入（蓝字），计算单元格必须是公式（黑字），跨表链接用绿字；另建 Checks 表做资产负债平衡、现金流勾稽等 TRUE/FALSE 检查。一个文件只放一个模型。若会话里已有 `mcp__office__excel_*`（Cowork 插件模式），应改用那些工具去驱动用户正在打开的工作簿，本 skill 只作为无窗口时的出文件兜底。

## Recipe / links
- SKILL.md（本轮发现帖所用路径）：https://github.com/anthropics/financial-services/blob/main/plugins/agent-plugins/kyc-screener/skills/xlsx-author/SKILL.md
- 同内容也出现在 `plugins/agent-plugins/model-builder/skills/xlsx-author/SKILL.md`（[lbo-model](anthropic-lbo-model.md) 条目已提到这一份）
- 预览：`gh skill preview anthropics/financial-services plugins/agent-plugins/kyc-screener/skills/xlsx-author/SKILL.md`
- 安装到 Codex 用户级（`gh skill` 仍为 preview）：`gh skill install anthropics/financial-services plugins/agent-plugins/kyc-screener/skills/xlsx-author/SKILL.md --agent codex --scope user`
- 示例调用：`$xlsx-author`，如把 `AAPL.csv` 做成 `./out/aapl.xlsx`（输入放 Inputs，计算用公式，Checks 核勾稽）
- 装前读完 SKILL.md、LICENSE、脚本与权限；仓库 Apache-2.0 可免费使用，模型与依赖可能收费，不含行情

## Why it made the cut
官方可执行配方，把「无 Excel 窗口也要交出可复核工作簿」收成明确输出约定，并与 audit-xls 的蓝/黑/绿和勾稽检查一致。
