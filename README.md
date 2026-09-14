## Shubham Kale

**AI Engineer.** I build LLM systems with hard boundaries around what the model may decide, agentic RAG with published evaluations, applied ML with measured impact, and the data platforms underneath them.

Analytics Engineer at Quantegy Analytics, where I shipped an LLM-powered navigation assistant (Claude API) into a production analytics platform serving 50+ daily users, and own the Dagster-orchestrated ELT moving 4M+ records into Snowflake behind it. M.S. Data Science, Stony Brook University.

I publish the evaluation numbers, including the unflattering ones.

---

### Selected work

**[AI Auditor](https://github.com/shubham8kale/ai-auditor)** · **[live demo](https://ai-auditor-o2ym.onrender.com/)** *(repository and demo are currently access-restricted)*

An audit preparation and review workspace: five gated stages from client onboarding through invoice testing, each drafted by the system and approved by a human before the next can run. A vision LLM extracts document facts from PDFs, scans and spreadsheets through a strict JSON-schema contract and proposes judgments; deterministic Python owns materiality, sample selection, and the amount, entity and period checks, so **the model drafts but never signs off**. 16 policy-cited evidence checks, row-level security on every table, versioned approvals under row locks, and a staleness cascade on every correction. FastAPI, React/TypeScript/Vite, Supabase, one Docker service on Render, 53 tests.

**[Financial Research Agent](https://github.com/shubham8kale/financial-research-agent)** · **[live demo](https://financial-research-agent-pi.vercel.app/)**

Agentic RAG over SEC 10-K filings. A LangGraph ReAct agent discovers its tools at runtime from a FastMCP server, retrieves over ~67K ChromaDB chunks from five companies' filings, and streams source-grounded answers to a Next.js/TypeScript UI over Server-Sent Events. Two-service FastAPI + MCP backend on Docker Compose, GitHub Actions CI with 85 tests. Evaluated on a 71-item labelled RAGAS benchmark with every per-item result committed and a cross-family judge check: swapping the agent model lifted **faithfulness 0.71 to 0.88** and cut terminal failures from 12 to 6 of 66, with empty and recursion-limit answers counted as zero rather than dropped. The evaluation record also documents what the metrics cannot see, which I think is the more useful half.

**[Grid Resilience](https://github.com/shubham8kale/grid-resilience)**

Real-time anomaly detection on New York grid load. Streams ~89K hourly NYISO forecast-vs-actual records across all 11 zones through Apache Kafka (Docker, KRaft mode), with a causal rolling z-score detector on adaptive per-zone, per-hour thresholds. Scored against an offline pass over the same data at **Cohen's kappa 0.52**, reported that way on purpose: at a ~5% positive rate, accuracy is a trap.

**[Portfolio site](https://github.com/shubham8kale/portfolio)** · **[shubham8kale.vercel.app](https://shubham8kale.vercel.app)**

Next.js and TypeScript on Vercel, with a profile chatbot deliberately built without a vector database: the whole curated profile fits in the model's context, so it is prompt-stuffed through a rate-limited server-side streaming proxy instead. Every metric on the site lives in exactly one typed file.

---

### Toolkit

**Languages** Python · SQL · TypeScript · JavaScript · Java · R · Bash

**AI** LangChain · LangGraph · MCP / FastMCP · Claude API · Gemini API · Groq API · ChromaDB · RAGAS · Hugging Face · RAG · LLM agents · structured outputs · LLM evaluation · fine-tuning

**Data** Dagster · Apache Airflow · dbt · Snowflake · Redshift · Apache Kafka · PostgreSQL · BigQuery

**ML** scikit-learn · XGBoost · PyTorch · Transformers

**Platform** Docker · AWS (S3, Redshift, IAM) · Supabase · Render · GitHub Actions · FastAPI · Next.js · React · Vite · Streamlit · Pydantic · pytest

I work agent-first day to day, using Claude Code on deliverables that ship to clients and Codex under written working agreements on project builds.

---

### Elsewhere

[Portfolio](https://shubham8kale.vercel.app) · [LinkedIn](https://linkedin.com/in/shubham8kale) · [Resume](https://shubham8kale.vercel.app/ShubhamKishorKale_Resume.pdf) · [Kaggle](https://www.kaggle.com/shubham8kale)

Open to AI Engineer, Software Engineer and Data Engineer roles anywhere in the US, remote, hybrid or on-site. Reach me at **1842shubham@gmail.com**.
