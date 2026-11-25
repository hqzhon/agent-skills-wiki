# skill-distill（把一次成功会话蒸馏成便宜模型也能跑的技能）

**Tags:** distillation, skills, evaluation, open-weight, claude-code, codex, skill
**Source:** [@Zipopics](https://x.com/Zipopics/status/2125203364946624878) · 2026-11-24
**Engagement:** Daily Skills #13 介绍帖 12 赞 / 6 收藏；仓库 [sybil-solutions/skill-distill](https://github.com/sybil-solutions/skill-distill) 现 714★，MIT，2026-11-21 公开

## When to use
一次 Claude Code / Codex 会话已经把任务做对，希望把流程写成技能，让指定的开源权重模型在指定 harness 里复现同一任务时用。用户会说「把这次会话蒸馏成 skill」「让 DeepSeek / GLM / Qwen 也能做你刚才做的事」。不要用它从零写通用技能，也不要用它做微调。

## What it does
你是 **teacher**。技能 `skills/skill-distill/SKILL.md` 规定循环：写出学生技能 → 在 tmux 里用干净的起始状态跑学生 → 对照参考结果 → 改技能再跑，直到学生结果匹配且你接受。附带 `distill.py` 记账（init / trial / verdict / accept）、会话日志抽取、可选的无头浏览器截图，以及 omp / Codex / Claude Code 等学生适配器。学生只拿到原提示词、干净起点和技能本身。

## Recipe / links
- Repo: https://github.com/sybil-solutions/skill-distill（714★，MIT）
- Skill: [skills/skill-distill/SKILL.md](https://github.com/sybil-solutions/skill-distill/blob/main/skills/skill-distill/SKILL.md)
- 安装（需 tmux、git、Python 3.10+，以及已配置好的学生 harness）：
```
git clone https://github.com/sybil-solutions/skill-distill
ln -s "$PWD/skill-distill/skills/skill-distill" ~/.claude/skills/skill-distill    # Claude Code
ln -s "$PWD/skill-distill/skills/skill-distill" ~/.agents/skills/skill-distill    # Codex
```
  若要验收 Web 结果：`pip install playwright pillow && playwright install chromium`。
- 用法示例：在一次成功会话结束时说 `distill this session into a skill for omp with deepseek-v4.1-flash on my local server`。可用 `tmux attach -t distill-<task>` 看学生过程。仓库 `examples/` 里有完整跑通记录。

## Why it made the cut
可加载 SKILL.md、蒸馏循环和验收脚本都写得很清楚，场景不是「再写一份提示词」，而是对照参考会话把技能改到便宜模型也能复现。714★、MIT，本窗有专题拆解。和已关注的 SkillPlumber（诊断技能写坏）互补，这是生成/验收侧。
