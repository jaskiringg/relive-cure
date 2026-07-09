# Relive Cure — Healthcare Lead Ops (Showcase)

> **Public overview only.** Application source is private.  
> Screenshots use the real UI with **sensitive fields blurred** (names, phones, messages, URLs, rep rows).

Relive Cure is a LASIK clinic I operate and the software that runs it. Two surfaces do most of the work:

1. **Agent Console** — AI agents that drive **organic marketing** (content pipeline, drafts, multi-channel publishing).
2. **CRM Analytics** — the **ops command center** where leads, reps, SLAs, and funnel health live.

Inbound from ads, WhatsApp, and organic social flows through qualification → CRM → rep assignment → appointment.

---

## 1. Agent Console — organic marketing with AI agents

The Agent Console is not a chatbot skin. It is a **marketing operations layer**: agents run overnight, rank what matters, draft channel-specific content, and queue everything for founder approval before anything publishes.

**Medical-safe by design** — publishing is gated. Nothing goes live without explicit approval. Agents can be offline; the console still shows what ran and what is waiting.

### What the agents do

| Step | What happens |
|------|----------------|
| **Monitor** | Competitor signals, market context, overnight activity digest |
| **Rank** | Content insights scored and ordered into a growth plan |
| **Generate** | Pipeline ideas → channel-specific drafts (Facebook, Instagram, SEO blog, reels) |
| **Queue** | Drafts land in an inbox for review — Approve / Reject / Full editor |
| **Publish** | WordPress, WhatsApp, Instagram, LinkedIn, Facebook (when enabled) |

### Overnight loop (example)

```
Competitor + market signals
    → agents rank insights & create pipeline ideas
    → writers produce drafts per channel
    → founder reviews pending drafts
    → approved content publishes to organic channels
    → inbound interest routes to CRM / WhatsApp qualification
```

Typical overnight output: ranked insights, dozens of pipeline ideas, and multiple drafts ready for approval — without manual content research each morning.

### Screenshot — Agent Console (same view as portfolio)

![Agent Console — organic marketing pipeline, overnight digest, pending drafts](docs/screenshots/02-agent-console-organic-marketing.png)

*Agent runs, ranked insights, pipeline ideas, pending Facebook / Instagram / SEO drafts, and platform integrations. Sensitive fields blurred.*

---

## 2. CRM Analytics — the command center

The CRM is where operations actually run: **4,800+ leads** synced from Refrens, funnel health, rep performance, SLA breaches, and channel status — one screen the sales floor and I both use daily.

### What it tracks

| Area | Detail |
|------|--------|
| **Funnel** | Total leads, converted, lost, DNP, SLA breach counts |
| **Lead health** | Status distribution, city breakdown, hot intent |
| **Rep performance** | Per-rep conversion, response time, SLA, OPD booked |
| **Channels** | WhatsApp bot status, shadow mode, pipeline live indicator |
| **Sync** | Refrens CRM pull, CSV/Excel export, bulk download |

Five reps run on this daily. When a workflow breaks in the morning, I see it here and ship the fix the same day — operator and engineer in one seat.

### Screenshot — CRM Analytics (same view as portfolio)

![CRM Analytics — funnel, lead health, rep performance](docs/screenshots/03-crm-analytics-dashboard.png)

*Refrens-synced analytics: funnel metrics, lead health donut, rep table with conversion and SLA columns. Sensitive fields blurred.*

---

## How the two surfaces connect

```
Organic / paid inbound          Agent-generated content
        │                                │
        ▼                                ▼
   WhatsApp / forms              Social + SEO channels
        │                                │
        └──────────┬─────────────────────┘
                   ▼
        AI qualification (multi-language)
                   ▼
           CRM ingest + scoring
                   ▼
         Rep assignment + SLA bands
                   ▼
              Appointment booked
```

| Surface | Role |
|---------|------|
| **Agent Console** | Organic marketing engine — insights, drafts, approval, publish |
| **Consultation chatbot** | Qualifies inbound interest on WhatsApp ([overview](https://github.com/jaskiringg/lasik-consultation-bot)) |
| **CRM dashboard** | Ops inbox, KPIs, funnel, rep performance |
| **Lead scoring board** | Fair distribution + SLA-aware prioritization ([overview](https://github.com/jaskiringg/lead-scoring-dashboard)) |
| **Backend API** | Lead ingest, sync, scoring hooks, agent orchestration |

---

## More screenshots

### Consultation chatbot (WhatsApp qualification)
![Chatbot operations](docs/screenshots/01-chatbot-lore-tab.png)

### Lead detail panel
![Lead panel](docs/screenshots/04-analytics-lead-panel-overview.png)

---

## Stack (high level)

React · Vite · Node/Express · Supabase · WhatsApp Cloud API · Gemini · agent orchestration · Streamlit

---

## Related overviews

- [Consultation bot](https://github.com/jaskiringg/lasik-consultation-bot) — WhatsApp qualification flow
- [Lead scoring](https://github.com/jaskiringg/lead-scoring-dashboard) — fair assignment + SLA bands

## Private source (invite-only)

- `relive-cure-dashboard` — CRM UI + Agent Console
- `relive-cure-backend` — API, WhatsApp engine, agent jobs
- `lasik-whatsapp-bot` · `lead-intelligence`

Collaborator: [@siddharth555555](https://github.com/siddharth555555)

---
*No application source in this repository — showcase README and blurred screenshots only.*
