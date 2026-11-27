[Previous](../12%20Recommended%20Career%20Direction/12%20Recommended%20Career%20Direction.md) | [Index](../INDEX.md) | [Next](../14%20Company%20Target%20List/14%20Company%20Target%20List.md)

# 13. Primary technology stack: Python-first production LLM systems, nothing more

The stack below is deliberately narrow. Every element is either a hard requirement that appears across categories in Section 6, or a tool that produces proof of one. A recruiter reading the resume should see **one coherent system**, not a keyword inventory. The evidence supports this. Product companies accept framework equivalents, and named tools mostly sit under "preferred" (Section 6.3). Interview loops dig into one project, testing evaluation, trade-offs and outcomes ([eugeneyan.com, Jul 2024](https://eugeneyan.com/writing/how-to-interview/)).

| Depth | Technology | Why (evidence) | Proof artifact |
|---|---|---|---|
| **Master deeply** | **Python** (asyncio, FastAPI, pydantic, pytest, packaging) | 78% of AI JDs, 73% mandatory; also the interview language | All three portfolio projects |
| Master deeply | **LLM application core**: provider APIs behind one abstraction (Anthropic / OpenAI / Gemini), tool calling, structured outputs, streaming | Multi-provider lists at Infosys and Whatfix; structured outputs mandatory whenever named | Project 2 gateway |
| Master deeply | **Agents with LangGraph**: state graphs, retries, budget/step caps, human-in-the-loop, guardrails | Agents 76%; LangGraph is the most-named product framework | Project 2 |
| Master deeply | **RAG on PostgreSQL + pgvector**: hybrid (BM25 + vector) search, reranking, citations, structure-aware chunking | RAG 63%; Sarvam and workwise must-haves; Postgres 67% of India startup SDE JDs | Project 1 |
| Master deeply | **Eval and quality engineering**: golden sets, recall@k / MRR / nDCG, faithfulness, LLM-as-judge calibrated to human labels, CI regression gates; **tracing** with Langfuse (or LangSmith) | Evals 63% (100% at AI startups); the take-home format | Projects 1–3 |
| Master deeply | **DSA in Python** and **system design** (HLD, LLD machine coding, LLM system design) | Interview gates (Section 16) | Mock-interview log |
| **Intermediate** | **TypeScript** (MCP servers, a small Next.js/React demo UI) | 33% of AI JDs; FDE demo speed | Project 2 UI and MCP server |
| Intermediate | **MCP** server authoring with OAuth and scoped tools | 18% (38% at Big Tech); mandatory at Sarvam/Wipro; Swiggy, Groww and Cisco build MCP servers | Project 2 |
| Intermediate | **Docker + GitHub Actions CI/CD**; **one cloud** (deploy, IAM, secrets, its managed LLM service) | Cloud 51%, usually "AWS/Azure/GCP"; CI/CD 29–41% | All projects deployed |
| Intermediate | **Redis**, background jobs/queues, idempotent retries, SSE streaming | Sarvam/Seekho/Transak language; Redis 20% of SDE JDs | Project 3 |
| Intermediate | **Kubernetes** at deploy/debug level | 41% of SDE JDs, mostly preferred | Project 3 deployment |
| Intermediate | **LLM cost/latency engineering** (caching, routing, token budgets; LiteLLM/Portkey pattern) | Razorpay "token economics"; LLM cost metrics in Big Tech FDE JDs | Project 3 |
| Intermediate | **Coding-agent workflow** (Claude Code / Cursor) with review discipline | 32% of SDE JDs; tested directly at Seekho | Documented workflow in each repo |
| **Understand conceptually** | Fine-tuning (LoRA/SFT/DPO; when to fine-tune vs retrieve vs prompt) | 24% of AI JDs, concentrated in ML-heavy employers | Interview answers |
| Understand conceptually | Inference serving (vLLM, batching, KV cache, quantisation, tokens/sec) | Senior Big Tech FDE / NVIDIA JDs; "inference batching for a single GPU" design prompt | Interview answers |
| Understand conceptually | Kafka/event-driven design, Terraform/IaC, Go and Java at reading level | Preferred in SDE JDs; Google FDE GECX uses Terraform | Interview answers |
| Understand conceptually | Voice pipelines, multimodal/document AI, AI security (prompt injection, PII, governed tool access), A2A | Niche or emerging | Interview answers |
| **Safely deprioritise** | CrewAI, AutoGen, Semantic Kernel, DSPy, LlamaIndex; second and third vector DBs; second cloud; C++/Rust/Scala/Kotlin/CUDA; Spark/Airflow; Spring Boot; Kaggle; GenAI certificates | Preferred-only or role-specific (Section 8) | — |

**Cloud rule [E].** Choose the cloud already used in production at the Tokyo employer, because production evidence beats tutorial depth. Most JDs accept "AWS, Azure or GCP". If there is a free choice, AWS gives the broadest reach: it is the most-named cloud in SDE-2 JDs (32%), and the AWS-heavy Amazon pages were not even sampled. Switch to GCP (Vertex AI + ADK) only if Google Cloud FDE becomes the single dream target.

**Resume skills line (illustrative).** Use one line, with no more than eight groups: *Python (FastAPI, asyncio) · TypeScript · LLM agents (LangGraph, MCP, tool calling) · RAG (Postgres/pgvector, hybrid search, reranking) · Evals & observability (golden sets, LLM-as-judge, Langfuse) · AWS · Docker, CI/CD · Kubernetes (basic).*

## Skills inventory: have, strengthen, acquire

This inventory is an estimate for a ~1-YOE Tokyo AI Engineer/FDE and should be self-audited against current work.

| Area | Likely already has [E] | Should strengthen | Must acquire |
|---|---|---|---|
| Python | Daily scripting and services | Async, typing, tests, packaging, profiling | — |
| LLM apps | API integration, prompting, basic RAG, a demo agent | Production agent patterns: state, retries, caps, guardrails, structured outputs | Multi-provider gateway design, cost engineering |
| Retrieval | Vector search via a framework | Hybrid search, reranking, chunking experiments | Retrieval metrics on a labelled set |
| Evals | Manual spot-checks, some prompt comparison | Golden-set discipline | LLM-as-judge calibration, regression gates in CI, a written eval methodology |
| Customer / FDE | Requirements gathering, demos, stakeholder communication with Japanese enterprise clients | Structured discovery write-ups, quantified business impact | Decomposition-interview fluency (vague prompt → schema/API/plan in 45 min) |
| Production | Some deployment, logs | Tracing, dashboards, incident write-ups | Kubernetes basics, CI/CD pipelines owned end to end |
| Data layer | SQL basics | Postgres schema/indexing, pgvector | Redis caching and rate limiting |
| Fundamentals | Practical coding | — | **DSA to the LeetCode-medium/30-min standard; LLD machine coding; HLD** |
| Tooling | Copilot/Cursor/Claude Code use | Documented workflows and review practice | MCP server authoring with auth |
| Positioning | Japan experience | Framing it as an asset (Section 15) | Network of India referrers |

---
[Previous](../12%20Recommended%20Career%20Direction/12%20Recommended%20Career%20Direction.md) | [Index](../INDEX.md) | [Next](../14%20Company%20Target%20List/14%20Company%20Target%20List.md)
