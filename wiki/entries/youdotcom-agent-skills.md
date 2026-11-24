# You.com Agent Skills（官方：实时搜索 / 抽取 / 带引用调研）

**Tags:** official, you.com, web-search, research, finance, mcp, skill-pack
**Source:** [@cheery9998](https://x.com/cheery9998/status/2125175846457770015) · 2026-11-24
**Engagement:** 本窗为第三方推荐帖（4 赞）；仓库 [youdotcom-oss/agent-skills](https://github.com/youdotcom-oss/agent-skills) 现 108★，MIT，2026-11-24 仍在推送

## When to use
编码 agent 需要**训练数据之后的**信息时用：查当前文档/API/changelog、核对报错与版本、读指定网页，或做带引用的多源调研、公司与市场资料。不要用它替代代码库内部的已有事实。

## What it does
You.com 官方技能包，当前公开技能包括：
- \`you-web\`：用 You.com MCP 的 \`you-search\` / \`you-extract\` 搜索并阅读全文，答案需有引用；
- \`you-research\`：多源综合调研；
- \`you-finance\`：行情、财报与公司基本面；
- \`you-discover\`：查找合适的 You.com API / MCP / SDK。
基础网页搜索在未配置 You.com 凭据时，可通过免费 MCP profile 走通；付费/OAuth 路径另有说明。技能要求先读证据再下结论，证据不全时给出有标注的部分答案。

## Recipe / links
- Repo: https://github.com/youdotcom-oss/agent-skills（108★，MIT）
- Claude Code 插件：
  \`\`\`bash
  /plugin marketplace add youdotcom-oss/agent-skills
  /plugin install you@you-com
  \`\`\`
- 通用安装：\`npx skills add youdotcom-oss/agent-skills\`
- 技能目录：\`skills/you-web\`、\`skills/you-research\`、\`skills/you-finance\`、\`skills/you-discover\`
- MCP：\`https://api.you.com/mcp\`（免费 profile 可先用；完整能力可能需要 You.com 账号或付费读取）

## Why it made the cut
厂商官方包，有明确「何时用」、可加载 \`SKILL.md\` 和安装命令，强调引用而不是让模型直接背网页。和已收录的各类官方搜索/数据技能互补，专攻 You.com 的实时网页与调研通路。本窗是中文推荐帖，按官方仓库补收。
