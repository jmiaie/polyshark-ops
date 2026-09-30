# polyshark-ops

> **Primary role (2026-09-30):** **Polyshark team knowledge base** — ops briefs and handoff notes under `team/`, `micap-ai/`, and related docs.  
> See [`STATUS.md`](STATUS.md). Canonical pliamem recall/router is **[`jmiaie/pliamem`](https://github.com/jmiaie/pliamem)**; memory SKU is **[`jmiaie/ompa`](https://github.com/jmiaie/ompa)**.

## Team knowledge base (start here)

| Path | Contents |
|------|----------|
| `team/` | Team ops / catch-up notes |
| `micap-ai/` | Micap-related briefs |
| `docs/` | Additional ops documentation when present |
| [`STATUS.md`](STATUS.md) | Honest repo role, install re-verify notes, next actions |
| [`SPEC.md`](SPEC.md) | Spec text tied to the **embedded** pliamem-shaped tree (historical) |

Treat dated briefs as **historical** unless an owner has refreshed them. This remote is **not** a claim that Polyshark services are shipping from here.

## Embedded pliamem tree (stale snapshot — not the SKU)

The repo root still contains a **pliamem-shaped** Node tree (`src/`, root `package.json`, cloud-ui, etc.). That tree is a **stale embedded copy** kept for history / local `npm test` continuity.

- **Do not** dual-maintain product features here.
- **Do not** large-delete the embedded tree without an explicit owner decision (data loss / broken relative links risk).
- Prefer contributing recall/router work to [`jmiaie/pliamem`](https://github.com/jmiaie/pliamem) and memory-SKU work to [`jmiaie/ompa`](https://github.com/jmiaie/ompa).

### Optional: run the embedded unit suite

On Node ≥18, from repo root:

```bash
npm test
```

Last hygiene re-verify (2026-09-30): **65 passed**. That only exercises the embedded snapshot — it does **not** validate live Polyshark services or prove a publishable npm/PyPI release from this remote.

### Historical CLI sketch (embedded snapshot only)

```bash
# These entrypoints belong to the embedded tree — prefer canonical pliamem for real use
npm start   # if defined in package.json
# pliamem-style commands may exist only after local wiring; see STATUS.md
```

## License

See [`LICENSE`](LICENSE).
