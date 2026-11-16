# BofAI Skills（TRON 钱包 / 链上技能包）

**Tags:** skill-pack, crypto, tron, wallet, cli
**Source:** [@Ashtonexi](https://x.com/Ashtonexi/status/2121909641399427267) · 2026-11-15
**Engagement:** 发现帖互动低；仓库 [BofAI/skills](https://github.com/BofAI/skills) 现 163★，MIT

## When to use
要用 coding agent 操作 TRON 官方 `wallet-cli`、查 Tronscan、走 SunSwap / SunPump / SunPerp 或 USDD 相关流程，并希望技能先守安全边界（尤其是密码不进命令行），而不是让模型直接拼带密钥的命令。

## What it does
BANK OF AI 的 MIT 技能包，本轮核到 6 条 `SKILL.md`：`wallet-cli`、`tronscan-skill`、`sunswap`、`sunpump-agent-skill`、`sunperp-skill`、`usdd-skill`。发帖强调的 `wallet-cli` 覆盖账户、转账、质押、治理、合约、签名和链上查询，并写了拒绝规则：钱包密码不得放入 argv（须走受支持的 stdin），不驱动 Java REPL，DEX 兑换交给 SunSwap 技能。确定性逻辑留给命令行工具，skill 负责选命令、划授权边界、解释结果。

## Recipe / links
- Repo: https://github.com/BofAI/skills（163★，MIT）
- 稳定安装：`npx skills add https://github.com/BofAI/skills/tree/main`
- 默认开发分支 `develop` 可能含未发布改动，只在有意测试时使用
- `wallet-cli` 说明：仓库 `wallet-cli/README.md` 与 `wallet-cli/SKILL.md`

## Why it made the cut
可安装的技能包，场景和安全规则具体（密码不进 argv、分工清楚），有许可证和可核验仓库。面向 TRON 生态，转账和签名仍需人工确认授权；不要把这条当成自动交易或托管钱包建议。
