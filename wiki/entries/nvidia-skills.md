# NVIDIA Agent Skills（官方目录）

**Tags:** nvidia, cuda, physical-ai, skill-pack, official, verified
**Source:** [@EveryDevAi](https://x.com/EveryDevAi/status/2114722468128804895) · 2026-10-26
**Engagement:** discovery post (low) · repo ~3.7K★ · NVIDIA verified catalog

## When to use
When agents invent almost-working CUDA / NeMo / Jetson / Physical AI / RAG Blueprint code — load NVIDIA’s verified, signed skill catalog so the agent follows product-maintained recipes instead of guessing APIs.

## What it does
Official NVIDIA Agent Skills catalog mirrored from product repos (security scanned + benchmarked). Covers Physical AI/robotics, simulation, CUDA-X, BioNeMo NIMs, RAG/AI Blueprints, and platform tools. Install via skills CLI; agent picks the matching skill for the task (e.g. cuOpt, DiffDock, OpenFold).

## Recipe / links
- Repo: https://github.com/NVIDIA/skills
- Docs: https://docs.nvidia.com/skills
- Install: `npx skills add nvidia/skills`
- Note: BioNeMo-specific toolkit is also catalogued separately as [bionemo-agent-toolkit](bionemo-agent-toolkit.md)

## Why it made the cut
Clear official catalog + install path + verified/scanned skills with product docs — distinct from single-domain BioNeMo pack already in the wiki.
