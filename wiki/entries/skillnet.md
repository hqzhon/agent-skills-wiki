# SkillNet（技能发现 / 安装 / 评估 / 路由基础设施）

**Tags:** catalog, discovery, evaluation, routing, meta, skill
**Source:** [@bkdgiffug](https://x.com/bkdgiffug/status/2124828810235256864) · 2026-11-23
**Engagement:** 发现帖信号低（2 赞）；仓库 [zjunlp/SkillNet](https://github.com/zjunlp/SkillNet) 1,460★ / 153 forks，MIT。另有 PyPI 包 `skillnet-ai`、站点与论文。

## When to use
本地技能越装越多，需要按意图搜索、安装、做质量评估，或从本机技能库里为当前任务做路由；也可以从仓库/文档/轨迹生成结构化 skill。它是技能生命周期工具，不是某一个业务配方。

## What it does
浙江大学 NLP 实验室（zjunlp）的开源基础设施，覆盖：
- **Discovery：** 按关键词或语义意图检索公开技能库（站点称索引 50 万+ GitHub skills）
- **Installation：** 从 GitHub 下载技能目录到本地 agent 工作区
- **Creation：** 从仓库、文档、提示词或执行轨迹生成结构化 skill
- **Evaluation：** 从安全、完整性、可运行性、可维护性、成本意识等维度评分
- **Analysis / Routing：** 抽出能力与场景、推断本地技能关系，并为任务选出技能及理由

提供 Python SDK / CLI（`skillnet search`、`skillnet download`、`skillnet ui` 本地浏览），以及论文 [arXiv:2603.04448](https://arxiv.org/abs/2603.04448)。社区另有 MCP 封装（CycleChain/skillnet-mcp）。公开搜索不必 API Key，私有仓库需要 `GITHUB_TOKEN`。

## Recipe / links
- Repo: https://github.com/zjunlp/SkillNet（1,460★，MIT）
- 站点：http://skillnet.openkg.cn/
- 安装：`pip install skillnet-ai`（Python 3.10+）；可选 `pip install "skillnet-ai[graph]"` 等额外依赖
- 示例：`skillnet search "pdf" --mode vector`，再 `skillnet download <skill_url> -d ./my_skills`
- 论文：https://arxiv.org/abs/2603.04448

## Why it made the cut
不是又一份 awesome 列表：有可安装的 SDK/CLI、评估维度和路由，星数与论文都可核对。和 [VoltAgent Awesome Agent Skills](voltagent-awesome-agent-skills.md)（人工精选目录）互补——那边是策展清单，这边是检索/评估/安装基础设施。装来的上游 skill 仍需自行审阅。
