[Previous](../05%20Emerging%20Startup%20and%20Industry%20Landscape/05%20Emerging%20Startup%20and%20Industry%20Landscape.md) | [Index](../INDEX.md) | [Next](../07%20Technology%20Stack%20Demand%20Matrix/07%20Technology%20Stack%20Demand%20Matrix.md)

# 6. Actual job description analysis: 90 India JDs converge on agents, RAG and evals on top of production basics

Two independent samples were hand-coded from India-located postings viewed on **27 Nov 2026**:

- **Sample A:** 49 AI/GenAI/LLM, ML, MLOps, AI-infra and FDE/solutions JDs. 31 were still live; 18 had closed, most of them posted in 2026.
- **Sample B:** 41 SDE-2-equivalent backend, full-stack, platform and AI-platform JDs.

Sources were the Indeed connector, company ATS boards (Greenhouse, Ashby, Lever, Workday, amazon.jobs, Microsoft careers), YC/Wellfound, VC job boards and Cutshort. Both samples have a single coder and known skews. Sample A over-represents Google (8 JDs) and Bengaluru (~80%). Sample B over-represents MNCs (29 of 41) and misses the Java/Go-heavy unicorns (Flipkart, Swiggy, PhonePe, Razorpay backend). Both under-represent IT services, because Indeed rate-limited full-JD fetches after 14–20 calls. Within a category, one JD moves the percentage by 6–20 points. Read every figure below as directional. As a robustness check, the live-only Sample A subset (n=31) gives almost the same headline rates: Python 77%, agents 74%, RAG 68%, evals 65%.

| Sample | n | Category mix | Role mix | Stated minimum YOE |
|---|---|---|---|---|
| A: AI / FDE | 49 | Big Tech 16, Enterprise SaaS/GCC 7, Indian product 5, funded AI startup 5, early-stage 9, IT services 7 | AI/GenAI engineer 28, FDE/solutions 15, AI infra 3, MLOps 1, classic MLE 2 | 80% of the 45 stating a minimum set it at 2–5 yrs; most common is 4–5 (21 JDs) |
| B: SDE-2 / platform | 41 | Big Tech 13, SaaS/MNC 16, Indian product 6, India startups 6 | Backend, full-stack, platform/SRE, AI platform | Most common is "3+" (20 of 38); range 1+ (Google SWE II) to 5+ |

## 6.1 AI and FDE JDs: frequency by company category (Sample A, any mention)

| Skill | All (n=49) | Mandatory | Big Tech (16) | Enterprise/GCC (7) | Indian product (5) | AI startup (5) | Early-stage (9) | IT services (7) |
|---|---|---|---|---|---|---|---|---|
| Python | **78%** | 73% | 75% | 71% | 80% | 100% | 56% | 100% |
| Agents / agentic workflows | **76%** | 47% | 75% | 86% | 80% | 80% | 67% | 71% |
| RAG / retrieval | **63%** | 43% | 62% | 57% | 20% | 100% | 56% | 86% |
| Evals | **63%** | 37% | 50% | 57% | 60% | 100% | 78% | 57% |
| Any LLM framework | 53% | 29% | 50% | 57% | 40% | 60% | 33% | 86% |
| Any cloud | 51% | 41% | 62% | — | — | 20% | — | 71% |
| Observability (general) | 47% | 14% | 44% | 57% | 60% | 60% | 33% | 43% |
| Vector DB (any) | 39% | 22% | 44% | 14% | 0% | 60% | 44% | 57% |
| LangChain | 37% | 22% | 31% | 43% | 40% | 40% | 11% | 71% |
| Prompt engineering | 35% | 24% | 38% | 0% | 40% | 80% | 11% | 57% |
| Tool / function calling | 33% | 22% | 25% | 29% | 40% | 40% | 44% | 29% |
| TypeScript / JS | 33% | 22% | 25% | 43% | 40% | 20% | 44% | 29% |
| LangGraph | 31% | 16% | 38% | 14% | 0% | 20% | 22% | 71% |
| CI/CD | 29% | 14% | 31% | 29% | 0% | 20% | 22% | 57% |
| System design | 27% | 18% | 19% | 29% | 60% | 40% | 33% | 0% |
| Fine-tuning | 24% | 16% | 12% | 57% | 20% | 60% | 11% | 14% |
| Docker | 22% | 10% | 12% | 0% | 20% | 20% | 22% | 71% |
| Kubernetes | 20% | 10% | 19% | 14% | 40% | 0% | 11% | 43% |
| MCP | 18% | 4% | 38% | 0% | 0% | 40% | 0% | 14% |
| Guardrails | 18% | 14% | 6% | 29% | 20% | 20% | 11% | 43% |
| DSA | 16% | 12% | 31% | 29% | 20% | 0% | 0% | 0% |
| Java / Go | 16% / 16% | 10% / 12% | 31% / 25% | 29% / 0% | 0% / 40% | 0% / 0% | 11% / 22% | 0% / 0% |
| Voice / ASR / TTS | 14% | 2% | 6% | 0% | 20% | 40% | 33% | 0% |
| Context engineering / memory | 12% | 10% | 0% | 14% | 40% | 40% | 11% | 0% |
| Coding agents (Claude Code, Cursor, Copilot) | 10% | 8% | — | — | — | — | — | — |
| LLM observability tools (Langfuse, LangSmith) | 10% | 2% | 6% | 0% | 20% | 40% | 0% | 14% |
| vLLM / Triton / TensorRT | 6% / 2% / 2% | — | NVIDIA only | — | — | — | — | — |

Example sources: [Google GenAI FDE](https://to.indeed.com/aah9w6f7xm9p), [Cisco AI Engineer](https://to.indeed.com/aabtcp7sghz9), [Whatfix FDE-AI](https://to.indeed.com/aazjxf46s9zc), [Sarvam Applied AI Engineer](https://jobs.khoslaventures.com/companies/sarvam-ai-2/jobs/80711937-applied-ai-engineer-sarvam-agents), [Wipro Agentic AI Engineer](https://careers.wipro.com/job/Agentic-AI-Engineer/207412-en_US/). All were viewed 27 Nov 2026.

The qualitative language matters as much as the counts. Sarvam asks for "shipped AI features to real users in production, not just notebooks or prototypes". Vahan wants someone who "shipped an LLM-backed system in production, with real users, long enough for it to break". Vahan also says "every behaviour change ships behind a golden set and a regression gate" ([Vahan](https://www.ycombinator.com/companies/vahan/jobs/7zvIddz-lead-ai-engineer)). Whatfix lists LangChain, LlamaIndex, CrewAI and AutoGen only as "Good to Have". Its must-haves are LLM APIs, retrieval, agents and tool use, evaluation, and "Spec Driven development and coding agents such as Claude Code, Cursor or Copilot" ([Whatfix, 16 Nov 2026](https://to.indeed.com/aazjxf46s9zc)). Product companies screen for underlying capability and accept framework equivalents ("LangGraph, ADK, or equivalent"). Services firms list frameworks by name: 71% of their JDs name both LangChain and LangGraph. That is keyword matching, and it is the pattern a clean resume should not imitate.

## 6.2 SDE-2 JDs: frequency by company category (Sample B, any mention)

| Skill | All (n=41) | Required | Big Tech (13) | SaaS/MNC (16) | Indian product (6) | India startups (6) |
|---|---|---|---|---|---|---|
| Python | **63%** | 37% | 54% | 62% | 67% | 83% |
| Java | **61%** | 24% | 85% | 62% | 50% | 17% |
| AI/LLM product work (RAG, agents, LLM APIs) | **49%** | 20% | 46% | 50% | 33% | 67% |
| Kubernetes | 41% | 15% | 23% | 44% | 50% | 67% |
| CI/CD | 41% | 22% | — | — | — | — |
| System design | 41% | 37% | — | — | — | — |
| Distributed systems | 39% | 15% | — | — | — | — |
| Observability | 37% | 22% | — | — | — | — |
| Go | 34% | 15% | 8% | 50% | 33% | 50% |
| DSA | 32% | 29% | — | — | — | — |
| AI coding tools (Copilot, Cursor, Claude Code) | 32% | 22% | 23% | 31% | 50% | 33% |
| Docker | 32% | 12% | — | — | — | — |
| AWS / Azure / GCP | 32% / 27% / 24% | 5% / 7% / 2% | — | — | — | — |
| Microservices | 27% | 12% | — | — | — | — |
| PostgreSQL | 22% | 17% | 8% | 12% | 33% | 67% |
| Kafka | 22% | 5% | — | — | — | — |
| Redis | 20% | 10% | ~8% | ~6% | 33% | 67% |
| MongoDB | 17% | 7% | — | — | — | — |
| Spring Boot | 15% | 15% (always required when named) | — | — | — | — |
| React | 12% | 5% | — | — | — | — |
| MCP | 10% | — | — | — | — | — |
| Terraform / IaC | 10% | 7% | — | — | — | — |

Example sources: [Amazon SDE II](https://www.amazon.jobs/en/jobs/10611676/software-development-engineer-ii-icon), [Sarvam SDE2 API Platform](https://to.indeed.com/aa779t9klyz7), [Seekho SDE 2](https://to.indeed.com/aak8d4rrrgw9), [Adobe CS-I Java](https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist--I--Java-_R173771), [HackerRank](https://job-boards.greenhouse.io/hackerrank/jobs/7693789). All were viewed 27 Nov 2026.

Three findings from Sample B matter most for an AI engineer. First, **27% of SDE-2 JDs are language-agnostic**, mostly at Big Tech. Amazon's template asks for "at least one software programming language". So interviewing in Python carries no penalty. Second, **AI-coding-tool fluency has become a screening item**. Adobe makes "AI-assisted engineering, leveraging tools such as Claude, Codex, or Copilot" a must-have. Seekho says coding agents are "the baseline, not a perk … and we test that directly". HackerRank wants candidates who "have developed workflows and best practices around them" ([Seekho](https://to.indeed.com/aak8d4rrrgw9); [HackerRank](https://job-boards.greenhouse.io/hackerrank/jobs/7693789)). Third, about half of these "plain" SDE-2 roles are **AI-platform roles in disguise**: Microsoft Foundry and IQ, Google Model Armor, Databricks AI, Sarvam's LLM APIs. Their core is still distributed systems. Distributed-systems language recurs across startups: "idempotency, consistency trade-offs, what happens when the webhook arrives twice" (Seekho), and "SSE for Chat Completions … backpressure" (Sarvam).

## 6.3 Mandatory versus preferred

Required sections are short and generic. Named tools mostly sit under "preferred". This is the strongest evidence-based argument for a clean, non-sprawling resume. Breadth rarely gets a candidate past a screen. Depth in the core does.

| Skill | Mandatory share of mentions, Sample A | Required share of mentions, Sample B | Reading |
|---|---|---|---|
| Python | 36 / 38 (95%) | 15 / 26 (58%) | Hard gate for AI roles |
| Customer-facing ability | 10 / 12 | — | Hard gate for FDE (present in 73% of FDE JDs vs 3% of non-FDE) |
| Agents | 23 / 37 | — | Core |
| RAG | 21 / 31 | — | Core |
| Evals | 18 / 31 | — | Core |
| Any cloud | 20 / 25 | AWS 2 / 13 | One cloud required; which one rarely matters |
| System design | 9 / 13 | 15 / 17 | Required whenever named |
| DSA | 6 / 8 | 12 / 13 | Required whenever named; interviews test it even when the JD is silent |
| Spring Boot | — | 6 / 6 | Required when a team is Java-based |
| PostgreSQL | — | 7 / 9 | Startup and AI-platform gate |
| AI coding tools | 4 / 5 | 9 / 13 | Becoming a gate |
| LangChain / LangGraph | 11 / 18 · 8 / 15 | — | Usually "or equivalent" at product companies |
| Kubernetes / Docker | 5 / 10 · 5 / 11 | 6 / 17 · 5 / 13 | Mostly preferred |
| MCP | 2 / 9 | — | Mostly preferred or listed as a responsibility; mandatory at Sarvam and Wipro |
| Kafka | — | 2 / 9 | Preferred |
| CrewAI / LLM observability tools | 0 / 5 · 1 / 5 | — | Nice-to-have |

## 6.4 Cross-category intersection

The portable core is the set of skills that appears at substantial rates in **every** company category. In Sample A, three skills meet that bar: **agents (≥67% in every category), Python (≥56%) and evals (≥50%)**. Production observability and at least one named LLM framework reach ≥33% everywhere. RAG is high everywhere except the small Indian-product cell (20%, n=5). In Sample B, the skills present in all four categories are Python, Java, Kubernetes, Docker, CI/CD, observability, system design, DSA, Kafka, Redis, PostgreSQL, MongoDB, AI/LLM product work and AI coding tools. Of the 20 Sample B JDs that involve AI/LLM product work, **Python appears in 17**, Java in 12, Go in 6 and TypeScript in 2.

| Skill | FDE JDs (n=15) | Non-FDE AI JDs (n=34) | Implication |
|---|---|---|---|
| Customer-facing | 73% | 3% | The defining FDE filter |
| Agents | 87% | 71% | Core for both |
| RAG | 73% | 59% | Core for both |
| Evals | 73% | 59% | Core for both |
| Any cloud | 73% | 41% | FDEs deploy inside customer clouds |
| Observability | 67% | 38% | FDEs own production |
| System design | 20% | 29% | Tested as LLM system design and decomposition |
| DSA | **0%** | 24% | FDE JDs never state it, but FDE loops still keep one coding round (Section 16) |

The intersection gives a clear specification [E]. A **2–5 YOE AI engineer who works across all categories** ships Python production services, agents with tool calling used by real people, RAG with retrieval-quality evals, an eval and observability harness, and deployment on one major cloud. Specialisation sits on top of that core and depends on the target:

- **Big Tech:** DSA and distributed systems, plus MCP.
- **Startups:** voice/real-time, coding-agent fluency and fine-tuning.
- **FDE:** customer discovery, cloud architecture, and GCP/ADK where the employer is Google-aligned.
- **Services:** keyword coverage of LangChain/LangGraph and Docker/Kubernetes.

## 6.5 Experience floors: the binding constraint at 2 YOE

Counting the stated minimums gives a decisive result [E]. In Sample A, only **8 of 45 JDs (18%) set a minimum of 2 years or less**, and **18 of 45 (40%) set one of 3 years or less**. In Sample B the figures are **5 of 38 (13%)** at 2 years or less and **25 of 38 (66%)** at 3 years or less. Median minimums by category in Sample A are 5 years at Big Tech, Enterprise/GCC and services, 4 at Indian product companies, and 3 at AI startups and early-stage companies. These floors bend in practice:

- One LeetCode poster at 2 YOE reports an Amazon SDE-2 loop ([LeetCode](https://leetcode.com/discuss/post/7027366/amazon-sde-2-interview-experience-2yoe-h-ynf0/)).
- Sarvam's Agent Engineer JD says shipped work "matters more than years" ([Sarvam careers](https://www.sarvam.ai/careers/jobs/36f89b00-2010-4d23-aae3-17a2f53d9eaa)).
- Many startup "Senior" titles accept 3–5 years.

Even so, the numbers explain why this report splits applications into two waves. A move from 2 to 3 years of experience roughly **triples to quintuples the number of reachable JDs** in the SDE-2 band.

---
[Previous](../05%20Emerging%20Startup%20and%20Industry%20Landscape/05%20Emerging%20Startup%20and%20Industry%20Landscape.md) | [Index](../INDEX.md) | [Next](../07%20Technology%20Stack%20Demand%20Matrix/07%20Technology%20Stack%20Demand%20Matrix.md)
