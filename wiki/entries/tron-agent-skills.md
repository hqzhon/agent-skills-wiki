# TRON Agent Skills（TronGrid）

**Tags:** blockchain, tron, trongrid, mcp, skill-pack, official
**Source:** [@Ashtonexi](https://x.com/Ashtonexi/status/2114842664701243715) · 2026-10-26
**Engagement:** discovery post (low) · official TRON developer docs

## When to use
When an agent needs to query TRON on-chain data in natural language — wallet profiling, token scans, tx decode, contract inspection, network metrics — without hand-rolling TronGrid REST calls.

## What it does
Official TronGrid MCP server (`https://mcp.trongrid.io/mcp`) plus standalone skill packages (ClawHub / OpenClaw) that orchestrate those tools into eight workflows: Account Profiling, Block Info, Contract Analysis, Data Insights, Token List, Token Scanner, Transaction Info, TRX Info. MCP exposes tools; skills define the multi-step analysis recipes. Both should be configured for best results.

## Recipe / links
- Skills overview: https://developers.tron.network/docs/skills
- MCP guide: https://developers.tron.network/docs/mcp
- MCP endpoint: `https://mcp.trongrid.io/mcp` (optional `TRON-PRO-API-KEY` header)
- Example OpenClaw install: `openclaw skills install @greason/trongrid-account-profiling`
- Developer hub: https://developers.tron.network

## Why it made the cut
Vendor docs with installable skill packages + live MCP, clear when-to-use table, and verifiable public documentation — reusable for any TRON data / security research agent.
