# inference-optimisation（本地 LLM 推理爬坡）

**Tags:** inference, llm, performance, benchmarking, skill
**Source:** [@TheArthiAI](https://x.com/TheArthiAI/status/2122718192426721583) · 2026-11-17
**Engagement:** 发现帖为 GitHub Trending 转帖、几乎无互动；仓库 [sybil-solutions/inference-optimisation-skill](https://github.com/sybil-solutions/inference-optimisation-skill) 现 914★ / 80 forks，MIT（2026-11-16 建仓）

## When to use
在自己的机器或已有模型服务上，要把本地 LLM 的 decode / prefill / 投机解码 / KV / 启动 / TTFT 调快，并且需要可复现的测量（先算理论上限，再交错 A/B），而不是凭一次跑分下结论。

## What it does
一套可加载的 agent skill，加上可单独跑的脚本：`ceiling.py` 先估硬件与量化下的上限，`bench.py` 做实测，`queue.sh` 把对照和候选交错排队，结果记到账本里。原则写在 skill 里：噪声常见 ±5–10%、要用中位数、量真实 token 和显存（含统一内存上的 GPU 驻留），并在宣称「最优」前做满上下文稳定性和并发浸泡。也可不经 agent，直接跑 `skills/inference-optimisation/scripts/`。

## Recipe / links
- Repo: https://github.com/sybil-solutions/inference-optimisation-skill（MIT，914★）
- Claude Code（用户级，仓库文档写法）：
  ```bash
  git clone https://github.com/sybil-solutions/inference-optimisation-skill
  mkdir -p ~/.claude/skills
  cp -r inference-optimisation-skill/skills/inference-optimisation ~/.claude/skills/
  ```
- 其他宿主：指向 `skills/inference-optimisation/SKILL.md`，或把仓库 `PROMPT.md` 当作任务提示
- 无 agent 试用：见 README「Quick start without an agent」（`ceiling.py` / `bench.py` / `queue.sh`）

## Why it made the cut
使用场景清楚，有 SKILL.md 和可独立运行的测量脚本，社区星标在一天内到了 900+。发现帖本身几乎无互动；装上后仍应按脚本要求记录硬件、模型和测量方法，避免把单次波动当成优化成果。
