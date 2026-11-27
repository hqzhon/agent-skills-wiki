# Fingerprint Leaderboard Skill（给 Sentient 指纹排行榜准备提交）

**Tags:** llm, fingerprinting, evaluation, research, skill
**Source:** [@qzxcle](https://x.com/qzxcle/status/2126037390863278238) · 2026-11-27
**Engagement:** 作者发布帖 14 赞 / 5 收藏 / 2 转；仓库 [qzxcle/fingerprint-leaderboard-skill](https://github.com/qzxcle/fingerprint-leaderboard-skill) 现 0★，MIT。本窗新建（2026-11-26）。

## When to use
要把一种模型指纹方案提交到 [Sentient Fingerprinting Leaderboard](https://fingerprint.sentient.foundation)，并希望 agent 先按已知攻击面做设计预审、写齐提交文件、做常见拒稿检查，再在本地按排行榜规则回放评测时用。不是通用的「给模型加水印」教程。

## What it does
技能按固定顺序工作：对照 Sentient provenance 报告和 [arXiv:2509.26598](https://arxiv.org/abs/2509.26598) 预审设计并估计保持率/鲁棒性；按 [MLprints](https://github.com/sentient-agi/mlprints) 约定写出 Python + YAML 提交文件；检查常见拒稿问题；在本地重放评测（单卡资格赛或完整五模型跑）；再讲解如何提交和读结果。Claude 应用里可做设计预审、写文件和静态检查；GPU 步骤在你本机跑，技能负责给出命令并解读你贴回的输出。

## Recipe / links
- Repo: https://github.com/qzxcle/fingerprint-leaderboard-skill（0★，MIT）
- Claude Code：
  ```
  /plugin marketplace add qzxcle/fingerprint-leaderboard-skill
  /plugin install fingerprint-leaderboard@sentient-fingerprinting
  ```
  也可在 shell 里用 claude plugin marketplace add / claude plugin install。之后可用 /fingerprint-leaderboard:fingerprint-leaderboard 显式调用。
- Claude 应用：从 [Releases](https://github.com/qzxcle/fingerprint-leaderboard-skill/releases/latest) 下载 fingerprint-leaderboard.zip，在 Customize → Skills 里上传。需开启代码执行 / 文件创建。
- 排行榜：https://fingerprint.sentient.foundation

## Why it made the cut
完整的可加载配方，使用场景、提交合同和本地回放步骤都写清了。介绍帖有一些互动，仓库还是 0★，按可验证材料收录。
