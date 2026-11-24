# safe-anything（代码漏洞 / 密钥 / 依赖 / Agent 配置扫描）

**Tags:** security, audit, rust, cli, mcp, agent-hygiene, skill
**Source:** [@GitTrend0x](https://x.com/GitTrend0x/status/2125190362742374569) · 2026-11-24
**Engagement:** 本窗为技能圈盘点帖（1 赞）；仓库 [erkamyaman/safe-anything](https://github.com/erkamyaman/safe-anything) 现 567★，MIT，Rust 实现，有 npm / crates.io 与 GitHub Action

## When to use
发版或合并前要做一次安全体检，刚加了依赖、MCP、第三方 skill / 插件，或担心仓库里有注入、泄密、错误云/移动配置时用。它负责找问题；是否误报、要不要改，仍由人判断。

## What it does
\`skills/safe-anything/SKILL.md\` 让 agent 调用 \`safe-anything\` CLI 或 MCP 工具 \`scan\` / \`list_rules\`。扫描覆盖代码漏洞（SQL/命令注入、XSS、SSRF、路径遍历、不安全反序列化、弱加密等）、泄露的密钥、移动和云配置、已知 CVE 依赖，以及不安全的 AI agent 配置（MCP、hooks、skills、权限）。每条发现带文件、行号、严重级别、CWE、原因和修复建议。默认可能向 OSV.dev 查询包名；用户不想联网时用 \`--offline\`。

## Recipe / links
- Repo: https://github.com/erkamyaman/safe-anything（567★，MIT）
- 安装技能：\`npx skills add erkamyaman/safe-anything\`
- CLI：\`npx safe-anything\` 或 \`cargo install safe-anything\`，然后 \`safe-anything <path> --json\`
- Skill: [skills/safe-anything/SKILL.md](https://github.com/erkamyaman/safe-anything/blob/main/skills/safe-anything/SKILL.md)
- 另有 GitHub Action（\`action.yml\`）。装前仍应阅读规则与权限边界。

## Why it made the cut
可加载 skill + 可独立运行的扫描器，场景明确，覆盖「代码漏洞」和「agent 配置」两边，和已收录的 [SkillSpector](skillspector.md)、[vibe-shield](vibe-shield.md)、[cloudflare-security-audit-skill](cloudflare-security-audit-skill.md) 互补：这边是通用仓库扫描器，不是只扫 skill 投毒或只做 Cloudflare 风格的漏洞狩猎。567★、MIT、有 CI/Action，按仓库信号补收。
