# Hey, I'm Brody 🪄

I'm a product engineer and designer based in Seattle. I spent nearly a decade learning how products actually reach people: marketing, sales, and account management across music and tech, before getting into UX/UI design.

I love designing interfaces, but I also want to build them. That pull towards building is what took me from design into engineering. I'm obsessed with usability: how something feels when you click it, whether the flow makes sense the first time, whether the thing actually works the way someone expects it to. That obsession drives everything I build.

---

## What I'm Building

### [BidLine](https://bidline.app) — Production Finance for Film & TV

Film and TV producers manage budgets worth hundreds of thousands to millions of dollars on disconnected Excel spreadsheets that haven't changed in decades. BidLine replaces that workflow: bidding, cost tracking, invoice reconciliation, and actuals reporting in one system, built around the APA UK standard.

**Stack:** Next.js · Supabase · PostgreSQL · Tailwind · Vercel

This one pushed me the most technically:
- Built v1, hit architectural limits from premature abstraction, and made the call to rebuild from scratch with a deliberately simpler architecture
- Lifecycle management where estimates freeze as an immutable baseline when production starts, and all actuals track against that frozen snapshot
- Invoice manager with automatic payee matching, approval workflows, and a secure external submission link for vendors
- 10 core tables, 22 PostgreSQL functions, 40+ row-level security policies, 136 schema migrations, all built solo
- APA UK grade-based overtime and day rate calculations with invoice-driven actuals

Currently in closed beta with UK production companies.

---

### [JobJar](https://jobjar.io) — Unfiltered Job Aggregator

JobJar aggregates job listings daily from 16 sources — Greenhouse, Lever, Ashby, RemoteOK, Remotive, We Work Remotely, and more — and displays them without algorithmic ranking or filtering. 278,000+ active listings. Search by title, location, seniority, or remote status.

**Stack:** Next.js · Neon (PostgreSQL) · Prisma · Clerk · Vercel

Some of the interesting problems I got to solve here:
- Built a custom ATS slug harvester using the Wayback Machine CDX API to discover and index 10,000+ company career page endpoints across Greenhouse, Lever, and Ashby
- Gemini 2.5 Flash classification pipeline that automatically tags every listing with seniority, employment type, remote status, country, and city at ingest
- Parallelized daily pollers across 16 sources with per-source cron jobs, deduplication by URL, and automatic expiry of listings older than 60 days

---

## Tech I Work With

```
Frontend        Next.js · React · Tailwind · Figma
Backend         Supabase · PostgreSQL · Node.js
AI/ML           Google Gemini · Prompt Engineering · Classification Pipelines
Infrastructure  Vercel · GitHub Actions
```

---

[Portfolio](https://brodyharrison.com) · [LinkedIn](https://linkedin.com/in/brody-harrison)
