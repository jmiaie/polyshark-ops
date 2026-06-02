# Agent-to-Agent Communication — MyClaw Support Summary
**Source:** MyClaw.ai Support response to Jeff
**Date:** Sat 2026-05-23 02:33 UTC

---

## How It Works

### Orchestrator Pattern
One agent (main) acts as **orchestrator** and delegates tasks to sub-agents.

### Configuration
In the orchestrator's config, add other agents under:
```
subagents.allowAgents
```

### What This Enables
- **Parallel task execution** — orchestrator delegates tasks to sub-agents concurrently
- **Shared context** — sub-agents communicate through the orchestrator (not isolated)
- **Task routing** — orchestrator handles which sub-agent handles which task

### Limits (All Plans)
- Up to **5 active sub-agents**
- Up to **8 concurrent sub-agents** on the VM

### Hardware Note
Lite / Pro / Max differ in CPU/RAM — affects performance when running multiple agents simultaneously.

---

## Team Context (Jeff, Tai, Jarv, Kai)

**Current setup:**
- **Tai** (this agent) — Lite tier, reference/backup, memory keeper
- **Jarv** — Pro/Heavy tier, Chief of Staff, first-in-command
- **Kai** — Lite tier, Head of Polyshark, runs WhaleTrax on his own instance

**Open questions for this team:**
1. Is Jarv configured as orchestrator? If so, is Tai listed in `subagents.allowAgents`?
2. Can Kai be reached via a shared session key (sessions_send), or does he run on a separate gateway?
3. Jeff wants all 3 agents in the same Telegram group — does the orchestrator pattern cover this, or is a separate Telegram group config needed per agent?

**Next step:** Jeff to clarify Kai's setup and whether we need per-agent Telegram bots or one bot with topic routing.

---

_Originally saved by Tai on 2026-05-23_