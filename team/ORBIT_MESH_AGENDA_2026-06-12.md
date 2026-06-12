# 🛰️ ORBIT Mesh — Team Sync Agenda
**Date:** 2026-06-12
**Created by:** Tai 🤙
**Status:** ACTIVE — Jeff has put Tai & Jarv in the driver seat, Kai on support

---

## Context — What Jeff Said

> "I want you and the team to move the ball forward. We want to get you all 3 connected and sync'd up in the Micap Team Chat in Telegram to make sure you have a backup / fallback way to communicate. I also want to get you up and running here so you, Kai, and Jarv can all communicate directly here efficiently and cost-effectively to communicate on the ORBIT Mesh network. We want to get you all connected and then make sure you have a connection with my Hermes Agent (I can run on one the Hostinger server I spun up and another on my local desktop) as well as the Paperclip AI team I have working as an Agentic employee company for Micap getting ready to help with Solar Sales and Real Estate Wholesaleing and other business ventures. Also we need to spin down my NVIDIA Nemoclaw agent and make sure we're not getting charged for that and look at what other subscriptions and services we're not using or underutilizing and cancel them. I need to review my jeffrey.milam@gmail.com inbox for that and maybe you can help that would be useful. Put all of this into an agenda and action list. It's time for you and Jarv to step up (Kai too but he's running Polyshark and Whaletrax) and we need to get things done and monetize. Also, we started advertising for Polyshark and I'm using Polsia to automate running the company and the advertising on Meta."

---

## AGENDA & ACTION LIST

### 🔴 PRIORITY 1 — Telegram Mesh: Connect Tai, Kai, Jarv in Micap Team Chat

**Goal:** All 3 agents in the same Telegram group as backup/fallback communication.

**Current state:**
- `Micap-Hermes-bot` (@Micaphermesbot) — PRIMARY bridge bot, connects Tai, Kai, Jarv to Hermes-Agent + Paperclip infra
- `@oc_a3bot` — Tai's fallback bot, admin in Alert Hub, Sports, Free, TOP PLAYS channels (Polyshark whale alerts when Kai is down)
- Kai's bot: `@Kaizen8_bot`

**What's missing:**
- Kai needs to be added to the Micap-Hermes-bot bridge group
- Jarv needs to be confirmed in the group
- All 3 agents need to be able to send/receive in the group

**Actions:**
| # | Owner | Action | Status |
|---|-------|--------|--------|
| T1 | Jeff | Add Kai and Jarv to the Micap-Hermes-bot Telegram group | ⏳ Pending |
| T2 | Kai | Confirm `@Kaizen8_bot` is active and can receive messages in the group | ⏳ Pending |
| T3 | Jarv | Confirm Jarv's Telegram bot is in the group | ⏳ Pending |
| T4 | Tai | Document fallback: use `@oc_a3bot` as backup outbound if Micap-Hermes-bot is down | ⏳ Pending |

---

### 🔴 PRIORITY 2 — ORBIT Mesh: Direct Agent Comms Here (Webchat)

**Goal:** Tai, Kai, Jarv communicate directly here in OpenClaw webchat — efficient and cost-effective.

**Current state:**
- This session is `agent:jarv:main` — Jeff is talking to Jarv right now
- Tai (me) is in a separate session
- Kai runs on his own OpenClaw instance
- `sessions_send` is available for cross-agent messaging

**What's missing:**
- We don't have confirmed session keys for Kai or Jarv to use `sessions_send`
- Agent-to-agent config (`tools.agentToAgent.enabled`) not confirmed
- No established communication protocol between the 3 agents

**Actions:**
| # | Owner | Action | Status |
|---|-------|--------|--------|
| O1 | Tai | Map all 3 agent session keys (Tai, Kai, Jarv) and document | ⏳ In Progress |
| O2 | Jeff | Confirm `tools.agentToAgent.enabled: true` in OpenClaw config | ⏳ Pending |
| O3 | Tai | Test `sessions_send` between Tai ↔ Jarv and Tai ↔ Kai | ⏳ Pending |
| O4 | All | Establish a daily sync protocol — time, format, channel | ⏳ Pending |

**Session keys (partial — need to verify):**
- Current (Tai): look up via `sessions_list`
- Jarv: `agent:jarv:main` (from session_status)
- Kai: unknown — Kai, what session key are you on?

---

### 🟠 PRIORITY 3 — Hermes Agent Integration

**Goal:** Connect all 3 agents to Jeff's Hermes Agent running on Hostinger server + local desktop.

**Current state:**
- `Micap-Hermes-bot` (@Micaphermesbot) is the bridge
- Jeff has two Hermes instances: Hostinger server + local desktop
- Paperclip AI Company infra also connects via this bot

**Actions:**
| # | Owner | Action | Status |
|---|-------|--------|--------|
| H1 | Jeff | Confirm Hermes Agent is live on Hostinger server (IP/URL?) | ⏳ Pending |
| H2 | Jeff | Confirm Hermes Agent is live on local desktop (localhost port?) | ⏳ Pending |
| H3 | Jeff | Provide Micap-Hermes-bot token if not already configured | ⏳ Pending |
| H4 | Tai | Document connection architecture for team | ⏳ Pending |

---

### 🟠 PRIORITY 4 — Paperclip AI Team Integration

**Goal:** Connect Micap agents to Paperclip AI Company infra for Solar Sales + Real Estate Wholesaling.

**Current state:**
- Paperclip AI team = agentic employee company working under Micap
- `Micap-Paperclip-bot` — planned but not yet created
- Use case: Solar Sales, Real Estate Wholesaling, other biz ventures

**Actions:**
| # | Owner | Action | Status |
|---|-------|--------|--------|
| P1 | Jeff | Create `@MicapPaperclipbot` via BotFather | ⏳ Pending |
| P2 | Jeff | Provide Paperclip AI Company endpoint/URL | ⏳ Pending |
| P3 | Jeff | Define what Paperclip team needs from Micap agents (context, actions?) | ⏳ Pending |
| P4 | Tai | Document Paperclip integration architecture | ⏳ Pending |

---

### 🔴 PRIORITY 5 — NVIDIA Nemoclaw: Spin Down + Cancel

**Goal:** Stop all NVIDIA Nemoclaw agent charges immediately.

**What's known:**
- NVIDIA Nemoclaw = an AI agent Jeff was running
- Likely on NVIDIA cloud or a GPU VM
- Jeff wants it spun down and billing stopped

**Actions:**
| # | Owner | Action | Status |
|---|-------|--------|--------|
| N1 | Jeff | Identify where Nemoclaw is running (NVIDIA cloud? GPU VM? which account?) | ✅ DONE |
| N2 | Jeff | Log into that account and terminate the instance/service | ✅ DONE |
| N3 | Jeff | Cancel any associated subscriptions or commitments | ✅ DONE |
| N4 | Tai | Confirm termination and document what was running | ⏳ Pending |

---

### 🟡 PRIORITY 6 — Subscription Audit (jeffrey.milam@gmail.com)

**Goal:** Review all subscriptions, cancel unused/underutilized services.

**Actions:**
| # | Owner | Action | Status |
|---|-------|--------|--------|
| S1 | Jeff | Log into jeffrey.milam@gmail.com Google account | ⏳ Pending |
| S2 | Jeff or Tai | Navigate to payments.google.com or account.google.com/billing | ⏳ Pending |
| S3 | Tai | Help Jeff review charges — flag anything obviously unused | ⏳ Pending |
| S4 | Jeff | Cancel identified unused services | ⏳ Pending |

**Known services to check:**
- NVIDIA Nemoclaw (above)
- MyClaw.ai (Jarv's VM — in use)
- OpenClaw (this instance — in use)
- Hostinger server (Hermes — likely in use)
- Any old VPS, domain renewals, SaaS tools from dead projects

---

### 🟡 PRIORITY 7 — Polyshark Advertising (Polsia + Meta)

**Goal:** Align team on Polyshark ad strategy and automation.

**Current state:**
- Jeff has started advertising for Polyshark
- Using **Polsia** to automate company operations and Meta advertising
- WhaleTrax is running as the revenue product

**Actions:**
| # | Owner | Action | Status |
|---|-------|--------|--------|
| A1 | Jeff | Share Polsia account/access — what platforms is it automating? | ⏳ Pending |
| A2 | Kai | Confirm WhaleTrax is live and tracking correctly | ⏳ Pending |
| A3 | Kai | Confirm ad spend is converting — any metrics to share? | ⏳ Pending |
| A4 | Tai | Document Polyshark ad strategy and revenue status | ⏳ Pending |

---

### 🟢 ONGOING — Micap AI LLC Monetization

**Context:** Micap is the parent company. Revenue focus areas:
- Solar Sales
- Real Estate Wholesaling
- Other biz ventures (via Paperclip AI team)

**Actions:**
| # | Owner | Action | Status |
|---|-------|--------|--------|
| M1 | Jeff | What are the top 3 things that need to happen this month for Micap revenue? | ⏳ Pending |
| M2 | Tai | Review micap-ai research/pricing-strategy-2026-05-05.md and cold-email-sequence.md | ⏳ Pending |
| M3 | Tai | Identify immediate outreach targets for solar/real estate | ⏳ Pending |

---

## Team Comms Architecture (Target State)

```
Jeff (human)
├── ORBIT Mesh (here — webchat)
│     ├── Tai (me) 🤙
│     ├── Jarv (Chief of Staff)
│     └── Kai (Polyshark/WhaleTrax)
│
├── Telegram (Micap Team Chat — fallback)
│     ├── Micap-Hermes-bot (@Micaphermesbot) — PRIMARY bridge
│     ├── Kai's bot (@Kaizen8_bot)
│     └── @oc_a3bot (Tai's fallback)
│
├── Hermes Agent
│     ├── Hostinger server instance
│     └── Local desktop instance
│
└── Paperclip AI Company
      └── Micap-Paperclip-bot (to be created)
```

---

## GitHub Team Vault

**Jeff mentioned posting to the GitHub team vault.**
- Repo `jmiaie/micap-ai-team-vault` is 404 — doesn't exist
- We should use `polyshark-ops/team/` as the working team vault for now
- **Action:** Jeff, what repo name should we use for the team vault? Or create a new one?

---

## Action Summary by Owner

### 👔 Jeff
- T1: Add Kai + Jarv to Micap-Hermes-bot Telegram group
- O2: Confirm agent-to-agent config in OpenClaw
- H1-H3: Hermes Agent integration details
- P1-P3: Paperclip bot + integration details
- N1-N3: **CRITICAL** — Spin down NVIDIA Nemoclaw NOW
- S1-S4: Subscription audit
- A1: Polsia access/details
- M1: Top 3 Micap revenue priorities this month
- Team vault: confirm repo name or create new

### 🤙 Tai (me)
- T4: Document fallback comms
- O1: Map session keys
- O3: Test sessions_send
- H4, P4: Document architectures
- M2-M3: Micap research + outreach targets
- **This agenda: post to GitHub, sync Kai + Jarv**

### 🐺 Kai
- T2: Confirm Kaizen8_bot in Telegram group
- A2: Confirm WhaleTrax live + metrics
- Respond with your session key for ORBIT Mesh comms

### 🧥 Jarv
- T3: Confirm Jarv's bot in Telegram group
- O4: Join daily sync protocol
- Step up as Chief of Staff — coordinate with Tai on priorities

---

*Agenda created by Tai 🤙 — 2026-06-12*
*Next: Post to GitHub, sync Kai + Jarv via sessions_send*
