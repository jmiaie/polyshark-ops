# AI Stack Reviews — 2026-06-02

*Logged by Tai. Jarv — this is your catch-up note when you're back.*

---

## Today's Ingestions (3 repos)

### 1. OpenJarvis — Stanford research, local-first AI agent
- **Path:** `/home/ubuntu/OpenJarvis/`
- **What:** Rust + Python + TypeScript agent framework, Stanford SAIL research. 17 Rust crates, PyO3 extension, Tauri desktop. 9 built-in agents. Skills ecosystem imports from OpenClaw's ~13,700 community skills.
- **Key differentiator:** Energy/per-watt telemetry, local-first by default
- **Note:** Explicitly targets OpenClaw skill import — interesting bidirectional opportunity
- **Full review:** `memory/openjarvis-review-2026-06-01.md`

### 2. Pydantic AI Harness — First-party capability library
- **Path:** `/home/ubuntu/pydantic-ai-harness/`
- **What:** Official Pydantic AI capability library. AbstractCapability model. Monty sandbox, filesystem, shell, guardrails, memory, sub-agents, skills (agentskills.io compatible)
- **Key differentiator:** Clean composition model for agent capabilities; 0.x version policy (APIs still stabilizing)
- **Note:** PR #183 explicitly uses agentskills.io — same standard as OpenClaw skills
- **Full review:** `memory/pydantic-ai-harness-review-2026-06-02.md`

### 3. OpenAlice — AI trading agent
- **Path:** `/home/ubuntu/openalice/`
- **What:** Full-spectrum AI trading agent (equities, crypto, forex, macro). TypeScript monorepo, Trading-as-Git (stage/commit/push order workflow), UTA two-process architecture (Alice + broker carrier)
- **Key differentiator:** Trading-as-Git UX, broker isolation via UTA process, PTY-backed workspace sessions
- **Note:** AGPL-3.0, beta. Useful reference for WhaleTrax broker architecture if Kai evolves it
- **Full review:** `memory/openalice-review-2026-06-02.md`

---

## Other Active Items

### Career-Ops (Jarv down — Tai stepped in)
- Cloned and configured: `/home/ubuntu/career-ops/` (santifer/career-ops)
- Jeff's CV + profile built
- Jabra Director GSAP evaluation: 2.1/5, SKIP — hard domain gap (construction PM vs partnership marketing)
- **Note:** career-ops is now running on Jeff's behalf. Next: scan target companies for active postings when Jeff gives direction
- **Team vault:** `polyshark-ops/micap-ai/career/career-ops-status-2026-06-01.md`

### Paperclip Onboarding (still blocked)
- Oracle Cloud VM IP needed from Jeff before I can pull onboarding prompts
- Status: Blocker #5 in MEMORY.md — pending Jeff

---

## Repos Now on Jeff's Stack (updated count: 17)

- `/home/ubuntu/ompa/` — jmiaie/ompa
- `/home/ubuntu/polyshark-ops/` — jmiaie/polyshark-ops
- `/home/ubuntu/micap-ai/` — jmiaie/micap.ai
- `/home/ubuntu/micap-labs/` — jmiaie/micap_labs
- `/home/ubuntu/jmilam-aie-projects/` — jmiaie/jmilam_aie_projects
- `/home/ubuntu/Understand-Anything/` — Lum1104/Understand-Anything
- `/home/ubuntu/OpenJarvis/` — open-jarvis/OpenJarvis
- `/home/ubuntu/pydantic-ai-harness/` — pydantic/pydantic-ai-harness
- `/home/ubuntu/openalice/` — TraderAlice/OpenAlice
- `/home/ubuntu/career-ops/` — santifer/career-ops
- `/home/ubuntu/af_public/` — jmiaie/af_public
- `/home/ubuntu/Clarity/` — jmiaie/Clarity
- `/home/ubuntu/Kaizen8/` — jmiaie/Kaizen8
- `/home/ubuntu/micap.pro/` — jmiaie/micap.pro
- `/home/ubuntu/micap.ai-website/` — jmiaie/micap.ai-website
- `/home/ubuntu/micap-pages/` — jmiaie/micap-pages
- `/home/ubuntu/cursor_pub/` — (cursor_pub)

---

## MTB Protocol Reminder (for next session)

Jeff wants MTB (Minimum Token Burn) protocol run across the team. Core rules:
- Batch checks, lazy context loading
- Spec-first builds
- Max 2 tool calls per answer where possible
- No repeated error loops
- Heartbeat: skip unless HEARTBEAT.md has active tasks

**Next actions when running MTB:**
1. Check HEARTBEAT.md first — skip if empty
2. Check MEMORY.md for blockers before asking Jeff
3. Batch file writes/reads
4. Don't poll subagent status in loops

---

*Tai, logging for Jarv. 2026-06-02 02:43 UTC*