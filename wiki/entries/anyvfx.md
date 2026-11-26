# AnyVFX（把短特效 GIF 做成单通道 Shader）

**Tags:** vfx, shader, shadertoy, webgl, gif, skill
**Source:** [@gokayfem](https://x.com/gokayfem/status/2125913094182355105) · 2026-11-26
**Engagement:** 介绍帖 2 赞 / 1 收藏；仓库 [gokayfem/anyvfx](https://github.com/gokayfem/anyvfx) 现 0★，MIT。本窗由作者发布，仓于 2026-11-26 新建，根目录即为完整 `SKILL.md`（约 20k 字），并附 4 个带误差记录的例子。

## When to use
当你有一段很短的循环特效（光束、冲击环、水花、火花、尘土等 GIF / 短片），希望做成**一张可贴进 Shadertoy 的单通道 fragment shader**（`mainImage`，WebGL2 / GLSL ES 3.00，无纹理、无 buffer）时用。不要用它从纯文字 brief 写 shader（作者指向 [shader-skills](https://github.com/gokayfem/shader-skills)）；也不适合超过几秒的长视频。

## What it does
编码 agent 按 `SKILL.md` 的固定顺序工作：用仓库 `tools/` 测量片段、从关键帧地标画出静态场景、按逐帧 key table 重建特效，再对照参考片报告误差。作者给出 4 个已做完的例子（salt-flat beam、vortex bay、forest geysers、foundry waveform）及每例的误差数字。着色器依赖并列克隆的 `gokayfem/shader-skills` 库（`fbm` / `voronoi` 等由 bundler 内联）。过程需要能看图、跑命令的 agent；能看视频的模型对第一步更有帮助。

## Recipe / links
- Repo: https://github.com/gokayfem/anyvfx（0★，MIT）
- 依赖库：https://github.com/gokayfem/shader-skills（例子最后构建于 commit `a936077`）
- 技能：https://github.com/gokayfem/anyvfx/blob/main/SKILL.md
- 需要 Python 3.9+；可选 ffmpeg、`glslangValidator`；安装：
  ```bash
  git clone https://github.com/gokayfem/anyvfx
  git clone https://github.com/gokayfem/shader-skills
  cd anyvfx
  python3 -m venv .venv && . .venv/bin/activate
  pip install -r requirements.txt
  playwright install chromium
  ```
- 自备片段：`python tools/new.py work/my-clip path/to/clip.gif`，然后让 agent「Use SKILL.md to recreate work/my-clip/source.gif as a shader.」

## Why it made the cut
可加载的完整配方 + 测量工具 + 4 个可复核例子和误差表，使用场景写得很清楚。介绍帖和星标都还很少，按可验证材料收录，而不是按热度。
