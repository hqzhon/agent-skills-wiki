# CF Daml Skill（Canton Network 上的 Daml 智能合约）

**Tags:** official, daml, canton, smart-contracts, skill
**Source:** [@Jpandya26](https://x.com/Jpandya26/status/2125173050018848911) · 2026-11-24
**Engagement:** 本窗为 v2.0.0 更新说明（6 赞）；仓库 [canton-network-devs/CF-Daml-Skill](https://github.com/canton-network-devs/CF-Daml-Skill) 现 4★，package.json 标明 Apache-2.0（根目录未见 LICENSE 文件）

## When to use
在 Canton Network 上编写、审阅或调试 Daml 智能合约，或需要跟上 Canton 3.5–3.7、Token Standard、DAR 依赖等当前约定时用。它用来减少「听起来对、上链就错」的授权和语法错误，不是通用 Solidity 技能，也不代替自己做的测试与审计。

## What it does
Canton Foundation Developer Relations 维护的 Claude 技能（\`SKILL.md\` + \`references/\`）。技能在你问模板、choice、授权错误、多方工作流、Daml Script 测试或 SDK 变更时加载，帮助核对授权链、识别 Propose Accept / Delegation 等模式，并抓住 \`createCmd\` 与 \`create\` 这类上下文相关语法。v2.0.0 的说明包括：Canton 3.5–3.7 覆盖（3.7 去掉 PV 34/35，默认 LF 2.3）、Splice 0.10（Token Standard V2 等）、dpm 1.1（Git 托管的 DAR 依赖），以及 8 个新的错误捕捉器。

## Recipe / links
- Repo: https://github.com/canton-network-devs/CF-Daml-Skill（4★，Apache-2.0，见 package.json）
- 安装：
  \`\`\`bash
  npx @canton-network-devs/cf-daml-skill
  \`\`\`
  安装器会尝试写入 Claude Desktop 的 skills 目录；若未检测到，则打包 \`CF-daml-skill.zip\`，再在 Claude.ai → Settings → Skills 里手动上传。也可以把仓库里的 \`SKILL.md\` 装进其他支持 Agent Skills 的客户端。
- 项目页：https://dev-hub.canton.foundation

## Why it made the cut
官方开发者关系包，有明确领域场景、可加载 \`SKILL.md\` 和一键安装器。星数很低，但本窗是可核对的 v2.0.0 更新，而不是空喊。许可以 package.json 的 Apache-2.0 为准，根目录没有单独 LICENSE 文件，使用前建议再确认。
