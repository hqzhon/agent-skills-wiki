# Unbroker（Hermes Agent）

**Tags:** privacy, security, data-broker, hermes, skill
**Source:** [@iPuneetSingh](https://x.com/iPuneetSingh/status/2114555560603324826) · 2026-10-26
**Engagement:** explanatory quote of viral Nous post; skill lives in hermes-agent (~257K★ org repo)

## When to use
When the user (with **recorded consent**) wants an agent to find personal info on data-broker / people-search sites and file removals—then re-check months later—without bypassing CAPTCHAs or touching public records.

## What it does
Optional Hermes skill (`optional-skills/security/unbroker/SKILL.md`) plus Python CLI `scripts/pdd.py`: dossiers + consent, broker DB, tiered opt-outs, email verify polling, autonomous `next` action queue. Agent drives browse/forms; human only for hard CAPTCHA / ID / phone / fax, surfaced once in a digest.

## Recipe / links
- Skill path: https://github.com/NousResearch/hermes-agent/tree/main/optional-skills/security/unbroker
- Docs: https://hermes-agent.nousresearch.com/docs/user-guide/skills/optional/security/security-unbroker
- Install (Hermes): `hermes skills install official/security/unbroker`
- Author credit in skill: SHL0MS · MIT

## Why it made the cut
Full SKILL.md with consent/autonomy contract, installable recipe, and verifiable repo path—not a privacy rant.
