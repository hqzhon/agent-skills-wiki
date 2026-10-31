# teardown（可拆解的 3D 机械模拟器）

**Tags:** 3d, simulator, threejs, explainer, video, education, skill
**Source:** 用户推荐（jackie zhong）· 2026-10-31 · 仓库 [elvarofficial/teardown](https://github.com/elvarofficial/teardown)
**Engagement:** 98★ / 17 forks（2026-10-31 查询；仓库 2026-10-30 创建），MIT

## When to use
想弄懂或讲清楚一台真实机器 / 机构怎么工作（发动机、起落架、连杆机构、泵、变速箱……），需要「可视化讲解」「模拟器」「剖视图」「爆炸视图」或交互式 3D 课件，而不是一段文字描述；也可顺手录一段讲解短片。

## What it does
1. 让 Claude Code 把机器做成**一个离线 HTML 页面**（three.js 与字体内联，约 800 KB）：机器在中间运转，周围面板显示真实数值，每个子系统一个按钮，点开就把正在干活的部件隔离 / 剖开 / 透视。
2. 无人操作时页面按脚本**自动巡游**（带光标）；任何点击 / 拖动 / 滚轮 / 按键即交还控制，静默 25 秒后恢复巡游。
3. 同一份代码可**逐帧录制 60 fps mp4**，并在同一时间轴上生成程序化配乐（母带至 −14 LUFS）。
4. SKILL.md 规定了做对的规则：从真实参考图起步、不凭想象；先查真实尺寸，所有仪表 / 图表 / 标注与驱动零件的是同一函数；单一输入（曲轴角 / 行程 / 风速）驱动一切，不手打关键帧；浅色棚拍 + 单一强调色；按机构选机位；附审阅循环。
5. 自带 3 个完整示例：横置曲轴 V8（点火顺序 1-8-4-3-6-5-7-2、缸压模型）、Cessna 337 主起落架（齿条齿轮收放）、Theo Jansen 的 Strandbeest（20 条腿的连杆求解）。

## Recipe / links
- Repo: https://github.com/elvarofficial/teardown （`SKILL.md` 为技能本体；`sims/kit/` 运行时；`sims/build.mjs` 打包单页；`sims/capture.mjs` 录片；`sfx/` 配乐）
- 安装：`npx skills add elvarofficial/teardown -g -a claude-code`，然后在安装目录执行一次 `npm install && npx playwright install chromium`
- 依赖：Node.js 20+；录视频需 `ffmpeg`，配乐需 Python 3
- 用法（直接用自然语言问 Claude Code）：
  - "Build me a simulator of a 4-stroke motorcycle engine I can take apart."
  - "How does a mechanical watch keep time? Show me as a simulator."
  - "Make a teardown of a hydraulic excavator arm and record a 20-second video of it."
- 先看示例：`node sims/build.mjs v8-live` → `teardown-out/dist/v8-live.html`（另有 `cessna-live`、`strandbeest-live`）

## Why it made the cut
用户推荐，且过质量关：场景明确（解释机器怎么工作）、`SKILL.md` 给了构建结构与硬规则、仓库带 3 个可直接构建验证的完整示例，交付物是离线单页 + 可录制成片。基于 [whaleyxbt/claude-motion](https://github.com/whaleyxbt/claude-motion)（MIT）的运行时、逐帧捕获、音效引擎与审阅规则；采样为 Freesound CC0。与 [Anatomy](anatomy.md)（等距讲解图）、[scan-to-threejs](scan-to-threejs.md)（3D 场景）互补，专攻「可拆解、数值真实」的交互机械讲解。仓库很新（发布约 1 天），信号仍在积累。
