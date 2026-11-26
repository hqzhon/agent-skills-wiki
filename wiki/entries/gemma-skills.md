# Gemma Skills（Gemma 4 应用开发与微调）

**Tags:** gemma, finetune, google, training, skill-pack
**Source:** [@JJBondBuilds](https://x.com/JJBondBuilds/status/2125779152334704820) · 2026-11-26
**Engagement:** 介绍帖 6 赞 / 1 收藏；仓库 [google-gemma/gemma-skills](https://github.com/google-gemma/gemma-skills) 现 1,074★ / 84 forks，2026-11-24 仍有推送。根目录未放 LICENSE 文件。README 写明：**不是 Google 官方支持的产品**，也不在 Google OSS 漏洞赏金范围内。

## When to use
要基于 Gemma（尤其是 Gemma 4）做应用，或在本机 / 多 GPU 上微调、对齐、导出模型时用。`gemma-trainer` 覆盖 LoRA / QLoRA、全参微调、MoE、继续预训练、视觉/音频、DPO、GRPO，以及 GGUF / LiteRT-LM 导出。不要用它做纯推理应用选型（那是 `gemma-dev`），也不要把它和已收录的 [Gemini API Skills](gemini-skills.md)（Gemini API / 媒体生成）搞混。

## What it does
两个技能：

- `gemma-dev`：用 Gemma 做应用，或查询 Gemma 模型本身的知识；
- `gemma-trainer`：按硬件选 Unsloth（单卡）或 Hugging Face TRL + PEFT（多卡 / 自定义流水线），并对照官方 [Gemma 微调指南](https://gemma.ai/tuning/)。

## Recipe / links
- Repo: https://github.com/google-gemma/gemma-skills（1,074★；根目录无 LICENSE）
- 微调指南：https://gemma.ai/tuning/
- 浏览后安装：`npx skills add google-gemma/gemma-skills --list`
- 只装训练技能：`npx skills add google-gemma/gemma-skills --skill gemma-trainer --global`
- Antigravity：`agy plugin install https://github.com/google-gemma/gemma-skills`
- 训练技能：[skills/gemma-trainer/SKILL.md](https://github.com/google-gemma/gemma-skills/blob/main/skills/gemma-trainer/SKILL.md)

## Why it made the cut
可加载的 Gemma 4 微调/开发配方，和官方调参文档对得上，1,074★，场景清楚。必须标明仓库自己写的「非官方支持产品」，以及根目录没有 LICENSE 文件。
