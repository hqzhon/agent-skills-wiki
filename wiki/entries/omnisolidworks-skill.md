# OmniSolidWorks Skill（有证据的 SolidWorks 机械建模与装配）

**Tags:** cad, solidworks, mechanical, engineering, windows, chinese, skill
**Source:** [@CommunismHaruh1](https://x.com/CommunismHaruh1/status/2126322823522357315) · 2026-11-27
**Engagement:** 作者第一方发布帖约 310 赞 / 302 书签；安装说明见同串 [回复](https://x.com/CommunismHaruh1/status/2126322868158177734)。仓库 [Haruhi764/OmniSolidWorks-Skill](https://github.com/Haruhi764/OmniSolidWorks-Skill) 现 28★，MIT，当天建仓并带验收记录。

## When to use
要在 **Windows 本机 SolidWorks** 里做可编辑的参数化零件、多级装配、原生爆炸视图和二维工程图，并且需要用真实几何、配合、干涉和重开结果做验收时用。它不是「让模型直接生成一个好看的 3D 预览」；作者强调证据驱动，会回读原生 API 数据，不合格就拒绝。实测宿主是 SolidWorks 2014 x64 SP0，其他版本需自行兼容性测试。不要指望它覆盖 BIM、其他 CAD 厂商，或尚未完成的高级爆炸 / 连续碰撞检测。

## What it does
根目录 [SKILL.md](https://github.com/Haruhi764/OmniSolidWorks-Skill/blob/main/SKILL.md)（技能名 `solidworks-mechanical`）通过本地 COM 提交结构化作业，流程包括：先 `python -B scripts/v03_jobs.py --preflight` 检查环境，再建模 / 装配 / 出图，保存关闭后重开核对几何与配合，合格装配还要验证爆炸与折合。仓库附三工位夹爪、减速器等案例，以及单元测试与验收报告。这是同一作者已收录的 [OmniCAD](omnicad-skill.md)（二维 DXF/DWG）在三维机械方向上的后续。

## Recipe / links
- Repo: https://github.com/Haruhi764/OmniSolidWorks-Skill（28★，MIT）
- 需要 Windows x64，本机已安装并授权的 SolidWorks；先按仓库 `ENVIRONMENT_COMPATIBILITY.md` 检查环境。
- 安装：
  ```bash
  npx skills add Haruhi764/OmniSolidWorks-Skill
  ```
  或把仓库发给 Codex，让它阅读 `SKILL.md` 与安装文档后完成本地配置。
- 发布说明、验收记录和已知限制都在仓库根目录，未实现的能力不要当已经可用。

## Why it made the cut
使用场景和边界都很清楚，有 SKILL.md、MIT 许可、测试与实机案例；本窗第一方介绍帖信号很强。和已收录的 OmniCAD 是同一套「证据驱动」思路，值得单列。平台限制（Windows + 特定 SolidWorks 版本）必须在条目里写明。
