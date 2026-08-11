## Shubham Kale

**AI Engineer.** I build agentic LLM systems, applied ML with measured impact, and the data
platforms underneath them.

Analytics Engineer at Quantegy Analytics, where I shipped an LLM-powered navigation assistant
(Claude API) into a production analytics platform serving 50+ daily users, and own the
Dagster-orchestrated ELT moving 4M+ records into Snowflake behind it. M.S. Data Science,
Stony Brook University.

I publish the evaluation numbers, including the unflattering ones.

---

### Selected work

**[Financial Research Agent](https://github.com/shubham8kale/financial-research-agent)** ·
**[live demo](https://financial-research-agent-pi.vercel.app/)**

Agentic RAG over SEC 10-K filings. A LangGraph ReAct agent discovers its tools at runtime from a
FastMCP server, retrieves over ~67K ChromaDB chunks from five companies' filings, and streams
source-grounded answers to a Next.js/TypeScript UI over Server-Sent Events. Two-service
FastAPI + MCP backend on Docker Compose, GitHub Actions CI. Evaluated with a RAGAS harness using a
separate judge model: **0.80 faithfulness, 0.80 context recall.**

**[Grid Resilience](https://github.com/shubham8kale/grid-resilience)**

Real-time anomaly detection on New York grid load. Streams ~89K hourly NYISO forecast-vs-actual
records across all 11 zones through Apache Kafka (Docker, KRaft mode), with a causal rolling
z-score detector on adaptive per-zone, per-hour thresholds. Scored against an offline pass over the
same data at **Cohen's kappa 0.52**, reported that way on purpose: at a ~5% positive rate,
accuracy is a trap.

**[Portfolio site](https://github.com/shubham8kale/portfolio)** ·
**[shubham8kale.vercel.app](https://shubham8kale.vercel.app)**

Next.js and TypeScript on Vercel, with a profile chatbot deliberately built without a vector
database: the whole curated profile fits in the model's context, so it is prompt-stuffed through a
rate-limited server-side streaming proxy instead. Every metric on the site lives in exactly one
typed file.

---

### Toolkit

**Languages** Python · SQL · TypeScript · JavaScript · Java · R · Bash

**AI** LangChain · LangGraph · MCP / FastMCP · Claude API · Gemini API · ChromaDB · RAGAS ·
Hugging Face · RAG · LLM agents · fine-tuning

**Data** Dagster · Apache Airflow · dbt · Snowflake · Redshift · Apache Kafka · PostgreSQL ·
BigQuery

**ML** scikit-learn · XGBoost · PyTorch · Transformers

**Platform** Docker · AWS (S3, Redshift, IAM) · GitHub Actions · FastAPI · Next.js · Streamlit ·
Pydantic · pytest

I work agent-first day to day, using Claude Code on deliverables that ship to clients.

---

### Elsewhere

[Portfolio](https://shubham8kale.vercel.app) ·
[LinkedIn](https://linkedin.com/in/shubham8kale) ·
[Resume](https://shubham8kale.vercel.app/ShubhamKishorKale_Resume.pdf) ·
[Kaggle](https://www.kaggle.com/shubham8kale)

Open to AI Engineer, Machine Learning Engineer, Data Engineer and Software Engineer roles anywhere
in the US, remote, hybrid or on-site. Reach me at **1842shubham@gmail.com**.
