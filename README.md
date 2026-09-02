# Aviv Gur

### High-Agency Builder · AI Automation · Business Operations

I spent years running business operations — finance, CRM, multi-entity workflows — and kept hitting the same wall: critical processes held together by manual work and spreadsheets. So I learned to build. Now, when I see an operational bottleneck, I design and ship the system that removes it: from workflow mapping through architecture, code, deployment, and adoption.

I'm not a classical algorithms engineer. I'm the person who understands the business problem, opens a laptop, and builds the end-to-end solution — with production discipline: typed code, tests, CI, human-review controls, and safe failure modes.

## Selected projects

### 📊 [Adtex — Executive Operations Platform](https://github.com/avivgur/adtex-management-platform)

**The problem:** Leadership at a multi-entity AdTech company relied on four disconnected systems — a performance API, Monday.com CRM, Google Sheets finance ledgers, and an operational database. No single view showed what was happening, whether the data was fresh, or where to intervene.

**The build:** A unified executive command center: typed connector contracts isolate each provider's schema, a snapshot orchestrator pulls all sources concurrently with independent health reporting, and a business-rules layer turns raw events into KPIs, alerts, and goal pacing. In the production system this runs on scheduled syncs with self-healing backfills — and serving optimization cut dashboard TTFB from 3.4s to ~30ms.

**What it demonstrates:** Multi-system integration architecture (CRM, finance, performance data), operational reliability engineering, and translating executive decision-making needs into a data platform. The public repo is a clean-room edition with synthetic data.

**Stack:** Next.js · TypeScript · React · Monday.com API · Google Sheets API · Supabase · Vercel Cron · Vitest · GitHub Actions

### 🎹 [KeySight — Piano Practice Tracker](https://github.com/avivgur/piano-tracker)

**The problem:** Music teachers see students once a week, but the learning happens between lessons — and that practice is invisible. Manual practice logs add friction and rarely reflect what was actually played.

**The build:** An end-to-end B2B2C system. A Raspberry Pi captures MIDI from the piano, a FastAPI backend compares each performance against the uploaded sheet music (MusicXML parsed with music21), and **GPT-4o turns the structured error report into two tailored outputs** — a technical report for the teacher, an encouraging one for the student.

**What it demonstrates:** LLM integration on top of deterministic analysis, edge-to-cloud architecture, and role-specific product thinking.

**Stack:** Python · FastAPI · PostgreSQL · OpenAI GPT-4o · music21 · Next.js · TypeScript · Raspberry Pi

### 🧾 [Invoice Operations Automation](https://github.com/avivgur/invoice-operations-automation)

**The problem:** Finance teams burn hours copying invoice data between systems — and a single bad sync can silently overwrite valid financial records. Built from real multi-entity finance-operations experience.

**The build:** A reconciliation pipeline that treats sync as a controlled workflow, not a blind import: deterministic diffing by stable IDs, automatic handling of safe changes, and **human-review routing for suspicious ones** (amounts zeroing out, sign flips, material changes). Dry-run by default; nothing is written without an explicit `--apply`.

**What it demonstrates:** Automation with auditability and guardrails — the difference between a script and a system a finance team can trust.

**Stack:** Python · Pydantic · Google Sheets API · pytest · mypy · GitHub Actions CI

## How I work

1. Start with the operational problem and the people living with it
2. Map the workflow, constraints, and failure modes
3. Build the smallest system that creates real leverage
4. Ship with controls: typing, tests, dry-runs, human review where it matters
5. Deploy, measure adoption, iterate

## Technology

**Languages:** Python, TypeScript, SQL  
**AI:** OpenAI API (GPT-4o), LLM workflow design, prompt engineering for structured outputs  
**Backend & data:** FastAPI, PostgreSQL, SQLAlchemy, Pydantic, Supabase  
**Frontend:** Next.js, React  
**Integrations & automation:** Google Workspace APIs, Monday.com, REST APIs  
**Delivery:** GitHub Actions, CI/CD, Docker, Alembic, Raspberry Pi

## Connect

Looking for roles at the intersection of AI, operations, and implementation — where understanding the business is as important as shipping the code.

[LinkedIn](https://www.linkedin.com/in/aviv-gur-1a56a4211/) · [Repositories](https://github.com/avivgur?tab=repositories)
