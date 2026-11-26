# last30days-cn（中文互联网近 30 天讨论调研）

**Tags:** research, chinese, weibo, xiaohongshu, bilibili, zhihu, skill
**Source:** [@JackyPengcnm](https://x.com/JackyPengcnm/status/2125803416416841851) · 2026-11-26
**Engagement:** 介绍帖互动很低（逐步教程）；仓库 [Jesseovo/last30days-skill-cn](https://github.com/Jesseovo/last30days-skill-cn) 现 2,245★ / 221 forks，MIT（标明为 mvanhorn/last30days-skill 的中文本土化 fork），2026-11-24 仍有推送。技能版本 4.0.0-cn。

## When to use
想知道一个话题最近在**中文平台**怎么被讨论，或先看今天的全网热榜时用。默认覆盖微博、小红书、B 站、知乎、抖音、微信公众号、百度、今日头条。不要用它做大规模商用采集（使用约定写明仅供学习研究，并建议请求间隔 5 秒以上）。海外 Reddit / X / YouTube / Polymarket 调研仍走已收录的 [last30days](last30days-skill.md)；本包可用 `--global` 或已安装的上游 skill 作补充。

## What it does
按相关性 45% + 时效 25% + 互动 30% 排序，跨平台合并同一事件，输出带原链接的 Markdown / JSON / 可离线 HTML 报告。也提供全网热榜（网页版每天北京时间 08:00 / 12:00 / 20:00 更新）。小红书、微博、知乎、抖音登录后互动数据更完整（扫码登录态存在本机）；不登录也能跑，报告会注明只有公开链接。抖音、公众号、百度有可选付费 Key，不填走免费路径。B 站、头条、公众号不登录也能用。

## Recipe / links
- Repo: https://github.com/Jesseovo/last30days-skill-cn（2,245★，MIT）
- 热榜：https://jesseovo.github.io/last30days-skill-cn/
- 手册：https://github.com/Jesseovo/last30days-skill-cn/blob/main/docs/usage.zh-CN.md
- 交给 agent 安装（官方推荐原句）：
  ```
  帮我安装并配置 last30days-cn（https://github.com/Jesseovo/last30days-skill-cn），检查可用数据源，然后查看今天的全网热榜。
  ```
- 或：`npx skills add Jesseovo/last30days-skill-cn -g`
- 诊断：`python scripts/last30days.py --diagnose`
- 登录示例：`python scripts/last30days.py login xiaohongshu`
- 调研示例：`python scripts/last30days.py "豆包小豆" --days 7`

## Why it made the cut
与 last30days 互补的中文平台研究技能，配方和限制写得很清楚，2,245★、MIT，且保留了对原作者的署名。本窗为高星漏收 + 逐步教程帖。
