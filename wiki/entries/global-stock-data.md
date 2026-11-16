# global-stock-data（美股港股公开数据工具包）

**Tags:** finance, market-data, sec, macro, skill
**Source:** [@huangcheng943](https://x.com/huangcheng943/status/2121915406378303741) · 2026-11-15
**Engagement:** 发现帖互动低；仓库 [simonlin1212/global-stock-data](https://github.com/simonlin1212/global-stock-data) 现 1881★，Apache-2.0

## When to use
要用公开接口查美股 / 港股行情与基本面、Form 4 内部人申报、13F、期权链 / 0DTE、FINRA 空头、VIX 期限结构、央行利率与汇率、台股官方源或美国 CPI / 非农等宏观数据，并希望 agent 按合规分级取数，而不是替你做买卖判断。

## What it does
一份自包含的 `SKILL.md`（Markdown + 内嵌 Python）：17 层、50+ 端点、18 个数据源，官方源优先、调用侧零鉴权（只需 `requests`）。每个数据源标注合规级别并摘录条款原文，「官方」不等于「可任意商用」。作者声明负责取数，不提供投资建议。使用 SEC 或美国宏观（BLS）层前，需在 `SKILL.md` 里把 `SEC_CONTACT` 改成真实姓名和邮箱，否则可能被拒。A 股请用姊妹项目 [a-stock-data](https://github.com/simonlin1212/a-stock-data)。

## Recipe / links
- Repo: https://github.com/simonlin1212/global-stock-data（1881★，Apache-2.0）
- 安装到 Claude Code：

```bash
mkdir -p ~/.claude/skills/global-stock-data
curl -o ~/.claude/skills/global-stock-data/SKILL.md \
  https://raw.githubusercontent.com/simonlin1212/global-stock-data/main/SKILL.md
pip install requests
```

- Codex / OpenClaw：把 `SKILL.md` 放进系统提示或项目上下文；内嵌 Python 可直接跑
- 使用前先读完整 `SKILL.md`、README 和 LICENSE：它会联网，并写入文件；只使用条款允许的公开源

## Why it made the cut
可验证的高星仓库、场景清楚（取数不是下单），SKILL.md 把数据源、合规分级和调用方式写进同一份文件。第三方技能内嵌 Python 且会联网，安装前应检查请求域名、读写和权限。
