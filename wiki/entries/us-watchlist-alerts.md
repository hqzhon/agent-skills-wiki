# us-watchlist-alerts（美股观察名单提醒）

**Tags:** finance, investing, alerts, skill-pack, python
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2119739293589774716) · 2026-11-09
**Engagement:** 推广帖 · eli-alvarado/us-watchlist-alerts · MIT · ~4★

## When to use
维护美股自选股：按价格、涨跌幅、52 周高低、均线、RSI、成交量或财报等条件提醒，或要开盘/收盘简报；**只做信息提示、不下单**，希望 Claude Code / Codex / Cursor / Gemini CLI 直接加载 SKILL.md。

## What it does
三个 Agent Skills：`price-alerts`、`watchlist-brief`、`watchlist-manager`。默认用 Python 标准库 + 非官方 Yahoo Finance chart，无需 API key（行情可能延迟）。可选 cron / ntfy 做 agent 关掉后的工作日提醒。数据落在项目或用户配置目录，不进 skill 安装目录。

## Recipe / links
- Repo: https://github.com/eli-alvarado/us-watchlist-alerts （MIT）
- 安装：`npx skills add eli-alvarado/us-watchlist-alerts -y -a codex`（`-a` 按 agent 换）
- 验证：`python3 .agents/skills/price-alerts/scripts/quickstart.py`（离线 fixture）
- 安全：先读 [`SECURITY.md`](https://github.com/eli-alvarado/us-watchlist-alerts/blob/main/SECURITY.md) 与各 `SKILL.md`

## Why it made the cut
有具体 SKILL.md 三件套、安装与验证路径、明确「不下单」边界；与 InvestSkill（基本面框架）互补，偏观察名单与提醒。
