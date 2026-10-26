# 3D Asset Agent Skills（simready-3d-assistant）

**Tags:** 3d, assets, nvidia, simready, skill
**Source:** [@An_zuoan](https://x.com/An_zuoan/status/2114661269441855509) · 2026-10-26
**Engagement:** discovery post (~90 impressions, 1 like); repo ~2★ · NVIDIA SimReady + Scenario

## When to use
When an agent should find, preview, and download free 3D models (USD/GLB/blend packs) before modeling from scratch—especially NVIDIA SimReady assets and Scenario collection items—with license checks and a modeling handoff.

## What it does
Skill `simready-3d-assistant` plus CLI scripts: hybrid search across NVIDIA SimReady Central (with repo fallback) and Scenario; gallery HTML + candidates.md; inspect/download with pinned commits and SHA checks; handoff markdown for Blender/adaptation. Stdlib-only Python 3.10+ for discovery/download.

## Recipe / links
- Repo: https://github.com/jeak01/3d-asset-agent-skills (~2★)
- Skill: `simready-3d-assistant/SKILL.md` (or `dist/simready-3d-assistant.zip`)
- Clone into agent skills dir, then e.g. “Use $simready-3d-assistant to find models for a sci-fi maintenance cart…”
- CLI: `python simready-3d-assistant/scripts/simready.py search --query "mobile cart" --out ./candidates`

## Why it made the cut
Concrete SKILL.md + scripts recipe; clear 3D asset-hunting use case; verifiable public catalogs (SimReady / Scenario) and download/handoff pipeline.
