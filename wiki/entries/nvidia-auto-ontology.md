# NVIDIA Auto Ontology（官方：从元数据建本体并给 agent 用）

**Tags:** official, nvidia, ontology, text-to-sql, mcp, skill-pack
**Source:** [@tirthaexe](https://x.com/tirthaexe/status/2126572705155854399) · 2026-11-28
**Engagement:** 本窗为仓库链接帖（0 赞）；仓库 [NVIDIA/auto-ontology](https://github.com/NVIDIA/auto-ontology) 现 16,159★ / 1,460 forks，Apache-2.0，官方维护（作者元数据为 NVIDIA <opensource@nvidia.com>）。配套评测仓 [NVIDIA/auto-ontology-eval](https://github.com/NVIDIA/auto-ontology-eval) 202★，同为 Apache-2.0。

## When to use
业务问题说法含糊、数据散在多套系统、同一指标定义还对不上，需要先有一份可治理的「概念 → 数据」地图，再让 agent 问数时用。它适合问题开放、定义要在多次运行和多个 agent 之间复用的场景。如果只有一个建模清楚的数据源和固定问题，直接写 SQL 可能就够了。不要把它和已收录的 [NVIDIA Agent Skills](nvidia-skills.md)（CUDA / Physical AI）或 [BioNeMo Agent Toolkit](bionemo-agent-toolkit.md) 当成同一个包。

## What it does
NVIDIA 开源的 Auto Ontology 可从企业元数据自动生成本体，调和不一致的定义，再通过 MCP、CLI 和 API 暴露给任意 agent 运行时。仓库带三个可加载技能（均附 evals 和 skill-card，许可证 Apache-2.0）：

- `nvidia-ontology-setup`：用官方 Helm（推荐）或 Docker Compose 装运行时，或把 MCP 接到已有实例；失败时先读仓库内排错说明，不要临时编第二套安装器。密钥只让用户写进 values / `.env`，不要贴进对话或命令行参数
- `nvidia-ontology-query`：按本体里的业务含义回答问题，把指标和实体落到可验证的查询，并带回步骤与依据
- `nvidia-ontology-management`：编写、校验和发布本体中的术语与关系

README 写明它在 BIRD-Interact 和 BEAVER 等 Text-to-SQL 基准上靠前。运行栈需要 NVIDIA API key（`nvapi-...`），官方安装路径见 `DEPLOYMENT.md`。

## Recipe / links
- Repo: https://github.com/NVIDIA/auto-ontology（16,159★，Apache-2.0）
- 评测 / 示例数据种子：https://github.com/NVIDIA/auto-ontology-eval（202★，Apache-2.0）
- 技能目录：https://github.com/NVIDIA/auto-ontology/tree/main/skills
- 安装技能（把三个技能文件夹拷进 agent 的 skills 目录），或：
  ```bash
  npx skills add NVIDIA/auto-ontology
  ```
- 部署说明：https://github.com/NVIDIA/auto-ontology/blob/main/DEPLOYMENT.md
- MCP 说明：https://github.com/NVIDIA/auto-ontology/blob/main/docs/mcp.md

## Why it made the cut
官方仓库，许可清楚，星数高，三个技能分工明确还带评测材料。本窗介绍帖几乎没有互动，依据是可核对的官方技能包，值得单列。
