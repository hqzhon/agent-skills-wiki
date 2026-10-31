# commerce-agent-skills

**Tags:** skill-pack, e-commerce, payments, woocommerce, shopify, webhooks, evals
**Source:** [@nasersadrmanesh](https://x.com/nasersadrmanesh/status/2116295745015894508) · 2026-10-31
**Engagement:** new (~1★ on GitHub); included for depth of material, not popularity

## When to use
编码 agent 在做**电商 / 市场平台**功能时：结账、支付网关（Stripe、Zarinpal 等）、订单与支付 webhook、退款/退货、多仓库存、B2B 定价、税运费、订阅计费、商品目录导入迁移、店铺 SEO/无障碍/性能、给店铺暴露 MCP 工具。专治「看着对、但漏了 webhook 幂等、退款边界、超卖」的代码。

## What it does
**29** 个 Agent Skills（Agent Skills 规范：文件夹 + SKILL.md），每个配一条短 Markdown rule、评测任务与示例；`scripts/run-evals.mjs` 按 fixtures 给回答打分，CI 里有严格校验器（版本、必需章节、每个评测词都在技能里教过）。

## Recipe / links
- Repo: https://github.com/sadrmanesh/commerce-agent-skills (MIT)
- Docs: https://sadrmanesh.github.io/commerce-agent-skills/
- Install: `npx @sadrmanesh/commerce-agent-skills init`（复制到 `.agents/skills/` 与 `.agents/rules/`）；`list` / `add <skill…>` / `--dry-run` / `--layout root`
- 代表技能：`payment-gateway-integration`、`order-and-webhook-reliability`、`inventory-and-multi-warehouse`、`returns-and-refunds`、`mcp-store-tooling`

## Why it made the cut
具体配方 + 清晰场景 + 可验证材料（每个技能有 eval fixtures 和评分脚本），一条命令安装；社区信号尚弱，属「材料过硬、热度待观察」。
