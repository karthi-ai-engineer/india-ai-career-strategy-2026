[Previous](../07%20Technology%20Stack%20Demand%20Matrix/07%20Technology%20Stack%20Demand%20Matrix.md) | [Index](../INDEX.md) | [Next](../09%20Compensation%20Benchmark/09%20Compensation%20Benchmark.md)

# 8. Technology priority ranking: seven skills to master, a long tail to ignore

The ranking weighs four things: frequency in both samples, mandatory share, what interview loops test (Section 16), and the 2026–28 forecast (Section 10). It is a hiring-strategist ranking. It asks what moves a recruiter screen and an interview loop for this candidate, not what is interesting to learn. The "likely status" column is an estimate for a ~1-YOE Tokyo AI Engineer/FDE and should be self-checked.

| Rank | Technology / skill | Class | Evidence | Why it ranks here | Likely status [E] |
|---|---|---|---|---|---|
| 1 | **Python for production services** (async, typing, testing, packaging, FastAPI) | Must Master | 78% / 73% mandatory (A); most-required language in B | The universal gate, and an accepted interview language at Big Tech | Have → strengthen (async, testing) |
| 2 | **Agent engineering**: tool calling, structured outputs, state, retries, cost caps, human-in-the-loop, guardrails | Must Master | Agents 76% (A), ≥67% in every category | The core of current hiring; production-grade work is scarce | Have (basic) → strengthen |
| 3 | **RAG engineering**: chunking, embeddings, hybrid search, reranking, citations, retrieval metrics | Must Master | 63% (A); Sarvam must-have list | Most common GenAI pattern in Indian companies (InterviewBit) | Have (basic) → strengthen |
| 4 | **Evals and LLM quality engineering**: golden sets, recall@k/MRR, faithfulness, LLM-as-judge calibration, regression gates | Must Master | 63% (A); 100% of AI-startup JDs; "weed-out" interview round (Hamel Husain) | The clearest differentiator against certificate-holders | Likely partial → **acquire rigour** |
| 5 | **DSA in Python** (15–20 patterns, LeetCode medium in ~30 min) | Must Master (for interviews) | 1–3 rounds at Big Tech and Indian product companies; 32% of SDE-2 JDs | Gates the highest-paying lanes | Likely weak → **acquire** |
| 6 | **System design**: HLD + LLM system design (RAG/agent platforms, gateways, eval pipelines) + LLD machine coding | Must Master (for interviews) | 41% of SDE-2 JDs (37% required); machine coding is a knockout round at Flipkart/Swiggy/Razorpay | Required at SDE-2; the AI-flavoured version differentiates | Likely weak → **acquire** |
| 7 | **Production ownership**: Docker, CI/CD, logs/metrics/traces, incident debugging | Must Master (baseline) | Observability 47% (A) / 37% (B); FDE 67% | "Ran it in production" is a near-universal expectation | Partial → strengthen |
| 8 | **MCP server authoring** (with OAuth / governed tool access) | Strongly Recommended | 18% (A), 38% at Big Tech; mandatory at Sarvam and Wipro; Swiggy and Groww ship MCPs | The preferred skill most likely to become mandatory next | Acquire |
| 9 | **LLM observability and tracing** (Langfuse/LangSmith; OpenTelemetry concepts) | Strongly Recommended | 10% named tools; implied in eval and observability JDs | Makes eval stories credible | Acquire |
| 10 | **PostgreSQL (+ pgvector)** | Strongly Recommended | 22% / 17% required (B); 67% of India startups | One database that also does retrieval | Strengthen |
| 11 | **One cloud, deep**, incl. its managed LLM service (Bedrock, Vertex AI or Azure OpenAI) | Strongly Recommended | Cloud 51% (A), mostly "AWS/Azure/GCP" | Deployment proof; the specific vendor rarely matters | Have → deepen |
| 12 | **LangGraph** (one orchestration framework) | Strongly Recommended | 31% (A); "LangGraph, ADK, or equivalent" | Portfolio legibility; services firms screen by name | Acquire or strengthen |
| 13 | **AI coding-agent workflow** (Claude Code / Cursor / Copilot, plus review discipline) | Strongly Recommended | 32% of SDE-2 JDs (22% required); Adobe, Seekho, Whatfix must-haves | Now tested directly at some employers | Likely have → document it |
| 14 | **TypeScript** (working level: MCP servers, agent UIs, Next.js demos) | Strongly Recommended | 33% (A), driven by FDE and early-stage roles | FDE demo speed; full-stack AI products | Partial |
| 15 | **Customer discovery and communication** | Strongly Recommended (FDE) | 73% of FDE JDs; customer-simulation rounds | The FDE gate; Japan client work is the asset | Have → package it |
| 16 | Redis; queues and async jobs; idempotency/retries; SSE/WebSocket streaming | Important Supporting | B: Redis 20%; Sarvam/Seekho language | Distributed-systems literacy for AI platforms | Acquire |
| 17 | Kubernetes (deploy, debug, autoscale, not internals) | Important Supporting | 41% (B), 20% (A) | Startup and services checklists | Acquire (basic) |
| 18 | LLM cost and latency economics (gateways, caching, routing, token budgets) | Important Supporting | Razorpay: "token economics"; LLM cost metrics 10% (A) | Senior signal; also an FDE selling point | Acquire |
| 19 | React (working level) | Important Supporting | 12% (B) | Unlocks full-stack AI-product roles | Optional |
| 20 | Fine-tuning / post-training (LoRA, SFT, DPO) | Specialized-Niche | 24% (A), concentrated in enterprise ML and AI startups | Understand conceptually; one small experiment at most | Conceptual |
| 21 | Voice stack (LiveKit/Pipecat, ASR/TTS, latency) | Specialized-Niche | 14% (A); 4 of 7 ≥₹48L-cap startup JDs | High-paying niche if a voice employer is targeted | Optional specialisation |
| 22 | Inference serving (vLLM, TensorRT, Triton, quantisation, KV cache) | Specialized-Niche | 2–6% (A), NVIDIA/inference startups | Only for an AI-infra pivot | Conceptual |
| 23 | Google ADK / Vertex specifics | Specialized-Niche | 16% (A), Google and Wipro | Only if Google Cloud FDE is the dream target | Optional |
| 24 | Go | Specialized-Niche | 34% (B), platform/infra; Sarvam gateway rewrite | Third language only for a platform track | Deprioritize |
| 25 | Java + Spring Boot | Specialized-Niche | 61% (B), Big Tech/enterprise | Only for a pure SDE-2 switch | Deprioritize |
| 26 | Kafka, Terraform, Temporal, Spark/Airflow, PyTorch/HF | Specialized-Niche | ≤22%, mostly preferred | Know what they are and when to use them | Conceptual |
| 27 | CrewAI, AutoGen, Semantic Kernel, DSPy, A2A, LlamaIndex | Low Priority | Preferred-only, 2–18% | Framework collecting reads as keyword-stuffing | Skip |
| 28 | Multiple vector DB products; multiple clouds | Low Priority | Qdrant 0; Pinecone 2; pgvector 3 mentions | One of each is enough | Skip |
| 29 | C++, Rust, Scala, Kotlin, CUDA | Low Priority | ≤8% (A), role-specific | No payoff for this lane | Skip |
| 30 | Classical ML theory / Kaggle; standalone "prompt engineering"; GenAI certificates | Low Priority | Classic ML whiteboarding "largely dropped" for LLM roles (techinterview.org, Jul 2026); prompt-engineer titles absorbed | Commoditised (Section 10) | Skip |

---
[Previous](../07%20Technology%20Stack%20Demand%20Matrix/07%20Technology%20Stack%20Demand%20Matrix.md) | [Index](../INDEX.md) | [Next](../09%20Compensation%20Benchmark/09%20Compensation%20Benchmark.md)
