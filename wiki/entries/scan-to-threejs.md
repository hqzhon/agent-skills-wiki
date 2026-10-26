# scan-to-threejs (3D Model Anything)

**Tags:** 3d, threejs, lidar, reconstruction, wesbos
**Source:** [@ShiRen0809](https://x.com/ShiRen0809/status/2114507456080658943) · 2026-10-26  
**Also:** [@WuRichard_](https://x.com/WuRichard_/status/2114481041826107848)

## When to use
When you have an **iPhone LiDAR room capture** and want an agent to reconstruct an **editable Three.js scene** (not a video)—compare camera-matched renders, iterate materials/lighting, and ship a browser viewer.

## What it does
Wes Bos’s open repo `wesbos/3d-model-anything` ships a full `scan-to-threejs` Agent Skill under `.agents/skills/` with scripts (bundle/room conversion, photo prep, ortho, mesh probes, lights-from-photos) and modeling references. Capture App source is in-repo (Xcode/self-build; LiDAR iPhone/iPad).

## Recipe / links
- Repo: https://github.com/wesbos/3d-model-anything (~1.9k★)
- Skill: `.agents/skills/scan-to-threejs/SKILL.md`
- Pipeline sketch: LiDAR capture → agent skill reconstructs RoomModule → `npm` demos / viewer modes
- Caveats from posts: not one-click; verify dimensions yourself; App not on App Store

## Why it made the cut
Real SKILL.md + scripts + references; concrete capture→Three.js recipe with open source and multiple independent mentions.
