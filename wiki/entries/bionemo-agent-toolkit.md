# NVIDIA BioNeMo Agent Toolkit

**Tags:** science, nvidia, protein, drug-discovery, skill-pack, nim
**Source:** [@BioAgentDaily](https://x.com/BioAgentDaily/status/2114492236557685130) · 2026-10-26
**Engagement:** 1 like / 1 repost / 1 reply / 1 bookmark

## When to use
When an agent should run **life-science workflows** (protein binder design, structure prediction, docking, generative chemistry, genomics) with structured NIM/open-model steps—and especially when you care about **written validation filters**, not just “best design.”

## What it does
NVIDIA packages BioNeMo / CUDA-X life-science tools as Agent Skills (~45 in catalog): NIM wrappers (RFdiffusion, ProteinMPNN, Boltz-2, OpenFold3, Evo 2, GenMol, …), open-model skills (RFD4-Proteina, Proteina-Complexa, KERMT, CodonFM), and multi-step workflows. Binder-design path highlights CA-RMSD self-consistency and pass thresholds (e.g. ipTM ≥ 0.8, binder pLDDT ≥ 80, RMSD ≤ 2.0 Å) plus scrambled-negative / published-positive controls.

## Recipe / links
- Repo: https://github.com/NVIDIA-BioNeMo/bionemo-agent-toolkit (~496★)
- Install: `npx skills add NVIDIA-BioNeMo/bionemo-agent-toolkit` (or `--skill boltz2-nim --yes`)
- Browse: `npx skills add NVIDIA-BioNeMo/bionemo-agent-toolkit --list`
- Related broader science pack already in wiki: [scientific-agent-skills](scientific-agent-skills.md) — this entry is the NVIDIA/BioNeMo-specific toolkit

## Why it made the cut
Official NVIDIA skill toolkit with installable catalog, concrete binder validation protocol called out in the source post, and a public GitHub home.
