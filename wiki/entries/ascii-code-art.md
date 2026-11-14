# ascii-code-art（网页实时 ASCII 动效）

**Tags:** frontend, canvas, webgl, ascii, animation, skill
**Source:** [@efearabaci_dev](https://x.com/efearabaci_dev/status/2121540605469737436) · 2026-11-14
**Engagement:** 发现帖互动低；仓库 [Woffluon/ascii-code-art](https://github.com/Woffluon/ascii-code-art) 当日新建、0★，MIT；有可点开的 live demo

## When to use
要在网站、React/Next.js 或静态页上做实时 ASCII 动效：hero 动画、3D 点云雕塑、黑洞/海浪一类 WebGL 场、Logo/图片/SVG 转 ASCII，或终端风动能排版；希望 agent 按固定引擎和 glyph 规则写，而不是随便堆 `<pre>`。

## What it does
一条完整 SKILL.md，按目标选最轻的引擎：

1. **3D 点云 / 粒子雕塑**：Canvas 2D 引擎 + 数学参考
2. **连续数学 / 物理场**：优先 WebGL2/GLSL，简单场可用 Canvas 2D
3. **图像 / Logo / SVG 转 ASCII**：Canvas 2D，含轮廓对齐
4. 还有动能字体等排版范式

统一用四档亮度 glyph、方向轮廓字符（`| / \ - _ +`）、帧间拖尾和双通道 bloom；在 `<canvas>` 上跑 30–60fps，`ResizeObserver` + 限制 `devicePixelRatio`，尊重 `prefers-reduced-motion`，运行时零依赖。仓库带引擎模板和 references。

## Recipe / links
- Repo: https://github.com/Woffluon/ascii-code-art
- SKILL.md: https://github.com/Woffluon/ascii-code-art/blob/main/SKILL.md
- Live demo: https://woffluon.github.io/ascii-code-art/
- 安装：`npx skills add Woffluon/ascii-code-art`

## Why it made the cut
使用场景清楚，SKILL.md 按范式给出引擎、模板和参考文档，还有零依赖的 live showcase，不是只丢一张 ASCII 截图。星标尚无，质量看配方和演示，不看热度。
