# Hugging Face Skills（官方）

**Tags:** official, huggingface, ml, datasets, training, skill-pack
**Source:** [@Astrodevil_](https://x.com/Astrodevil_/status/2125446900103209152) · 2026-11-25
**Engagement:** 本窗官方盘点帖（0 赞）；仓库 [huggingface/skills](https://github.com/huggingface/skills) 现 11,397★，Apache-2.0，2026-11-23 仍有推送

## When to use
编码 agent 需要操作 Hugging Face Hub、数据集、训练/评测、Spaces / Gradio，或在本地跑模型时用。官方建议先装 `hf-cli`：它按本机已安装的 `hf` CLI 生成，能跟上当前命令。

## What it does
官方技能包（约 26 个 SKILL.md）。`hf-cli` 覆盖搜模型、管数据集和 bucket、启动 Spaces、跑 jobs。其余技能按需安装，涵盖 datasets、训练与 LoRA、transformers.js、Papers、Trackio、SageMaker / AWS 部署规划、评测等。格式遵循 Agent Skills 标准；不支持 skills 的宿主可退回仓库里的 `agentsmd/AGENTS.md`。

## Recipe / links
- Repo: https://github.com/huggingface/skills（11,397★，Apache-2.0）
- 文档：https://huggingface.co/docs/hub/agents-cli
- Claude Code：`/plugin marketplace add huggingface/skills`，再 `/plugin install hf-cli@huggingface/skills`；其他技能用 `hf skills add <skill-name>`
- 也可按宿主使用 Cursor Marketplace 或 Codex Plugins Directory 中的 `hf-cli`

## Why it made the cut
Hugging Face 官方包，有明确的「先装 hf-cli、再按需加工作流」路径，SKILL.md 可加载，11,397★、Apache-2.0。本窗盘点帖互动低，按官方仓库补收。
