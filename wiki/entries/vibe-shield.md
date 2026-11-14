# vibe-shield（AI 生成代码的静态安全扫描）

**Tags:** security, appsec, static-analysis, nextjs, mcp, skill
**Source:** [@FoundryVibe](https://x.com/FoundryVibe/status/2121530062575174091) · 2026-11-14
**Engagement:** 发现帖互动低；仓库 [avivgerz-hue/vibe-shield](https://github.com/avivgerz-hue/vibe-shield) 39★，2 forks，MIT；有 npm 包

## When to use
在授权项目里审查 Next.js / Supabase / TypeScript 应用，或刚让 agent 改过 API、鉴权、数据策略、LLM 工具和 MCP/Skill 配置，需要一份基于静态证据的防御性安全评审，而不是口头「注意安全」。也适用于怀疑技能/MCP 配置被投毒。

## What it does
根目录 SKILL.md 把评审写成六段协议，强调只在授权范围内工作、静态发现是证据不是漏洞证明、不外传源码或密钥：

1. 攻击面侦察：入口、鉴权、中间件、数据策略、存储、LLM/工具、webhook、agent/MCP 配置
2. 自动静态扫描 + skill 审计（`scan` / `audit-skills`）
3. 按证据分类与复核
4. 在不改变行为的前提下修复
5. 复扫验证
6. 写明扫描看不到的限制

规则集面向 OWASP Top 10:2025 以及 MCP/Skill poisoning。可用 `explain <RULE_ID>` 查看单条规则。同作者套件还有 [unslop](unslop.md)（去 AI 味 UI）和 [ghost-qa](ghost-qa.md)（真浏览器 QA）。

## Recipe / links
- Repo: https://github.com/avivgerz-hue/vibe-shield
- SKILL.md: https://github.com/avivgerz-hue/vibe-shield/blob/main/SKILL.md
- 扫描：`npx -y @vibefoundry/vibe-shield@latest scan .`
- Skill 审计：`npx -y @vibefoundry/vibe-shield audit-skills . --format json`
- 也可当 MCP / Agent Skill 使用

## Why it made the cut
有可安装的 SKILL.md、分阶段协议和可运行的扫描器，场景明确（AI 生成应用 + 技能投毒），仓库和 npm 包可验证。和 [aig-skill-scan](aig-skill-scan.md)、[skill-guard](skill-guard.md)、[xss-audit](xss-audit.md) 互补，更偏应用代码与 MCP 配置的静态审查。
