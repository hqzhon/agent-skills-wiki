# Google Cloud HPC Skills（gke-batch-hpc 等）

**Tags:** google-cloud, hpc, gke, batch, official, skill
**Source:** [@Zen_with_AI](https://x.com/Zen_with_AI/status/2122531682603688430) · 2026-11-17
**Engagement:** 发现帖 7 赞 / 1 转帖 / 3 收藏 / 约 1,045 次展示；仓库 [google/skills](https://github.com/google/skills) 约 24.4k★，Apache-2.0

## When to use
要让智能体在 Google Cloud 上跑批处理或 HPC 工作负载：在 GKE 上排队与并行作业、配置 HPC 节点池、用 JobSet / Kueue 做多租户调度，或处理 MPI 任务。通用模型缺少集群与领域上下文时（例如给计算节点配了不兼容的存储、多节点 MPI 报错后卡住）尤其有用。不替代你自己的配额、预算和变更审批。

## What it does
官方 `gke-batch-hpc` 技能（`skills/cloud/gke-batch-hpc/SKILL.md`）指导在 GKE 上跑 batch/HPC：作业队列与并行、节点池（含 scale-to-zero）、Spot/成本、Kubeflow MPI Operator 的 `MPIJob`，以及 Kueue / JobSet 与检查点等生产注意点。它会引用同仓的 `gke-compute-classes` 等技能。

Google Cloud 在 SC26 博文中把这类技能与 Cluster Toolkit 蓝图配对：先核配额、做金丝雀容量检查、匹配已验证蓝图，经人工批准后再部署；并提到排队排障（如 `gke-kueue-debugging`）以及与 DeepMind Science Skills 搭配的领域工作负载（OpenFOAM、GROMACS、AlphaFold 3 等）。以仓库里实际存在的 `SKILL.md` 为准。

与已收录的 [Google Cloud Skills（IAM Helper）](google-cloud-skills.md) 同仓、互补：那边偏 IAM / 策略，这边偏批处理与 HPC。

## Recipe / links
- SKILL.md: https://github.com/google/skills/blob/main/skills/cloud/gke-batch-hpc/SKILL.md
- 仓库: https://github.com/google/skills （~24.4k★，Apache-2.0）
- 安装示例：`npx skills add google/skills --skill gke-batch-hpc`
- 博文: https://cloud.google.com/blog/topics/hpc/whats-new-in-hpc-and-ai-at-sc26/

## Why it made the cut
厂商官方技能，场景与步骤可在仓库和 Cloud 博文中核对；补上官方包里此前未单独记录的 HPC/批处理切片。部署类命令仍应先审阅再执行。
