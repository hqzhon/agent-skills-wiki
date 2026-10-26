# tv-fresh（小米电视改造）

**Tags:** android-tv, adb, debloat, xiaomi, skill-pack
**Source:** [@iLegend_AI](https://x.com/iLegend_AI/status/2114522775331414263) · 2026-10-26
**Engagement:** 0 likes / 0 repost / 0 replies (discovery post; repo ~361★)

## When to use
When an agent should **改造小米 / Redmi MIUI TV**：去广告、换 Launcher、装代理 / YouTube / 影视仓、批量清预装，或远程在电视上点按输入——用户提到小米电视、电视盒子 ADB、去开机广告时加载。

## What it does
Root-free, reversible ADB workflow (`pm uninstall --user 0` only for system packages). Routes by task into `references/` (debloat, launcher-swap, proxy-youtube, streaming-apps, cleanup-permissions, remote-toolbox) plus one-shot scripts under `scripts/`. Hard safety rules: confirm package lists, never touch settings/systemui/tvplayer/installer/voice/cast packages, roll back home on black screen. Validated on MiTV-ASTP0 / Android 9.

## Recipe / links
- Repo: https://github.com/wangrongding/tv-fresh (~361★, MIT)
- Skill: root `SKILL.md` + `references/` + `scripts/mitv-debloat.sh`
- Needs `adb`; TV and host on same LAN with ADB debugging on (`adb connect <TV_IP>:5555`)

## Why it made the cut
Concrete installable Agent Skill with when-to-use frontmatter, task routing, reversible safety rules, and a public repo—not just a tip thread.
