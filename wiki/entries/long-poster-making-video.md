# long-poster-making-video（长海报 + 42 光标制作过程）

**Tags:** design, poster, video, motion, chinese, skill
**Source:** [@Feljoy_ix](https://x.com/Feljoy_ix/status/2121654553452175400) · 2026-11-15
**Engagement:** 发现帖 11 赞 / 2 转 / 2 回复；仓库 [zhu558573-ux/long-poster-making-video](https://github.com/zhu558573-ux/long-poster-making-video) 约 9★ / 3 forks，MIT

## When to use
要做 1:4 四页竖版长海报（先锁风格再纵向延展），或要一条「线框到成片」的高密度多光标制作过程动画（目标同屏 35–42 个工作光标锁在选框手柄或打字光标上）。不是真实设计软件的操作录屏，也不是 Gemini 官方技能。

## What it does
工作流分两段：① 先生成 3:4 视觉锚点主海报，再以该图为参考延展为封面 + 三页内容的 1:4 长图；② 制作 1080p / 30fps 的模拟制作过程视频。路径 A 把中英提示词交给 Grok Video、Sora、可灵、Runway、Veo 等；路径 B 把 `SKILL.md` 里内嵌的约 420 行 Python 渲染引擎另存为 `render_making_video.py`，在本地用 ffmpeg 逐帧合成。原文文件头是 `## name:` 而不是标准 YAML（`---`），部分宿主（例如发帖里提到的 Muse）需要自行补文件头才能识别。

## Recipe / links
- Repo: https://github.com/zhu558573-ux/long-poster-making-video（~9★，MIT）
- Skill 原文：https://github.com/zhu558573-ux/long-poster-making-video/blob/main/SKILL.md
- 本地渲染（路径 B）需自行从 SKILL.md 拆出脚本，依赖 Python 3、Pillow、numpy、opencv-python 和系统 ffmpeg；示例：`python3 render_making_video.py --poster input.png --output out.mp4`
- 注意：仓库 README 写明未在发布环境实跑内嵌脚本，硬性指标（42 光标等）是执行目标，不保证任意模型或本机一次跑通

## Why it made the cut
有完整 SKILL.md 和清晰的两阶段海报 + 制作过程视频配方，仓库与内嵌渲染代码可核对。发帖还说明了非标准文件头的适配方法。社区星数一般，但材料扎实，不是空喊。
