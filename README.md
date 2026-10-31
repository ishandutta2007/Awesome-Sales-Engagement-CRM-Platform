# Awesome-Sales-Engagement-CRM-Platform

## Top Sales Engagement & CRM Platform Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Unified Sales Engagement, Pipeline Management & Self-Hosted CRM Platforms*  

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Sales Engagement & CRM Platforms**. These tools enable revenue teams to combine contact management, multi-channel outreach sequences, and deal pipeline tracking in one system—turning disconnected prospecting and CRM tools into a unified revenue engine.



**Examples** include HubSpot Sales Hub, Salesforce Sales Cloud, Salesloft, Outreach, Pipedrive, Apollo.io, Freshsales, Zoho CRM, Close, and Groove (the category leaders).



**Open-source emphasis**: Sales Engagement & CRM is a domain where open-source tooling is **mature at the CRM layer and emerging at the engagement layer, but rarely unified**. **Twenty** is the strongest open-source CRM—AGPLv3 licensed, actively developed, with customizable objects, Kanban pipelines, and MCP support for AI agents . **AgentSDR** is the most complete open-source sales engagement workspace—MIT licensed, self-hosted, with email/LinkedIn/WhatsApp sequences and an AI CRM that classifies replies and drafts responses for human approval . **Horilla CRM** provides a production-grade Django CRM with built-in sales cadences (scheduled outreach sequences), multi-tenancy, and a modern HTMX frontend . **OutreachPro** offers a lightweight Instantly.ai clone with Google Maps lead scraping, Claude AI personalization, and a Kanban CRM pipeline . The critical caveat: **no single open-source project combines Twenty's CRM depth with AgentSDR's multi-channel engagement**—you either run two systems side-by-side or accept feature gaps in one layer.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[HubSpot Sales Hub](https://www.hubspot.com/)**  

  Unified sales engagement and CRM; sequences, deal pipelines, email tracking, and calling tied directly to contact records and marketing automation.



- **[Salesforce Sales Cloud](https://www.salesforce.com/)**  

  The enterprise CRM standard with customizable pipelines, forecasting, and the AppExchange ecosystem for extending engagement capabilities.



- **[Salesloft](https://salesloft.com/)**  

  Sales engagement platform with multi-channel cadences, dialer, and conversation intelligence; positioned for enterprise SDR teams.



- **[Outreach](https://www.outreach.io/)**  

  Sales engagement platform with sequences, conversation intelligence, and revenue intelligence analytics; the benchmark for enterprise sales engagement.



- **[Pipedrive](https://www.pipedrive.com/)**  

  Sales-focused CRM built around a visual pipeline; known for simplicity and activity-based selling with deal rotting alerts.



- **[Apollo.io](https://www.apollo.io/)**  

  All-in-one prospecting and engagement platform with a massive B2B contact database, enrichment, email sequences, and dialer.



- **[Freshsales](https://www.freshworks.com/freshsales/)**  

  CRM from Freshworks with visual pipeline, AI-powered deal insights, and built-in phone/email engagement.



- **[Zoho CRM](https://www.zoho.com/crm/)**  

  Comprehensive CRM within the Zoho ecosystem; pipeline management, forecasting, and sales automation with competitive pricing.



- **[Close](https://close.com/)**  

  Conversation-first CRM with built-in calling, email, and SMS; sequences, smart views, and reporting for small sales teams .



- **[Groove](https://www.groovehq.com/)**  

  Sales engagement platform for Salesforce and Gmail/Outlook; sequences, auto-logging, and meeting scheduling.



## Open-Source GitHub Projects



### Full CRM Platforms (Pipeline + Deal Tracking)



- **[Twenty](https://github.com/twentyhq/twenty)**  

  The **most actively developed open-source CRM** (AGPLv3, ~58k GitHub stars) . Explicitly built as a Salesforce alternative with a modern UX. Features: **customizable objects and fields**, Kanban and table views, custom roles and permissions, **trigger-based workflow automation**, emails, tasks, notes, and **MCP support for AI agent access to CRM data** . **Best for teams wanting a modern, extensible CRM foundation**—but it is a CRM, not a sales engagement sequencer.



- **[Horilla CRM](https://github.com/horilla/horilla-crm)**  

  Production-grade **Django CRM** (open-source) with **sales cadences** (scheduled outreach sequences for email, call, task steps), opportunities with configurable stages and forecasting, campaigns, multi-tenancy, WebSocket real-time notifications, and a four-layer permission model . Features a modern HTMX + Tailwind frontend (no SPA overhead) and DRF API for every module. **Best for teams wanting a CRM with built-in cadences**—the closest open-source option to a unified CRM + engagement platform, though cadences are less sophisticated than dedicated sequencers.



### Full Sales Engagement Workspaces (Multi-Channel + CRM)



- **[AgentSDR](https://github.com/kandid-ai/agentsdr)**  

  The most comprehensive open-source **self-hosted AI SDR** (MIT, v0.3.1) . Features: **email sequences** from Google Workspace mailboxes with merge fields, per-mailbox daily limits, and sending windows; **LinkedIn campaigns** via Unipile (invite, accept message, follow-ups, paced at 30 invites/day on premium); **WhatsApp** message campaigns and calls via Chrome extension, recorded and transcribed . **AI CRM** classifies every reply and drafts responses for human approval—nothing sends automatically . Enrichment tables with AI columns and 15 providers (Apollo, Hunter, Lusha) . Docker Compose with PostgreSQL 16. **Best for teams wanting multi-channel engagement with AI assistance and full data ownership**—the closest open-source equivalent to an integrated sales engagement platform.



- **[OutreachPro](https://github.com/vvlars-cmd/outreachpro)**  

  Open-source **Instantly.ai clone** (MIT) with Google Maps lead scraping via Apify, Claude AI personalization, multi-step email campaigns with stop-on-reply and daily limits, a unified reply inbox with AI auto-labeling, **Kanban CRM pipeline** (Prospect → Won), email warmup, and analytics . Docker-first deployment with JSON file storage. **Best for small teams wanting a lightweight, self-hosted cold email + CRM pipeline**—but it is early-stage (2 weekly npm downloads as of March 2026) and uses JSON files rather than a database .



### Additional Strong Open-Source Options



- **Signal** — Open-source **AI sales intelligence and outreach automation** alternative to Clay/Apollo/Outreach; watches the web for buying signals (hiring, funding, launches), enriches contacts, drafts personalized outreach, and runs multi-step email sequences . Self-hosted on Supabase + Anthropic keys. **Best for teams wanting signal-based prospecting**—but requires significant setup and is single-tenant by design.

- **openoutreach** — Open-source **AI agent for B2B lead generation** (GPLv3); describes your product and target market, the LLM finds and qualifies leads with a stated reason per lead, exports CSV in Instantly/Smartlead format, and includes a Django Admin CRM . **Best for teams wanting autonomous lead discovery**—but it is a CLI/agent, not a full sales engagement UI.



**Frameworks for building custom systems**: For a **modern CRM foundation with pipeline and automation**, Twenty provides the strongest open-source option . For **CRM with built-in cadences**, Horilla CRM . For **multi-channel engagement with AI reply handling**, AgentSDR . For **lightweight cold email + pipeline**, OutreachPro . No single open-source project matches HubSpot's **integrated marketing-sales-service suite** or Salesforce's **AppExchange ecosystem**—you either assemble Twenty + AgentSDR or accept feature gaps.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Sales engagement and CRM platforms handling customer and deal data must comply with applicable privacy regulations (GDPR, CCPA) and platform terms of service; **LinkedIn automation, bulk WhatsApp messaging, cold email, and call recording carry legal and platform risks** that self-hosted tools do not eliminate .

- **Open-source sales engagement and CRM is mature at the CRM layer and emerging at the engagement layer**—Twenty and Horilla provide production-grade CRMs , and AgentSDR provides multi-channel engagement . However, **no single open-source project matches HubSpot's integrated marketing-sales-service suite or Salesforce's AppExchange ecosystem**—organizations requiring that depth should evaluate commercial platforms or plan for assembly.

- Verify license terms for commercial use; Twenty uses AGPLv3 , AgentSDR uses MIT , and Horilla CRM is open-source .



---



**Made for sales leaders, revenue operations teams, and organizations choosing their CRM and engagement stack.**  

Let's make sales engagement and CRM more open, but with clear eyes about the integration gaps that commercial suites still fill.
