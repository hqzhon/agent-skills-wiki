# 达尔文.skill 3.0（实跑盲评进化 SKILL.md）

**Tags:** meta, skill-optimization, evaluation, autoresearch, chinese, skill
**Source:** [@AlchainHust](https://x.com/AlchainHust/status/2121744774877389261) · 2026-11-15
**Engagement:** 发布帖刚发出（约 4 赞）；仓库 [alchaincyf/darwin-skill](https://github.com/alchaincyf/darwin-skill) 约 6916★ / 715 forks，MIT；微软 SkillOpt 集成名单收录

## When to use
你已经有可装的 agent skill，但不确定改 SKILL.md 是真的让 agent 把活干得更好，还是只是「读起来更完整」。要用可重复的评估→改进→实测→保留或回滚循环去进化它，而不是靠评委读两版文档投票。

## What it does
受 Karpathy autoresearch 启发，把自主实验循环用在 Skill 优化上。核心流程仍是：评估 → 改进 → 实测验证 → 人类确认 → 保留或回滚 → 成果卡片；9 维 rubric、独立评委、git 回滚和人工检查点都还在。

v3.0（2026-11）改的是棘轮量什么：2.x 让评委读改前改后两版 SKILL.md 投票；3.0 改为评委盲评两版 skill 的实跑产出。作者给出的依据包括：NVIDIA 研究里读文档分数与实跑增益几乎不相关；2.x 自己的记录里，评委 3 比 0 通过的改动上真机反而多绕了 33 次工具调用。证据分 E0 体检 / E1 读评 / E2 实跑 / E3 真机四档，keep 或 revert 至少要到 E2。

三种用法：给全部 skill 做几乎零成本的 E0 体检；「评估/打分」跑到 Phase 2 不改文件；「优化/进化」走完整流程。

## Recipe / links
- Repo: https://github.com/alchaincyf/darwin-skill（~6916★，MIT，当前 3.0.1）
- 根目录 `SKILL.md`（触发：优化 skill、skill 打分/体检、达尔文、darwin、optimize skill）
- 安装：`npx skills add alchaincyf/darwin-skill`
- 相关：微软 [SkillOpt](https://github.com/microsoft/SkillOpt) 将其列为已集成项目；与本 wiki 的 [Autoresearch](autoresearch.md)、[EvoSkill](evoskill.md)、[Microsoft SkillOpt](microsoft-skillopt.md) 互补（达尔文专门优化 SKILL.md，而不是从失败轨迹生成 skill 或隔夜迭代代码指标）

## Why it made the cut
可安装的完整优化配方，使用场景清楚，仓库与 3.0 重建文档可验证，社区信号强。3.0 把「读文档投票」改成「盲评实跑产出」，是对 skill 工程里一个常见误区的直接修正。
