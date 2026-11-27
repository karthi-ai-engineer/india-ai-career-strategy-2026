# JD Skill-Frequency Analysis: AI / GenAI / LLM / Applied AI / ML / MLOps / AI-Infra and Forward-Deployed / Solutions Engineer roles in India (observed 2026-11-27)

## Sample composition, method and biases

### Takeaway
I coded 49 real India-located JDs, all viewed on 2026-11-27: 8 full JDs from the Indeed connector and 41 from company career pages, YC/Wellfound, VC job boards, Cutshort, Bayt and Built In. They cover Big Tech (16), enterprise SaaS / global product / GCC (7), Indian product companies (5), funded AI-native startups (5), early-stage startups (9) and IT services (7). 31 of the 49 were still listed or open when I looked; 18 had already closed. Most closed ones were posted in 2026. Read every percentage as a directional signal from a small, non-random sample, not a market estimate.

### Cited Findings
- **Sources.** 8 full JDs came from the Indeed connector (`get_job_details`). All 8 were open and posted between 2026-10-14 and 2026-11-24 (J1–J8 in the Appendix). Examples: [Google GenAI FDE](https://to.indeed.com/aah9w6f7xm9p), [Whatfix FDE-AI](https://to.indeed.com/aazjxf46s9zc), [Cisco AI Engineer](https://to.indeed.com/aabtcp7sghz9).
- **Why only 8 from Indeed.** After 14 successful connector calls, the Indeed connector returned "Rate limit exceeded for account … on toolset claude" on every later attempt for about 45 minutes, even after waits of 3, 5 and 10 minutes. That blocked the full-JD fetch for ~25 more Indeed listings I had shortlisted. These included Sarvam Platform Engineer – AI Infrastructure, Smartsheet Senior AI/ML Ops, TransUnion Lead AI Platform, Cerebras ML Systems Performance, Infosys, Capgemini, CGI, EPAM, Deloitte, BCG, Optum, Barclays, GE HealthCare and AT&T FDE. The rest of the sample therefore comes from the web (Indeed connector tool output, observed 2026-11-27).
- **Indeed's search mix skews to services and GCC employers.** Across 9 relevant Indeed searches (Bengaluru, Hyderabad, Pune, Gurugram/NCR, Chennai, India-wide), the 90 listing slots I classified break down as:

  | Employer type | Slots | Share |
  |---|---|---|
  | IT services / consulting (EPAM, HCLTech, Deloitte ×6, Capgemini, CGI, BCG ×4, Bain, Infosys ×2, Wipro, L&T Tech, Prodapt, Tarento, Calpion, EXL, Agilisium, Relevance Lab and others) | 30 | 33% |
  | Non-tech enterprise or SaaS GCCs (TE Connectivity, TransUnion, Boeing, Wells Fargo, Barclays, Optum, GE, DHL, Smartsheet, Dolby, Equinix and others) | 29 | 32% |
  | Big Tech (Google/YouTube, Apple, Cisco) | 11 | 12% |
  | Small or unknown firms | 15 | 17% |
  | AI startups (Cerebras, Sarvam, Aion) | 3 | 3% |
  | Indian product (Whatfix) | 1 | 1% |
  | Other product (Poshmark) | 1 | 1% |

  Titles such as "Solutions Engineer AI" and "Customer Engineer AI" mostly returned unrelated manufacturing or sales roles (Indeed search_jobs output, observed 2026-11-27).
- **Indeed shows no pay.** All 90 Indeed listing slots showed "Compensation: N/A" (Indeed search_jobs output, observed 2026-11-27).
- **Services firms are kept separate.** All 7 services JDs are tagged SVC: [Wipro Agentic AI Engineer](https://careers.wipro.com/job/Agentic-AI-Engineer/207412-en_US/), [Wipro GenAI Engineer](https://careers.wipro.com/job/Generative-AI-Engineer/187523-en_US/), [Wipro Gen AI Engineer Lead/FDE](https://careers.wipro.com/job/Gen-AI-Engineer-Lead/198667-en_US/), Infosys ×2 ([1](https://www.bayt.com/ar/india/jobs/genai-agentic-ai-engineer-75181647/), [2](https://www.bayt.com/en/india/jobs/gen-ai-llm-engineer-75383098/)), and Ampera and VY Systems (via [Cutshort](https://cutshort.io/job/AI-ML-Engineer-Bengaluru-Bangalore-CombineHealth-ln9ygN40)). The product-company subset is 42 JDs.
- **Role mix.** AI/GenAI/LLM engineer 28, FDE/solutions/customer-facing 15, AI infra/inference 3, MLOps 1, classic MLE 2.
- **Stated minimum YOE.** 36 of the 45 JDs that state one (80%) set it between 2 and 5 years.
- **Coding rules.**
  - Each JD was coded into canonical tags as M (minimum/required), P (preferred / nice-to-have / bonus) or R (named only in responsibilities or the description).
  - "Any mention" means M ∪ P ∪ R.
  - When a JD lists alternatives (e.g. "LangChain/LangGraph, Amazon Bedrock, or OpenAI/Anthropic SDKs" in [Cisco AI Engineer](https://to.indeed.com/aabtcp7sghz9)), each named alternative is counted.
  - "AWS, Azure or GCP" with no preference is coded as generic cloud.
  - A single coder (me) did all the coding, with no second-rater check.

### Inferences
- **Remaining source biases.**
  - **Over-represented:** Google (8 JDs), Bengaluru (≈80% of JDs) and YC/VC-board startups. This reflects which pages could be fetched.
  - **Under-represented:** TCS, Accenture, HCLTech, Deloitte and Capgemini at the JD level, Flipkart, Swiggy, Microsoft, Salesforce and Amazon, and Mumbai/Chennai/NCR.
  - **The services gap.** Indeed is services- and GCC-heavy (≈65% of slots), yet the coded sample has only 7 services JDs (14%). The headline percentages therefore describe product companies more than the overall Indian JD market.
- **Closed postings.** 18 of 49 JDs had closed by the observation date (most were posted Jun–Sep 2026). On the 31 JDs that were still live, the headline rates barely move: Python 77%, agents 74%, RAG 68%, evals 65%. The skill mix looks stable over 2026.

### Gaps
- No full-JD coverage for TCS, Accenture, HCLTech, Deloitte, Capgemini, EPAM or CGI. Capgemini pages said "position filled", and the Indeed details were rate-limited.
- No full-JD coverage for Flipkart, Swiggy or Amazon. Aggregator pages (foundit, nodeflair) returned 403. Search snippets mentioned RAG, LangChain, CrewAI, LangGraph, AutoGen, Kafka and MCP, but I did not view those JDs, so they are excluded.
- Atlassian and Microsoft current career pages were JS-rendered or blocked.
- Per-category n is small (5–16), so a single JD moves a category percentage by 6–20 points.

## 1. Programming languages

### Takeaway
Python is close to universal: 78% of all JDs and 73% as a hard requirement. TypeScript/JavaScript is second at 33%, driven by FDE, full-stack and early-stage roles. Java, Go and C++ show up mainly at Big Tech (Cisco, NVIDIA, Google) and Walmart.

### Cited Findings
Frequencies by language (computed over the 49 JDs in the Appendix):

| Language | Any mention (N=49) | Mandatory | Big Tech (n=16) | Enterprise/GCC (7) | Indian product (5) | AI startup (5) | Early-stage (9) | Services (7) |
|---|---|---|---|---|---|---|---|---|
| Python | 38 (78%) | 36 (73%) | 75% | 71% | 80% | 100% | 56% | 100% |
| TypeScript/JS | 16 (33%) | 11 (22%) | 25% | 43% | 40% | 20% | 44% | 29% |
| SQL | 11 (22%) | 9 (18%) | 38% | 0% | 0% | 0% | 33% | 29% |
| Java | 8 (16%) | 5 (10%) | 31% | 29% | 0% | 0% | 11% | 0% |
| Go | 8 (16%) | 6 (12%) | 25% | 0% | 40% | 0% | 22% | 0% |
| C++ | 4 (8%) | 4 (8%) | 25% | 0% | 0% | 0% | 0% | 0% |
| Rust / C# | 1 each | – | 6% | – | – | – | – | – |

- **Java with Python.** [Cisco SWE (AI & Full-Stack)](https://to.indeed.com/aazyf74jdrxb) requires "Strong programming skills in Java (Spring Boot, OOP) and Python".
- **C++ for inference runtimes.** [NVIDIA Local AI](https://jobs.anitab.org/companies/nvidia/jobs/87547967-senior-system-software-engineer-local-ai) requires "Excellent C++ programming and debugging skills".
- **Go or Python for LLM gateways.** [Razorpay Lead AI Engineer](https://builtin.com/job/lead-ai-engineer/8974755) asks for "Strong in Go or Python" for its LLM gateway.
- **TypeScript-first startups.** Several early-stage JDs lead with TypeScript:
  - [Tsenta](https://www.ycombinator.com/companies/tsenta/jobs/hYAeFGp-founding-engineer): "Strong TypeScript and real backend depth".
  - Craft My Plate: TypeScript plus AWS serverless ([Cutshort](https://cutshort.io/job/AI-ML-Engineer-Bengaluru-Bangalore-CombineHealth-ln9ygN40)).
- **Async Python.** [Vahan](https://www.ycombinator.com/companies/vahan/jobs/7zvIddz-lead-ai-engineer) asks for "Strong async Python — you write services, not notebooks".

### Inferences
- Python plus one production backend language is the safe target: TypeScript for FDE and startup roles, Java or Go for Big Tech and GCC platform teams.
- C++ matters only for inference and runtime roles.

### Gaps
- Too few infra and MLOps JDs (4) to rate CUDA, C++ or Rust demand reliably.

## 2. Frameworks (LangChain, LangGraph, LlamaIndex, CrewAI, AutoGen, Semantic Kernel, OpenAI Agents SDK, ADK, DSPy, FastAPI, ML stacks)

### Takeaway
About half the JDs (53%) name at least one LLM orchestration framework. Few make a specific framework a hard requirement: LangChain is mandatory in 22% and LangGraph in 16%. Product companies usually write "LangGraph, ADK, or equivalent". Services firms are the exception: 71% of their JDs name LangChain and LangGraph explicitly, which is closer to keyword-matching. CrewAI and AutoGen appear only as preferred. I found no explicit "OpenAI Agents SDK" requirement.

### Cited Findings
Frequencies by framework (computed over the 49 JDs in the Appendix):

| Framework | Any (N=49) | Mandatory | Preferred-only | Big Tech | Enterprise | Indian product | AI startup | Early | Services |
|---|---|---|---|---|---|---|---|---|---|
| Any LLM framework | 26 (53%) | 14 (29%) | 10 (20%) | 50% | 57% | 40% | 60% | 33% | 86% |
| LangChain | 18 (37%) | 11 (22%) | 6 (12%) | 31% | 43% | 40% | 40% | 11% | 71% |
| LangGraph | 15 (31%) | 8 (16%) | 6 (12%) | 38% | 14% | 0% | 20% | 22% | 71% |
| LlamaIndex | 9 (18%) | 5 | 3 | 12% | 14% | 20% | 40% | 11% | 29% |
| Google ADK | 8 (16%) | 5 | 3 | 25% | 0% | 0% | 20% | 0% | 43% |
| CrewAI | 5 (10%) | 0 | 5 | 19% | 0% | 20% | 0% | 11% | 0% |
| AutoGen | 3 (6%) | 1 | 2 | 12% | 0% | 20% | 0% | 0% | 0% |
| Semantic Kernel | 2 (4%) | 1 | 1 | 6% | – | – | – | – | 14% |
| DSPy | 2 (4%) | 1 | 0 | – | 14% | – | – | 11% | – |
| OpenAI/Anthropic SDKs | 1 (2%) | 1 | 0 | 6% | – | – | – | – | – |
| FastAPI | 4 (8%) | 4 | 0 | 0% | 0% | 20% | 0% | 11% | 29% |
| PyTorch | 8 (16%) | 7 | 0 | 12% | 43% | 0% | 20% | 11% | 14% |
| Hugging Face | 5 (10%) | 4 | 1 | 0% | 43% | 0% | 20% | 11% | 0% |

- **Product companies accept equivalents.** [Sarvam Applied AI Engineer](https://jobs.khoslaventures.com/companies/sarvam-ai-2/jobs/80711937-applied-ai-engineer-sarvam-agents) asks for "Agentic framework experience: LangGraph, ADK, or equivalent".
- **The multi-agent trio is preferred-only at Google.** [Google GenAI FDE](https://to.indeed.com/aah9w6f7xm9p) lists LangGraph, CrewAI and ADK as preferred: "Experience implementing multi-agent systems using frameworks (e.g., LangGraph, CrewAI, ADK)".
- **ADK is a hard requirement at Google's onboarding team.** [Google Cloud AI Engineer (Technical Onboarding Center)](https://jobs.anitab.org/companies/google-24698/jobs/93056314-cloud-ai-engineer-technical-onboarding-center) requires "Experience building and orchestrating agents using ADKs, LangChain, LlamaIndex, AutoGen".
- **Wipro bundles frameworks with protocols and an eval stack.**
  - [Wipro GenAI Engineer](https://careers.wipro.com/job/Generative-AI-Engineer/187523-en_US/) lists LangChain, LangGraph, LlamaIndex, MCP, A2A and ADKs together.
  - [Wipro Agentic AI Engineer](https://careers.wipro.com/job/Agentic-AI-Engineer/207412-en_US/) requires "Hands-on experience with Google ADK, LangGraph, and Agentic AI frameworks".
- **DSPy appears twice.**
  - [Databricks AI Engineer FDE](https://jobs.thrivecap.com/companies/databricks/jobs/51700487-ai-engineer-fde-forward-deployed-engineer) requires GenAI frameworks "HuggingFace, LangChain, DSPy".
  - [Infer](https://www.ycombinator.com/companies/infer/jobs/1DhbYdF-applied-ai-engineer) targets "DSPy or GEPA-style prompt optimization" by Day 90.
- **Framework-only knowledge is not enough at an Indian product company.** [Whatfix](https://to.indeed.com/aazjxf46s9zc) makes LangChain, LlamaIndex, CrewAI and AutoGen "Good to Have". The must-haves are LLM APIs, retrieval, agents/tool use, evaluation, and coding agents.

### Inferences
- LangGraph is the de-facto agent framework to show in a portfolio, with Google ADK as a strong second for anyone targeting Google Cloud partners or Wipro/Infosys.
- Product companies screen for the underlying skills (agent loop, tool design, evals) rather than a framework name.
- PyTorch and Hugging Face still matter in enterprise ML and fine-tuning JDs (Adobe, Databricks, Avathon).

### Gaps
- None of the sampled India JDs names the OpenAI Agents SDK, CrewAI as mandatory, or LangChain alternatives like Pydantic-AI. I cannot tell whether that reflects the market or the sample.

## 3. Cloud platforms (AWS / Azure / GCP, Bedrock, Azure OpenAI, Vertex)

### Takeaway
About half the JDs (51%) mention any cloud, usually as "AWS, Azure, or GCP". GCP over-indexes here because 8 Google JDs are in the sample. Managed LLM platforms are named rarely: Vertex 4, Azure OpenAI 3, Bedrock 2. They appear mainly where the employer is a hyperscaler or a services firm aligned to one.

### Cited Findings
Frequencies by cloud (computed over the 49 JDs):

| Cloud | Any (N=49) | Mandatory | Notes |
|---|---|---|---|
| Any cloud | 25 (51%) | 20 (41%) | Big Tech 62%, Services 71%, AI startup 20% |
| Generic "AWS/Azure/GCP" | 16 (33%) | 13 | – |
| GCP | 9 (18%) | 5 | mostly Google, plus Wipro |
| AWS | 6 (12%) | 3 | – |
| Azure | 4 (8%) | 1 | – |
| Vertex AI | 4 (8%) | 1 | – |
| Azure OpenAI | 3 (6%) | 1 | – |
| Bedrock | 2 (4%) | 2 | – |

- **Bedrock at Infosys.** [Infosys GenAI/Agentic AI Engineer](https://www.bayt.com/ar/india/jobs/genai-agentic-ai-engineer-75181647/) requires "AWS Bedrock - Model invocation (Claude/Titan, etc.), Knowledge bases or retrieval integration".
- **Azure-native at Microsoft and NVIDIA.**
  - [Microsoft SWE II (Full Stack with AI)](https://jobs.anitab.org/companies/microsoft-2/jobs/89747334-software-engineer-ii) prefers Azure OpenAI, AKS, Functions, Service Bus and Azure Monitor.
  - [NVIDIA Enterprise Agentic AI](https://jobs.anitab.org/companies/nvidia/jobs/91148317-senior-ai-ml-software-engineer) prefers "Azure AI Services, Azure OpenAI, AI Search".
- **GCP stack at Wipro.** [Wipro Agentic AI Engineer](https://careers.wipro.com/job/Agentic-AI-Engineer/207412-en_US/) lists GCP, Vertex AI, GKE and Cloud Run.
- **AWS serverless at an early-stage startup.** [Craft My Plate](https://cutshort.io/job/AI-ML-Engineer-Bengaluru-Bangalore-CombineHealth-ln9ygN40) says: "AWS, serverless first … Lambda, API Gateway, DynamoDB, Step Functions".
- **Multi-provider LLM API lists.**
  - [Infosys Gen AI LLM Engineer](https://www.bayt.com/en/india/jobs/gen-ai-llm-engineer-75383098/) lists OpenAI, Azure OpenAI, Gemini and Claude.
  - [Whatfix](https://to.indeed.com/aazjxf46s9zc) names "OpenAI, Anthropic Claude, Gemini, or similar".

### Inferences
- Depth in one hyperscaler's AI platform is a differentiator mainly for services firms and hyperscaler FDE roles (Google Cloud, Microsoft). Product startups are largely provider-agnostic and care more about multi-model routing and cost.

### Gaps
- No AWS or Amazon JDs were sampled (Amazon pages were not reached), so AWS demand is likely understated.

## 4. AI/LLM technologies (RAG, vector DBs, agents, MCP, tool calling, fine-tuning, evals, guardrails, LLM observability, serving, multimodal)

### Takeaway
The core stack is agents (76%), RAG (63%) and evals (63%), followed by vector DBs (39%), prompt engineering (35%) and tool calling (33%). Fine-tuning appears in 24% but concentrates in enterprise ML and AI-startup JDs. Serving and inference engines (vLLM, Triton, TensorRT) appear in under 10% and only in infra-flavoured roles. When a vector DB product is named, it is pgvector, Weaviate, Pinecone, Milvus or FAISS/Chroma; Qdrant never appears.

### Cited Findings
Frequencies by AI/LLM skill (computed over the 49 JDs):

| Skill | Any (N=49) | Mandatory | Big Tech | Enterprise | Indian product | AI startup | Early | Services |
|---|---|---|---|---|---|---|---|---|
| Agents / agentic workflows | 37 (76%) | 23 (47%) | 75% | 86% | 80% | 80% | 67% | 71% |
| RAG / retrieval | 31 (63%) | 21 (43%) | 62% | 57% | 20% | 100% | 56% | 86% |
| Evals | 31 (63%) | 18 (37%) | 50% | 57% | 60% | 100% | 78% | 57% |
| Vector DB (any) | 19 (39%) | 11 | 44% | 14% | 0% | 60% | 44% | 57% |
| Prompt engineering | 17 (35%) | 12 | 38% | 0% | 40% | 80% | 11% | 57% |
| Tool / function calling | 16 (33%) | 11 | 25% | 29% | 40% | 40% | 44% | 29% |
| Fine-tuning | 12 (24%) | 8 | 12% | 57% | 20% | 60% | 11% | 14% |
| Multi-agent | 11 (22%) | 5 | 25% | 29% | 0% | 0% | 22% | 43% |
| MCP | 9 (18%) | 2 | 38% | 0% | 0% | 40% | 0% | 14% |
| Guardrails | 9 (18%) | 7 | 6% | 29% | 20% | 20% | 11% | 43% |
| Embeddings | 9 (18%) | 6 | – | – | – | – | – | – |
| Voice / ASR / TTS | 7 (14%) | 1 | 6% | 0% | 20% | 40% | 33% | 0% |
| Context engineering / memory | 6 (12%) | 5 | 0% | 14% | 40% | 40% | 11% | 0% |
| LLM observability tools (LangSmith/Langfuse/etc.) | 5 (10%) | 1 | 6% | 0% | 20% | 40% | 0% | 14% |
| Structured outputs | 4 (8%) | 4 | – | – | – | – | – | – |
| LLM serving (general) | 4 (8%) | 1 | – | – | – | – | – | – |
| vLLM | 3 (6%) | – | – | – | – | – | – | – |

Specific vector DB products: pgvector 3, Weaviate 3, Pinecone 2, Milvus 1, Qdrant 0. The only FAISS and ChromaDB mention is [Infosys](https://www.bayt.com/en/india/jobs/gen-ai-llm-engineer-75383098/). Triton and TensorRT each appear once (both at NVIDIA). TGI never appears. Multimodal/vision appears once. LoRA is never named explicitly.

- **Production-grade RAG detail.** [workwise AI Engineer](https://cutshort.io/job/AI-Engineer-Agents-Vision-Document-Intelligence-Bengaluru-Bangalore-Hello-Edge-abAhMELn) asks to "Build RAG pipelines covering ingestion, retrieval, reranking and answers with source references".
- **Sarvam's must-have list.** [Sarvam](https://jobs.khoslaventures.com/companies/sarvam-ai-2/jobs/80711937-applied-ai-engineer-sarvam-agents) requires RAG with "chunking, embeddings, hybrid search, reranking, vector databases" as a must-have.
- **Post-training preferred for agentic work.** [Adobe MLE, Agentic Marketing](https://jobs.accel.com/companies/frame-io/jobs/87707135-machine-learning-engineer-agentic-marketing) prefers "Fine-tuning or post-training experience (SFT, DPO, GRPO) applied to tool use or agent behavior".
- **Inference internals at NVIDIA.** [NVIDIA Local AI](https://jobs.anitab.org/companies/nvidia/jobs/87547967-senior-system-software-engineer-local-ai) requires knowledge of inference backends "including scheduling, memory management, KV-cache behavior", plus quantization, vLLM, llama.cpp and TensorRT.
- **NVIDIA MLOps preferred stack.** [NVIDIA Senior MLOps](https://jobs.anitab.org/companies/nvidia/jobs/91918453-senior-mlops-engineer-dsx-enablement) prefers "DGX systems, CUDA, NeMo, RAPIDS, Triton, NIM".
- **Evals as a gating discipline at startups.**
  - [Vahan](https://www.ycombinator.com/companies/vahan/jobs/7zvIddz-lead-ai-engineer): "every behaviour change ships behind a golden set and a regression gate".
  - [Infer](https://www.ycombinator.com/companies/infer/jobs/1DhbYdF-applied-ai-engineer): "Built LLM-as-judge eval pipelines and know their failure modes".
- **Hyperscaler FDEs own evals and observability.** [YouTube FDE](https://to.indeed.com/aalr27vg7bzy) and [Google GenAI FDE](https://to.indeed.com/aah9w6f7xm9p) both say: "Build high-performance evaluation pipelines and observability frameworks".

### Inferences
- The table-stakes AI skill set for a 2–5 YOE candidate is:
  - shipped agents with tool calling;
  - RAG with reranking and citations;
  - a written eval suite.
- The common differentiators are MCP servers, LLM observability tooling and fine-tuning or post-training.
- Serving and inference engines (vLLM, TensorRT, Triton) are a separate specialist track (NVIDIA, Razorpay, Cerebras-type roles), not a general AI-engineer expectation.

### Gaps
- Too few dedicated MLOps or inference JDs (4 in total) to give reliable frequencies for vLLM, TGI, Triton, KServe or Ray.
- The Sarvam Platform – AI Infrastructure and Cerebras JDs were shortlisted on Indeed but could not be fetched (rate limit).

## 5. Databases and infrastructure (Postgres, Redis, Kafka, Kubernetes, Docker, Terraform, CI/CD, observability)

### Takeaway
General production observability is the most-cited infra skill (47%), though it is usually framed as a responsibility rather than a requirement. CI/CD (29%), Docker (22%) and Kubernetes (20%) follow. Specific databases are named rarely: Postgres 2, Redis 1, MongoDB 1, Snowflake 2. Kafka (10%) and Terraform (4%) are marginal. Services firms list Docker and Kubernetes more than product companies do (Docker 71% vs 14%).

### Cited Findings
Frequencies by infra skill (computed over the 49 JDs):

| Skill | Any (N=49) | Mandatory | Big Tech | Enterprise | Indian product | AI startup | Early | Services |
|---|---|---|---|---|---|---|---|---|
| Observability (general) | 23 (47%) | 7 | 44% | 57% | 60% | 60% | 33% | 43% |
| CI/CD | 14 (29%) | 7 | 31% | 29% | 0% | 20% | 22% | 57% |
| Docker | 11 (22%) | 5 | 12% | 0% | 20% | 20% | 22% | 71% |
| Kubernetes | 10 (20%) | 5 | 19% | 14% | 40% | 0% | 11% | 43% |
| MLOps (general) | 7 (14%) | 3 | – | – | – | – | – | – |
| Spark | 6 (12%) | 3 | – | – | – | – | – | – |
| Kafka | 5 (10%) | 1 | – | – | – | – | – | – |
| NoSQL (generic) | 4 (8%) | 3 | – | – | – | – | – | – |
| Postgres | 2 (4%) | 1 | – | – | – | – | – | – |
| Snowflake | 2 (4%) | 2 | – | – | – | – | – | – |
| Airflow | 2 (4%) | 2 | – | – | – | – | – | – |
| Terraform | 2 (4%) | 1 | – | – | – | – | – | – |
| Redis | 1 (2%) | 1 | – | – | – | – | – | – |
| MongoDB | 1 (2%) | 1 | – | – | – | – | – | – |

- **Razorpay's platform requirements.** [Razorpay Lead AI Engineer](https://builtin.com/job/lead-ai-engineer/8974755) requires:
  - Kubernetes and distributed systems;
  - "Prometheus, Grafana, OpenTelemetry, or equivalent";
  - high-availability patterns such as "circuit breakers, graceful degradation, retry logic".
- **Sarvam's data layer.** [Sarvam](https://jobs.khoslaventures.com/companies/sarvam-ai-2/jobs/80711937-applied-ai-engineer-sarvam-agents) requires "PostgreSQL or MySQL, Redis" and "Signoz, Datadog, or any equivalent stack".
- **Terraform for agent infrastructure.** [Google FDE GECX](https://jobs.anitab.org/companies/google-24698/jobs/83694174-forward-deployed-engineer-generative-ai-gecx-google-cloud) requires "deploying resources via Terraform or similar tools to automate the setup of agents, functions, or networking".
- **Cisco's data pipeline stack.** [Cisco AI Engineer](https://to.indeed.com/aabtcp7sghz9) requires Snowflake and Airflow, and uses PySpark and Athena.

### Inferences
- For AI-engineer roles at 2–5 YOE, the infra bar is "can containerise, deploy, monitor and debug an LLM service". Deep Kubernetes, Kafka or Terraform is expected mainly in platform or infra roles (Razorpay, NVIDIA) and in services-firm checklists.

### Gaps
- Specific database products are seldom named, so I cannot rank Postgres, Mongo and Redis demand from this sample.

## 6. Experience requirements

### Takeaway
The modal stated minimum is 4–5 years (21 of 45 JDs), followed by 2–3 years (15). Medians by category:

| Category | Median minimum YOE |
|---|---|
| Big Tech | 5 |
| Enterprise/GCC | 5 |
| Services | 5 |
| Indian product | 4 |
| AI startups | 3 |
| Early-stage | 3 |

Many "Senior" or "Lead" titles at startups still accept 3–5 years. Almost every JD wants experience shipping to production, not demos.

### Cited Findings
- **YOE buckets** for the 45 JDs that state a minimum:

  | Minimum YOE | JDs |
  |---|---|
  | 0–1 | 3 |
  | 2–3 | 15 |
  | 4–5 | 21 |
  | 6–7 | 3 |
  | 8+ | 3 |

  The 8+ group is Google GenAI FDE, Apple Senior Applied AI and NVIDIA Senior MLOps (computed over the Appendix).
- **Big Tech minimums range from 2 to 8 years.**
  - [Google FDE V Data Cloud](https://to.indeed.com/aasc8sxtn2sh) asks for "2 years of experience in software engineering, data engineering…".
  - [Google GenAI FDE](https://to.indeed.com/aah9w6f7xm9p) asks for "8 years of experience in cloud computing or a technical customer-facing role".
- **AI-specific tenure on top of general tenure.**
  - [Microsoft SWE II](https://jobs.anitab.org/companies/microsoft-2/jobs/89747334-software-engineer-ii) prefers "4+ years" plus "1–3+ years of experience working with Generative AI technologies".
  - [Google Cloud AI Engineer](https://jobs.anitab.org/companies/google-24698/jobs/93056314-cloud-ai-engineer-technical-onboarding-center) asks for 3 years plus "2 years of experience in building and deploying GenAI applications".
  - [Atlassian Senior FDE](https://builtin.com/job/senior-forward-deployed-engineer-ai-remote/7303438) asks for 5+ years of backend plus "3+ years of experience delivering impactful AI/ML solutions in production".
- **"Production, not prototypes" language is common.**
  - [Sarvam](https://jobs.khoslaventures.com/companies/sarvam-ai-2/jobs/80711937-applied-ai-engineer-sarvam-agents): "Shipped AI features to real users in production, not just notebooks or prototypes".
  - [Vahan](https://www.ycombinator.com/companies/vahan/jobs/7zvIddz-lead-ai-engineer): "Shipped an LLM-backed system in production, with real users, long enough for it to break".
  - [Hirebound](https://careers.antler.co/companies/hirebound/jobs/82645033-founding-ai-engineer): "Experience building production-grade AI systems (not just prototypes)".
- **Inconsistent YOE on the same page.**
  - [Wipro GenAI Engineer](https://careers.wipro.com/job/Generative-AI-Engineer/187523-en_US/) shows "4 to 7yrs" and "3-5 Years".
  - [Walmart Senior SWE](https://jobs.anitab.org/companies/walmart/jobs/88934657-ind-senior-software-engineer) shows "6+ years" and "5 years".
  - [Vahan](https://www.ycombinator.com/companies/vahan/jobs/7zvIddz-lead-ai-engineer) shows 6+ in the header and 5+ in the body.
- **Entry-level FDE titles exist at small firms.** Zirodigital (0–2 yrs, ₹7 LPA) and appscrip (0–2 yrs, ₹1.8–5 LPA), both via [Cutshort](https://cutshort.io/job/AI-ML-Engineer-Bengaluru-Bangalore-CombineHealth-ln9ygN40).

### Inferences
- A ~3 YOE engineer clears most startup bars and roughly half of Big Tech mid-level bars (Google SWE III and FDE V at 2 years; Cisco AI Engineer at 3).
- By ~5 years, the 4–5-year Big Tech, GCC and services band opens up.
- Hyperscaler FDE roles at L5+ (8 years) are out of band for 2–5 YOE.

### Gaps
- Several JDs give no number (Databricks FDE says "Extensive years"). Avathon and Enterpret give none at all.

## 7. System design expectations and 8. Core fundamentals (DSA, distributed systems)

### Takeaway
System design is stated explicitly in 27% of JDs, but it is spread across product categories (Indian product 60%, AI startups 40%, early-stage 33%) and is absent from services JDs. DSA is stated in only 16% and clusters at Big Tech (31%) and Walmart/Adobe. It never appears in AI-startup, early-stage or services JDs in this sample. Distributed systems appear in 14%, mainly Big Tech and Indian product platform roles.

### Cited Findings
- **Counts** (computed over the 49 JDs):

  | Fundamental | Any (N=49) | Mandatory | Big Tech | Enterprise | Indian product | AI startup | Early | Services |
  |---|---|---|---|---|---|---|---|---|
  | System design | 13 (27%) | 9 | 19% | 29% | 60% | 40% | 33% | 0% |
  | DSA | 8 (16%) | 6 | 31% | 29% | 20% | 0% | 0% | 0% |
  | Distributed systems | 7 (14%) | 4 | 25% | 14% | 40% | 0% | 0% | 0% |

  Among FDE JDs, DSA is 0 of 15.
- **Google's DSA minimums.** [Google SWE III Full Stack Cloud AI](https://jobs.anitab.org/companies/google-24698/jobs/80587393-software-engineer-iii-full-stack-cloud-ai) requires "2 years of experience with data structures and algorithms" and "Experience in cloud computing, back-end, and distributed systems".
- **Cisco makes DSA mandatory.** [Cisco SWE (AI & Full-Stack)](https://to.indeed.com/aazyf74jdrxb) requires "In-depth knowledge of Data Structures, Algorithms, and Design Patterns".
- **Adobe pairs fundamentals with agentic skills.** [Adobe Agentic Marketing](https://jobs.accel.com/companies/frame-io/jobs/87707135-machine-learning-engineer-agentic-marketing) lists data structures, algorithms, distributed systems and API composition alongside agentic skills.
- **Apple prefers both.** [Apple Senior Applied AI](https://to.indeed.com/aa8g6g7j6mdb) prefers "Data Structures & Algorithms: Foundation and application experience" and "Distributed Systems … (e.g. Hadoop, Kafka, Spark, Flink etc.)".
- **Startups frame design as architecture ownership rather than interview DSA.**
  - [Whatfix](https://to.indeed.com/aazjxf46s9zc): "Architecture-level ownership of at least one production system — you can design agent topology, tool-calling chains, human escalation points".
  - [Lab0](https://www.ycombinator.com/companies/lab0/jobs/hlPvGkT-founding-engineer) lists "Software Architecture" as a skill.
  - [Hirebound](https://careers.antler.co/companies/hirebound/jobs/82645033-founding-ai-engineer): "Strong problem-solving and system design skills".
- **YouTube FDE requires system design.** [YouTube FDE](https://to.indeed.com/aalr27vg7bzy) asks for "4 years of experience in full-stack software development and system design".

### Inferences
- DSA prep matters mainly for Big Tech and GCC loops, which are among the few JDs that state it.
- For startups and FDE roles, the JDs signal "LLM system design" instead: agent topology, evaluation and escalation design, cost and latency trade-offs.

### Gaps
- JDs under-report interview content. DSA rounds may be standard even where the JD omits them. That is a question for the interviews research thread, not this one.

## 9. Mandatory vs preferred skills

### Takeaway
The hard requirements are mostly:
- Python;
- the core agent/RAG/eval loop;
- cloud and backend basics;
- customer-facing ability, for FDE roles.

Named frameworks, MCP, CrewAI/AutoGen, LLM observability tools, Kubernetes and Docker are mostly preferred or only mentioned in responsibilities.

### Cited Findings
For each skill, the share of its mentions that are mandatory (computed over the 49 JDs):

| Skill | Mandatory / any mention | Note |
|---|---|---|
| Python | 36 / 38 | – |
| Customer-facing | 10 / 12 | – |
| Guardrails | 7 / 9 | – |
| Structured outputs | 4 / 4 | – |
| Any cloud | 20 / 25 | – |
| Context engineering | 5 / 6 | – |
| RAG | 21 / 31 | – |
| System design | 9 / 13 | – |
| Tool calling | 11 / 16 | – |
| Agents | 23 / 37 | – |
| DSA | 6 / 8 | – |
| Evals | 18 / 31 | – |
| Vector DB | 11 / 19 | – |
| LangChain | 11 / 18 | – |
| LangGraph | 8 / 15 | – |
| Kubernetes | 5 / 10 | – |
| Docker | 5 / 11 | – |
| Observability (general) | 7 / 23 | – |
| MCP | 2 / 9 | 5 preferred, 2 responsibilities-only |
| LLM observability tools | 1 / 5 | – |
| CrewAI | 0 / 5 | – |

- **Mandatory MCP, twice.**
  - [Sarvam](https://jobs.khoslaventures.com/companies/sarvam-ai-2/jobs/80711937-applied-ai-engineer-sarvam-agents): "Production experience running MCP servers at scale".
  - [Wipro GenAI Engineer](https://careers.wipro.com/job/Generative-AI-Engineer/187523-en_US/): "Strong understanding of Model Context Protocols (MCP), A2A protocols, and Agent Developer Kits".
- **MCP preferred elsewhere.** It is preferred at:
  - [Cisco AI Engineer](https://to.indeed.com/aabtcp7sghz9): "Hands-on experience building MCP servers";
  - [Apple](https://to.indeed.com/aa8g6g7j6mdb);
  - [NVIDIA](https://jobs.anitab.org/companies/nvidia/jobs/91148317-senior-ai-ml-software-engineer);
  - [Google harness](https://jobs.anitab.org/companies/google-24698/jobs/93056306-software-engineer-iii-ai-ml-agentic-ai-platform-and-hardware-harness);
  - [Vahan](https://www.ycombinator.com/companies/vahan/jobs/7zvIddz-lead-ai-engineer): "MCP server authoring", under "Genuinely Not Required".
- **Microsoft's required section is a degree only.** In [Microsoft SWE II](https://jobs.anitab.org/companies/microsoft-2/jobs/89747334-software-engineer-ii), every technical skill sits under preferred qualifications.
- **Wipro labels only one item mandatory.** It marks only "Mandatory Skills: Generative AI" or "GenAI Consulting for Apps & Infra"; everything else is a flat technical list ([Wipro Agentic AI](https://careers.wipro.com/job/Agentic-AI-Engineer/207412-en_US/), [Wipro Gen AI Lead](https://careers.wipro.com/job/Gen-AI-Engineer-Lead/198667-en_US/)).

### Inferences
- Candidates should prove mastery of the mandatory core (Python, agents with tool calling, RAG, evals, cloud deployment) before collecting preferred badges.
- MCP is the preferred skill most likely to become mandatory next: it is already "Responsibilities" at Google and YouTube FDE, and mandatory at Sarvam and Wipro.

### Gaps
- Services JDs often do not separate mandatory from preferred, so their M/P split is a coder judgement: I coded the flat list as M.

## 10. Skills associated with higher-paying / senior postings (where salary is listed)

### Takeaway
Only 10 of 49 JDs list salary, all at startups or small firms. No Big Tech, GCC, services or Indeed JD lists pay. Among those 10, the postings with an upper bound of ₹48 LPA or more (7 JDs, ₹12–60L bands) cluster on four things:
- owning production agents and evals (5 of 7);
- voice/real-time agents (4 of 7);
- fine-tuning (3 of 7);
- coding-agent fluency.

The ≤₹7L postings are 0–2-year FDE or generalist roles with framework-list requirements. That is an association within a tiny sample, not a pay model.

### Cited Findings
Salary-listed JDs (₹ lakh per annum):

| JD | YOE | Band | Notable requirements |
|---|---|---|---|
| [Vahan Lead AI Engineer](https://www.ycombinator.com/companies/vahan/jobs/7zvIddz-lead-ai-engineer) | 5 | ₹30–60L | agents, eval suites, Claude Code, voice stack (LiveKit/Pipecat/Deepgram), MCP authoring (pref) |
| [100ms Senior Product Engineer – AI Agents](https://jobs.lever.co/100ms/c6a9c8b8-ae0f-447c-a44b-eb95d09de3a9) | 4 | ₹25–60L | Python/Go, React, REST with observability, DSA |
| [Sei AI LLM Engineer](https://wellfound.com/jobs/3162567-llm-engineer) | 4 | ₹20–50L + 0.02–0.2% equity | prompts measured and optimised, RAG, evals, GraphRAG |
| [100ms AI Engineer – AI Agents](https://jobs.accel.com/companies/100ms-2/jobs/64657380-ai-engineer-ai-agents-healthcare) | 2 | ₹20–50L | prompting, fine-tuning, evaluation, guardrails, system design |
| [Infer Applied AI Engineer](https://www.ycombinator.com/companies/infer/jobs/1DhbYdF-applied-ai-engineer) | 3 | ₹20–50L + 0.01–0.2% | agents, LLM-as-judge evals, ASR/TTS |
| Craft My Plate Founding Engineer Lead ([Cutshort](https://cutshort.io/job/AI-ML-Engineer-Bengaluru-Bangalore-CombineHealth-ln9ygN40)) | 5 | ₹30–50L | TypeScript, AWS serverless, LangGraph multi-agent, HLD |
| [Tsenta Founding Engineer](https://www.ycombinator.com/companies/tsenta/jobs/hYAeFGp-founding-engineer) | 3 | ₹12–48L | TypeScript, queue-driven backends, tool use / retrieval / evals |
| [workwise AI Engineer](https://cutshort.io/job/AI-Engineer-Agents-Vision-Document-Intelligence-Bengaluru-Bangalore-Hello-Edge-abAhMELn) | 3 | ₹20–30L | RAG, agents, multimodal, evals |
| Zirodigital Associate AI FDE ([Cutshort](https://cutshort.io/job/AI-ML-Engineer-Bengaluru-Bangalore-CombineHealth-ln9ygN40)) | 0–2 | ₹7L | – |
| appscrip FDE ([Cutshort](https://cutshort.io/job/AI-ML-Engineer-Bengaluru-Bangalore-CombineHealth-ln9ygN40)) | 0–2 | ₹1.8–5L | body says comp "still to be confirmed" |

- **USD pay at one YC startup.** [Lab0 Founding Engineer](https://www.ycombinator.com/companies/lab0/jobs/hlPvGkT-founding-engineer) (3 years) lists USD 30–60K plus 0.10–1.00% equity.
- **Senior / non-salary proxy.** The 8+ year postings, [Google GenAI FDE](https://to.indeed.com/aah9w6f7xm9p), [Apple Senior Applied AI](https://to.indeed.com/aa8g6g7j6mdb) and [NVIDIA Senior MLOps](https://jobs.anitab.org/companies/nvidia/jobs/91918453-senior-mlops-engineer-dsx-enablement), add:
  - architecting AI systems on cloud;
  - leading discovery with customers;
  - LLM serving and inference knowledge;
  - distributed systems;
  - "LLM-native metrics (e.g., tokens/sec, cost-per-request)".

### Inferences
- Within startups, the premium skills look like production agent ownership with eval discipline, real-time or voice, and fine-tuning, not framework breadth.
- At senior Big Tech levels, the differentiators are architecture, customer discovery and inference economics.

### Gaps
- No Big Tech, GCC or services salary appears in any sampled JD, and Indeed showed "N/A" on all 90 listing slots. Use the compensation research thread for pay levels.
- n=10 is too small for any statistical association.

## Newly appearing skills (MCP, A2A, evals, context engineering, agent observability, coding agents)

### Takeaway
Evals are already mainstream (63%; 37% mandatory). MCP (18%) is concentrated in Big Tech JDs (38%: Google, YouTube, Cisco, Apple, NVIDIA) and one AI startup. Context engineering/memory (12%), coding-agent fluency (10%), LLM observability tools (10%) and LLM cost metrics (10%) are early but present. A2A appears in exactly one JD (Wipro). "Agent-as-a-judge", trajectory evals and spec-driven development appear in single JDs.

### Cited Findings
Emerging-skill frequencies (computed over the 49 JDs):

| Skill | Any (N=49) | Mandatory | Where it appears |
|---|---|---|---|
| Evals | 31 (63%) | 18 | – |
| Tool calling | 16 (33%) | 11 | – |
| Multi-agent | 11 (22%) | 5 | – |
| MCP | 9 (18%) | 2 | Big Tech 6, AI startup 2, services 1 |
| Guardrails | 9 (18%) | 7 | – |
| Voice agents | 7 (14%) | – | – |
| Context engineering / memory | 6 (12%) | 5 | – |
| Coding agents (Claude Code / Cursor / Copilot) | 5 (10%) | 4 | – |
| LLM observability tools | 5 (10%) | – | – |
| LLM cost/token metrics | 5 (10%) | – | – |
| Structured outputs | 4 (8%) | – | – |
| DSPy | 2 (4%) | – | – |
| A2A | 1 (2%) | 1 | Wipro |
| Human-in-the-loop approval flows | 1 (2%) | – | – |

- **MCP servers as a responsibility.** [Google GenAI FDE](https://to.indeed.com/aah9w6f7xm9p) lists "production-grade agentic workflows (e.g., multi-agent systems, model context protocol (MCP) servers)". [Cisco AI Engineer](https://to.indeed.com/aabtcp7sghz9) says: "Build and maintain Model Context Protocol (MCP) servers and tool integrations that give AI agents secure, governed access".
- **A2A.** It appears only in [Wipro GenAI Engineer](https://careers.wipro.com/job/Generative-AI-Engineer/187523-en_US/): "MCP, A2A protocols, and Agent Developer Kits".
- **Agent observability and eval stack named.** [Wipro Agentic AI Engineer](https://careers.wipro.com/job/Agentic-AI-Engineer/207412-en_US/) lists:
  - tools: Braintrust, Arize Phoenix, OpenTelemetry, Promptfoo, Galileo, DeepEval, Confident AI, Ragas, Langfuse, LangSmith;
  - methods: "LLM-as-a-Judge, Agent-as-a-Judge, Pass@k", trajectory/trace-based evaluation.
- **Avathon prefers a similar stack.** [Avathon Forward AI Engineer](https://avathon.com/company/careers/forward-ai-engineer-agentic-ai-4701359005/) prefers Langfuse, LangSmith, Arize Phoenix, W&B, RAGAS, DeepEval, "prompt versioning, cost/latency tracking, guardrails, hallucination detection".
- **Context engineering by name.**
  - [Whatfix](https://to.indeed.com/aazjxf46s9zc): "prompt and context design".
  - [Vahan](https://www.ycombinator.com/companies/vahan/jobs/7zvIddz-lead-ai-engineer): "context management".
  - [Sarvam](https://jobs.khoslaventures.com/companies/sarvam-ai-2/jobs/80711937-applied-ai-engineer-sarvam-agents): memory/context engineering (Honcho).
  - [Postman](https://builtin.com/job/senior-applied-ai-engineer/8887872): "context management, tool use patterns".
- **Coding-agent fluency as a must-have.**
  - [Whatfix](https://to.indeed.com/aazjxf46s9zc): "Real experience with Spec Driven development and coding agents such as Claude Code, Cursor or Copilot".
  - [Vahan](https://www.ycombinator.com/companies/vahan/jobs/7zvIddz-lead-ai-engineer): "Use coding agents hard and well — Claude Code from Day 1".
  - appscrip: "You work with coding agents daily" ([Cutshort](https://cutshort.io/job/AI-ML-Engineer-Bengaluru-Bangalore-CombineHealth-ln9ygN40)).
- **LLM economics.**
  - [Razorpay](https://builtin.com/job/lead-ai-engineer/8974755): "Solid understanding of LLM APIs and token economics"; prefers LiteLLM, Portkey and Langfuse.
  - [Infosys](https://www.bayt.com/ar/india/jobs/genai-agentic-ai-engineer-75181647/): "Monitor basic latency, token usage, and cost metrics".

### Inferences
- MCP is moving from "nice to have" to "responsibility" at hyperscaler FDE and Big Tech AI-platform teams. A shipped, secured MCP server (OAuth, governed tool access) is a high-signal portfolio item.
- Eval engineering is no longer emerging; it is core.
- A2A has not yet reached India product JDs in this sample.

### Gaps
- None of the 49 JDs uses the exact phrase "context engineering". I coded close equivalents (context design or management, memory).
- Tool-level frequencies (LangSmith vs Langfuse) rest on 3–4 mentions each.

## Cross-category intersection of skills

### Takeaway
Three skills appear at substantial rates in every company category:
- agents / agentic workflows (≥67% in every category);
- Python (≥56%);
- evals (≥50%).

These form the cross-category core. The next layer, general production observability and at least one named LLM framework, reaches ≥33% everywhere. RAG is high everywhere except Indian product companies (20%). Customer-facing ability defines FDE roles regardless of category.

### Cited Findings
- **Per-category share for the core skills** (computed over the 49 JDs; categories with n≥3):

  | Skill | Big Tech | Enterprise | Indian product | AI startup | Early | Services |
  |---|---|---|---|---|---|---|
  | Agents | 75% | 86% | 80% | 80% | 67% | 71% |
  | Python | 75% | 71% | 80% | 100% | 56% | 100% |
  | Evals | 50% | 57% | 60% | 100% | 78% | 57% |
  | Observability | 44% | 57% | 60% | 60% | 33% | 43% |
  | Any LLM framework | 50% | 57% | 40% | 60% | 33% | 86% |
  | RAG | 62% | 57% | 20% | 100% | 56% | 86% |

- **FDE vs non-FDE.**

  | Skill | FDE (15 JDs) | Non-FDE (34 JDs) |
  |---|---|---|
  | Customer-facing | 73% | 3% |
  | Observability | 67% | 38% |
  | Any cloud | 73% | 41% |
  | RAG | 73% | 59% |
  | Agents | 87% | 71% |
  | Evals | 73% | 59% |
  | DSA | 0% | 24% |
  | System design | 20% | 29% |

- **FDE role framing.**
  - [Google GenAI FDE](https://to.indeed.com/aah9w6f7xm9p) describes FDEs who "code, debug, and jointly ship bespoke agentic solutions directly within the customer's environment".
  - [Cisco Senior FDE](https://to.indeed.com/aazkgffg846l) requires "Excellent communication skills and the ability to work directly with enterprise customers".
  - [Whatfix](https://to.indeed.com/aazjxf46s9zc) requires "A track record of running discovery independently".
- **Robustness checks.**
  - **Live JDs only (n=31):** Python 77%, agents 74%, RAG 68%, evals 65%, any LLM framework 55%, observability 52%, MCP 19% (computed).
  - **Indeed-only current postings (n=8, Oct–Nov 2026):** agents 7/8, RAG 7/8, Python 6/8, evals 5/8, observability 5/8, vector DB 5/8, MCP 4/8 (computed).

### Inferences
- The portable 2–5 YOE AI-engineer profile across all six categories is:
  - Python production services;
  - agents with tool calling, shipped to real users;
  - RAG with retrieval-quality evals;
  - an eval and observability harness;
  - deployment on one major cloud.
- On top of that core, specialise by target:
  - **Big Tech:** DSA and distributed systems, plus MCP.
  - **Startups:** voice/real-time, coding-agent fluency and fine-tuning.
  - **FDE / solutions:** customer discovery, cloud architecture and GCP/ADK where the employer is Google-aligned.
  - **Services:** keyword coverage of LangChain/LangGraph, Docker/Kubernetes and a hyperscaler AI platform.

### Gaps
- With n=5–9 in four of the six categories, "intersection" thresholds are sensitive to single JDs. A larger Indeed pull, once the rate limit clears, should be used to confirm the services and GCC columns.

## Appendix — JD register (all observed 2026-11-27)

### Takeaway
49 JDs, each recorded with company, title, category, role type, location, minimum YOE asked, posting date and status as shown, and URL. Category codes: BIG = Big Tech; ENT = enterprise SaaS / global product / GCC; INP = Indian product; AIS = funded AI-native startup; EARLY = early-stage/founding; SVC = IT services/consulting. Role codes: AIE = AI/GenAI/LLM engineer; FDE = forward-deployed/solutions/customer; INFRA = AI infra/inference; MLOPS; MLE = classic ML engineer.

### Cited Findings

| ID | Company | Title | Cat | Role | Location | Min YOE | Posted / status as shown | URL |
|---|---|---|---|---|---|---|---|---|
| J1 | Google (Cloud) | Generative AI Forward Deployed Engineer, Google Cloud | BIG | FDE | Mumbai/Pune/Bengaluru | 8 | 2026-11-02, open | https://to.indeed.com/aah9w6f7xm9p |
| J2 | Whatfix | Forward Deployed Engineer-AI | INP | FDE | Bengaluru | 3 (3–7) | 2026-11-16, open | https://to.indeed.com/aazjxf46s9zc |
| J3 | Google (Cloud) | Forward Deployed Engineer V, GenAI, Google Cloud (Data Cloud) | BIG | FDE | Bengaluru | 2 | 2026-11-04, open | https://to.indeed.com/aasc8sxtn2sh |
| J4 | YouTube (Google) | Forward Deployed Engineer, GenAI, YouTube | BIG | FDE | Bengaluru | 4 | 2026-11-13, open | https://to.indeed.com/aalr27vg7bzy |
| J5 | Apple | Senior Applied AI Engineer - AiDP | BIG | AIE | Bengaluru | 8 | 2026-11-04, open | https://to.indeed.com/aa8g6g7j6mdb |
| J6 | Cisco | Software Engineer (AI & Full-Stack) | BIG | AIE | Bengaluru | 5 (3 w/ MS) | 2026-11-20, open | https://to.indeed.com/aazyf74jdrxb |
| J7 | Cisco | AI Engineer (CloudX) | BIG | AIE | Bengaluru | 3 | 2026-11-24, open | https://to.indeed.com/aabtcp7sghz9 |
| J8 | Cisco | Senior Forward Deployed Engineer | BIG | FDE | Bengaluru | 7 (4 w/ MS) | 2026-10-14, open | https://to.indeed.com/aazkgffg846l |
| W1 | Razorpay | Lead AI Engineer (AI platform / LLM gateway) | INP | INFRA | Bengaluru | 5 (5–8) | removed 2026-04-24 | https://builtin.com/job/lead-ai-engineer/8974755 |
| W2 | Sarvam AI | Applied AI Engineer, Sarvam Agents | AIS | AIE | Bengaluru | 3 (3–5) | posted 6+ mo before obs.; closed | https://jobs.khoslaventures.com/companies/sarvam-ai-2/jobs/80711937-applied-ai-engineer-sarvam-agents |
| W3 | NVIDIA | Senior System Software Engineer - Local AI | BIG | INFRA | Pune | 5 | 2026-07-25; closed | https://jobs.anitab.org/companies/nvidia/jobs/87547967-senior-system-software-engineer-local-ai |
| W4 | NVIDIA | Senior AI/ML Software Engineer (Enterprise Agentic AI Platform) | BIG | AIE | Bengaluru/Pune | 6 | 2026-08-26; closed | https://jobs.anitab.org/companies/nvidia/jobs/91148317-senior-ai-ml-software-engineer |
| W5 | NVIDIA | Senior MLOps Engineer - DSX Enablement | BIG | MLOPS | Bengaluru/Hyderabad/Pune | 8 | 2026-09-02; listed | https://jobs.anitab.org/companies/nvidia/jobs/91918453-senior-mlops-engineer-dsx-enablement |
| W6 | Sei AI (YC) | LLM Engineer | EARLY | AIE | Chennai | 4 | reposted ~1 mo before obs.; listed | https://wellfound.com/jobs/3162567-llm-engineer |
| W7 | 100ms | AI Engineer - AI Agents (Healthcare) | INP | AIE | Bengaluru | 2 (2–5) | posted 6+ mo before obs.; still on Lever board | https://jobs.accel.com/companies/100ms-2/jobs/64657380-ai-engineer-ai-agents-healthcare |
| W8 | Vahan (YC S19) | Lead AI Engineer / AI Engineer III | AIS | AIE | Bengaluru | 5 (header 6) | n/s; listed | https://www.ycombinator.com/companies/vahan/jobs/7zvIddz-lead-ai-engineer |
| W9 | Infer (YC S21) | Applied AI Engineer | EARLY | AIE | Bengaluru | 3 | n/s; listed | https://www.ycombinator.com/companies/infer/jobs/1DhbYdF-applied-ai-engineer |
| W10 | Lab0 (YC P26) | Founding Engineer | EARLY | AIE | Bengaluru | 3 | n/s; listed | https://www.ycombinator.com/companies/lab0/jobs/hlPvGkT-founding-engineer |
| W11 | Tsenta (YC S26) | Founding Engineer | EARLY | AIE | Bengaluru | 3 | n/s; listed | https://www.ycombinator.com/companies/tsenta/jobs/hYAeFGp-founding-engineer |
| W12 | Hirebound (Antler) | Founding AI Engineer | EARLY | AIE | Bengaluru | 1 (1–5) | 2026-06-13; closed | https://careers.antler.co/companies/hirebound/jobs/82645033-founding-ai-engineer |
| C1 | Zirodigital | Associate AI Forward Deployed Engineer | EARLY | FDE | Hyderabad | 0 (0–2) | 2026-10-18 (Cutshort) | https://cutshort.io/job/AI-ML-Engineer-Bengaluru-Bangalore-CombineHealth-ln9ygN40 |
| C2 | appscrip | Forward Deployed Engineer (FDE) | EARLY | FDE | Bengaluru | 0 (0–2) | 2026-10-12 (Cutshort) | same Cutshort page |
| C3 | Ampera Technologies | Senior GenAI Engineer, RAG (Full-Stack) | SVC | AIE | Chennai/Remote | 5 (5–15) | 2026-09-24 (Cutshort) | same Cutshort page |
| C4 | Craft My Plate | Founding Engineer Lead | EARLY | AIE | Hyderabad | 5 (5–7) | 2026-09-23 (Cutshort) | same Cutshort page |
| C5 | VY Systems | Python + Agentic AI | SVC | AIE | Hyderabad | 7 (7–10) | 2026-09-23 (Cutshort) | same Cutshort page |
| W13 | Databricks | AI Engineer - FDE (Forward Deployed Engineer) | ENT | FDE | Mumbai/Bengaluru/Delhi/Pune | n/s ("extensive") | posted 6+ mo before obs.; closed | https://jobs.thrivecap.com/companies/databricks/jobs/51700487-ai-engineer-fde-forward-deployed-engineer |
| W14 | Databricks | Specialist Solutions Architect - AI/ML | ENT | FDE | Bengaluru | 5 | 2026-06-16; listed | https://jobs.thrivecap.com/companies/databricks/jobs/82848270-specialist-solutions-architect-ai-ml |
| W15 | Atlassian | Senior Forward Deployed Engineer, AI | ENT | FDE | Bengaluru (in-office/remote) | 5 | removed 2026-02-12 | https://builtin.com/job/senior-forward-deployed-engineer-ai-remote/7303438 |
| W16 | Microsoft | Software Engineer II (Full Stack with AI) | BIG | AIE | Hyderabad | 4 (pref) | 2026-08-13; closed | https://jobs.anitab.org/companies/microsoft-2/jobs/89747334-software-engineer-ii |
| W17 | Uber | Senior Machine Learning Engineer | BIG | MLE | Bengaluru | 5 (2 w/ MS/PhD) | posted 6+ mo before obs.; closed | https://jobs.anitab.org/companies/uber/jobs/65596101-senior-machine-learning-engineer |
| W18 | Enterpret | Applied AI Research Engineer | AIS | AIE | Bengaluru | n/s | n/s; listed | https://job-boards.greenhouse.io/enterpret/jobs/7580532003 |
| W19 | 100ms | Senior Product Engineer - AI Agents (Healthcare) | INP | AIE | Bengaluru | 4 | listed on Lever at obs. | https://jobs.lever.co/100ms/c6a9c8b8-ae0f-447c-a44b-eb95d09de3a9 |
| W20 | Adobe | Machine Learning Engineer, Agentic Marketing | ENT | AIE | Bengaluru | 5 | 2026-07-28; closed | https://jobs.accel.com/companies/frame-io/jobs/87707135-machine-learning-engineer-agentic-marketing |
| W21 | Adobe | Machine Learning Engineer 3 (Genuine Engineering) | ENT | MLE | Bengaluru/Noida | 5 | 2026-08-27; listed | https://jobs.accel.com/companies/frame-io/jobs/91349408-machine-learning-engineer-3 |
| W22 | Postman | Senior Applied AI Engineer | INP | AIE | Bengaluru (hybrid) | 5 | removed 2026-04-20 | https://builtin.com/job/senior-applied-ai-engineer/8887872 |
| W23 | Observe.AI | AI Agent Engineer (client-facing) | AIS | FDE | Bengaluru | 3 | 2026-07-22; closed | https://jobs.ngpcap.com/companies/observe-ai/jobs/87088835-ai-agent-engineer |
| W24 | workwise (via Hello Edge) | AI Engineer - Agents, Vision & Document Intelligence | EARLY | AIE | Bengaluru | 3 (3–5) | 2026-10-20; listed | https://cutshort.io/job/AI-Engineer-Agents-Vision-Document-Intelligence-Bengaluru-Bangalore-Hello-Edge-abAhMELn |
| W25 | Avathon | Forward AI Engineer - Agentic AI | AIS | FDE | Bengaluru | n/s | 2026-06-01; listed | https://avathon.com/company/careers/forward-ai-engineer-agentic-ai-4701359005/ |
| W26 | Google | Software Engineer III, Full Stack, Cloud AI | BIG | AIE | Bengaluru | 2 | posted 6+ mo before obs.; closed | https://jobs.anitab.org/companies/google-24698/jobs/80587393-software-engineer-iii-full-stack-cloud-ai |
| W27 | Google | Software Engineer III, AI/ML, Agentic AI Platform and Hardware Harness | BIG | INFRA | Bengaluru | 2 | 2026-09-12; closed | https://jobs.anitab.org/companies/google-24698/jobs/93056306-software-engineer-iii-ai-ml-agentic-ai-platform-and-hardware-harness |
| W28 | Google (Cloud) | Cloud AI Engineer, Technical Onboarding Center | BIG | FDE | Bengaluru/Hyderabad/Gurugram/Pune | 3 | 2026-09-12; closed | https://jobs.anitab.org/companies/google-24698/jobs/93056314-cloud-ai-engineer-technical-onboarding-center |
| W29 | Google (Cloud) | Forward Deployed Engineer, Generative AI, GECX | BIG | FDE | Bengaluru | 5 | 2026-06-23; closed | https://jobs.anitab.org/companies/google-24698/jobs/83694174-forward-deployed-engineer-generative-ai-gecx-google-cloud |
| W30 | Wipro | Agentic AI Engineer | SVC | AIE | Bengaluru | 5 (5–8) | "10/12/26"; listed | https://careers.wipro.com/job/Agentic-AI-Engineer/207412-en_US/ |
| W31 | Wipro | Generative AI Engineer | SVC | AIE | Bengaluru/Pune/Chennai | 4 (page also says 3–5) | "9/10/26"; listed | https://careers.wipro.com/job/Generative-AI-Engineer/187523-en_US/ |
| W32 | Wipro | Gen AI Engineer Lead (Forward Deployed Engineer) | SVC | FDE | Bengaluru/Hyderabad/Chennai/Pune | 5 (5–16) | "10/1/26"; listed | https://careers.wipro.com/job/Gen-AI-Engineer-Lead/198667-en_US/ |
| W33 | Infosys | GenAI / Agentic AI Engineer | SVC | AIE | Bengaluru | n/s | Bayt shows "2026/12/25" and "30+ days ago" (inconsistent); listed | https://www.bayt.com/ar/india/jobs/genai-agentic-ai-engineer-75181647/ |
| W34 | Infosys | Gen AI, LLM Engineer | SVC | AIE | Bengaluru | 2 (2–5) | ~2026-11-04 ("23 days ago"); listed | https://www.bayt.com/en/india/jobs/gen-ai-llm-engineer-75383098/ |
| W35 | Walmart Global Tech | (IND) Software Engineer II | ENT | AIE | Bengaluru | 3 (or degree) | 2026-06-25; closed | https://jobs.anitab.org/companies/walmart/jobs/84130611-ind-software-engineer-ii |
| W36 | Walmart Global Tech | (IND) Senior Software Engineer (agentic AI full-stack) | ENT | AIE | Bengaluru/Remote | 5 (summary says 6+) | 2026-08-06; closed | https://jobs.anitab.org/companies/walmart/jobs/88934657-ind-senior-software-engineer |

### Inferences
- About 63% of the register (31 of 49) was live at observation. The closed 2026 postings are retained because they are real, recent JDs, and the live-only robustness check shows similar skill rates.

### Gaps
- **Excluded: out of YOE band.** Walmart Staff SWE (Full Stack with AI), 10–15 yrs ([link](https://jobs.anitab.org/companies/walmart/jobs/94413524-staff-software-engineer-full-stack-with-ai)).
- **Excluded: page did not render the JD.** Flipkart (foundit / nodeflair / weekday), Swiggy (foundit), Atlassian careers 27643, Capgemini ("position filled"), Brillio (hirist), Lenskart.
- **Excluded: no full JD fetched.** All Indeed listings other than J1–J8, because of the connector rate limit.
- **Cutshort JDs (C1–C5) came from a listing page.** Their skill lists were extracted by a summarising fetch of that page, not from individual JD pages, so treat them as lower-fidelity.
