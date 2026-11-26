# Inkworks（工程图纸风的可交互 3D 原理页）

**Tags:** 3d, threejs, explainer, animation, skill
**Source:** [@TianciZhutc](https://x.com/TianciZhutc/status/2125790819906924767) · 2026-11-26
**Engagement:** 介绍帖 3 赞；同窗另有 [@fngly343149](https://x.com/fngly343149/status/2125817601540678009)。仓库 [Moh4696/inkworks-skill](https://github.com/Moh4696/inkworks-skill) 现 277★ / 30 forks，MIT，2026-11-25 新建并推送。同一作者另有已收录的 [Open 3D Skills](open-3d-skills.md)。

## When to use
想让编码 agent 做一页「某台机器怎么工作」的可交互 3D 说明时用：发动机、泵、锁、变速箱、涡轮、心脏等有周期的机构。页面是白底工程图：浅灰零件、墨线轮廓、编号气球，可以暂停、单步、拖动循环图、绕相机。不要用它做通用游戏场景或写实渲染（更近的是 [Open 3D Skills](open-3d-skills.md)）；若要可拆解的离线模拟器，见 [teardown](teardown.md)。

## What it does
技能 `inkworks`：你写一份机构文件（几何、运动学、文案），配套 `kit/` 生成完整页面，无需打包步骤。两种布局可 `?layout=` 切换：`sheet`（图框、仪表、循环图，适合探索）和 `figure`（干净模型卡，适合嵌入或剪辑）。运动由单一驱动角计算，慢放和拖动始终精确；也可录 60fps 讲解片并加代码合成的音轨。仓库带发动机和打气筒两个已完成示例。全程 three.js 基本体，不依赖模型文件或生成视频。

## Recipe / links
- Repo: https://github.com/Moh4696/inkworks-skill（277★，MIT）
- 通用：`npx skills add Moh4696/inkworks-skill`（Node 22.20+）
- Claude Code：`/plugin marketplace add Moh4696/inkworks-skill` 后 `/plugin install inkworks-skill@inkworks-skill`
- Codex：`codex plugin marketplace add Moh4696/inkworks-skill` 后 `codex plugin add inkworks-skill@inkworks-skill`
- 无 Node：`curl -fsSL https://raw.githubusercontent.com/Moh4696/inkworks-skill/main/install.sh | bash`
- 技能：[skills/inkworks/SKILL.md](https://github.com/Moh4696/inkworks-skill/blob/main/skills/inkworks/SKILL.md)

## Why it made the cut
本窗新发布的完整可加载技能，场景很具体，有示例、两种布局和录制路径，MIT，并与作者已有的 Open 3D Skills 分开。按完整配方收录。
