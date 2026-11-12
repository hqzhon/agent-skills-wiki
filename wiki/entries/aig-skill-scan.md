# aig-skill-scan（腾讯朱雀 A.I.G，Skill 安装前安全审计）

**Tags:** security, skill-safety, scanning, install-hygiene, sarif, tencent
**Source:** [@justforfunnai](https://x.com/justforfunnai/status/2120720749459870141) · 2026-11-12
**Engagement:** 帖子互动低 · Tencent/AI-Infra-Guard ~7.5k★ · PyPI `aig-skill-scan` 0.2.2

## When to use
安装或上架第三方 Agent Skill 之前，想让 LLM 读一遍代码判断有没有恶意或漏洞；或想把 skill 审计接进 CI，把结果送进 GitHub Code Scanning 等 SARIF 工具。

## What it does
LLM 驱动的多阶段静态审计：默认先做代码审计，首次判定为 `suspicious` 时再做一轮聚焦复核；`malicious` / `normal` 走快速路径。漏洞按 SkillTrustBench T01–T09 分类，结论分 malicious / suspicious / normal。默认输出 SARIF 2.1.0。属于腾讯 AI-Infra-Guard 的一个子项目，同套还有 MCP 扫描、运行中 agent 红队、模型越狱评测等独立包。

## Recipe / links
- 文档：https://github.com/Tencent/AI-Infra-Guard/tree/main/skill-scan
- 安装：`pip install aig-skill-scan`（Python ≥ 3.9）
- 运行：`export LLM_API_KEY=...` → `aig-skill-scan --repo /path/to/skill -m <model> --language zh -o result.sarif.json`（默认走 OpenRouter，可用 `-u` 换 base URL）
- 单机使用不要开 `--aig-mode`（那是给平台后端的结构化输出）
- 结论当线索，仍要自己读 SKILL.md 和 scripts/

## Why it made the cut
大厂开源、命令具体、输出接得进标准安全工具链；和已收录的 [SkillSpector](skillspector.md)、[skill-guard](skill-guard.md) 互补（这个偏 LLM 语义审计）。
