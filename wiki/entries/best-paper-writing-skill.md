# best-paper-writing-skill（按获奖论文笔法写摘要/引言/方法）

**Tags:** academic, paper-writing, cvpr, figures, skill
**Source:** [@fngly343149](https://x.com/fngly343149/status/2124679935302480122) · 2026-11-23
**Engagement:** 发现帖 19 赞 / 6 转发；仓库 [gulucaptain/Best-Paper-Writing-Skill](https://github.com/gulucaptain/Best-Paper-Writing-Skill) 424★ / 22 forks，CC BY 4.0（文中所引论文片段另有例外说明）

## When to use
要为机器学习 / 计算机视觉论文起草或改写标题、摘要、引言、方法、实验，或规划 Figure 1 / 方法总览 / 结果图，并希望接近 CVPR / ICCV / NeurIPS 获奖论文的写法。也可把已有摘要贴进去按获奖结构改。不适合相关工作综述、rebuttal，或只做语言润色。

## What it does
从 60 篇获奖论文（55 篇标注、5 篇留作测试）提炼论证路线：具体点名前人、写清缺口及其原因、用问题本身的洞察带出方法，少数数字撑起主张；方法组件按「需要 → 机制 → 性质」展开。按八类论文路由（方法改进、新能力、规模规律、再检验、机理分析、理论、数据集、测量）。没提供的数字、基线和引用一律写成 `[TODO]`，并附 `report.md`（主张-证据表、待补清单）。自带检查器抓 AI 腔、破折号和凭空数字；`check_figures.py` 检查图注与占位图。Claude 与 Codex 共用同一份 `SKILL.md`。

## Recipe / links
- Repo: https://github.com/gulucaptain/Best-Paper-Writing-Skill（424★，CC BY 4.0）
- 项目页：https://gulucaptain.github.io/Best-Paper-Writing-Skill/
- Skill 路径：`skills/bestpaper-writing/SKILL.md`
- 安装：
  ```bash
  git clone https://github.com/gulucaptain/Best-Paper-Writing-Skill.git
  cd Best-Paper-Writing-Skill
  ./install.sh claude     # → ~/.claude/skills/
  ./install.sh codex      # → ~/.agents/skills/
  ./install.sh all        # 两个都装；加 --project 则装到当前项目
  ```
  辅助脚本需要 Python 3。也可手动复制 `skills/bestpaper-writing/`。

## Why it made the cut
配方完整（intake → 主张图 → 写作 → 配图 → 检查），有语料统计和「不编造」硬门，424★ 可验证。与已收录的 [SciWrite](sciwrite.md)（审校已有文稿）和 [figures4papers](figures4papers.md)（投稿级 Matplotlib 作图）互补，不是同一件事。
