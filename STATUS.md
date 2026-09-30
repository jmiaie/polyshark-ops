# Status — polyshark-ops

**Updated:** 2026-09-30 (PT)  
**Described purpose:** Polyshark **team knowledge base** / ops notes (`team/`, `micap-ai/`, Jarv/real-estate briefs).  
**Maturity:** Stalled ops dump with an embedded **stale pliamem source tree** at repo root.

## What this repo is (honest)

| Path | Role |
|---|---|
| `team/`, `micap-ai/`, catch-up briefs | Primary value — Polyshark/Micap **ops and handoff notes** |
| Root `src/`, `SPEC.md`, pliamem-shaped `README.md`, `package.json` | **Stale copy** of the pliamem recall/router tree — **not** the product SKU |

## Canonical homes (do not dual-maintain from here)

| Concern | Canonical repo |
|---|---|
| pliamem recall/router | [`jmiaie/pliamem`](https://github.com/jmiaie/pliamem) (private) + public twin [`pliamem-public`](https://github.com/jmiaie/pliamem-public) |
| Memory product SKU | [`jmiaie/ompa`](https://github.com/jmiaie/ompa) |
| This repo | Keep as **team KB**; treat root pliamem files as historical snapshot unless deliberately synced |

## Install / test re-verify (2026-09-30)

On a Node ≥18 box, from repo root:

```bash
npm test
```

Observed this wave: **65 passed / 0 failed** (same suite shape as private pliamem). That only proves the **embedded pliamem tree** still runs unit tests — it does **not** mean this repo is the shipping SKU, and it does **not** validate team docs or live Polyshark services.

No CI workflow changes in this hygiene pass (token lacks `workflow` scope).

## Gaps

- Root README still reads as a pliamem product pitch — misleading for a team KB
- No package publish story claimed from this remote
- Ops notes under `team/` may be dated; treat as historical unless refreshed

## Next (owner)

1. ~~Rewrite root README to lead with team KB~~ **done** (2026-09-30 follow-up)
2. Strip/archive the embedded pliamem tree **only after** Jeff confirms KB-only (no large delete in bot waves)
3. Keep career/recruiting material out of automated outbound (CAREER gate off for bots)
