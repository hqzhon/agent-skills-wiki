# Science Skills（Google DeepMind 科研技能包）

**Tags:** official, deepmind, science, genomics, literature, skill-pack
**Source:** [@Fonsi_AI123](https://x.com/Fonsi_AI123/status/2125789962247483404) · 2026-11-26
**Engagement:** 介绍帖 3 赞；仓库 [google-deepmind/science-skills](https://github.com/google-deepmind/science-skills) 现 3,536★ / 410 forks，Apache-2.0，2026-11-10 仍有推送。约 40 个 `SKILL.md`。

## When to use
编码 agent 要做有依据的科研任务时用：查文献（arXiv / bioRxiv / OpenAlex / Europe PMC）、读蛋白/基因组公共库（UniProt、PDB、AlphaFold DB、ChEMBL、ClinVar、Ensembl 等）、跑 AlphaGenome 变异影响，或搭可复用的分析流程。不要把它当成临床或投资建议。和已收录的 [Scientific-Agent-Skills](scientific-agent-skills.md)（通用科研工作流）、[nature-skills](nature-skills.md)（论文润色/科研图）不是同一包。

## What it does
DeepMind 的 Science skills：每个技能目录含 `SKILL.md`、脚本和可选参考资料。优先在 [Google Antigravity](https://antigravity.google/) 里启用 Science 插件；也可用 `npx skills` 整包安装。依赖 `uv` 管理 Python 环境，第一次触发时 agent 会请求安装。部分技能（如 AlphaGenome）需要 API key；ClinVar、OpenAlex 等无 key 也能用，有 key 则限额更高。

## Recipe / links
- Repo: https://github.com/google-deepmind/science-skills（3,536★，Apache-2.0）
- 通用安装：`npx skills add google-deepmind/science-skills/`
- Antigravity：`Customizations` → `Build with Google` → `Science` → `Add`
- 自改技能不要写进插件安装目录（更新会覆盖），放到如 `~/.gemini/config/skills/`
- 用例：https://antigravity.google/use-cases/science
- 配套博文（本窗帖所引）：https://deepmind.google/blog/interpreting-mass-spectra-with-google-antigravity/

## Why it made the cut
官方科研技能包，配方可装、场景清楚，约 40 个带脚本的 `SKILL.md`，3,536★、Apache-2.0。本窗为高星漏收 + 安装说明帖。需标明：部分技能要 API key，输出不是医疗或投资建议。
