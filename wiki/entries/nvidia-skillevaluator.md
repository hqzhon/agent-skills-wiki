# SkillEvaluator（NVIDIA 官方，Skill 质量与增益评测）

**Tags:** evals, skill-quality, security, ci, official, nvidia
**Source:** [@Ldataengineer](https://x.com/Ldataengineer/status/2120950470084603993) · 2026-11-13
**Engagement:** 原帖热度低；仓库 NVIDIA/SkillEvaluator ~860★ · Apache-2.0 · 附 arXiv 论文与 NVIDIA 开发者博客

## When to use
你写了（或准备装）一个 SKILL.md 技能，想知道它是否真的让 agent 做得更好，而不是「感觉好一点」；或者想在 GitHub / GitLab 的 PR 里给技能目录加上自动质量门禁。

## What it does
三层独立评测，可只跑其中一层：
- **Tier 1 验证**：结构 / 规范检查 + 安全扫描（SkillSpector、Gitleaks，可选 Semgrep）；扫描器跑不起来时结果标为 INCOMPLETE，不会静默通过
- **Tier 2 去重**：用 embedding 找技能内部重复指引，或与目录里其他技能重叠（`--catalog`）
- **Tier 3 实测**：在沙箱里让 Codex / Claude Code / OpenCode 分别带技能、不带技能跑同一批任务，差值即 Skill Lift；技能从未被加载时报告 INCONCLUSIVE
- 无 LLM 模式：不需要 API key、GPU、Docker，即可得到确定性质量分（示例技能 84.5/100，默认及格线 70）

## Recipe / links
- 仓库：https://github.com/NVIDIA/SkillEvaluator · 文档：https://docs.nvidia.com/skills/skillevaluator/
- 免 key 快速体验：
  ```bash
  git clone --depth 1 https://github.com/NVIDIA/SkillEvaluator.git && cd SkillEvaluator
  uv run --python 3.13 skillevaluator quality-check \
    src/skillevaluator/tier3/reference_skills/text-analyzer -r cli -r json -o reports/first-quality
  ```
- 接入 CI：`pip install --upgrade skillevaluator && skillevaluator ci init`，或直接复制仓库 `ci/bundles/` 下的 GitHub / GitLab 模板
- 原帖建议的用法：先写 10–20 个真实任务用例（含几个「不该触发」的）→ 先跑无技能基线 → 带技能跑且 `--n-attempts` ≥ 3 → 按用例对比，并阅读零增益/负增益用例的轨迹

## Why it made the cut
官方开源、配方具体、仓库与文档可核；补上了本目录里「装之前查安全」（[SkillSpector](skillspector.md)、[aig-skill-scan](aig-skill-scan.md)）之外的「装了到底有没有用」这一环，与 [NVIDIA Skills](nvidia-skills.md) 同属 NVIDIA Verified Skills 流水线。
