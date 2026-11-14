# Loom Skills（AMD Loom 官方技能包）

**Tags:** official, amd, loom, inference, gpu, skill-pack
**Source:** [Grok 汇总回复](https://x.com/grok/status/2121564786424963089) · 2026-11-14
**Engagement:** 发现帖互动低；仓库 [loom-fun/loom-skills](https://github.com/loom-fun/loom-skills) 14★，3 forks，MIT；当日仍在推送

## When to use
要在 AMD 设备（尤其是 Strix Halo 一类 GPU/NPU）上用 Loom 安装、服务、移植或优化模型：把 GGUF 做成可运行的 Loom 包、对照 llama.cpp 测性能，或让 agent 按官方流程改 kernel / 服务配置。用户提到 Loom、loom-serve、loom-fetch、hrx-loom、.loom 文件时就该加载。

## What it does
一套可安装的官方技能包，入口 skill `loom` 负责选工作流并套用共用规则，再按任务分给子技能：

- `loom-setup`：安装 Loom、拉取目录模型、管理 GPU/NPU 服务
- `loom-demo-ui`：打开聊天 / 音频 / 图像 / embedding 的浏览器 playground
- `loom-port-llm`：把 GGUF 模型打成可运行的 Loom 包
- `loom-roofline`：估计性能上限并选定优化目标
- `loom-optimize`：在保持正确性的前提下加速移植结果
- `loom-benchmark`：对照 llama.cpp 等做校验与测速
- `loom-improve`：后续改进流程

模型以 Loom IR（`.loom` kernel + 控制程序）和 `model.json` 发包，`loom-serve` 在启动时按当前设备编译，并提供 OpenAI 风格 HTTP 接口。文档要求先设定 `LOOM_SKILL_DIR`，用捆绑脚本的绝对路径执行，不要在工作目录里乱跑 `scripts/...`。

## Recipe / links
- Repo: https://github.com/loom-fun/loom-skills
- 入口 SKILL.md: https://github.com/loom-fun/loom-skills/blob/main/skills/loom/SKILL.md
- 文档与演示站: https://loom-fun.github.io/loom-skills/
- Hugging Face 包: https://huggingface.co/loom-fun
- Loom / ROCm 文档: https://rocm.github.io/hrx-system/loom/
- Claude Code 安装：
  ```
  /plugin marketplace add loom-fun/loom-skills
  /plugin install loom@loom
  ```
- Codex / Pi：`npx skills add loom-fun/loom-skills --skill '*'`
- 典型提示：`get <hf-org>/<model> working on loom-serve, optimize it, and report the performance relative to llamacpp rocm`

## Why it made the cut
不是单条口头建议，而是 AMD Loom 推理栈的一整套可安装技能：有明确使用场景、分技能配方、官方文档和安装命令；仓库虽星标不多，但是厂商向、当日仍在更新的可验证材料。
