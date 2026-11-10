# GIF 工厂（gif-factory）

**Tags:** sticker, gif, pixel, illustration, brand-film, skill
**Source:** [@ganfanren_ai](https://x.com/ganfanren_ai/status/2119633063902880065) · 2026-11-09
**Engagement:** 5 likes / 0 reposts / 0 replies / 4 bookmarks · WoYun520/gif-factory · MIT · 929★

## When to use
当你要给聊天做表情包 GIF、电子光栅变画卡、漫画印刷风动态海报、吉祥物品牌短片或紧凑动态绘本，手里有参考图，却不会画、不会逐帧动的时候——尤其适合 Codex / 能生成图并跑脚本的 coding agent。

## What it does
第三方 Codex 做事方法（非官方）：仓库主体是 `SKILL.md` + 多套风格/参考 + 6 个 Python 导出脚本。画风（像素 320px / 高清插画 512px / 真人照片保留）与动法（轻动效 vs 连续完整动作）分开选；还能做光栅卡、动态海报、品牌短片、动态绘本。质量规矩写明：成套表情包里每张表情与姿势要有区别，不是同一肖像换字。有独立 `skills/compact-storybook`。

## Recipe / links
- Repo: https://github.com/WoYun520/gif-factory （MIT，约 929★）
- 安装：把仓库链接发给 Codex，或按其 GUIDE 安装 Skill；调用标识 `$pixel-gif-sticker-pack`
- 入口：根目录 `SKILL.md` · [GUIDE.md](https://github.com/WoYun520/gif-factory/blob/main/GUIDE.md) · [styles/](https://github.com/WoYun520/gif-factory/tree/main/styles) · `scripts/` 导出器
- 先小样再批量：先做 1 张确认画风/动法，再扩成整包

## Why it made the cut
可安装 SKILL.md + 可运行导出脚本 + 清晰「何时用 / 画风×动法」矩阵，不是模板换脸包；929★ 与完整作品库可验证。
