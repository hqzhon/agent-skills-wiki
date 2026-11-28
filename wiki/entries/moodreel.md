# Moodreel（从参考片量出风格再写成代码片子）

**Tags:** video, motion, style-transfer, measurement, skill
**Source:** [@d5xOOAEVnr21525](https://x.com/d5xOOAEVnr21525/status/2126543153305899363) · 2026-11-28
**Engagement:** 本窗介绍帖赞数为 0，但给出了可执行的安装和渲染步骤；仓库 [gnipbao/moodreel](https://github.com/gnipbao/moodreel) 现 128★，MIT。2026-11-23 扫描时还在观察名单（预 alpha，当时 4★），现已有完整导演技能和对照测量流程。

## When to use
手里有参考图或参考片，想把「这种风格」量出来做成风格包，或按某个风格（含自带库里的风格）做片头、宣传片、讲解片、社媒口碑墙时用。不要用它剪实拍素材，也不要用它走扩散模型出片。它和 [motlab](motlab.md) 都是「视频写成代码」，但 Moodreel 的重点是**先测量再复刻风格**，不是通用广告引擎。

## What it does
可加载的导演技能 [`skills/moodreel/SKILL.md`](https://github.com/gnipbao/moodreel/blob/main/skills/moodreel/SKILL.md) 把代理设成导演，工具负责测量和核对：
1. **蒸馏**：参考进，风格包出（`STYLE.md`、可度量的绘图工具箱、示范片，以及把每个数字追溯到证据的 `LEDGER.md`）
2. **生产**：选题 + 风格进，代码逐帧画出成片
3. 本地 `measure` 跑参考片；草稿出来后 `compare` 把差得最多的片段排在前面，`diff` 能查出某个切点早了或晚了几帧，可以只改那一镜再对照

自带 First Light 示例不用 API 密钥，就能在本地渲出一条 12 秒短片。需要 Python 3.11+、uv、Node.js 22.18+，以及 ffmpeg / ffprobe；第一次安装会拉依赖和 Puppeteer 用的 Chrome。

## Recipe / links
- Repo: https://github.com/gnipbao/moodreel（128★，MIT）
- 技能路径：`skills/moodreel/SKILL.md`
- 安装并跑通示例（与本窗介绍帖一致）：
  ```bash
  git clone https://github.com/gnipbao/moodreel && cd moodreel
  uv sync --locked && npm ci
  uv run moodreel render video examples/first-light --size 1280x720 --fps 24 --engine chrome --out out/first-light.mp4
  ```
- 交给代理时，先让它读 `skills/moodreel/SKILL.md`，再用 `uv run moodreel`。

## Why it made the cut
从观察名单升级：仓库不再是预 alpha，技能把「先测量、每个数字要有出处、按窗口对照」写得很具体，许可和示例都可核。本窗介绍帖互动弱，收录依据是仓库材料而不是热度。
