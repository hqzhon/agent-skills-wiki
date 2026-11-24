# split-for-x（把一张图切成 X / Instagram 能对缝的多图）

**Tags:** image, twitter, instagram, social, design, skill
**Source:** [@tiborwell](https://x.com/tiborwell/status/2124975777762447462) · 2026-11-24
**Engagement:** 本窗作者介绍帖互动很低 · 仓库 [thibaud360/split-for-x](https://github.com/thibaud360/split-for-x) 现 0★，MIT，带示例 mockup 和可上传的 skill zip

## When to use
要把一幅画或照片发成 X 的多图（两张并排，三张及以上为滑动相册）或 Instagram 轮播，避免等分切断脸或文字，并希望裁切在接缝处看起来是连续的。

## What it does
Claude 技能会看图、躲开脸和文字下刀、把最强的一张放到首位，并在发布前给出拼贴预览。按 2026 年 11 月桌面端 X 版式测量接缝，并在缝两侧留出补偿条，让线条像隔着窗口延续。需要 Python 3，以及 `pillow` 和 `numpy`。手机端若略有偏差，可让 Claude 关掉缝隙补偿再切一次。

## Recipe / links
- Repo: https://github.com/thibaud360/split-for-x（0★，MIT）
- Claude 应用：下载仓库里的 `split-for-x-skill.zip`，在技能设置里上传（需开启代码执行）
- Claude Code：
  ```bash
  git clone https://github.com/thibaud360/split-for-x
  cp -r split-for-x/skills/split-for-x ~/.claude/skills/
  ```
- 不安装：把 `PROMPT.md` 和图片一起贴给 Claude

## Why it made the cut
场景窄但可执行：有 `SKILL.md`、示例（含公有领域《星月夜》）和发布前预览。星数为 0，材料完整，不是「帮我切图」的空提示。
