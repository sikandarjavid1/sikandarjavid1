# Hi, I'm Sikandar 👋

**Senior Full-Stack Engineer · 9 years building production software**

I build data-heavy, AI-powered platforms that ship and hold up in production — real-estate and fintech systems, automation and scraping pipelines, and SaaS products taken from idea to launch. I work the hard, logic-heavy parts most developers avoid: exact financial calculations, scraping that survives, clean data pipelines, and AI/LLM features that do real work, not demos.

Top Rated Plus on Upwork · 100% Job Success · live products with 5-star reviews.

I both **build deeply hands-on** for founders and **lead engineering teams** (8–10 developers) on larger products — so I can take something from a blank repo to a shipped, scalable system, solo or at the head of a team.

---

## 🧭 What I Focus On

**Real-estate & fintech platforms** — proptech is my home turf: lending, underwriting, investor accounting, property data, and the systems founders in this space actually need. I pair that domain depth with:

- **Financial-grade correctness** — decimal-only money math, append-only ledgers, idempotent posting, audit trails. When the numbers have to be exact, they are.
- **Resilient data pipelines & scraping** — collection that survives anti-bot systems, rate limits, and HTML drift, with retries and monitoring so it never silently dies.
- **AI that earns its place** — a rules-first / AI-second cascade: deterministic code for what's knowable, AI only for genuine judgment (classify, score, summarize, extract).
- **Self-hosted / local LLMs in production** — not just API calls. Phi-3 (llama.cpp, grammar-constrained JSON) and Qwen (Ollama) deployed for cost control and data privacy at volume.

---

## 🛠️ Selected work

**Private real-estate lending platform** — end-to-end origination → servicing with multi-investor accounting, a structured payment waterfall, decimal-exact money math, and an append-only audit ledger. *(Python · FastAPI · PostgreSQL)*

**Property-transparency platform** *(live, 5-star)* — consumer web app with map-based search, an OCR document pipeline, and community uploads. *(Next.js · FastAPI · PostgreSQL)*

**Multifamily underwriting / cap-rate platform** — nightly resilient scraping + Google Vision (image classification) + GPT (extracting unit data from descriptions) feeding a region-aware cap-rate engine, with QC flagging. *(Python · FastAPI · Celery/Redis)*

**Startup-intelligence engine** *(live, in commercial use, 5-star)* — scrapes and AI-scores companies from messy free-text into a clean, queryable database. *(Python · FastAPI · PostgreSQL)*

**Event- & championship-intelligence platforms** — two-stage and five-stage pipelines using **local LLMs** (Phi-3 / Qwen) for extraction, with a false-positive-proof detection algorithm and CRM sync. *(FastAPI · React · MongoDB/PostgreSQL · llama.cpp/Ollama)*

**Health-assessment SaaS** *(live, 5-star)* — configurable, admin-tunable scoring engine with booking and a secured admin dashboard. *(Next.js · FastAPI · PostgreSQL)*

> Leading 8–10 developer teams on larger product builds (freelance marketplace + AI recommendation app) over the past ~2 years, alongside hands-on solo delivery for founders.

---

## 🤖 AI & LLM Engineering

Most developers can call an API. I design AI into production systems so it's **reliable, affordable, and isolated** — and when hosted models don't fit, I run open-source models myself.

### Hosted LLM integration (OpenAI / Claude)
- Production use for classification, extraction, scoring, summarizing, and drafting across data-heavy platforms.
- Built for reliability, not demos: strict input validation before the call, **structured / constrained output** so responses are always machine-parseable, plus retries and fallbacks on bad responses.
- Every model call sits behind a **clean adapter interface** — the system asks to "run this task," not "call this specific model" — so swapping or upgrading a model is a config change, not a rewrite.

### Self-hosted / local LLMs in production
The part most freelancers can't offer. When data volume makes hosted APIs too expensive, or data is sensitive, I deploy open-source models on my own infrastructure:
- **Phi-3 via llama.cpp** with **grammar-constrained decoding** — the model is forced to emit only valid, schema-correct JSON, so downstream code can trust every response (no brittle text-parsing of LLM output).
- **Qwen via Ollama** on GPU instances for hybrid extraction workloads, orchestrated programmatically with monitoring.
- Driven by real constraints: **cost at volume** (most records never need a frontier model) and **data privacy** (sensitive data never leaves the box).

### The rules-first / AI-second cascade
A core pattern in how I build: rules attempt everything first; AI catches only what they can't.
- Deterministic code handles anything knowable directly from the data — fast, free, predictable.
- Records that don't match the expected structure, or need genuine judgment, escalate to an LLM (local or hosted, depending on the trade-off).
- Result: the large majority of work stays on cheap deterministic code, and AI cost is reserved for the genuinely hard cases.

### Engineering judgment around AI
- Knowing **when not to use AI** — wrong, slow, or expensive AI where a rule would do is a failure mode I design out.
- Isolating AI so a prompt or model change can never corrupt deterministic logic (e.g. financial calculations stay rule-based and untouchable).
- Validation guards and structured output so AI results are trustworthy enough to act on automatically.

---

## ⚙️ Tech Stack

**Languages:** Python · TypeScript · JavaScript · Go *(learning)* · PHP
**Backend:** FastAPI · Django · DRF · Flask · Node patterns · Celery · Redis · RabbitMQ
**Frontend:** Next.js · React · TypeScript · Tailwind · Redux
**Data/DB:** PostgreSQL · MongoDB · MySQL · Elasticsearch · SQLAlchemy
**AI/LLM:** OpenAI · Claude · local LLMs (Phi-3 via llama.cpp, Qwen via Ollama) · grammar-constrained decoding · pandas/NumPy
**Scraping:** Playwright · Scrapy · Selenium/undetected-chromedriver · Zyte · proxy rotation
**Cloud/DevOps:** AWS · Vercel · Render · DigitalOcean · Docker · Nginx · GitHub Actions · Cloudflare
**Payments/Auth:** Stripe · Clerk · JWT

---

## 📈 What I'm doing now

- Building production real-estate & fintech platforms for founders, solo and direct.
- Going deeper on local/self-hosted LLM deployment and Go for high-performance backends.

---

## 🌐 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/sikandarjavid) [![X](https://img.shields.io/badge/X-black.svg?logo=X&logoColor=white)](https://x.com/sikandar_javid)

![](https://github-readme-stats.vercel.app/api?username=sikandarjavid1&theme=dark&hide_border=true&count_private=true)
