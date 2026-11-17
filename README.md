# Hi, I'm Justin Yurasits

I'm a product leader and hands-on AI systems builder. Twelve-plus years leading enterprise software across SaaS, developer platforms, financial services, and conversational systems — and, since 2024, building AI applications myself with the Claude API, Claude Code, MCP/tool integrations, retrieval, and Postgres.

I'm also a licensed Massachusetts Construction Supervisor who ran $1M–$4M renovations. That's why most of what I build points at construction: I know what the work looks like when the software isn't there.

---

## What I've built

**Fieldscope** — [live demo](https://fieldscope-vm64.onrender.com/) · [source](https://github.com/justinyurasits/fieldscope)

login `fieldscope` / `safety` · free instance, so the first load can take up to a minute while the server wakes

Subcontractor safety compliance for general contractors. Generates OSHA-grounded protocols for specific tasks, tracks training and review cadence, and checks daily site photos against each protocol's PPE requirements using Claude Vision.

One design decision matters more than the rest: an AI-generated safety protocol is a draft, not a record, until a named person approves it. Safety documentation carries legal weight, and a model shouldn't be the last signature on it.

Built with Express, Postgres, Claude API, and Claude Vision.

This is intentionally pilot-scope. The repo documents its own limits, including no application-level user authentication, free-text approver identity, single-tenant architecture, and a deliberately narrow OSHA library. On a prototype, those gaps are more informative than pretending the demo is production-ready.

---

**Change Order Generator** — [try it](https://draftconstructionchangeorder.com/) · [source](https://github.com/justinyurasits/pco-generator)

Turns field notes and scope descriptions into a drafted construction change order using the contract references, scope language, and structure a general contractor actually works from.

The goal is not to automate approval or judgment. It's to turn messy field information into a structured first draft faster, while leaving the project manager in control of the final document.

---

**Construction OS** — [design docs](https://github.com/justinyurasits/design/tree/main/construction-os) · [source](https://github.com/justinyurasits/construction-os-workbench)

The larger construction-AI system behind this work: governed knowledge, document generation, and operational workflows.

Current work includes a 173-document corpus under version control and governance — permanent IDs, policy separated from procedure, configuration at the rule level — with a retrieval architecture designed on top of it.

The evaluation set was written before any retrieval code, and writing it exposed the real problem: the documents contradicted each other, and no amount of retrieval quality would have fixed that.

That changed the order of operations. Corpus quality, authority, and governance had to come before indexing and retrieval.

---

## How I approach AI products

**Evaluate before you optimize.**
Define what a correct answer looks like before tuning prompts, retrieval, or models.

**Treat the corpus as part of the system.**
Retrieval quality cannot compensate for contradictory, incomplete, or ungoverned source material.

**Use AI for judgment, and deterministic systems where certainty matters.**
Let models interpret ambiguous language and context; keep permissions, approvals, calculations, and hard business rules deterministic wherever possible.

**Design the failure path.**
A good AI product knows when to answer, when to clarify, when to reach for a tool, and when to hand the problem to a person.

**Measure the hard cases, not the average.**
Ambiguous requests, missing information, multi-intent inputs, and questions the system cannot answer often tell you more than the headline score.

---

## Earlier product work

- **Citizens** — owned roadmap, strategy, and delivery for the conversational-AI and intent-routing workstream of a major U.S. bank's phone-channel transformation. Reduced a 259-intent legacy catalog to 22 resolution paths after testing rejected an earlier 10-intent design, and launched the first capabilities to real retail customers.
- **Optimizely** — owned GenAI strategy across 10+ SaaS product lines and the internal model garden that gave engineering teams foundation-model access without each building its own integration. Established model evaluation on cost, quality, and response time as a product practice.
- **Optimizely Connect** — took a serverless developer platform from pilot to production: APIs, SDKs, an app marketplace where the number of apps in daily use grew from 3 to 35 in three months, outside companies building on it, and most of the original v1 developer documentation, whose core remains substantially intact today.
- **Jabra** — zero-to-one product development across software and hardware for a $250M ARR portfolio, including two headset lines taken from market analysis through manufacturing and launch.
- **Fidelity Investments** — led digital onboarding and self-service for 25M+ retail customers and later ran contact-center platform operations at scale.

---

## Tools

`Claude API` · `Claude Code` · `Claude Vision` · `MCP/tool integrations` · `Postgres` · `n8n` · `Supabase` · `Vercel` · `retrieval` · `structured outputs` · `Git/GitHub`

I use AI-assisted coding heavily. My strength isn't pretending to be a traditional software engineer — it's moving from user problem → system design → working prototype → evaluation → product decision without handing every intermediate step to someone else.

---

## Background

MBA, Babson College  
BS Chemical Engineering, Georgia Institute of Technology  
Massachusetts Construction Supervisor License  
Greater Boston, Massachusetts

[LinkedIn](https://www.linkedin.com/in/justinjyurasits)
