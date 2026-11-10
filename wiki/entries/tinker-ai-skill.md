# tinker-ai-skill（用自己的会话微调）

**Tags:** fine-tuning, tinker, claude-code, local-model, skill
**Source:** [@LiuweijiaVip](https://x.com/LiuweijiaVip/status/2119371366889849167) · [@oaichu95](https://x.com/oaichu95/status/2119248943813132341) · 2026-11-08
**Engagement:** drost-ai/tinker-ai-skill · 214★ / 30 forks · MIT · 2026-11-07 开源

## When to use
你想把 Claude Code / Codex / OpenCode 里积累的真实编程会话，蒸馏成能在本机跑的专属 agent 模型，而不是只靠提示词模仿自己的习惯。

## What it does
一套标准 Agent Skill，交出 Tess-4 背后的九步流水线：采集本地会话（带校验和）→ 清洗并按值替换凭证、随机化身份 → 按模型真实 renderer 切分且不拆开工具调用 → 为后续切片补工作上下文 → 按整段会话做 hold-out → 在 Tinker 上 LoRA 训练（先离线冒烟、启动前出示费用）→ 对比基座与 checkpoint → 合并导出 → 转 GGUF 并用匹配模板用 llama.cpp 提供服务。仓库含一份 `SKILL.md`、11 个脚本、6 篇参考笔记，以及五分钟合成会话预演（不碰真实数据、不产生费用）。产生费用的步骤之前会停下来等你确认。

## Recipe / links
- Repo: https://github.com/drost-ai/tinker-ai-skill （214★, MIT）
- 安装示例: `git clone https://github.com/drost-ai/tinker-ai-skill.git ~/.claude/skills/tinker-ai-skill`（Codex 用 `~/.agents/skills/`，OpenCode 用 `~/.config/opencode/skills/`）
- 对 agent 说类似：「fine-tune Qwen3.6-35B-A3B on my Claude Code sessions from the last three months.」
- 合成预演: `python scripts/make_sample_transcript.py` 后再跑 collect / normalize 等脚本

## Why it made the cut
新仓（11-07）但已有 214★，SKILL.md 把采集、脱敏、切分、训练、验收、导出写死成可执行步骤，而不是「用会话微调」一句空话。
