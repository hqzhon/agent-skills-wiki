# figures4papers（投稿级 Matplotlib 科研作图）

**Tags:** research, figures, matplotlib, academic, skill
**Source:** [@lawson_ste3476](https://x.com/lawson_ste3476/status/2122080475049259416) · 2026-11-16
**Engagement:** 讨论帖互动很少 · 仓库 [ChenLiu-1996/figures4papers](https://github.com/ChenLiu-1996/figures4papers) 现 11,837★ / 827 forks，CC BY-NC 4.0

## When to use
要用 Matplotlib 做论文、组会幻灯或报告里的投稿级图（分组柱、趋势、散点、热力图、多面板），并希望字体、配色、坐标轴和 PDF/SVG 导出跟仓库里的示范图一致。不要用于 Plotly/Altair 等交互图、纯探索性草图，或 Figma/Illustrator 优先的信息图。

## What it does
仓库主体是作者（耶鲁 CS 博士生刘晨）已发表于 *Nature Machine Intelligence*、ICML、NeurIPS、ECCV 等的 Python 作图脚本。配套的可加载技能在 `scientific-figure-making/`：`SKILL.md` 说明何时用，`references/` 提供 API/配色约定、常用布局、设计原则、教程，以及指向 `figure_*` 示范项目的索引。Agent 按这套家规写或改绘图脚本，再导出 PNG/PDF。

## Recipe / links
- Repo: https://github.com/ChenLiu-1996/figures4papers（11,837★，CC BY-NC 4.0）
- 技能目录：`scientific-figure-making/SKILL.md` 与 `scientific-figure-making/references/`
- 不必先安装：把仓库打开，在提示词里点名 `scientific-figure-making/SKILL.md`（以及需要时的 `references/design-theory.md`、`references/api.md`）
- 也可以软链到技能目录，例如：
  ```bash
  mkdir -p ~/.claude/skills
  ln -s "$(pwd)/scientific-figure-making" ~/.claude/skills/scientific-figure-making
  ```
  Cursor / Codex 把目标目录换成 `~/.cursor/skills` 或 `~/.codex/skills` 即可。
- **许可限制：** CC BY-NC 4.0，非商业使用。公司项目或商业出图不能直接用这套代码与技能，需另行取得授权或换别的方案。

## Why it made the cut
有完整 `SKILL.md` + 参考文档，示范图来自顶会/顶刊真实论文，仓库星标很高，和使用场景都很清楚。它和 [nature-skills](nature-skills.md) 互补：后者偏论文润色与审稿流程，这条专注 Matplotlib 投稿图的视觉规范。必须看清非商业许可。
