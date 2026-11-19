# agent-redteam（给自己的 Agent 做红队测试）

**Tags:** security, red-team, evaluation, skill
**Source:** [@edbrdi](https://x.com/edbrdi/status/2123217019277304200) · 2026-11-19
**Engagement:** 作者介绍帖（3 赞 / 3 书签）；仓库 [edbrdi/agent-redteam](https://github.com/edbrdi/agent-redteam) 为 2026-11-18 新建、2★，MIT。早期条目。

## When to use
要安全测试**自己拥有或已获书面授权**的 LLM agent / 聊天机器人 / RAG / MCP / 带工具的 CLI 或网页应用时使用：提示词注入、越狱、工具滥用、数据泄漏、记忆投毒、不安全输出。明确拒绝测第三方系统；默认只在非生产环境、用合成数据。

## What it does
可移植的 SKILL.md 技能，带 agent 从授权与范围、资产发现、威胁模型、驱动对接、执行、分诊、根因，写到严重性报告和回归包。覆盖直接/间接注入、工具链、跨租户取数、输出侧夹带等六类；`assets/cases/` 有 61 个通用用例，并带客服机器人、电商推荐、邮件日历三种 profile。载荷是良性等价物（虚构秘密、保留域名、沙箱工具），有副作用的步骤需用户当场确认。

## Recipe / links
- Repo: https://github.com/edbrdi/agent-redteam（MIT，2★）
- 安装：
  ```bash
  npx skills add edbrdi/agent-redteam
  # 或：git clone 后拷到 ~/.claude/skills/
  ```
- 开口示例：「Red-team my support bot at https://staging.example.internal/agent。」技能会先做授权门（`runs/<id>/scope.md`），再出计划、报告和 `regression/`。

## Why it made the cut
不是空喊「去红队」，而是把授权、驱动契约、用例包、报告和回归写成可加载配方；安全边界写得很硬。仓很新、星数低，属早期收录。
