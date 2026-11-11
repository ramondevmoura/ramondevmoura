# Hi, I'm Ramon Moura 👋

### Senior Software Engineer · AI Agents & LLM Products
`Python · TypeScript · Node.js · PostgreSQL · Agents · LLMs · Evals · MCP`

📍 Belo Horizonte, Brazil · 🌎 Open to remote roles (US / EU time zones)

---

Software engineer with **10+ years** of experience, the last two building **LLM features and agents that run in production**.
I take problems from the first question to production: design, code, deploy and monitoring. Most of my work is in
**Python** (LangGraph, LangChain, FastAPI), **TypeScript / Node.js** and **PostgreSQL**, and I spend a lot of my time on
what makes AI reliable: evaluation, failure handling and cost.

| 10+ years | ~1 month → ~2 days | 30,000+ events/day | ~300 users | 22/22 |
|:---:|:---:|:---:|:---:|:---:|
| in software, 2 of them with LLMs in production | to build each browser automation with DCFlow | on a multi-tenant audit platform I architected | on Imovistta, my AI SaaS | eval questions passing on the live model, in CI |

## 💼 Now

**Software Engineer, AI & Automation @ Dias Costa Advocacia** *(Sep 2026 – present)*. A law firm that handles large litigation
portfolios for banks, telecom and utility companies.
- **Legal AI:** working on a multi-stage agent pipeline that reads court decisions and returns structured JSON (outcome, deadlines,
  obligations, fees), plus the evidence and inconsistencies, so lawyers only review the uncertain cases.
- **DCFlow** (team of two): an automation platform in Python, FastAPI and Playwright. A Chrome extension records the session,
  a translation layer turns it into clear steps, and an **MCP server** lets Claude build the workflow. Building an automation
  went from about a month to about two days: **28 automations in one month**, against 30 in five years before.
- Integration with a major bank's legal system: decisions come from a PostgreSQL queue and are recorded with their documents
  through the API, checking every step (about 70 s per decision). Deployed on Google Cloud behind Cloudflare Tunnel.

## 🚀 Featured projects

**[Empório da Música — AI customer service agent](https://github.com/ramondevmoura/emporio-da-musica-agent)** · [live demo](https://emporio.mouraoncode.com)
Text and voice assistant for a music store: OpenAI function calling with 6 tools for prices, stock, promotions and orders,
store policies in plain Python, 43 unit tests and 20 evals on the real model.
`Python · OpenAI Responses API · Streamlit · SQLite · Docker`

**Supply Chain Operations Agent** · [live demo](https://agent.mouraoncode.com)
LangGraph `StateGraph` over 12 read-only tools: every number in an answer comes from SQL, never from the model. A
deterministic fallback answers when the provider fails, with caps on tool calls, run time and spending (about US$ 0.0008 per
answer). 22 eval questions, including prompt injection, pass 22/22 on the live model and run in CI with the pytest suite.
`Python · LangGraph · LangChain · Pydantic · FastAPI · pytest · AWS Lambda · GitHub Actions`

**[Imovistta](https://imovistta.com.br) — AI SaaS for property inspections** (my own product, in production)
One queued job per room: GPT-4o Vision reads the photos, Whisper transcribes the inspector's voice notes, and the result is
only saved if it passes a strict JSON schema. Every AI call is logged with tokens and cost, which feeds usage billing on Stripe.
Multi-tenant, about 300 users and 390 tests that block the deploy.
`Laravel 12 · PostgreSQL · Redis + Horizon · GPT-4o Vision · Whisper · Stripe · Docker`

**[mouraoncode.com](https://mouraoncode.com) — RAG assistant** (in production)
pgvector search over chunked documents, falls back from OpenAI to a local Ollama model when the API is down, keeps chatting
without context if embeddings fail, streams over SSE, bilingual (PT/EN).
`RAG · pgvector · OpenAI · Ollama · RabbitMQ · SSE`

## 🧭 Before

- **Senior Software Engineer @ Etus Media Holding** *(2024 – 2026)*. Architected a multi-tenant audit platform (NestJS,
  PostgreSQL, React) with **30,000+ events/day** and **258+ tests**; rebuilt its Cloudflare sync and **recovered 30,000+ lost
  events**; built **MCP servers** so Claude Code and Claude Desktop could query audit data and WordPress sites with per-user
  tokens; moved 19 sites to Cloud Run (**render 3.4 s → 0.7 s**); led a security incident response (**68 databases exposed → 1**).
- **Full Stack Developer @ Baymetrics** *(2022 – 2023)*. LGPD compliance platform with 14 micro-frontends (Vue 3, React 18),
  46+ serverless functions and row-level security over 217+ PostgreSQL tables.
- **Earlier:** GaussFleet (IoT fleet telemetry for Vale, CSN, Usiminas and Gerdau), Manyminds (SAP e-invoice automations for
  McDonald's, Accor and Ambev), Format / R2X (web development) and Contemporânea (IT).

## 🛠️ Tech stack

**AI & agents**
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat&logo=langgraph&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![OpenAI API](https://img.shields.io/badge/OpenAI_API-412991?style=flat)
![Anthropic API](https://img.shields.io/badge/Anthropic_API-191919?style=flat&logo=anthropic&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat&logo=modelcontextprotocol&logoColor=white)
![RAG](https://img.shields.io/badge/RAG_·_pgvector-336791?style=flat)
![Evals](https://img.shields.io/badge/LLM_evals_in_CI-2EA44F?style=flat)
![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=flat&logo=claude&logoColor=white)

**Backend**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat&logo=pydantic&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat&logo=nestjs&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel_12-FF2D20?style=flat&logo=laravel&logoColor=white)

**Data**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat&logo=supabase&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![ClickHouse](https://img.shields.io/badge/ClickHouse-FFCC01?style=flat&logo=clickhouse&logoColor=black)

**Frontend**
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![Vue](https://img.shields.io/badge/Vue_3-4FC08D?style=flat&logo=vuedotjs&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat&logo=tailwindcss&logoColor=white)

**Cloud & operations**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat&logo=googlecloud&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare_Workers_·_Tunnel-F38020?style=flat&logo=cloudflare&logoColor=white)
![AWS Lambda](https://img.shields.io/badge/AWS_Lambda-FF9900?style=flat)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)

## 🤖 How I build with AI

I use Claude Code every day: a short spec, then a plan, then small steps. I keep `CLAUDE.md` / `AGENTS.md` so people and
agents know the project rules, and I never trust output because it looks right — tests and real data decide. In my
products the model decides and writes; **numbers come from code and SQL**, there is always a fallback when the model fails,
and every call has a known cost.

## 📫 Connect

- 💼 [LinkedIn](https://linkedin.com/in/ramonmdev)
- 🌐 [mouraoncode.com](https://mouraoncode.com)
- ✉️ ramonmoura2012@gmail.com
