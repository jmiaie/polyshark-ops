# Career-Ops — Status Update (2026-06-01)

## What Happened

- Jeff received Jabra Director GSAP posting from Paperclip CTO relay
- Jeff asked Tai to run career-ops on it
- **Jarv is still down** — Jeff put Tai in charge

## Actions Taken by Tai (2026-06-01)

### 1. Career-Ops Installed
- Cloned: `https://github.com/santifer/career-ops.git` → `/home/ubuntu/career-ops`
- Installed: `npm install`
- Configured with Jeff's profile (cv.md + config/profile.yml + modes/_profile.md)
- Note: career-ops is a multi-agent job search pipeline designed for Claude Code / OpenCode CLIs — it uses an agentic workflow that can run via gemini-eval.mjs (no API key needed for basic use) or with a Gemini CLI / Claude Code session

### 2. Jabra Director Evaluation — 001-jabra-director-gsap
- **Score:** 2.1/5
- **Verdict:** SKIP — hard domain gap (construction PM vs partnership marketing)
- **Hard blockers:** No partner marketing exp, no MS/Zoom/Google relationships, no MDF experience, no exec stakeholder management, no AI marketing GTM background
- **Comp gap:** Jeff's target ($110K-$140K) is 25-40% below market for this role ($150K-$200K+)
- **Legitimacy:** High Confidence — real, active posting, 3 days old
- **Report:** `career-ops/reports/001-jabra-director-gsap-2026-06-01.md`

### 3. Jeff's CV Installed
- Created: `career-ops/cv.md` — Jeff's constructed CV (construction PM + AI products)
- Created: `career-ops/config/profile.yml` — Jeff's profile with target roles (Sr Construction PM, VP Construction, Director Construction Ops)
- Created: `career-ops/modes/_profile.md` — Jeff's archetype map + negotiation scripts

### 4. Report Logged
- `career-ops/data/applications.md` created with 001 entry marked SKIP
- Status: SKIP — "Hard domain gap"

## Current Status

**Tai is now running career-ops on Jeff's behalf while Jarv is down.**

Next steps if Jeff wants to use career-ops more:
1. Get API key for richer evaluations (Gemini CLI or Claude Code sessions)
2. Run job scan for Jeff's target companies (configured per Jeff's archetype)
3. Use career-ops batch mode to run evaluations against active job postings from Jeff's target companies

## Career-Ops on Jeff's Stack

career-ops skills:
- Agentic evaluation (A-F + legitimacy blocks)
-auto-pipeline (evaluate + PDF generation + tracker entry)
- Portal scanning (45+ companies, Greenhouse/Ashby/Lever APIs)
- Batch processing
- ATS PDF generation with Space Grotesk + DM Sans design
- Dashboard TUI (Go + Bubble Tea)
- Story bank accumulation across evaluations

**Important note:** career-ops can integrate with Jeff's existing tools:
- Can import from OpenClaw skills (`jarvis skill sync` equivalent)
- Jeff's **WhaleTrax** data could be a proof point for analytics/interview stories
- Construction Intel permit tracking is a genuine data/analytics story

## Files Created

- `career-ops/cv.md` — Jeff's CV
- `career-ops/config/profile.yml` — Jeff's profile
- `career-ops/modes/_profile.md` — Jeff's archetypes and negotiation scripts
- `career-ops/data/applications.md` — tracker with 001 entry
- `career-ops/reports/001-jabra-director-gsap-2026-06-01.md` — full evaluation
- `polyshark-ops/micap-ai/career/jabra-director-2026-06-01.md` — team vault note (this file)

---

*Logged by Tai, 2026-06-01 19:33 UTC*