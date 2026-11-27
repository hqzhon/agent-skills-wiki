# Safe Agent Skills（官方：读 Safe 状态并提出交易）

**Tags:** official, safe, ethereum, transactions, wallet, skill-pack
**Source:** [@SafeLabs_](https://x.com/SafeLabs_/status/2125955753622327612) · 2026-11-26
**Engagement:** 官方账号介绍帖 1 赞；仓库 [safe-global/safe-agent-skills](https://github.com/safe-global/safe-agent-skills) 现 1★，MIT。Safe 官方技能包，2026-11-02 创建，最近推送到 2026-11-26。

## When to use
要让 agent 通过 [Safe Transaction Service API](https://docs.safe.global/core-api/transaction-service-overview) 读取某个 Safe 的状态、解释 calldata，或作为 delegate **提出**交易、再由持有人在 Safe{Wallet} 里确认和执行时用。agent **不能**代持有人签名、执行或广播交易。

## What it does
四条技能：read-safe-state（owners、阈值、nonce、余额、历史、待处理队列，以及某 owner 名下的 Safe）；decode-and-explain（解码 calldata、说明效果、估算 safeTxGas）；register-delegate（在本机建 delegate key，并由一位 owner 为该 Safe 登记）；propose-transaction（以 delegate 提出交易）。API 不持有密钥；SAFE_API_KEY 只放环境变量，且只发往 https://api.safe.global。自托管 Transaction Service 则设 SAFE_TX_SERVICE_URL，此时脚本不会发送 SAFE_API_KEY。仓库提醒：delegate key 泄漏只会被用来提交垃圾提议，仍需 owner 批准。提供 Agent Skills discovery 的 .well-known/agent-skills/index.json。需要 Node.js 24+、bash、curl、jq。

## Recipe / links
- Repo: https://github.com/safe-global/safe-agent-skills（1★，MIT）
- 技能说明：仓库 skills/ 目录（如 skills/read-safe-state.md）
- 安装：
  ```bash
  git clone https://github.com/safe-global/safe-agent-skills.git
  cd safe-agent-skills
  npm ci
  export SAFE_API_KEY=<your key>   # 在 https://developer.safe.global 申请；不要写进仓库或命令行参数
  ```

## Why it made the cut
官方包，使用场景和「不能代签、不能广播」的边界写得很清楚，有可验证仓库和 discovery 清单。星标还很少，按官方材料收录。
