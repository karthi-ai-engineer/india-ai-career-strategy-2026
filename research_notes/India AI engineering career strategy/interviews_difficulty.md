# Interview Processes, Difficulty and Interview-Readiness Timelines in India (SDE-2, AI/GenAI Engineer, MLE, MLOps/AI Infra, FDE/Solutions roles), 2025 to Nov 2026

Research date: 27 Nov 2026. Most loop-level evidence comes from anonymous, self-reported candidate posts (LeetCode Discuss, Glassdoor, Blind, LinkedIn) and third-party prep sites (Exponent/aced.io, Hello Interview, techinterview.org, Educative). Treat it as community anecdote unless marked "documented". Official company documentation was rarely available. Several LeetCode and igotanoffer pages returned HTTP 403, so some details rely on search-result summaries rather than full-page reads.

## 1. Interview loop structure by company (rounds, DSA level, LLD/HLD, behavioral, AI rounds)

### Takeaway
India product-company SDE-2 loops are converging on about 4 to 6 rounds: OA or DSA screen, then 1 to 2 DSA rounds (LeetCode medium, sometimes hard), a 90-minute LLD or machine-coding round (Flipkart, Swiggy, Razorpay, Atlassian "code design"), an HLD round, and a behavioral or hiring-manager round (Amazon LPs, Atlassian values, Google "Googleyness"). FDE loops (Palantir, OpenAI, Anthropic) replace part of the DSA with decomposition, learning or customer-simulation rounds, but keep at least one coding round.

### Cited Findings
**Amazon SDE-2 (India, 2025)**
- Reported loop: OA (2 DSA problems plus a work-style/LP questionnaire and work simulation), then Round 1 DSA+LP, Round 2 LLD+LP, Round 3 HLD+LP, and Round 4 Bar Raiser (DSA plus deep LPs). Each round is about 45 min technical plus 15 min on 2 LPs. — [LeetCode Discuss, Amazon SDE-2 Bangalore](https://leetcode.com/discuss/post/7132680/amazon-sde-2-bangalore-onsite-interview-pr26m/); [LeetCode, Amazon SDE-2 India](https://leetcode.com/discuss/post/6699329/amazon-sde-2-india-interview-experience-5gzeo/)
- Reported LLD prompts: meeting/room reservation, bus ticket booking, network request cache, file filter by size/extension, school management system. — [LeetCode, Amazon SDE-2 June 2025 Selected](https://leetcode.com/discuss/post/6923887/amazon-sde-2-interview-experience-select-rwpm/); [LeetCode, Amazon L5 Bangalore May 2025](https://leetcode.com/discuss/post/6961911/amazon-l5-sde-ii-bangalore-may-2025-reje-3mrx/)
- Down-levelling happens. One candidate got "SDE-2 loop, offered SDE-1." A 2 YOE candidate also posted an SDE-2 experience, which shows SDE-2 at around 2 YOE is possible but not the norm. — [LeetCode, Amazon India SDE-2 loop offered SDE-1](https://leetcode.com/discuss/post/6657524/offer-amazon-india-sde-2-loop-offered-sd-yn0n/); [LeetCode, Amazon SDE-2 2YOE Hyderabad](https://leetcode.com/discuss/post/7027366/amazon-sde-2-interview-experience-2yoe-h-ynf0/)

**Google L4 (Bangalore, 2025 to 2026)**
- Typical: recruiter screen, DSA screen (elimination), 2 to 3 onsite DSA rounds, and a Googleyness round, with an occasional domain round (for example Android). A Dec 2025 account had only 3 rounds (2 DSA plus 1 Googleyness). — [LeetCode, Google L4 Android Oct 2025 Offer](https://leetcode.com/discuss/post/7563717/title-google-l4-swe-iii-android-framewor-jb9v/); [LeetCode, Google L4 Bangalore 2025](https://leetcode.com/discuss/post/7240829/)
- Reported problems: graphs (topological sort plus BFS), binary tree DFS with optimisation follow-ups, grid/islands DFS. Interviewers push on complexity and optimisation (roughly medium to hard). — [LeetCode, Google L4 April 2025](https://leetcode.com/discuss/post/6713084/google-l4-experience-for-phone-screen-an-6eyt/); [LeetCode, Google L4 India Aug 2026 Reject](https://leetcode.com/discuss/post/8551877/google-l4-software-engineer-india-aug-20-zgn1/)
- A Google India L4 MLE loop exists as a separate track. — [LeetCode, Google India L4 MLE](https://leetcode.com/discuss/post/6910405/google-india-l4-mle-interview-experience-qnys/)
- One poster warned that using AI tools during Google online interviews "will not work". — summarised in search results from [LeetCode Google L4 posts](https://leetcode.com/discuss/post/8301524/google-interview-experience-l4-by-anonym-gjl3/)

**Atlassian P40 (about SDE-2; India, 2025)**
- Reported loop: Karat or DSA screen, a code design (LLD) round, a system design round, a management/strategic-execution round, and a values round. — [LeetCode, Atlassian P40 India Offer](https://leetcode.com/discuss/post/7070747/); [LeetCode, Atlassian P40 Bangalore Offer](https://leetcode.com/discuss/post/7196860/atlassian-p40-bangalore-interview-exp-of-xgp4/)
- The code design question is drawn from a small, known pool: Customer Satisfaction/agent ratings (addAgentRating, getSortedAgentRatingsList with tie-breakers and concurrency), Middleware Router (Trie), Snake game, Cost Explorer. — [LeetCode, Atlassian P40 Bangalore](https://leetcode.com/discuss/interview-experience/7196860); [LeetCode, Atlassian P40 Aug 2025 Hold](https://leetcode.com/discuss/interview-experience/7057047)
- The values round is STAR-format and mapped to Atlassian's 5 values. One offer-holder called it "the most difficult round." Another was rejected solely on the strategic-execution round for "low quality of situations." — [LeetCode, Atlassian P40 India](https://leetcode.com/discuss/post/7070747/atlassian-p40-india-offer-by-anonymous_u-6mbf/); [LeetCode, Atlassian P40 5 YOE](https://leetcode.com/discuss/post/7495920/)

**Flipkart SDE-2 (2025)**
- Machine coding: 90 min to build working code (sometimes after a 30-min briefing), then about 30 to 45 min to discuss and extend it. It is described as a knockout round. One Jan 2025 drive ran it as a group video call with around 60 candidates and a 50/70 cutoff before evaluation. — [LeetCode, Flipkart SDE-2 2025](https://leetcode.com/discuss/post/6933851/flipkart-sde-2-interview-experience-2025-gcq9/); [LeetCode, Flipkart SDE-2 July 2025](https://leetcode.com/discuss/post/7560534/); [Glassdoor Flipkart review](https://www.glassdoor.co.in/Interview/Flipkart-Interview-E300494-RVW95488008.htm)
- Reported prompts: flight management, property management, food ordering, Splitwise with groups. Graded on SOLID principles, design patterns and full requirement coverage. Rejections were attributed to "requirement gaps." — [LeetCode, Flipkart SDE-2](https://leetcode.com/discuss/post/7591327/flipkart-sde-2-interview-experience-by-a-cqjk/); [Glassdoor Flipkart](https://www.glassdoor.co.in/Interview/Flipkart-Interview-E300494-RVW92016185.htm)

**Swiggy SDE-2 (2025)**
- 90-min LLD/machine-coding round focused on "basic coding patterns and clean OO structuring." A Sept 2025 report included a hard DSA problem (shortest path with k hops). A July 2025 offer report included a bar-raiser round on project depth and architecture. Splitwise is a recurring historical prompt. — [LeetCode, Swiggy SDE 2](https://leetcode.com/discuss/post/8314817/swiggy-sde-2-by-anonymous_user-izkb/); [LeetCode, Swiggy SDE-2 July 2025 Offer](https://leetcode.com/discuss/post/7073156/); [LeetCode, Swiggy SDE-2 4 yrs](https://leetcode.com/discuss/post/7197132/swiggy-sde-2-interview-exp-4-yrs-exp-by-4wadv/)

**Razorpay SDE-2 / SSE (Dec 2024 to 2025)**
- Machine coding/LLD: rating system, in-memory Splitwise, survey service with category search (Java), "parking-lot level" difficulty. Working, extensible, modular code that meets every requirement is expected. — [Glassdoor Razorpay](https://www.glassdoor.com/Interview/Razorpay-Interview-E1146550-RVW86702348.htm); [LeetCode, Razorpay SSE Dec 2024 Offer](https://leetcode.com/discuss/post/6180241/)
- HLD prompts: design Zepto, a multi-traffic-type notification service, a task scheduler with callbacks/retries, a recurring-payments subscription platform, and an in-memory SQL DB. Rejections occur at HLD and the HM round. — [LeetCode, Razorpay SSE Bangalore Dec 2024](https://leetcode.com/discuss/post/6179716/razorpay-sse-bangalore-dec-2024-intervie-37t5/); [Glassdoor Razorpay](https://www.glassdoor.com/Interview/Razorpay-Interview-E1146550-RVW85483249.htm)

**Databricks (Bengaluru, 2024 to 2026)**
- Varies by level. One loop had 5 structured rounds. A senior loop had 2 system design (single box plus distributed), 1 coding and 2 behavioral/deep-dive. Another had DSA plus a 45-min CRUD app (Node/React). Spark/big-data questions appear. Timelines run from 2 weeks to 3 to 4 months. — [Glassdoor Databricks](https://www.glassdoor.co.in/Interview/Databricks-Interview-E954734-RVW102430837.htm); [Jointaro, Databricks Senior SWE Bengaluru June 2025](https://www.jointaro.com/interviews/companies/databricks/experiences/senior-software-engineer-bengaluru-june-1-2025-no-offer-negative-33abc191); [Glassdoor Databricks Senior Solution Architect](https://static.glassdoor.ca/Interview/Databricks-Senior-Solution-Architect-Interview-Questions-EI_IE954734.0,10_KO11,36.htm)

**Palantir FDSE / Deployment Strategist**
- Loop: 30-min recruiter call (screens hard for specific "why Palantir"), then a technical screen (CodePair/Karat live coding plus behavioral, or a HackerRank with coding, SQL and API tasks), then onsite of three 60-min rounds drawn from decomposition, learning, coding, re-engineering and system design, then a 60-min hiring-manager round that re-tests weak areas, makes the final decision and handles team matching. AI use is prohibited throughout. About 3 to 4 weeks, with a company average of around 28 days. — [aced.io (formerly Exponent) Palantir FDE guide](https://www.aced.io/guides/palantir-forward-deployed-engineer-interview)
- **Decomposition**: a vague real-world prompt (e.g. "improve NYC traffic", "sync two employee record systems"). You scope a buildable solution covering data, schemas and APIs, with little or no code. **Learning**: you get docs for an unfamiliar library or codebase (Python/Java/TS) and extend it in stages. Reasoning and question-led navigation are weighted over syntax. **Coding**: standard DS&A framed as a user feature, mostly maps, dictionaries and strings; graph- and tree-heavy problems are uncommon. **Re-engineering**: several hundred lines of unfamiliar code with planted bugs (e.g. HashMap double-count). **Behavioral**: about 15 to 20 min embedded in most rounds. — [aced.io Palantir FDE guide](https://www.aced.io/guides/palantir-forward-deployed-engineer-interview)
- **Deployment Strategist** pairs decomposition with a SQL-heavy technical round. Details vary by team. — [aced.io Palantir FDE guide](https://www.aced.io/guides/palantir-forward-deployed-engineer-interview)
- Accounts conflict. Some Glassdoor reviews describe mainly LeetCode-style coding, and one reports 6 rounds with rejection at the HM round. — [Glassdoor Palantir review](https://www.glassdoor.co.in/Interview/Palantir-Technologies-Interview-E236375-RVW103750275.htm); [Educative FDE course, no-AI rule](https://www.educative.io/courses/forward-deployed-engineer/the-hiring-process-stages-timeline-and-no-ai-rule)

**OpenAI FDE**
- No official loop has been published. Prep sites describe: resume screen, a 30-min recruiter call (why FDE specifically), an HM screen, a technical coding assessment, a decomposition/case study or customer-facing take-home, a project deep dive defending past design choices, coding plus system design, and a virtual onsite of 4 to 6 interviews over 1 to 2 days. Total time is 2 weeks to 2 months. — [Exponent OpenAI FDE guide](https://www.tryexponent.com/guides/openai-forward-deployed-engineer-interview); [Design Gurus](https://www.designgurus.io/answers/detail/what-is-the-openai-forward-deployed-engineer-interview-like-round-by-round); [Paraform, June 2026](https://www.paraform.com/insights/openai-forward-deployed-engineer); [Educative OpenAI FDE loop](https://www.educative.io/courses/forward-deployed-engineer/the-openai-fde-interview-loop)

**Anthropic Applied AI Engineer (about FDE)**
- Anthropic mostly uses the title "Applied AI Engineer" rather than FDE. Reported loops have 6 stages over 4 to 6 weeks, or 8 to 9 rounds: recruiter, HM, take-home, CodeSignal, coding, system design, bug-fixing, behavioral. A high CodeSignal score is "necessary but not sufficient." — [Educative Anthropic Applied AI guide](https://www.educative.io/courses/forward-deployed-engineer/interview-guide-anthropic-applied-ai-engineers); [Exponent Anthropic FDE guide](https://www.tryexponent.com/guides/anthropic-forward-deployed-engineer-interview); [Yale CDO blog, May 2026](https://cdo.som.yale.edu/blog/2026/05/18/get-a-job-at-anthropic-interview-process-and-top-questions/)
- One 2026 guide describes the Applied AI loop as recruiter, technical phone screen, take-home or live coding, **customer-conversation simulation**, and an onsite weighted to system design. The customer round "quietly rejects a large share of people" who passed coding. — [techinterview.org, July 2026](https://www.techinterview.org/post/3233476824/ai-engineer-interview-rag-agents-evals/)
- One Applied AI candidate's prep advice: enterprise AI deployment, hosting, security, governance, rollout strategy, stakeholder alignment, measurable business impact. — [Glassdoor Anthropic](https://www.glassdoor.co.in/Interview/Anthropic-Interview-E8109027-RVW104248322.htm)

**Sarvam AI (India)**
- Inferred loop with thin, mostly single-source evidence: recruiter screen; a hands-on Python/PyTorch build round (one account had about 2.5 hours to build a voice activity detector from scratch); a fundamentals and trade-offs round (transformers, speech/Indic, Bulbul TTS latent-space decomposition). One Blind account reports **no LeetCode-style DSA round**. An 84 LPA ML offer was reported anecdotally. — [techinterview.org Sarvam guide, Nov 2026](https://www.techinterview.org/post/3233477952/sarvam-ai-interview-guide/)
- Current Sarvam postings include Applied AI Engineer (Sarvam Agents), Agent Engineer, ML Engineer (Inference) and Backend (Samvaad). They emphasise LLM agents, MCP servers, evals and production experience. — [Sarvam careers](https://www.sarvam.ai/careers/jobs/db89b576-2456-4cc4-ab0b-c45f8c6c27f0); search summary of [Sarvam careers pages](https://www.sarvam.ai/careers/jobs/30259734-50c3-4f1c-81cd-8bff07e585e7)
- Glassdoor "SarvM.ai" reviews belong to a different company. — [techinterview.org Sarvam guide](https://www.techinterview.org/post/3233477952/sarvam-ai-interview-guide/)

### Inferences
- Proposed difficulty scores (1 to 10) for a ~2 YOE candidate, synthesised from the evidence above:
  - Google L4: 8 to 9. DSA-heavy, medium-hard to hard.
  - Amazon SDE-2: 7.
  - Atlassian P40: 7 to 8. The values round is a frequent rejector.
  - Flipkart SDE-2: 7. Machine coding is a knockout round.
  - Razorpay, Swiggy: 6 to 7.
  - Databricks: 8 to 9.
  - Palantir FDSE: 7 to 8. Lower DSA, high ambiguity.
  - OpenAI/Anthropic FDE/Applied AI: 9 to 10, mainly on selectivity and customer and system-design depth rather than algorithm difficulty.
  - Sarvam ML/Inference: 8 to 9 for ML depth. Agent/Applied roles are probably 6 to 7.
- These scores are my judgement, not sourced figures.
- For someone at 2 YOE, SDE-2 loops at Amazon/Google can end in a down-level to SDE-1/L3, so a target list should include companies whose SDE-2 bar is around 2 to 3 YOE (Razorpay, Swiggy, Atlassian P40 typically want 2 to 5 YOE).

### Gaps
- No reliable 2025 to 2026 India-specific loop data was retrieved for Microsoft, Uber, Salesforce, Adobe, NVIDIA, Rippling, CRED or PhonePe (not searched due to the tool-call budget). The general community pattern (2 to 3 DSA, LLD, HLD, HM) probably applies, but this is unverified.
- No official published loop for OpenAI or Anthropic FDE. Stage counts conflict across prep sites.
- No primary source on Palantir Deployment Strategist round details beyond "decomposition plus SQL".

## 2. What AI Engineer / GenAI / MLE interviews ask in 2025 to 2026, and AI-tool policies

### Takeaway
Applied-AI loops (4 to 5 rounds) now centre on RAG/agent system design, evaluation design (retrieval metrics, LLM-as-judge calibration), practical take-homes and debugging integrations. Only one round typically looks like classic algorithms. Meta's AI-assisted coding round (from Oct 2025) is the best-documented case of AI tools being allowed live. Most companies (Google, Palantir, most live rounds elsewhere) still prohibit AI tools.

### Cited Findings
- A typical 2026 applied-AI/LLM loop has 4 to 5 rounds, and only one resembles a classic algorithms interview. Live coding focuses on fixing an integration or debugging an agent (for example one that loops). — [techinterview.org, July 2026](https://www.techinterview.org/post/3233476824/ai-engineer-interview-rag-agents-evals/)
- Take-home examples:
  - Build a Q&A system over 50 markdown docs with a 20-question eval set and report recall@5 and faithfulness.
  - Build an automated eval scoring faithfulness and relevance over 30 I/O pairs, calibrated against human labels.
  - Eval take-homes are typically time-boxed to 2 to 4 hours.
  - One format gives a feature spec plus 4 hours to submit an eval design with no implementation.
  - — [techinterview.org](https://www.techinterview.org/post/3233476824/ai-engineer-interview-rag-agents-evals/); [techinterview.org eval roles 2026](https://www.techinterview.org/post/3233475313/interviewing-ai-eval-engineering-roles-2026/); [tianpan.co, Apr 2026](https://tianpan.co/blog/2026/04/27/ai-engineer-interview-eval-design)
- System-design prompts:
  - "Design a support assistant and explain how you'd know it helps rather than makes things worse."
  - Design eval plus serving around a model you don't control.
  - Agents: tracing multi-step runs, capping tool calls and spend, unsafe-action handling, an 800 ms end-to-end latency target.
  - RAG: chunking (fixed vs structure-aware), choosing k, when retrieval is the wrong tool.
  - An inference batching system for a single GPU (attributed to Anthropic).
  - — [techinterview.org](https://www.techinterview.org/post/3233476824/ai-engineer-interview-rag-agents-evals/); search summary of [dev.to AI Engineer playbook](https://dev.to/truongpx396/the-ai-engineer-interview-playbook-45pb)
- Eval knowledge expected: recall@k, precision@k, MRR/NDCG, faithfulness vs relevance, LLM-judge biases (length, position, self-preference), and calibrating judges to human labels before trusting them. — [techinterview.org](https://www.techinterview.org/post/3233476824/ai-engineer-interview-rag-agents-evals/)
- Classic ML whiteboard questions (gradient descent, bias-variance, training from scratch) "have largely been dropped" for LLM/RAG/agent roles. Research and ML-engineer loops at labs, and Sarvam-type model companies, still probe diagnosing models, messy data and transformer internals. — [techinterview.org](https://www.techinterview.org/post/3233476824/ai-engineer-interview-rag-agents-evals/); [techinterview.org Sarvam](https://www.techinterview.org/post/3233477952/sarvam-ai-interview-guide/)
- Common GenAI question areas: transformer mechanics, RAG vs fine-tuning, chunking/embeddings, hallucination mitigation, evaluation, agent design, cost/latency. RAG is "the most common GenAI pattern in Indian companies" (banks, edtech bots). Enterprise-PDF chatbot and multi-tenant RAG with guardrails and prompt injection are common design prompts. — [InterviewBit GenAI questions](https://www.interviewbit.com/varsity/blog/?p=127); [buildfastwithai RAG prep](https://www.buildfastwithai.com/ai-interview-prep/rag); [DataCamp RAG questions](https://www.datacamp.com/blog/rag-interview-questions)
- An Infosys GenAI interview (Mar 2026) focused on GenAI concepts, RAG and practical problem-solving. — [Glassdoor Infosys](https://www.glassdoor.co.in/Interview/Infosys-Interview-E7927-RVW103169118.htm)
- Hamel Husain says evals appear in a growing number of AI job descriptions and "can often be the 'weed out' part of interviews". He has helped design eval interview challenges at small and large companies. This is from his course sales page. — [Maven, Cracking the AI Evals Interview](https://maven.com/p/07e7c7/cracking-the-ai-evals-interview)
- Eugene Yan and Jason Liu (July 2024) list what an ML/AI loop should assess:
  - About 5 one-hour interviews.
  - Coding (30 to 60 min practical exercises; LeetCode is not mentioned).
  - Data literacy.
  - Comfort with opaque models and evals.
  - Science breadth, plus science depth (a past-project deep dive).
  - Open-ended science application.
  - STAR behavioral (ambiguity, influence, complexity, execution).
  - — [eugeneyan.com, How to Interview ML/AI Engineers](https://eugeneyan.com/writing/how-to-interview/)
- **Meta AI-enabled coding (documented by multiple outlets; details from prep sites):**
  - Rolling out from Oct 2025 for SWE/EM up to E7/M2. It replaces one of two onsite coding rounds; the other stays a traditional no-AI algorithm round.
  - 60 min in CoderPad with a built-in assistant. Reported model choices include GPT-4o mini, GPT-5, Claude Haiku/Sonnet 4/4.5, Opus 4, Gemini 2.5 Pro and Llama 4 Maverick. A LeetCode report says only lightweight models were selectable, so sources conflict.
  - Format: one multi-file problem in 3 phases (bug fix, core implementation of 120+ lines that is "harder than a LeetCode medium", optimisation for larger inputs).
  - Graded on problem solving, code quality, verification and communication. Over-reliance on the AI is a negative signal; prompt engineering is not assessed.
  - — [Hello Interview](https://www.hellointerview.com/blog/meta-ai-enabled-coding); [404 Media](https://www.404media.co/meta-is-going-to-let-job-candidates-use-ai-during-coding-tests/); [LeetCode, Meta AI Coding Round](https://leetcode.com/discuss/interview-experience/7335102); [interviewing.io](https://interviewing.io/blog/how-to-use-ai-in-meta-s-ai-assisted-coding-interview-with-real-prompts-and-examples)
- LinkedIn and Shopify have also published AI-enabled coding interview guides (titles only seen). — [Hello Interview related posts](https://www.hellointerview.com/blog/meta-ai-enabled-coding)
- AI-tool policy pattern: most live coding, system design and debugging interviews prohibit AI. Take-homes may allow it, often with disclosure. Palantir prohibits AI throughout. — search summary of [dev.to 2026 AI engineer interview](https://dev.to/rishi_kora/the-ai-engineer-interview-in-2026-live-coding-ai-assisted-rounds-eii); [aced.io Palantir](https://www.aced.io/guides/palantir-forward-deployed-engineer-interview); [Educative no-AI rule](https://www.educative.io/courses/forward-deployed-engineer/the-hiring-process-stages-timeline-and-no-ai-rule)

### Inferences
- For an AI Engineer/FDE background, the highest-leverage prep is three things together: a polished eval story ("how I knew a change didn't make things worse"), RAG/agent design with cost, latency and failure modes, and one production project deep dive.
- Transformer-internals depth (attention maths, KV cache, quantisation) is needed mainly for MLE/inference roles (Sarvam inference, NVIDIA, labs), not for applied/FDE roles.

### Gaps
- No India-specific dataset of GenAI interview questions. Most sources are global prep blogs.
- No confirmed list of India-based companies that allow AI assistants in live rounds.

## 3. Is DSA still required for AI Engineer and FDE roles in India? To what level?

### Takeaway
Yes, mostly. Big tech and Indian product companies keep 1 to 3 DSA rounds at LeetCode medium (sometimes hard) even for AI-flavoured SDE roles. FDE loops keep at least one practical DS&A round (Palantir: maps/strings, rarely graphs). Some AI-native startups (Sarvam) reportedly skip LeetCode in favour of hands-on builds, but this rests on single-source evidence.

### Cited Findings
- Google L4 India: 2 to 3 DSA rounds with graph, tree and DFS problems and optimisation follow-ups. — [LeetCode Google L4 posts](https://leetcode.com/discuss/post/7240829/)
- Amazon SDE-2: OA with 2 DSA problems plus a DSA round plus DSA in the Bar Raiser. — [LeetCode Amazon SDE-2](https://leetcode.com/discuss/post/7132680/amazon-sde-2-bangalore-onsite-interview-pr26m/)
- Palantir FDSE coding: "standard DS&A" framed as a user feature, mostly maps, dictionaries and strings, with graph- and tree-heavy problems uncommon. — [aced.io](https://www.aced.io/guides/palantir-forward-deployed-engineer-interview)
- Anthropic Applied AI includes a CodeSignal stage where a high score is necessary but not sufficient. — [Educative Anthropic guide](https://www.educative.io/courses/forward-deployed-engineer/interview-guide-anthropic-applied-ai-engineers)
- Applied-AI loops: only one of 4 to 5 rounds looks like classic algorithms. — [techinterview.org](https://www.techinterview.org/post/3233476824/ai-engineer-interview-rag-agents-evals/)
- Sarvam: one Blind account reports no LeetCode-style DSA round. The guide advises against dropping algorithm practice. — [techinterview.org Sarvam](https://www.techinterview.org/post/3233477952/sarvam-ai-interview-guide/)
- Meta keeps one traditional no-AI algorithm round even with the AI-assisted round. — [Hello Interview](https://www.hellointerview.com/blog/meta-ai-enabled-coding)

### Inferences
- Target level for an AI Eng/FDE at 2 YOE: reliably solve LeetCode mediums in about 30 min, plus the common patterns (hashing, two-pointer/sliding window, BFS/DFS, heaps, binary search, intervals, basic DP).
- Hard-level fluency matters mainly for Google, Databricks and some Flipkart/Swiggy DSA rounds.

### Gaps
- No quantitative survey of the share of Indian AI-startup loops that skip DSA.

## 4. System design expectations at ~2 YOE (SDE-2) in India: LLD machine coding and HLD

### Takeaway
At SDE-2 in India, LLD/machine coding is often the knockout round. You get 90 minutes to produce runnable, extensible, OO code (SOLID, design patterns, in-memory storage, all requirements met), followed by an extension discussion. HLD is expected at a moderate depth: classic product designs plus fintech/infra prompts (notification service, scheduler, subscriptions, quick-commerce).

### Cited Findings
- Flipkart: 90-min machine coding plus 30 to 45 min discussion, graded on SOLID, patterns and requirement coverage; a knockout round. — [LeetCode Flipkart SDE-2](https://leetcode.com/discuss/post/6933851/flipkart-sde-2-interview-experience-2025-gcq9/); [Glassdoor Flipkart](https://www.glassdoor.co.in/Interview/Flipkart-Interview-E300494-RVW95488008.htm)
- Swiggy: 90-min LLD/machine coding, "very straightforward", focused on clean OO. Splitwise historically took about 3 hours including explanation. — [LeetCode Swiggy SDE 2](https://leetcode.com/discuss/post/8314817/swiggy-sde-2-by-anonymous_user-izkb/)
- Razorpay: "parking-lot level" machine coding; HLD on Zepto, notifications, a scheduler with retries, subscriptions. — [Glassdoor Razorpay](https://www.glassdoor.com/Interview/Razorpay-Interview-E1146550-RVW86702348.htm); [LeetCode Razorpay SSE](https://leetcode.com/discuss/post/6179716/razorpay-sse-bangalore-dec-2024-intervie-37t5/)
- Atlassian: a code design round from a known problem pool, with concurrency and tie-breaker follow-ups. — [LeetCode Atlassian P40](https://leetcode.com/discuss/interview-experience/7196860)
- Amazon: separate LLD and HLD rounds, each with LPs attached. — [LeetCode Amazon SDE-2](https://leetcode.com/discuss/post/7132680/amazon-sde-2-bangalore-onsite-interview-pr26m/)
- Databricks senior loops split system design into "single box" and "distributed". — [Glassdoor Databricks](https://static.glassdoor.ca/Interview/Databricks-Senior-Solution-Architect-Interview-Questions-EI_IE954734.0,10_KO11,36.htm)

### Inferences
- The recurring machine-coding set is small and predictable: Splitwise, parking lot, food ordering, booking systems, rating system, Snake, rate limiter/cache. Practising about 10 to 15 of them end-to-end in Java or Python under a 90-min timer is likely enough at 2 YOE.
- For an AI-background candidate, AI-flavoured HLD (RAG platform, LLM gateway, eval pipeline) can be a differentiator at AI-heavy teams, but standard HLD remains the baseline at Flipkart, Swiggy and Razorpay.

### Gaps
- No source quantifies HLD depth expected at 2 YOE vs 4+ YOE in India.

## 5. Take-home and portfolio expectations for AI startups; value of open source, GitHub, blogs, Kaggle

### Takeaway
AI startups and labs commonly use 2 to 4 hour (sometimes longer) take-homes that build a RAG or eval system and report metrics, or hands-on model builds (Sarvam VAD in about 2.5 hours). Project deep dives defending past design choices appear in OpenAI FDE and Eugene Yan-style loops. Little hard data exists on how much GitHub, blogs or Kaggle move outcomes.

### Cited Findings
- RAG/eval take-homes with metric reporting, typically time-boxed at 2 to 4 hours. — [techinterview.org](https://www.techinterview.org/post/3233476824/ai-engineer-interview-rag-agents-evals/); [techinterview.org eval roles](https://www.techinterview.org/post/3233475313/interviewing-ai-eval-engineering-roles-2026/)
- OpenAI FDE: a customer-facing take-home plus a project deep dive defending past system design choices. — [Exponent OpenAI FDE](https://www.tryexponent.com/guides/openai-forward-deployed-engineer-interview); [Educative OpenAI loop](https://www.educative.io/courses/forward-deployed-engineer/the-openai-fde-interview-loop)
- Sarvam: a 2.5-hour from-scratch VAD build (single account). — [techinterview.org Sarvam](https://www.techinterview.org/post/3233477952/sarvam-ai-interview-guide/)
- Eugene Yan: "science depth" is a deep dive into a past project covering evaluation, trade-offs and outcomes. — [eugeneyan.com](https://eugeneyan.com/writing/how-to-interview/)

### Inferences
- One or two public, eval-instrumented projects (e.g. a RAG system with a published eval set and metrics, or an agent with tracing and cost caps) map directly onto what take-homes and deep dives test. They are likely more valuable than many shallow repos or Kaggle medals for Applied AI/FDE roles.

### Gaps
- No sourced data on how much open-source contributions, blogs or Kaggle rank affect Indian recruiter screens. Not found in this session.

## 6. Learning-time estimates to interview readiness

### Takeaway
Community estimates for DSA: NeetCode 150 takes about 4 to 6 weeks at 4 to 6 hours/day, or about 2 to 3 months part-time (evenings/weekends). Mid-level engineers are typically "ready" 1 to 2 months into serious prep, and total serious prep is commonly 3 to 4 months. No reliable sourced timelines were found for Go/Java, Kubernetes, PyTorch, fine-tuning or vLLM.

### Cited Findings
- NeetCode 150: 4 to 6 weeks at 4 to 6 h/day (full-time). 2 to 3 months in evenings and weekends. 3 to 5 months at a moderate pace. — [Educative NeetCode roadmap](https://www.educative.io/blog/neetcode-roadmap); [Educative, is NeetCode 150 enough](https://www.educative.io/blog/is-neetcode-150-enough-to-crack-tech-interviews)
- Pacing: full NeetCode 150 at 12 to 15 problems/week over an 8 to 12 week runway. — [techinterview.org study plan](https://www.techinterview.org/post/3233476075/coding-interview-study-plan-around-your-schedule/)
- Readiness: apply when you can consistently solve interview-level problems in 30 min. New grads are usually ready 2 to 3 months in, mid-level 1 to 2 months in. Serious prep overall is 3 to 4 months. — [techinterview.org prep timeline by level](https://www.techinterview.org/post/3233474686/interview-prep-timeline-by-level/); [dev.to realistic timelines](https://dev.to/alex_hunter_44f4c9ed6671e/how-long-does-it-take-to-prepare-for-coding-interviews-realistic-timelines-4a3n)
- The goal is to internalise about 15 to 20 core patterns rather than a raw count. — [techinterview.org patterns by frequency](https://www.techinterview.org/post/3233474682/leetcode-patterns-by-frequency/)
- Anecdote: 4 to 6 weeks to interview-ready (Blind). — [Blind](https://www.teamblind.com/post/how-long-practicing-leetcode-before-interview-ready-6vk43pvj)

### Inferences
- These timelines are my estimates, not sourced. For a full-time-employed engineer at about 10 to 12 h/week:
  - DSA (NeetCode 150, then about 250 to 300 total including company-tagged problems): about 4 to 6 months.
  - LLD machine coding: about 4 to 6 weeks (10 to 15 timed problems).
  - HLD fundamentals (DDIA plus Alex Xu Vol 1): about 6 to 8 weeks.
  - These can overlap, so about 6 to 8 months is a realistic total for big-tech SDE-2 readiness.
- Applied AI/FDE readiness for someone already doing AI Engineer/FDE work is probably shorter: about 2 to 3 months to formalise eval, RAG and agent design stories plus medium-level DSA.

### Gaps
- No sourced community estimates retrieved for Go or Java proficiency, Kubernetes (e.g. CKA/CKAD prep), PyTorch basics, LLM fine-tuning (LoRA/QLoRA) or vLLM/inference optimisation. Searches were not run due to the tool budget. The report-writer should flag these as estimates, not data.

## 7. Recommended prep resources

### Takeaway
DSA prep revolves around NeetCode 150/250 (and Striver A2Z in India). AI-engineer prep increasingly points to eval-specific material (Hamel Husain's evals course and "Cracking the AI Evals Interview"). Practitioner writing (Eugene Yan) shapes how AI loops are run.

### Cited Findings
- NeetCode 150 is a standard list. Sources compare it with Blind 75 and LeetCode Top 75. — [techinterview.org patterns compared](https://www.techinterview.org/post/3233474682/leetcode-patterns-by-frequency/); [Educative NeetCode 150 vs patterns](https://www.educative.io/blog/neetcode-150-vs-leetcode-patterns)
- Hamel Husain: an AI Evals course plus a free "Cracking the AI Evals Interview" lesson. — [Maven](https://maven.com/p/07e7c7/cracking-the-ai-evals-interview); [hamel.dev](https://hamel.dev); [Simon Willison on Hamel's evals FAQ, Jul 2025](https://simonwillison.net/2025/Jul/3/faqs-about-ai-evals/)
- Eugene Yan and Jason Liu, "How to Interview and Hire ML/AI Engineers" (Jul 2024). — [eugeneyan.com](https://eugeneyan.com/writing/how-to-interview/)
- FDE-specific prep courses exist (Educative: Palantir, OpenAI, Anthropic FDE guides). — [Educative FDE course](https://www.educative.io/courses/forward-deployed-engineer/interview-guide-palantir-forward-deployed-ai-engineers)
- Meta AI-coding prep: Hello Interview and interviewing.io guides. — [Hello Interview](https://www.hellointerview.com/blog/meta-ai-enabled-coding); [interviewing.io](https://interviewing.io/blog/how-to-use-ai-in-meta-s-ai-assisted-coding-interview-with-real-prompts-and-examples)

### Inferences
- These are widely cited in the community, but I did not verify them with a source in this session: Striver A2Z / Striver SDE sheet, Grokking (Design Gurus), Kleppmann's *Designing Data-Intensive Applications*, Alex Xu's *System Design Interview* Vols 1 and 2, Chip Huyen's *AI Engineering* (2025) and *Designing Machine Learning Systems* (2022), and Full Stack Deep Learning. Machine-coding prep in India commonly uses Splitwise, parking-lot and similar practice sets.

### Gaps
- No sourced comparative ranking of these resources was retrieved.

## 8. Resume and LinkedIn norms, referrals, notice periods and Japan experience (India)

### Takeaway
Notice periods are a material hiring friction in India: they are contractual, run from about 15 days at startups to 90 days at large firms, and recruiters increasingly filter on them. Buyouts are possible but need the current employer to agree. I found no sourced evidence in this session on keyword-stuffing norms, the value of referrals, or how Japan-based experience is viewed.

### Cited Findings
- Notice periods are contractual, not statutory. They range from about 15 days (startups) to 90 days (large companies, IT services). — [Instahyre blog](https://resources.instahyre.com/blog/notice-period-in-india/); [The People's Board](https://www.thepeoplesboard.com/hr-compliance/notice-period-in-india/)
- About 1 in 3 IT roles has a 90-day notice period. — [Analytics India Magazine](https://analyticsindiamag.com/ai-features/report-notice-periods-in-india-it)
- A July 2026 piece says recruiters increasingly use notice length as an early filter. It cites SHRM India figures of 28% offer dropout at GCCs and 38% at Indian product startups in 2025. These figures are secondary and unverified. — [The People's Board, 90-day debate](https://www.thepeoplesboard.com/hr-voices/the-90-day-notice-period-debate-is-it-hurting-indian-tech-hiring/)
- Buyouts: an example cost is about ₹3.75 lakh to buy out 90 days on a ₹15 LPA salary. The new employer may fund it, but the current manager must agree. — [thehirehub.ai](https://www.thehirehub.ai/blog/notice-period-buyout); [Blind, 90-day stuck India](https://www.teamblind.com/post/np-90-days-stuck-india-ysvczcjr)
- Interviewers in Palantir and Atlassian loops probe motivation and concrete situations hard. Generic "why us" answers and weak STAR stories are cited rejection reasons. — [aced.io Palantir](https://www.aced.io/guides/palantir-forward-deployed-engineer-interview); [LeetCode Atlassian P40](https://leetcode.com/discuss/post/7070747/)

### Inferences
- A candidate currently employed in Japan should check their own notice terms. Japanese employment norms often allow about 1 month (unverified here), which would be an advantage against Indian candidates on 60 to 90 days. They should state availability clearly on LinkedIn and in recruiter calls.
- A focused stack and narrative ("AI Engineer/FDE: RAG plus evals plus agents in production, Python plus one backend language") fits how AI loops are structured (deep dives, eval stories) better than broad keyword lists. This is reasoning, not a sourced claim.

### Gaps
- No sourced evidence retrieved on Indian recruiter views of keyword-stuffed resumes, ATS behaviour, referral conversion rates, or perception of Japan-based experience. These need separate research, e.g. r/developersIndia threads or recruiter posts.
- The People's Board/NASSCOM-style statistics on notice periods are secondary and partly unsourced.
