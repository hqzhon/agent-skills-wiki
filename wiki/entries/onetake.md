# onetake（一镜到底的产品发布动效短片）

**Tags:** video, motion, launch-video, product-demo, html, skill
**Source:** [@HaidarA06515262](https://x.com/HaidarA06515262/status/2117436839602659747) · 2026-11-03
**Engagement:** 仓库 feitangyuan/onetake ~3.6k★；11 个案例片

## When to use
要给 app、网页、skill 或某个功能做 10–30 秒的发布片 / 预告片 / 功能演示（带配音的可到约 60 秒），并且不想要「一张张轮流出场的 PPT 式」效果；也适合审查一条动效视频为什么「像 PPT、没节奏、转场生硬」。长视频、口播、剪辑现成素材不适用。

## What it does
- 整部片是一个 HTML 合成文件（`window.__seek(t)`，每个值都是时间的纯函数），用约 38 个测量过曲线的动作库（弹簧、入场、承接、碰撞、镜头）搭建，镜头一镜到底跟随主体。
- 产品 UI 由截图在 HTML 里重建，不录屏，镜头可以推进到任意缩放。
- 逐帧渲染并模拟 180° 快门的真实运动模糊（草稿 1080p30，成片 4K60），合成音效放在同一混响空间。
- 自带「oracle」检查脚本（`probe.py` / `verify_promo.py`）：逐帧记录画面、找到每个段落边界并打承接分，均匀节奏、无停顿、主体出画等会直接判失败。

## Recipe / links
- Repo: https://github.com/feitangyuan/onetake · 入口 `SKILL.md`，配套 `lib/`、`references/`（含 `product-demo.md`）、`scripts/`、`cases/`
- 用法：把仓库放进 agent 的 skills 目录（如 `~/.claude/skills/onetake`），给几张产品截图并说明要做发布片 / 功能演示
- 许可：PolyForm Noncommercial 1.0.0，个人/非商业免费，接客户活需另购授权（作者在 onetakemotion.com 卖 Pro 版）

## Why it made the cut
SKILL.md 很完整（明确何时用/不用、分步协议），有可验证的连贯性评分脚本和 11 个案例，星数高；补足 wiki 中「产品发布动效」方向。注意非商业许可。
