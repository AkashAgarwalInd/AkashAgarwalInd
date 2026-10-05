---
```markdown
# Hi, I'm Akash Agarwal 👋
### Senior Software Engineer | Applied AI, LLMs, RAG & Agents | Agentic AI | Production-Scale Systems (1M+ req/hr) | IIMB

I’m a Senior AI Engineer with **8+ years of software engineering experience**, building production AI/ML systems alongside high-scale distributed platforms and cloud infrastructure.

My recent work focuses on **Agentic AI, LLM orchestration, MCP, RAG, multimodal/vision-language retrieval, and AI evaluation** — with a strong emphasis on the engineering challenges that appear when AI moves from prototype to production.

I bring a systems-engineering mindset to AI:
> **latency · reliability · scalability · evaluation · observability · cost · security**

---

## 🧠 What I Work On

- **🤖 Agentic AI** — LangGraph, stateful workflows, routing, tool calling, structured outputs
- **☁️ Infrastructure** — AWS, GCP, Kubernetes, Terraform, Airflow, distributed systems
- **🔌 MCP** — MCP servers/clients, tool discovery
- **🧩 LLM Systems** — orchestration, model routing, fallbacks, context engineering
- **🔎 RAG & Retrieval** — grounded RAG, semantic search, reranking, retrieval evaluation
- **👁️ Vision-Language AI** — ColPali, patch embeddings, Qdrant multi-vector retrieval
- **🎙️ AI Audio Intelligence** — Whisper, GPT, KeyBERT, multilingual pipelines
- **📊 AI Evaluation** — RAG evaluation, agent evaluation, LLM-as-a-judge
- **🛡️ AI Safety & Guardrails** — grounding, prompt-injection defense, controlled tool execution


---

## 🚀 Production AI Work

### 🤖 Agentic Domain Analyzer
`LangGraph` · `Agentic AI` · `Tool Calling` · ` Structured Outputs` · `Context Engineering`

Built an agentic workflow for automated consent-domain analysis and intelligence workflows.

```text
                    ┌─────────────────────┐
                    │      User / API     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Agent Workflow    │
                    │     LangGraph       │
                    └──────────┬──────────┘
                               │
                 ┌─────────────┼─────────────┐
                 ▼             ▼             ▼
            Routing        Context        Tools
                 │             │             │
                 └─────────────┼─────────────┘
                               ▼
                    ┌─────────────────────┐
                    │ Structured Outputs  │
                    └──────────┬──────────┘
                               ▼
                    ┌─────────────────────┐
                    │ Backend Workflows   │
                    └─────────────────────┘

```

**Focus Areas:**

* Stateful agent orchestration
* Dynamic routing & tool calling
* Structured outputs & context management
* Controlled backend execution
* Production reliability and observability

> *The goal was not simply to build an LLM wrapper, but to design an agent workflow that can reason, select capabilities, execute controlled actions, and produce structured results.*

---

### 🔌 MCP Server + Client

`Model Context Protocol` · `Tool Discovery` · `API Integration` · `Structured Tools`

Built an MCP server/client integration for the Assessments API. The system exposes backend assessment capabilities as structured tools that an AI agent can discover and invoke.

```text
                 ┌────────────────┐
                 │    AI Agent    │
                 └───────┬────────┘
                         │
                         │ MCP
                         ▼
                ┌──────────────────┐
                │    MCP Client    │
                └────────┬─────────┘
                         │
                         ▼
                ┌──────────────────┐
                │    MCP Server    │
                │                  │
                │ Tool Discovery   │
                │ Validation       │
                │ Request Handling │
                └────────┬─────────┘
                         │
                         ▼
                ┌──────────────────┐
                │ Assessments API  │
                └──────────────────┘

```

**Engineering Focus:**

* MCP server/client integration & tool discovery
* Structured tool schemas & validation
* Backend capability exposure & controlled workflow execution
* Agent-to-system integration

> *Turning existing enterprise APIs into safely consumable capabilities for autonomous agents.*

---

### 🔎 Multimodal / Vision-Language Retrieval

`ColPali` · `Qdrant Multi-Vector Search` · `Late Interaction`

Built a vision-language semantic search platform from scratch for **300+ vendor PDF catalogs**. Instead of relying only on traditional text extraction, the system uses ColPali patch embeddings and Qdrant's multi-vector retrieval with late interaction.

```text
PDF Catalogs
     │
     ▼
┌───────────────┐
│   Documents   │
└───────┬───────┘
        │
        ▼
┌────────────────┐
│     ColPali    │
│ Patch Embedding│
└───────┬────────┘
        │
        ▼
┌────────────────┐
│     Qdrant     │
│ Multi-Vector   │
│   Retrieval    │
└───────┬────────┘
        │
        ▼
┌────────────────┐
│ Late Interaction│
│    / MaxSim    │
└───────┬────────┘
        │
        ▼
     Results

```

**Impact & Metrics:**

* **Scale:** 300+ vendor PDF catalogs
* **Speed:** Search reduced from **minutes → ~2 seconds**
* **Savings:** **500+ operational hours** saved monthly
* **Evaluation Stack:** Measured via Recall@K, MRR, nDCG, reranking effectiveness, and retrieval latency trade-offs.

---

### 🎙️ AI Audio Intelligence Pipeline

`Whisper` · `GPT` · `KeyBERT` · `Python` · `Airflow` · `S3`

Built a multilingual AI pipeline for processing high-volume sales conversations.

```text
Audio
  │
  ▼
Transcription
  │
  ▼
Translation
  │
  ├───────────────┐
  ▼               ▼
Summarization   Keywords
  │               │
  └───────┬───────┘
          ▼
       Inference
          │
          ▼
     Application

```

**Pipeline Characteristics:**

* Whisper-based transcription & multilingual translation
* GPT-powered summarization & KeyBERT keyword extraction
* Independently orchestrated processing stages persisted to S3
* Parallel downstream processing managed via Apache Airflow

---

## 🏗️ Distributed Systems Background

AI is built on top of robust systems engineering. I've designed and operated production systems handling:

* **1M+** requests/hour
* **30ms** p95 latency
* **100K+** records/day
* **99.9%+** availability
* **100+** subdomains & **60+** locales

```text
                    Global Traffic
                          │
                          ▼
                     CDN / Edge
                          │
                          ▼
                    Lambda@Edge
                          │
              ┌───────────┴───────────┐
              ▼                       ▼
          Region A                Region B
              │                       │
              └───────────┬───────────┘
                          ▼
                 DynamoDB Global Tables

```

**Core Stack:** AWS · GCP · Kubernetes · Terraform · DynamoDB · S3 · Kafka · Pub/Sub · BigQuery · MongoDB · Airflow

---

## ⚡ Engineering Impact

| Problem | Result |
| --- | --- |
| **Global Request Processing** | 1M+ requests/hour |
| **API Latency** | 30ms p95 latency |
| **Critical-Path Optimization** | ~100x faster execution |
| **Multimodal Document Search** | Search time reduced from minutes → ~2 sec |
| **Vendor Catalog Search** | Processed 300+ complex PDFs |
| **Operational Savings** | ₹2 Cr+ saved annually |
| **Audio Intelligence** | Multi-language production pipeline |
| **Infrastructure** | Multi-region / edge-routed resilience |

---

## 🛠️ Technical Stack

* **AI / LLM / Agentic AI:** `Python` · `LangGraph` · `Agentic AI` · `Multi-Agent Systems` · `Tool Calling` · `MCP` · `Structured Outputs` · `Context Engineering` · `LLM Orchestration` · `Model Routing` · `Guardrails` · `Human-in-the-Loop`
* **RAG / Multimodal AI:** `RAG` · `Multimodal RAG` · `Vision-Language Retrieval` · `ColPali` · `Qdrant` · `Multi-Vector Retrieval` · `Semantic Search` · `Reranking` · `Grounded Generation`
* **AI Evaluation & Observability:** `LangSmith` · `LLM Tracing` · `Evaluation Datasets` · `LLM-as-a-Judge` · `RAG Evaluation` · `Agent Evaluation` · `Regression Testing` · `Cost / Token Monitoring`
* **Models / ML Frameworks:** `OpenAI GPT` · `Claude` · `Gemini` · `Whisper` · `HuggingFace` · `KeyBERT` · `PyTorch` · `TorchAudio`
* **Backend & Infrastructure:** `FastAPI` · `Django REST` · `Node.js` · `TypeScript` · `Go` · `AWS` · `GCP` · `Docker` · `Kubernetes` · `Terraform` · `Lambda@Edge` · `DynamoDB` · `S3`
* **Data & Streaming:** `MySQL` · `MongoDB` · `BigQuery` · `Kafka` · `Pub/Sub` · `Airflow` · `Airbyte`

---

## 📌 Selected Work History

* **🏢 Relyance AI** — *Senior Software Engineer 2*
Agentic Domain Analyzer (LangGraph), MCP integrations, enterprise consent platforms, 1M+ req/hr, 30ms p95 latency, edge routing, event-driven Terraform infrastructure.
* **🏠 Bonito Designs / Lodha Ventures** — *Senior Software Engineer*
ColPali + Qdrant vision-language retrieval, AI audio pipelines, SketchUp 3D → 2D automation (~100x latency optimization), Flutter apps, distributed backends.
* **🏡 HomeLane** — *Software Development Engineer 3*
Monolith to microservices migration (Django REST + React), Enterprise Order Management System, Salesforce/ERP integrations, metadata-driven deployments.

---

## 🎯 What I'm Exploring Now

```text
             ┌───────────────────────┐
             │       AI Agent        │
             └───────────┬───────────┘
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
       Memory          Tools           RAG
          │              │              │
          └──────────────┼──────────────┘
                         ▼
                  Agent Runtime
                         │
              ┌──────────┼──────────┐
              ▼          ▼          ▼
          Guardrails   Eval      Observability
              │          │          │
              └──────────┼──────────┘
                         ▼
                 Production Systems

```

Focusing deeply on agentic runtime design, MCP integrations, multi-agent systems, contextual memory engines, grounded evaluation metrics, and low-latency production guardrails.

---

## 📚 Education

* **IIM Bangalore** — Executive Certificate, *New Product Development* (2023)
* **CDAC Bangalore** — PG-DAC, *Advanced Computing* (2017–2018)
* **ABESIT, Ghaziabad** — B.Tech, *Electronics & Communication* (2011–2015)

---

## 🤝 Let's Connect

I'm interested in building production-grade AI systems where software engineering meets LLMs, agents, retrieval, and scalable infrastructure.

[LinkedIn](https://www.linkedin.com/in/akash-agarwal-a9479b90) · [GitHub](https://github.com/AkashAgarwalInd) · [Email](https://www.google.com/search?q=mailto%3Aakash.66.agarwal%40gmail.com)

```

```
