# Wallet Theft Detective（GoPlus 官方：只读排查加密资产被盗）

**Tags:** official, goplus, security, web3, wallet, incident-response, skill
**Source:** [@GoPlusSecurity](https://x.com/GoPlusSecurity/status/2126265943055896824) · 2026-11-27
**Engagement:** 官方更新帖 1 赞；仓库 [GoPlusSecurity/wallet-theft-detective](https://github.com/GoPlusSecurity/wallet-theft-detective) 现 5★。根目录有完整 `SKILL.md`。GitHub 许可证字段为 NOASSERTION，收录时不臆造许可。

## When to use
怀疑 Web3 钱包、交易所账户、手机或开发环境遭到**剪贴板劫持、信息窃取、恶意插件、钓鱼、恶意授权、盲签、地址投毒、假钱包、供应链攻击或 iOS 漏洞利用**，需要 agent 做**只读、本地、最小权限**的分诊和可能原因分析时用。它不是链上追赃工具：官方写明 v1 **不查询区块链、不分析交易或资金流，也不读取助记词、私钥、密码、Cookie、Token 或钱包文件**。

## What it does
GoPlus 提供的调查指南技能，给 Codex、Claude Code、OpenClaw 等宿主用。agent 负责提问、整理时间线、指导检查本地/设备线索，并给出处置建议；不要再叠一层「主 agent」编排。若宿主没有终端、文件或浏览器能力，就改提供手工只读步骤。macOS 与 Windows 都是一等公民。本窗更新强调了典型盗币场景覆盖，以及恶意二维码、仿冒站点、应用内浏览器/Safari 跳转、无交互漏洞等 iOS 利用链排查。不会使用技能的用户，官方另提供调查问卷收集事件时间线。

## Recipe / links
- Repo / SKILL.md: https://github.com/GoPlusSecurity/wallet-theft-detective/blob/main/SKILL.md
- 仓库：https://github.com/GoPlusSecurity/wallet-theft-detective（5★；许可未在 GitHub 明确标出）
- 安装：将仓库中的 `SKILL.md`（及同目录所需资源）导入 Codex / Claude Code / OpenClaw 等支持 Agent Skills 的环境。按官方说明保持只读、最小权限。
- 官方问卷（给无法跑 agent 的使用者）：见源帖中的 Google Form 链接

## Why it made the cut
厂商官方、场景清楚、有可核的 SKILL.md，而且主动把「不碰密钥和钱包文件」写进技能说明，适合作为应急分诊配方。星标和帖子互动都还弱，当作官方手册而不是高热社区项目。它不能代替专业取证或链上追踪，输出也需人工判断。
