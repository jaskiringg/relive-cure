# Relive Cure — Product CRM (Showcase)

> **Public overview only.** Application source is private.  
> Screenshots use the real UI with **sensitive fields blurred** (names, phones, messages, URLs, rep rows).

End-to-end patient lead operations for a specialty clinic: inbound chat → qualification → CRM sync → analytics → rep workflows.

## What it is

| Surface | Role |
|---|---|
| Consultation chatbot | Qualifies inbound interest on WhatsApp (multi-language) |
| CRM dashboard | Ops inbox, KPIs, funnel, rep performance |
| Backend API | Lead ingest, sync, scoring hooks |
| Lead scoring board | Fair distribution + SLA-aware prioritization |

## How it works

```
Inbound message → language-aware flow → structured lead capture
    → backend ingest → CRM dashboard (queues + analytics)
    → optional scoring / assignment for sales floor
```

## Screenshots (data blurred, UI intact)

### Analytics dashboard
![Analytics](docs/screenshots/05-login.png)

### Chatbot operations
![Chatbot](docs/screenshots/01-chatbot-lore-tab.png)

### Lead detail view
![Lead panel](docs/screenshots/04-analytics-lead-panel-overview.png)

## Stack (high level)

React · Vite · Node/Express · Supabase · WhatsApp Cloud API · Streamlit

## Related overviews

- [Consultation bot](https://github.com/jaskiringg/lasik-consultation-bot)
- [Lead scoring](https://github.com/jaskiringg/lead-scoring-dashboard)

## Private source (invite-only)

- `relive-cure-dashboard` — CRM UI
- `relive-cure-backend` — API / WhatsApp engine
- `lasik-whatsapp-bot` · `lead-intelligence`

Collaborator: [@siddharth555555](https://github.com/siddharth555555)

---
*No application source in this repository.*
