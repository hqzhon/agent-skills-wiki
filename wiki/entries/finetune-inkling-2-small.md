# finetune-inkling-2-small（在 Tinker 上微调 Inkling 2 Small 的完整配方）

**Tags:** finetune, llm, tinker, serving, skill
**Source:** [@migtissera](https://x.com/migtissera/status/2123849865679749342) · 2026-11-21
**Engagement:** 作者发布帖 181 赞 / 23 转 / 207 收藏；仓库 [drost-ai/finetune-inkling-2-small](https://github.com/drost-ai/finetune-inkling-2-small) 18★，MIT。本窗新建。

## When to use
要在 [Tinker](https://thinkingmachines.ai/tinker) 上用 LoRA **微调 Thinking Machines 的 Inkling 2 Small**（594B-A17B MoE），并接着在 Tinker 使用、自托管或发布时使用。从数据集校验、adapter 形状、学习率与费用，到合并、校验和 SGLang/vLLM 部署，都按同一条已验证配方走。

## What it does
把产出 Tess-4.5-594B-A17B 的完整路径写成 skill：`SKILL.md` + Python 脚本 + 依赖说明。它会明确写出容易踩坑的决定（分词器静默变更、4-bit expert 导致普通 LoRA 合不回去、64K cap 把输出 token 也算进去、reasoning effort 能让基准相差 18 分等）。默认离线步骤不花费用；训练、采样、probe 和移植会打 Tinker，**在可能产生费用的步骤前会停下来问**。未获明确要求时不上传模型。从编码 agent 对话记录做数据集时，可搭配同伴技能 `tinker-ai-skill`。

## Recipe / links
- Repo：https://github.com/drost-ai/finetune-inkling-2-small（MIT，18★）
- 把该技能装进 Claude Code / Codex / OpenCode，然后说：`fine-tune Inkling 2 Small on data/rows.jsonl`。
- 需要 Python 3.11+、Tinker API key；合并大约要 790 GB 磁盘（或 Modal），部署大约要 ≥500 GB GPU 显存。先读 SKILL.md 里的 compatibility 再动手。

## Why it made the cut
不是「帮我微调一下」的空提示，而是带脚本、停顿点和已发布模型对照指标的可复现配方。星数尚不高，但作者原帖和仓库材料都完整，按早期高完整度条目收录。
