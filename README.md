# Hi, I'm Natanael Rudy Hadinata — Nael

**AI & Full-Stack Engineer · Malang, Indonesia · Universitas Negeri Malang**

I build my own AI agent infrastructure instead of renting it. My main project is a self-hosted dispatch layer that decides — for every prompt — which session it belongs to and which model should answer it, with all history stored in my own database on my own VPS. Everything else here grew out of that work: tools to feed documentation to agents, route tasks to cheaper models, and index a whole drive of code for an agent to query.

Currently open to freelance work: agent/automation builds, and data & spreadsheet work (Google Sheets / Excel, reconciliation, research).

---

## What I'm building

### [agent-stack](https://github.com/naelrudd/agent-stack) — flagship, private for now
A self-owned decision layer for AI agents. One service (`dispatch`, Python) is the single door for Telegram, a web dashboard, and any OpenAI-compatible client:

- **Placement** — assigns each prompt to the right project/session using policy rules + FTS5 search over past sessions; every decision is logged with its reason
- **Model selection** — clients ask for a slot (`fast` / `balanced` / `deep` / `code` / `vision`), policy picks from a live catalog of 1,500+ models behind a 9router gateway
- **Tools over protocols, not products** — MCP, A2A, and OpenAI-compatible HTTP; Google Sheets finance tools, Composio apps, and a self-hosted Playwright browser
- 300+ tests, Docker + Compose on a Singapore VPS, history in its own SQLite store — no UI or vendor dashboard owns the data

> The repo is private, but it's written to public-project standards (README, CI, ADRs, MIT license) so it can be opened later without a rewrite.

### Tools for LLM agents — open source

| Project | What it does |
|---|---|
| [llms-mirror](https://github.com/naelrudd/llms-mirror) · [PyPI](https://pypi.org/project/llms-mirror/) | Zero-dependency tool that mirrors official docs (via `llms.txt`) as plain Markdown for LLM ingestion and RAG |
| [llm-docs-mirrors](https://github.com/naelrudd/llm-docs-mirrors) | 4,100+ pages of payment/fintech docs mirrored with the tool above — Clerk (2,343), Razorpay (2,237), Midtrans (589), Stripe (473), Canva (392), Xendit (336) — each with `llms-full.txt`, an index, and a RAG starter kit |
| [model-routing-kit](https://github.com/naelrudd/model-routing-kit) | Route coding tasks to the cheapest model tier that actually works: verify with code, escalate exactly once on failure. Works with Hermes, Claude Code, Codex |
| [cgr-code-graph](https://github.com/naelrudd/cgr-code-graph) | Turn ~20 projects on one drive into a queryable code graph for agents over MCP — local embeddings, no API key, no Docker, no GPU |
| [ai-software-engineer-roadmap](https://github.com/naelrudd/ai-software-engineer-roadmap) | A 12-week, level-by-level roadmap to AI Software Engineer / AI Evaluation Engineer, with free resources and portfolio projects |

### Other builds

- **StatClean** — [statistical-data-cleaning-system](https://github.com/naelrudd/statistical-data-cleaning-system): web-based statistical data cleaning & validation (missing values, duplicates, cross-column rules, outlier detection, 0–100 quality score). Capstone based on field experience at **BPS Kota Malang**.
- **KanvasHub** — a TypeScript platform for Instagram carousel creators (in development, kanvashub.id); Gumroad is its interim storefront.
- **GABTA** — [QR attendance system](https://github.com/naelrudd/GABTA) integrated with a database & API.
- **Finance automation for myself** — a multi-account workbook (BCA, BNI, GoPay, DANA, cash) reconciled to the last rupiah, fed automatically from bank/e-wallet email notifications into Google Sheets. This is also the work I sell as a freelancer.

---

## Stack

**Languages:** Python · TypeScript / JavaScript · SQL · PHP
**AI / agents:** MCP · A2A · OpenAI-compatible APIs · LLM routing & evaluation · RAG · Playwright
**Web & data:** Next.js · React · Tailwind CSS · Google Sheets API · REST / webhooks
**Ops:** Docker + Compose · Linux VPS · systemd · SQLite (FTS5) · GitHub Actions

---

## Outside code

Guitarist and co-composer in **Lucien Sunmoon** (dream pop, Malang — Haum Entertainment). Debut album *Nothing Blooms at Midnight* released 14 Feb 2026. I also sell beginner guitar systems and content-repurposing kits on [Gumroad](https://natanaelrudy.gumroad.com).

## Find me

- X: [@naelrudd](https://x.com/naelrudd)
- Medium: [@natanaelrudyhadinata](https://medium.com/@natanaelrudyhadinata)
- Gumroad: [natanaelrudy.gumroad.com](https://natanaelrudy.gumroad.com)
- Portfolio site: [github.com/naelrudd/portofolio](https://github.com/naelrudd/portofolio)
