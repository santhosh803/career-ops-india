# Article Digest -- Proof Points

Compact proof points from portfolio projects. Read by career-ops at evaluation time.

---

## Smart Safety Sentinel -- AI Workplace Safety Platform

**Hero metrics:** About 67% CPU/GPU load reduction through frame skipping, 640px inference resizing, and daemon-threaded async API calls; real-time violation event persistence with timestamp, type, image, and AI report.

**Architecture:** Streamlit frontend -> YOLOv8 and OpenCV video inference -> violation snapshot capture -> Gemini Vision-Language Model incident report generation -> SQLite audit trail -> LangChain and ChromaDB RAG over OSHA PDFs -> LangChain SQL Agent over SQLite evidence data.

**Key decisions:**
- Used YOLOv8 and OpenCV for real-time PPE violation detection.
- Added inference resizing and frame skipping to keep video usable under constrained compute.
- Used Gemini VLM to turn violation snapshots into OSHA-style incident reports.
- Built a RAG assistant over OSHA compliance documents and constrained it to refuse out-of-context answers.
- Added schema-locked SQL agent guardrails to reduce SQL injection and path leakage risks.

**Proof points:**
- Demonstrates computer vision, multimodal AI, RAG, SQL agents, and public-facing AI tool delivery in one system.
- Shows ability to combine live inference, business reporting, compliance Q&A, and auditability.
- Useful for workplace safety, manufacturing AI, compliance automation, and enterprise AI roles.

---

## ERP AI Procurement Assistant

**Hero metrics:** End-to-end Dockerized RAG application deployed on Hugging Face Spaces for enterprise procurement document lookup.

**Architecture:** Procurement SOP/document corpus -> semantic chunking -> embeddings -> FAISS vector index -> LangChain retrieval pipeline -> Qwen2.5-7B grounded responses -> Dockerized app -> Hugging Face Spaces deployment.

**Key decisions:**
- Focused on procurement SOP lookup because ERP users need accurate process answers, not generic chatbot responses.
- Used semantic chunking and vector search to retrieve relevant ERP context before generation.
- Containerized the application to prove deployability beyond a local demo.

**Proof points:**
- Bridges AI engineering with real ERP implementation experience.
- Strong fit for enterprise AI, procurement copilots, SAP/ERP automation, and workflow AI roles.
- Shows practical understanding of how business users adopt AI tools in production.

---

## AI SQL Data Analyst

**Hero metrics:** Mock ERP database with 300+ sales, vendor, and inventory records; real-time SQL execution logs and CSV export through Streamlit.

**Architecture:** Natural-language question -> LangChain ReAct agent -> Ollama qwen2.5-coder:1.5b local inference -> SQL tool call -> SQLite ERP-style database -> execution logs -> Streamlit UI -> CSV export.

**Key decisions:**
- Used ReAct to make tool use and reasoning steps visible.
- Built a mock ERP database with Faker to test realistic business questions.
- Added execution logs so users can inspect what SQL was generated before using results.

**Proof points:**
- Demonstrates agentic AI, tool use, local LLM inference, SQL reasoning, and enterprise analytics workflows.
- Strong fit for AI analyst tools, enterprise copilots, internal tools, and public-facing AI products.
- Shows ability to convert business questions into safe, structured data workflows.

---

## Business Insights 360

**Hero metrics:** Global hardware sales analytics driving a projected 10% revenue acceleration.

**Architecture:** MySQL database -> Power BI dimensional data model -> DAX measures -> dynamic multi-department dashboards (Finance, Sales, Marketing, Supply Chain, Executive).

**Key decisions:**
- Designed a star schema to optimize query performance and reporting speed across millions of transactions.
- Developed DAX metrics to track critical SaaS-like KPIs (gross margin, net sales, forecast accuracy).

**Proof points:**
- Shows strong capabilities in data modeling, business intelligence, and translating raw data into strategic executive dashboards.

---

## Adhoc Insights Analysis in Consumer Goods

**Hero metrics:** Solved 10+ complex business requests slicing FY2020 & FY2021 transactional records.

**Architecture:** MySQL database -> SQL scripting (CTEs, window functions, subqueries, group by aggregates) -> CSV data extraction.

**Key decisions:**
- Structured clean, modular SQL queries to answer high-priority ad-hoc business questions regarding sales volume and margin growth by customer segment.

**Proof points:**
- Demonstrates robust SQL competency, database schema understanding, and capability to build data sources for AI agents (e.g., SQL-speaking bots).

---

## IPL Analysis (2021-2023) & AtliQ Mart FMCG Promotion Analysis

**Hero metrics:** Multi-dimensional Power BI visualizations for sports performance and retail campaign ROI.

**Architecture:** CSV / Excel transaction databases -> Power BI data transformation & visualization dashboards.

**Key decisions:**
- Designed tailored visualization layouts mapping specific domain KPIs (sports stats, promotional incremental sales vs discount costs).

**Proof points:**
- Shows versatile domain data analysis capabilities, visual storytelling, and dashboard usability.
