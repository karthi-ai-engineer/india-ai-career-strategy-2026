# India SDE-2 / Backend / Platform / AI-Platform JD Skill-Frequency Analysis (observed 2026-11-27)

## Q0. Sample, method, and biases (read first)

### Takeaway
I read and hand-coded 41 real India-located JDs for SDE-2-equivalent roles (backend, full-stack, platform/infra, distributed systems, AI platform), all viewed on 2026-11-27. Most are from Big Tech and global SaaS/product companies (29 of 41). Indian product companies and India startups make up only 12 of 41, and several named Indian unicorns could not be sampled at all. Read the percentages as directional, not as a census.

### Cited Findings
- **Sample size:** N = 41 in-scope JDs. By category: Big Tech (Google, Microsoft, Amazon, Adobe) 13; global SaaS/product MNC GCCs 16 (Databricks, MongoDB, Rubrik, Rippling, CrowdStrike, Cisco, Mastercard, Wayfair, Coinbase); Indian product companies 6 (Freshworks, HighRadius, InMobi, Zeta, HackerRank, Increff); India-based startups 6 (Sarvam ×3, Seekho, Triomics, Transak). Every JD and URL is listed in the Appendix below.
- **Observation date:** All 41 were viewed on 2026-11-27. Posting dates run from 2026-01-30 to 2026-11-26. Four postings are older than 6 months: Mastercard (2026-03-25), HackerRank (2026-03-20), Triomics (2026-04-22) and HighRadius (2026-01-30). Each ATS still listed them as open.
- **Sources used:**
  - Indeed connector, India cities (Bengaluru, Hyderabad, Pune, Gurugram, Chennai): 16 JDs with full text.
  - Official employer ATS endpoints with full text: Greenhouse (Databricks, MongoDB, Rubrik, Stripe, HackerRank, InMobi, HighRadius, Coinbase), Ashby (Sarvam, Snowflake), Lever (Zeta, Meesho, CRED, Paytm), Workday (Adobe, Salesforce), SmartRecruiters (Freshworks, Swiggy), amazon.jobs and Microsoft careers.
  - Example sources: [Databricks Infra](https://databricks.com/company/careers/open-positions/job?gh_jid=8829029002), [Adobe Workday](https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist--I--Java-_R173771), [amazon.jobs](https://www.amazon.jobs/en/jobs/10611676/software-development-engineer-ii-icon), [Microsoft careers](https://apply.careers.microsoft.com/careers/job/1970393557041515).
- **Indeed rate limit:** The Indeed connector rate-limited `get_job_details` after about 20 calls and never recovered during the session. About 15 more Indeed JDs whose listings I saw (NetApp, GitLab, eBay, Disney, Cars24, MetLife, Photon, Capgemini, Deloitte, Accenture) were therefore **not** read in full and are **not** counted.
- **Indian unicorns barely hiring mid-level backend on public boards (2026-11-27):**
  - Razorpay's Greenhouse board listed only 2 engineering roles ("Engineering Manager", "Frontend Engineer") out of 23 openings ([Razorpay Greenhouse board](https://job-boards.greenhouse.io/razorpaysoftwareprivatelimited/jobs/4712147005)).
  - Meesho's Lever board had only Engineering Manager and Security Engineer roles among 60 postings.
  - CRED's Lever board had one engineering-titled role, "fraud analytics engineer".
  - Swiggy's SmartRecruiters board (149 postings) had no SDE roles, only business, ops and one Staff Data Scientist.
  - Groww's referral board listed "Software Development Engineer - II (MF)" with no JD text ([Groww referral board](https://job-boards.eu.greenhouse.io/growwreferrals/jobs/4999264101)).
  - PhonePe Greenhouse job URLs returned 404. Zerodha's careers page did not render. Postman's Greenhouse pages returned 404.
  - Snowflake's India Ashby listings had no mid-level SWE roles, only Solution Engineers, an FDE, an EM and Cloud Support.
- **Excluded as out of band (seen but too senior):**
  - Stripe's 4 Bengaluru SWE postings all require 7–8+ years ([Stripe Payin](https://stripe.com/jobs/search?gh_jid=8185012); [Stripe Core Technology](https://stripe.com/jobs/search?gh_jid=7618977)).
  - Atlassian's only India Senior SE posting requires 8+ years of Kotlin/Java ([Atlassian TDP](https://careers-apac-atlassian.icims.com/jobs/26751/senior-software-engineer---trusted-data-platform/job?mode=apply)).
  - Others: Microsoft "Software Engineer II" requiring 7+ years ([MS 200063482](https://apply.careers.microsoft.com/careers/job/1970393557045750)); Rubrik Sr SE Enterprise AI (7+) ([Rubrik](https://www.rubrik.com/company/careers/departments/job.8273699?gh_jid=8273699)); Adobe Computer Scientist-II (7–9 years, C++) ([Adobe](https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist---II_R172286)).
- **Coding method:**
  - Each JD was hand-coded per skill as R (required/minimum qualification), P (preferred/nice-to-have), M (named in the team's stack or responsibilities, not as a qualification) or E (one example in an "any of X, Y, Z" language list).
  - "Any mention" = R+P+M+E. "Required" = R only.
  - Tallies are from my own coding script over these 41 JDs (Appendix).
- **Secondary corpus:** All 156 India-located engineering-titled postings in the downloaded ATS feeds were keyword-scanned, all levels (Databricks 39, MongoDB 31, Rubrik 19, Sarvam 17, HackerRank 12, Stripe 10, Zeta 10, Snowflake 7, Meesho 5, others). This corpus is not hand-checked, includes non-SDE titles, and Rubrik has 7 near-identical "Senior AI Engineer – Enterprise Agentic Systems" postings that inflate AI counts.

### Inferences
- **Bias 1, toward global companies:** 29/41 are MNC/Big Tech/global SaaS. Language and tooling percentages therefore lean toward Big Tech conventions: language-agnostic hiring, Java/C#/C++ named as examples, and Azure/AWS.
- **Bias 2, toward AI-heavy startups:** The startup bucket is dominated by Sarvam (3 of 6), an LLM company. This inflates Python, FastAPI, Go and AI counts in that bucket.
- **Bias 3, Indian product thinly covered:** The classic Indian product companies most associated with "SDE-2 Java/Go + Kafka + LLD rounds" (Flipkart, Swiggy, Razorpay, PhonePe, Meesho, Zomato) are missing. Kafka, Java/Go and HLD/LLD are probably under-counted for Indian product companies.
- **Hiring signal:** On 2026-11-27, several named Indian unicorns and two named SaaS companies (Stripe, Atlassian) had little or no public mid-level backend hiring. In-band India openings skewed toward Big Tech GCCs, global SaaS, and AI-native startups.

### Gaps
- No full JDs could be read for Flipkart, Swiggy, Zomato, PhonePe, CRED, Meesho, Groww, Zerodha, Postman, Razorpay (backend), Uber, LinkedIn, Walmart Global Tech, Goldman Sachs, Salesforce (no in-band India MTS role returned), ServiceNow, Confluent or Cloudflare.
  - Uber and Walmart pages need JavaScript or blocked automated fetches.
  - A LinkedIn guest-API query was denied by the environment's permission policy, so it was not pursued.
- IT services firms: only listing titles were seen, no full JD text (see Q13).

### Appendix: JD register (all viewed 2026-11-27)
| ID | Company | Category | Title | Location | Min YOE | Posted | URL |
|---|---|---|---|---|---|---|---|
| G1 | Google | Big Tech | Software Engineer II, Google Cloud | Hyderabad | 1 | 2026-11-23 | https://to.indeed.com/aa9bklnrtcsn |
| G2 | Google | Big Tech | Software Engineer II, AI Security (Model Armor) | Pune | 1 | 2026-11-24 | https://to.indeed.com/aassmm9djyx9 |
| MS3 | Microsoft | Big Tech | Software Engineer II (Core AI – Foundry Agentic Core Services) | Hyderabad (MS site: also Noida, Bangalore) | 3 | 2026-10-22 (Indeed) / 2026-11-15 (MS) | https://to.indeed.com/aaqt8sly8q49 ; https://apply.careers.microsoft.com/careers/job/1970393557041948 |
| MS4 | Microsoft | Big Tech | Software Engineer II (Microsoft Data Security) | Hyderabad | 4 | 2026-11-26 | https://to.indeed.com/aaykvwd4gqrt ; https://apply.careers.microsoft.com/careers/job/1970393557073551 |
| MS5 | Microsoft | Big Tech | Software Engineer II (Microsoft IQ) | Hyderabad | 5 | 2026-11-25 | https://apply.careers.microsoft.com/careers/job/1970393557047620 |
| MS6 | Microsoft | Big Tech | Applied AI Engineer II | Hyderabad | 3 | 2026-10-19 | https://apply.careers.microsoft.com/careers/job/1970393557041515 |
| A7 | Amazon | Big Tech | SDE II, Workplace Productivity | Hyderabad | 3 | 2026-09-29 | https://to.indeed.com/aahjj2snjxpx |
| A8 | Amazon | Big Tech | SDE II, Tax Services | Hyderabad | 3 | 2026-09-15 | https://to.indeed.com/aa9yq7q8yb6x |
| A9 | Amazon | Big Tech | SDE II (ACD Lifecycle) | Bengaluru | 3 | 2026-11-24 | https://www.amazon.jobs/en/jobs/10613545/software-development-engineer-ii |
| A10 | Amazon | Big Tech | SDE II, TFS | Bengaluru | 3 | 2026-09-08 | https://www.amazon.jobs/en/jobs/10531789/software-development-engineer-ii-tfs |
| A11 | Amazon | Big Tech | SDE II, ICON | Bengaluru | 3 | 2026-11-24 | https://www.amazon.jobs/en/jobs/10611676/software-development-engineer-ii-icon |
| AD12 | Adobe | Big Tech | Computer Scientist-I (Java), Document Cloud | Noida | 4 | 2026-11-23 | https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist--I--Java-_R173771 |
| AD13 | Adobe | Big Tech | Computer Scientist-I (Python), Document Cloud GenAI/ML | Noida | 5 | 2026-11-17 | https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist-I--Python-_R173660 |
| DB14 | Databricks | SaaS/MNC | Software Engineer, Infrastructure (IT CorpEng) | Bengaluru | 3 (3–5) | 2026-09-30 | https://databricks.com/company/careers/open-positions/job?gh_jid=8829029002 |
| DB15 | Databricks | SaaS/MNC | Sr Software Engineer – Agentic Applications (Full Stack) | Bengaluru | 5 | 2026-08-20 | https://databricks.com/company/careers/open-positions/job?gh_jid=8679982002 |
| DB16 | Databricks | SaaS/MNC | Sr. Software Engineer – Databricks AI | Bengaluru | 5 | 2026-11-02 | https://databricks.com/company/careers/open-positions/job?gh_jid=8924868002 |
| MG17 | MongoDB | SaaS/MNC | Software Engineer 3 (Ops Manager/Automation) | Gurugram | 4 | 2026-09-24 | https://www.mongodb.com/careers/job/?gh_jid=8208074 |
| MG18 | MongoDB | SaaS/MNC | Software Engineer 3 (Modernization frameworks) | Gurugram | 3 (3–4) | 2026-09-29 | https://www.mongodb.com/careers/job/?gh_jid=8239047 |
| MG19 | MongoDB | SaaS/MNC | Software Engineer 3 (Martech) | Gurugram | 3 | 2026-08-03 | https://www.mongodb.com/careers/job/?gh_jid=8083366 |
| MG20 | MongoDB | SaaS/MNC | Software Engineer 3, AI Framework Integrations | Gurugram | 3 | 2026-09-11 | https://www.mongodb.com/careers/job/?gh_jid=8127772 |
| RB21 | Rubrik | SaaS/MNC | Software Engineer – Cloud Native Protection | Bangalore | 2 | 2026-11-11 | https://www.rubrik.com/company/careers/departments/job.8327940?gh_jid=8327940 |
| RB22 | Rubrik | SaaS/MNC | Software Engineer (IAM, Golang) [duplicate Pune posting 7956918, 2026-08-31] | Bangalore | not stated | 2026-11-16 | https://www.rubrik.com/company/careers/departments/job.8349847?gh_jid=8349847 |
| RP23 | Rippling | SaaS/MNC | Software Engineer II (App Components) | Bengaluru | 3 | 2026-11-12 | https://to.indeed.com/aak7rvqqbt9x |
| CS24 | CrowdStrike | SaaS/MNC | Backend Engineer II (NG-SIEM Data Onboarding) | Pune | 4 | 2026-08-31 | https://to.indeed.com/aa4rvpnjssc9 |
| WF25 | Wayfair | SaaS/MNC (e-commerce GCC) | Software Engineer II – Java Backend (Customer Data Platform) | Bengaluru | 3 (3–5) | 2026-11-04 | https://to.indeed.com/aacqzg6fh9zl |
| MC26 | Mastercard | SaaS/MNC (fintech GCC) | Software Engineer II (Backend Developer) | Pune | not stated | 2026-03-25 | https://to.indeed.com/aat7hdgncrpp |
| CI27 | Cisco | SaaS/MNC | Software Engineer (AI & Full-Stack) | Bengaluru | 5 (3 with MS) | 2026-11-20 | https://to.indeed.com/aatktq786h9k |
| CB38 | Coinbase | SaaS/MNC (fintech) | Software Engineer, Security Platform | Remote – India | 3 | 2026-08-28 | https://www.coinbase.com/careers/positions/8165441?gh_jid=8165441 |
| CB39 | Coinbase | SaaS/MNC (fintech) | Senior Software Engineer – Data Platform | Remote – India | 5 | 2026-10-27 | https://www.coinbase.com/careers/positions/8325213?gh_jid=8325213 |
| SV28 | Sarvam | India startup | SDE2 – API Platform (LLM APIs) | Bengaluru | 3 | 2026-10-29 | https://to.indeed.com/aa779t9klyz7 ; https://jobs.ashbyhq.com/sarvam/fd9ca9f7-c546-4264-acc6-ee4e58c0e693 |
| SV29 | Sarvam | India startup | SDE2 – Full Stack (Cowork agent product) | Bengaluru | 3 | 2026-11-17 | https://jobs.ashbyhq.com/sarvam/fa96b55d-0c77-423d-8eef-f579c8496adb |
| SV30 | Sarvam | India startup | Software Engineer – Model API Platform | Bengaluru | 4 (4–6) | 2026-10-13 | https://jobs.ashbyhq.com/sarvam/0371342b-5cb8-487b-9310-4d0eb5b37f47 |
| SK31 | Seekho | India startup | SDE 2 – Backend Platforms | Bengaluru | not stated | 2026-10-05 | https://to.indeed.com/aak8d4rrrgw9 |
| TR33 | Triomics (posted via PinnacleU) | India startup | SDE 2 Backend | Bengaluru | 3 (3–5) | 2026-04-22 | https://to.indeed.com/aa2gdqzk8gr8 |
| TK34 | Transak | India startup (Web3 fintech) | Software Engineer, Backend (SDE1–EM; SDE2 ≈3–6 yrs) | Bengaluru | 3 | 2026-08-17 | https://to.indeed.com/aazdfcfbyy6q |
| IN32 | Increff | Indian product (retail SaaS) | SDE-II | Bengaluru | 2 (2–4; header 3–5) | 2026-09-15 | https://to.indeed.com/aaqhlhnbmf4s |
| HR35 | HackerRank | Indian product (SaaS) | Senior Backend Engineer | Bangalore (hybrid) | 3 (3–6) | 2026-03-20 | https://job-boards.greenhouse.io/hackerrank/jobs/7693789 |
| ZT36 | Zeta | Indian product (banking tech) | Site Reliability Engineer II | Bangalore | 2 | 2026-11-18 | https://jobs.lever.co/zeta/f827a249-2537-4f7f-aade-25b829fc13f2 |
| FW37 | Freshworks | Indian product (SaaS) | Lead Software Engineer – Full Stack (IC3) [upper boundary] | Chennai | 5 (5–8) | 2026-09-21 | https://jobs.smartrecruiters.com/Freshworks/744000150608630-lead-software-engineer-full-stack |
| HRD40 | HighRadius | Indian product (fintech SaaS) | Python SDE-III [upper boundary] | Hyderabad | 5 | 2026-01-30 | https://www.highradius.com/about/careers-list/?gh_jid=7490263003 |
| IM41 | InMobi | Indian product (adtech) | SDE II – AI | Bangalore | 3 (3–5) | 2026-07-20 | https://job-boards.greenhouse.io/inmobi/jobs/8073988 |

(IDs are labels only and are not consecutive; the table has 41 rows.)

## Q1. Languages (Java, Go, Python, TypeScript/Node, C++, Rust, Kotlin, Scala)

### Takeaway
Python and Java tie on overall frequency. Python is the most often **required** language (15/41 vs Java 10/41) and dominates AI-adjacent and startup JDs. Java dominates Big Tech and is the default for Spring Boot shops. Go is a strong third, concentrated in platform, infra and security teams at SaaS companies and startups. TypeScript/Node, Kotlin, Scala and Rust are marginal in this sample.

### Cited Findings
- **Overall counts (41 JDs, any mention / required):** Python 26 (63%) / 15 (37%); Java 25 (61%) / 10 (24%); Go 14 (34%) / 6 (15%); C++ 8 (20%) / 0; C# 8 (20%) / 2; JavaScript 6 (15%) / 1; TypeScript 4 (10%) / 1; Node.js 3 (7%) / 1; Scala 3 (7%) / 1; Ruby 2; Kotlin 1; Rust 1. Source: coded sample (Appendix).
- **Excluding "example-only" mentions:** Python 18/41 (44%), Java 16/41 (39%), Go 10/41 (24%), C# 4, TypeScript 2, Node 2, Scala 2, Rust 1, C++ 0, Kotlin 0. Every C++ mention in an in-band JD was an example in an any-of list, e.g. Google "Python, C, C++, Java, JavaScript" ([Google SE II Cloud](https://to.indeed.com/aa9bklnrtcsn)).
- **By category (any mention):**
  - Java: Big Tech 85%, SaaS/MNC 62%, Indian product 50%, India startups 17%.
  - Python: 54%, 62%, 67%, 83%.
  - Go: 8%, 50%, 33%, 50%.
- **11 of 41 JDs (27%) are language-agnostic** (no language named except as an example): Google ×2, Microsoft ×2, Amazon ×3, Rubrik CNP, HackerRank, Zeta, Freshworks. Amazon's template says "Experience programming with at least one software programming language" ([Amazon SDE II Tax](https://to.indeed.com/aa9yq7q8yb6x)). Stripe India says its "interview process is language agnostic" ([Stripe Core Technology](https://stripe.com/jobs/search?gh_jid=7618977), out of band).
- **Go as an explicit requirement:**
  - CrowdStrike: "Develop systems in Go"; "Fluency in at least one programming language, preferably Go" ([CrowdStrike Backend Engineer II](https://to.indeed.com/aa4rvpnjssc9)).
  - Rubrik IAM: "Strong hands-on programming skills in Golang" ([Rubrik SE IAM](https://www.rubrik.com/company/careers/departments/job.8349847?gh_jid=8349847)).
  - MongoDB: "4+ years experience with a language such as Java or GO" ([MongoDB SE3](https://www.mongodb.com/careers/job/?gh_jid=8208074)).
  - Sarvam: "Today it's FastAPI and Python; we're in the middle of rewriting it in Go" ([Sarvam SDE2 API Platform](https://to.indeed.com/aa779t9klyz7)).
- **Python + Go pairing:** Rippling wants "scalable backend services using Python and Golang" ([Rippling SE II](https://to.indeed.com/aak7rvqqbt9x)). Sarvam Model API wants "willingness to work in both Python and Golang" ([Sarvam Model API](https://jobs.ashbyhq.com/sarvam/0371342b-5cb8-487b-9310-4d0eb5b37f47)).
- **Java + Python pairing:**
  - Cisco requires "Strong programming skills in Java (Spring Boot, OOP) and Python" ([Cisco AI & Full-Stack](https://to.indeed.com/aatktq786h9k)).
  - Triomics: "Backend: Java / Spring Boot; AI Services: Python" ([Triomics SDE2](https://to.indeed.com/aa2gdqzk8gr8)).
  - Wayfair: "at least one backend programming language, such as Java or Python" ([Wayfair SE II](https://to.indeed.com/aacqzg6fh9zl)).
- **Co-occurrence in the sample:** Python & Java 15 JDs; Python & Go 11; Java & Go 7.
- **C# is Microsoft-specific:** "proficient in C# (Java or C++)" ([MS SE II Data Security](https://to.indeed.com/aaykvwd4gqrt)); "3+ years of software engineering experience in C# and/or Python" ([MS Applied AI Engineer II](https://apply.careers.microsoft.com/careers/job/1970393557041515)).
- **Scala:** appears as "Strong experience with backend technical stacks such as Scala or Java" ([Databricks AI](https://databricks.com/company/careers/open-positions/job?gh_jid=8924868002)).
- **Kotlin:** appears only for Sarvam's client apps ("Kotlin Multiplatform + Compose Multiplatform") ([Sarvam SDE2 Full Stack](https://jobs.ashbyhq.com/sarvam/fa96b55d-0c77-423d-8eef-f579c8496adb)).
- **Rust:** appears only as nice-to-have ("Working knowledge of Java, Go, C#, or Rust") ([MongoDB AI Framework Integrations](https://www.mongodb.com/careers/job/?gh_jid=8127772)).
- **Secondary corpus (156 India eng postings, all levels, keyword scan):** Python 54%, Go 33%, Java 28%, TypeScript/Node 13%, Scala 11% (mostly Databricks), C++ 10%, Rust 5%, Kotlin 1%. Source: ATS feeds listed in Q0, e.g. [Databricks](https://databricks.com/company/careers/open-positions/job?gh_jid=8829029002), [MongoDB](https://www.mongodb.com/careers/job/?gh_jid=8208074), [Sarvam](https://jobs.ashbyhq.com/sarvam/fa96b55d-0c77-423d-8eef-f579c8496adb).

### Inferences
- For Big Tech India SDE-2, the language rarely gates you. DSA and design do (see Q8). The language matters more at SaaS companies and startups, where Go and Python are named outright.
- Java's lower count at India startups is partly a sample artifact, since the Java-heavy unicorns are missing (Q0). Third-party search snippets suggest Swiggy SDE roles ask for Java/Go, but these were not verified as 2026 JDs ([foundit Swiggy SDE II](https://www.foundit.in/job/software-dev-engineer-ii-swiggy-bengaluru-bangalore-60469452), aggregator).

### Gaps
- Without Flipkart, Swiggy, PhonePe or Razorpay JDs, the Java vs Go split at Indian unicorns could not be measured.

## Q2. Backend frameworks (Spring Boot, FastAPI, Django, Node/NestJS, gRPC)

### Takeaway
Spring Boot is the only framework that recurs as a hard requirement: 6/41, all required, spread across Big Tech, SaaS/MNC, an Indian product company and a startup. Python frameworks (FastAPI, Django, Flask) appear in 5 JDs, mostly at startups and Indian SaaS. Node/NestJS and gRPC are rare.

### Cited Findings
- **Counts (any / required):** Spring Boot 6 / 6; FastAPI 2 / 1; Django 2 / 0; Flask 1 / 1; Node.js as a framework 3 / 1; gRPC 0 in band. Source: coded sample.
- **Spring Boot as a hard requirement:**
  - Adobe: "Proficiency in Java and J2EE, including deploying, monitoring, and troubleshooting Spring Boot services" ([Adobe CS-I Java](https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist--I--Java-_R173771)).
  - Triomics: "Java and Spring Boot, strong proficiency is non-negotiable" ([Triomics](https://to.indeed.com/aa2gdqzk8gr8)).
  - Increff: "Strong fundamentals in [Java / Spring Boot]" ([Increff SDE-II](https://to.indeed.com/aaqhlhnbmf4s)).
  - MongoDB: "Strong Spring Boot ... MongoDB ... and JDBC/JPA skills required" ([MongoDB SE3 Modernization](https://www.mongodb.com/careers/job/?gh_jid=8239047)).
  - Also Mastercard ([Mastercard SE II](https://to.indeed.com/aat7hdgncrpp)) and Cisco ([Cisco](https://to.indeed.com/aatktq786h9k)).
- **Python frameworks:**
  - FastAPI: "Strong Python in production: asyncio, FastAPI or similar" ([Sarvam SDE2 API](https://to.indeed.com/aa779t9klyz7)).
  - Django: "existing systems are Django" ([Seekho](https://to.indeed.com/aak8d4rrrgw9)); "Python, Django, Golang, MongoDB, and AWS is highly preferred" ([Rippling](https://to.indeed.com/aak7rvqqbt9x)).
  - Flask: "Extensive experience with Flask and its ecosystem" ([HighRadius Python SDE-III](https://www.highradius.com/about/careers-list/?gh_jid=7490263003)).
- **Node.js:** "Strong hands-on experience building APIs with Node.js" ([Transak](https://to.indeed.com/aazdfcfbyy6q)).
- **gRPC:** appears only in out-of-band JDs: Stripe ("gRPC, GraphQL, Docker and Kubernetes") ([Stripe FBI](https://stripe.com/jobs/search?gh_jid=7543868)) and Atlassian ([Atlassian TDP](https://careers-apac-atlassian.icims.com/jobs/26751/senior-software-engineer---trusted-data-platform/job?mode=apply)).
- **LLM-app frameworks function as "backend frameworks" in AI-platform JDs:** LangChain/LangGraph appear in 3 JDs ([Databricks Agentic](https://databricks.com/company/careers/open-positions/job?gh_jid=8679982002); [Cisco](https://to.indeed.com/aatktq786h9k); [InMobi SDE II AI](https://job-boards.greenhouse.io/inmobi/jobs/8073988)).

### Inferences
- If one framework is worth listing for Java-track India roles, it is Spring Boot. For Python-track AI-platform roles, FastAPI (async) plus an LLM orchestration framework is the closest equivalent.

### Gaps
- No NestJS mentions in band. GoKwik's SDE II listing (Node/NestJS + Go + Kafka) was seen only as a search snippet and requires 8–10 years ([hirist GoKwik](https://www.hirist.tech/j/gokwik-software-development-engineer-ii-backend-technologies-1673132?jobPos=4)).

## Q3. Event-driven / messaging, microservices, API design

### Takeaway
Kafka is the most named broker (9/41 any, 22%), but it is usually preferred rather than required (2/41 required). Microservices (27%) and distributed-systems fundamentals (39%) are more common than any specific broker. API-contract design is called out explicitly by platform-type teams.

### Cited Findings
- **Counts (any / required):** Kafka 9 / 2; RabbitMQ 5 / 3; SQS 2 / 0; generic "event-driven" 4 / 2; Pulsar 0; microservices 11 / 5; distributed systems 16 / 6. Source: coded sample.
- **Kafka required:**
  - CrowdStrike: "Experience with at least one streaming system like Apache Kafka, Rabbit MQ" ([CrowdStrike](https://to.indeed.com/aa4rvpnjssc9)).
  - HackerRank: "asynchronous messaging (Kafka/RabbitMQ), and event-driven architectures" ([HackerRank](https://job-boards.greenhouse.io/hackerrank/jobs/7693789)).
- **Kafka preferred:**
  - Wayfair: "Kafka, Spark, Dataflow, Airflow or BigQuery" ([Wayfair](https://to.indeed.com/aacqzg6fh9zl)).
  - Adobe: "Kafka, RabbitMQ, SQS/Service Bus, and event-driven operations" ([Adobe CS-I Java](https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist--I--Java-_R173771)).
  - Triomics: "Kafka, RabbitMQ, or similar" ([Triomics](https://to.indeed.com/aa2gdqzk8gr8)).
- **Kafka as team stack:** "Kafka, Flink, and AWS" ([Rippling](https://to.indeed.com/aak7rvqqbt9x)).
- **API design and distributed-correctness language:**
  - Seekho: "API design as a first-class skill — contracts, versioning, backwards compatibility, deprecation"; "idempotency, consistency trade-offs, what happens when the webhook arrives twice" ([Seekho](https://to.indeed.com/aak8d4rrrgw9)).
  - Transak: "consistency, idempotency, retries, and failure handling" ([Transak](https://to.indeed.com/aazdfcfbyy6q)).
  - Sarvam Full Stack: "async processing, queues or event streams, idempotency, retries" ([Sarvam SDE2 Full Stack](https://jobs.ashbyhq.com/sarvam/fa96b55d-0c77-423d-8eef-f579c8496adb)).
- **Streaming protocols for LLM platforms (SSE/WebSockets):** "SSE for Chat Completions and Responses, long-lived connections ... backpressure" ([Sarvam SDE2 API](https://to.indeed.com/aa779t9klyz7)).
- **Durable workflow engines:** Temporal appears at Triomics and Sarvam ([Triomics](https://to.indeed.com/aa2gdqzk8gr8); [Sarvam Full Stack](https://jobs.ashbyhq.com/sarvam/fa96b55d-0c77-423d-8eef-f579c8496adb)).
- **Secondary corpus:** Kafka in 21/156 (13%) India eng postings across ATS feeds (e.g. [Databricks](https://databricks.com/company/careers/open-positions/job?gh_jid=8829029002)).

### Inferences
- Interview-relevant knowledge is broker-agnostic: idempotency, retries, backpressure, consistency. Kafka is the safest single broker to know. For AI-platform roles, SSE/WebSocket streaming and durable workflows (Temporal) are emerging differentiators.

### Gaps
- Pulsar and SQS-as-requirement were not observed in band. Indian unicorns' Kafka usage could not be measured (Q0).

## Q4. Frontend (React, Next.js, TypeScript) in full-stack roles

### Takeaway
Frontend skills appear in only 7/41 JDs. Where they appear, React is the framework (5/41). Full-stack SDE-2 roles in this sample are "backend-heavy full stack": React is required alongside a Python, Java or Node backend, not instead of it.

### Cited Findings
- **Counts (any / required):** React 5 / 2; Next.js 1 / 0 (any-of option); TypeScript as frontend 2; generic "frontend fundamentals" 2 / 2. Source: coded sample.
- **React required:**
  - Rippling: "Comfortable in writing and shipping production code in React and React Native" in a backend-primary role ([Rippling](https://to.indeed.com/aak7rvqqbt9x)).
  - Databricks: "strong expertise in Python and React.js" ([Databricks Agentic Full Stack](https://databricks.com/company/careers/open-positions/job?gh_jid=8679982002)).
- **Backend-heavy full stack:** "The role is full stack, but the centre of gravity is the backend" (web: "Next.js, React, TypeScript") ([Sarvam SDE2 Full Stack](https://jobs.ashbyhq.com/sarvam/fa96b55d-0c77-423d-8eef-f579c8496adb)).
- **Generic frontend required:**
  - Increff: "Good-to-moderate understanding of frontend development and UI fundamentals" ([Increff](https://to.indeed.com/aaqhlhnbmf4s)).
  - Freshworks: "modern frontend development frameworks" ([Freshworks Lead FS](https://jobs.smartrecruiters.com/Freshworks/744000150608630-lead-software-engineer-full-stack)).
- **Frontend preferred:** "Angular 2 or modern SPA frameworks such as React + Redux ... Typescript" ([Mastercard](https://to.indeed.com/aat7hdgncrpp)). MongoDB lists "Javascript/React" in its team languages ([MongoDB SE3](https://www.mongodb.com/careers/job/?gh_jid=8208074)).
- **Frontend-only SDE-II (not counted):** Groww's "Web Developer - SDE II" requires "ReactJS, NextJS, Typescript, JavaScript" and 3+ years ([Groww](https://groww.sensehq.com/careers/jobs/54557)). It is undated and frontend-only, so it is excluded.

### Inferences
- For a backend/AI-leaning engineer, "React + TypeScript at a working level" is the add-on that unlocks full-stack AI-product roles (agent UIs, BFFs) without a career switch.

### Gaps
- Postman, a classic Node/TypeScript full-stack employer in India, could not be sampled (Greenhouse 404s).

## Q5. Databases

### Takeaway
PostgreSQL is the most frequently required database (7/41 required, 9 any). Redis is the most common cache (8 any). MongoDB is common at SaaS companies and in Node/Python stacks. Big Tech JDs rarely name databases. Elasticsearch, Cassandra and ClickHouse are near-absent in band.

### Cited Findings
- **Counts (any / required):** PostgreSQL 9 / 7; Redis 8 / 4; MongoDB 7 / 3; MySQL 3 / 2; DynamoDB 2 / 0; Oracle 2 / 2; Cosmos DB 2 / 1; Elasticsearch 2 / 0; Cassandra 0; ClickHouse 0; vector DB 1 (P). Source: coded sample.
- **By category:** Postgres any-mention is 67% for India startups, 33% Indian product, 12% SaaS/MNC, 8% Big Tech. Redis: 67% startups, 33% Indian product, ~6–8% elsewhere.
- **Examples:**
  - Sarvam: "Strong PostgreSQL and Redis fundamentals: schema design, query performance, caching, and rate limiting" ([Sarvam SDE2 API](https://to.indeed.com/aa779t9klyz7)).
  - Triomics: "PostgreSQL ... SQL, query optimization, schema design, indexing" ([Triomics](https://to.indeed.com/aa2gdqzk8gr8)).
  - HackerRank: "relational databases (PostgreSQL, MySQL) and NoSQL stores" ([HackerRank](https://job-boards.greenhouse.io/hackerrank/jobs/7693789)).
  - Adobe preferred: "PostgreSQL/RDS, DynamoDB/MongoDB, and Redis" ([Adobe CS-I Java](https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist--I--Java-_R173771)).
  - Microsoft AI roles name Cosmos DB for RAG: "Build retrieval-augmented generation (RAG) solutions using technologies such as Azure Cosmos DB and semantic search" ([MS SE II Microsoft IQ](https://apply.careers.microsoft.com/careers/job/1970393557047620)).
  - Vector DB: "vector databases (e.g., Weaviate)" preferred ([Cisco](https://to.indeed.com/aatktq786h9k)); "Integrate vector databases for semantic search, contextual retrieval, RAG" ([InMobi](https://job-boards.greenhouse.io/inmobi/jobs/8073988)).
  - Elasticsearch is good-to-have at Triomics ([Triomics](https://to.indeed.com/aa2gdqzk8gr8)).

### Inferences
- PostgreSQL + Redis is the highest-yield database pair for India startup and AI-platform roles. Postgres also hosts pgvector-style retrieval, though no sampled JD named pgvector.

### Gaps
- Cassandra and ClickHouse demand (typical at Swiggy, Zomato, Flipkart scale) could not be assessed.

## Q6. Cloud / DevOps / observability

### Takeaway
Kubernetes (17/41, 41%) and CI/CD (17/41) are the most common infra terms. Observability is named in 15/41 (37%) and is required in 9. Specific clouds are usually "any of AWS/GCP/Azure" (AWS 32%, Azure 27%, GCP 24%). Terraform and IaC are platform-role-specific (10%). Prometheus/Grafana are named in only 3, and OpenTelemetry in 0 in-band JDs.

### Cited Findings
- **Counts (any / required):** K8s 17 / 6; Docker 13 / 5; CI/CD 17 / 9; observability (logging/metrics/tracing/monitoring/SLOs) 15 / 9; AWS 13 / 2; Azure 11 / 3; GCP 10 / 1; Terraform/IaC 4 / 3; Prometheus/Grafana 3 / 1; OpenTelemetry 0. Source: coded sample.
- **K8s any-mention by category:** India startups 67%, Indian product 50%, SaaS/MNC 44%, Big Tech 23%.
- **Platform/infra role profiles:**
  - Databricks Infra: "Terraform (modules, state management) or Pulumi"; "AWS ... Kubernetes and Docker"; "GitHub Actions"; "Datadog, Prometheus, or Grafana" ([Databricks SE Infrastructure](https://databricks.com/company/careers/open-positions/job?gh_jid=8829029002)).
  - Zeta: "K8s, envoy, API gateway (Kong or Ambassador or Traefik), Service Mesh (istio ...)", "Terraform, Ansible" ([Zeta SRE II](https://jobs.lever.co/zeta/f827a249-2537-4f7f-aade-25b829fc13f2)).
- **K8s in product backend roles:** "Comfort running services on Kubernetes in production" ([Sarvam SDE2 API](https://to.indeed.com/aa779t9klyz7)); "Production experience on Kubernetes or a similar platform, with observability you actually used to debug an incident" ([Sarvam Full Stack](https://jobs.ashbyhq.com/sarvam/fa96b55d-0c77-423d-8eef-f579c8496adb)).
- **Big Tech cloud framing:** "In-depth knowledge of cloud development (Azure, AWS, Google Cloud)" ([MS SE II Data Security](https://to.indeed.com/aaykvwd4gqrt)). Amazon ICON: "Hands-on experience with AWS (e.g. Lambda, EC2, DynamoDB, S3, Step Functions, SQS/SNS) and infrastructure-as-code (CDK, CloudFormation)" ([Amazon SDE II ICON](https://www.amazon.jobs/en/jobs/10611676/software-development-engineer-ii-icon)).
- **OpenTelemetry appears only outside the in-band sample:**
  - Rubrik Sr SE (7+): "Prometheus, Grafana, Datadog, OpenTelemetry" ([Rubrik Enterprise AI](https://www.rubrik.com/company/careers/departments/job.8273699?gh_jid=8273699)).
  - HighRadius SRE (7+): "Hands-on experience implementing OpenTelemetry" ([HighRadius SRE](https://www.highradius.com/about/careers-list/?gh_jid=7107816003)).
  - Atlassian (8+): "Terraform, CloudWatch, Prometheus, and OpenTelemetry" ([Atlassian TDP](https://careers-apac-atlassian.icims.com/jobs/26751/senior-software-engineer---trusted-data-platform/job?mode=apply)).
- **Secondary corpus:** Kubernetes in 53/156 (34%) India eng postings (ATS feeds; e.g. [MongoDB](https://www.mongodb.com/careers/job/?gh_jid=8208074)).

### Inferences
- "Ran it on K8s in production and debugged it with logs/metrics/traces" is a near-universal mid-level expectation outside Big Tech. Named tools (Prometheus/Grafana/OTel) become explicit at senior and SRE levels.

### Gaps
- Too few infra-titled in-band JDs (Databricks Infra, Zeta SRE II) to profile Cloud/Infrastructure roles separately with confidence.

## Q7. Experience requirements

### Takeaway
"3+ years" is the modal SDE-2 floor (20 of 38 JDs that state YOE). The range is 1+ (Google SE II) to 5+ (several "SE II/Sr" roles). Several "II" titles at Microsoft, and all of Stripe and Atlassian India, require far more.

### Cited Findings
- **Distribution of minimum YOE (38 stating YOE):** 1 yr ×2, 2 yrs ×3, 3 yrs ×20, 4 yrs ×5, 5 yrs ×8. Three JDs state none (Rubrik IAM, Mastercard, Seekho). Source: coded sample.
- **Google SE II:** "1 year of experience with software development ... 1 year of experience with data structures and algorithms" ([Google SE II Cloud](https://to.indeed.com/aa9bklnrtcsn)).
- **Amazon SDE II:** "3+ years of non-internship professional software development experience; 2+ years of non-internship design or architecture" ([Amazon SDE II Workplace](https://to.indeed.com/aahjj2snjxpx)).
  - Template anomaly: three India SDE II postings list "3+ years of Video Games Industry ... experience" as a basic qualification, which looks like a template error (Chennai Books/AbeBooks; Bengaluru compliance; ICON) ([Amazon ICON](https://www.amazon.jobs/en/jobs/10611676/software-development-engineer-ii-icon); [Amazon 10581088](https://www.amazon.jobs/en/jobs/10581088/software-development-engineer-ii)).
  - One AWS Infrastructure Services SDE II requires 5+ years ([Amazon 10560180](https://www.amazon.jobs/en/jobs/10560180/software-development-engineer-ii)).
- **Microsoft "Software Engineer II" varies widely:** 3+ ([MS Core AI](https://apply.careers.microsoft.com/careers/job/1970393557041948)), 4+ ([MS Data Security](https://apply.careers.microsoft.com/careers/job/1970393557073551)), 5+ ([MS IQ](https://apply.careers.microsoft.com/careers/job/1970393557047620)), and one at 7+ ([MS 200063482](https://apply.careers.microsoft.com/careers/job/1970393557045750)).
- **MongoDB "Software Engineer 3" (its mid level):** 3+ to 4+ years ([MongoDB SE3](https://www.mongodb.com/careers/job/?gh_jid=8208074); [MongoDB SE3 Modernization](https://www.mongodb.com/careers/job/?gh_jid=8239047)).
- **Startup SDE2 bands:** "3+ years (SDE 2) or 5+ years (SDE 3)" ([Sarvam Full Stack](https://jobs.ashbyhq.com/sarvam/fa96b55d-0c77-423d-8eef-f579c8496adb)); "Software Development Engineer 2 (about 3–6 years)" ([Transak](https://to.indeed.com/aazdfcfbyy6q)); "2–4 years" ([Increff](https://to.indeed.com/aaqhlhnbmf4s)).
- **"Senior" at Indian SaaS can mean 3–6 years:** "Senior backend engineer with 3-6 years of experience" ([HackerRank](https://job-boards.greenhouse.io/hackerrank/jobs/7693789)).

### Inferences
- A 2–5 YOE engineer fits Amazon, Microsoft (some), Google, MongoDB, Rubrik and startup SDE2 bands. Titles are not comparable across companies, so filter on stated YOE, not on title.

### Gaps
- None material for this sample.

## Q8. System design (HLD/LLD) and DSA expectations

### Takeaway
System or architecture design is explicitly required in 15/41 (37%) and DSA in 12/41 (29%). Explicit "HLD/LLD" wording appears only at Indian product companies (Increff, Freshworks). Big Tech encodes design as YOE ("2+ years design or architecture").

### Cited Findings
- **Counts (any / required):** system design 17 / 15; DSA 13 / 12; HLD/LLD explicit 2 / 1. Source: coded sample.
- **Amazon:** every India SDE II sampled requires "2+ years of non-internship design or architecture (design patterns, reliability and scaling)" ([Amazon SDE II Tax](https://to.indeed.com/aa9yq7q8yb6x)).
- **Google:** "1 year of experience with data structures and algorithms" is a minimum qualification ([Google SE II AI Security](https://to.indeed.com/aassmm9djyx9)).
- **Explicit HLD/LLD:**
  - Increff: "Write HLDs/LLDs"; "System design ability — you can defend your choices and name what you traded away" ([Increff](https://to.indeed.com/aaqhlhnbmf4s)).
  - Freshworks: "System Design (HLD/LLD): Proven capability to design scalable, highly available, and fault-tolerant end-to-end multi-tenant systems" and "Strong expertise in Data Structures, Algorithms (DSA)" ([Freshworks](https://jobs.smartrecruiters.com/Freshworks/744000150608630-lead-software-engineer-full-stack)).
- **DSA + system design in AI roles:** "Understanding of data structures, algorithms, and system design fundamentals" ([MS Applied AI Engineer II](https://apply.careers.microsoft.com/careers/job/1970393557041515)); "Strong foundation in algorithms, data structures, and system design" ([Databricks AI](https://databricks.com/company/careers/open-positions/job?gh_jid=8924868002)).
- **Interview-loop evidence (third-party, not JDs):** A Groww SDE-II loop (July 2025) had DSA, a 2-hour machine-coding round (Splitwise) and HLD ([LeetCode Groww](https://leetcode.com/discuss/post/7046387/groww-sde-ii-bengaluru-july25-by-anonymo-sqwx/)). A Flipkart summary cites machine coding, DSA, LLD and techno-managerial rounds (aggregated search snippet, not verified).

### Inferences
- JDs understate DSA/LLD. Indian product companies test them via machine-coding and LLD rounds even when the JD does not say so.
- Design-doc writing ("RFCs before code") is increasingly explicit at startups ([Sarvam](https://to.indeed.com/aa779t9klyz7)).

### Gaps
- No 2026 Flipkart, Swiggy or PhonePe JD text to confirm LLD wording.

## Q9. Mandatory vs preferred

### Takeaway
Required lists are short and generic: YOE, one language, design/DSA, production ownership. Specific technologies mostly sit in "preferred". The exceptions are Spring Boot (always required when named), PostgreSQL (7/9 required) and AI-coding-tool fluency (9/13 mentions required).

### Cited Findings
- **Required share of mentions (coded sample):**
  - Spring Boot 6/6
  - PostgreSQL 7/9
  - system design 15/17
  - DSA 12/13
  - AI coding tools 9/13
  - CI/CD 9/17
  - observability 9/15
  - Kubernetes 6/17
  - Docker 5/13
  - Kafka 2/9
  - AWS 2/13
  - AI/LLM product work 8/20
- **Explicit framing:** Stripe states "The preferred qualifications are a bonus, not a requirement" ([Stripe](https://stripe.com/jobs/search?gh_jid=7618977)). Sarvam labels its good-to-haves "(not required)" ([Sarvam Model API](https://jobs.ashbyhq.com/sarvam/0371342b-5cb8-487b-9310-4d0eb5b37f47)).
- **Typical pattern, Adobe Java:** Java/Spring Boot, distributed systems and AI-assisted engineering are must-haves. Postgres/Dynamo/Mongo/Redis, Kafka/RabbitMQ/SQS, Docker/K8s, Grafana and Jenkins are all "Preferred" ([Adobe CS-I Java](https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist--I--Java-_R173771)).

### Inferences
- Breadth in infra and messaging helps you stand out but rarely gates entry. Language depth, design, DSA and (increasingly) AI-tool fluency do gate it.

### Gaps
- None material.

## Q10. Higher-pay associations

### Takeaway
None of the 41 India JDs disclosed compensation, so skill-to-pay associations cannot be measured from this sample. Only indirect signals are available.

### Cited Findings
- **Compensation shown:** Indeed showed "Compensation: N/A/None" for every viewed JD (e.g. [Rippling](https://to.indeed.com/aak7rvqqbt9x), [Google](https://to.indeed.com/aa9bklnrtcsn)). Ashby compensation summaries for Sarvam India roles were null ([Sarvam](https://jobs.ashbyhq.com/sarvam/fa96b55d-0c77-423d-8eef-f579c8496adb)).
- **Qualitative pay claims in JDs:**
  - MongoDB: "Generous compensation package (top-range salary, equity ...)" ([MongoDB SE3](https://www.mongodb.com/careers/job/?gh_jid=8208074)).
  - CrowdStrike: "Market leader in compensation and equity awards" ([CrowdStrike](https://to.indeed.com/aa4rvpnjssc9)).
  - Triomics: "best-in-industry compensation" ([Triomics](https://to.indeed.com/aa2gdqzk8gr8)).
- **Third-party self-reported pay:** Grapevine puts Flipkart SDE-2 (4–6 yrs) at about 28 LPA on average, a weak, aggregated source surfaced in a search snippet ([Grapevine Flipkart](https://www.grapevine.in/tal/jobs/aa4b0f60-6bc1-4843-8be1-5f9ee2eabc7d)).

### Inferences
- Indirect only: the employers that pair LLM/agent platform work with distributed-systems requirements are top-of-market payers in India (Microsoft Core AI, Google Cloud, Databricks, MongoDB, Sarvam). This hints that AI-platform plus distributed-systems skills sit in high-pay buckets, but this sample cannot prove it.

### Gaps
- Pay must come from levels.fyi, AmbitionBox, Glassdoor or offer data in another researcher's notes. These JDs do not support quantitative skill-pay claims.

## Q11. AI/LLM skills and AI coding-tool expectations in plain SDE JDs

### Takeaway
AI is now mainstream in India SDE-2 JDs. 27/41 (66%) mention AI/LLM product work or AI coding tools, and 16/41 (39%) require one or the other. AI coding-tool fluency (Copilot, Cursor, Claude Code, Codex, or "AI-assisted development") appears in 13/41 (32%) and is required in 9/41 (22%). It is most explicit at Indian product companies and startups, and now appears as a must-have at Adobe.

### Cited Findings
- **AI/LLM product work (building with LLMs, RAG, agents):** 20/41 any (49%), 8/41 required. By category: Big Tech 46%, SaaS/MNC 50%, Indian product 33%, startups 67%. Source: coded sample.
- **AI coding tools:** 13/41 any (32%), 9/41 required. By category: Big Tech 3/13 (1 required), SaaS/MNC 5/16 (3 required), Indian product 3/6 (3 required), startups 2/6 (2 required).
- **Verbatim AI-tool requirements:**
  - Adobe (must-have): "Strong proficiency in AI-assisted engineering, leveraging tools such as Claude, Codex, or Copilot to accelerate development" ([Adobe CS-I Java](https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist--I--Java-_R173771)).
  - Seekho: "We use coding agents daily — Claude Code and similar ... That's the baseline, not a perk, and we expect fluency"; "AI-generated code fails differently from human code ... We expect it reviewed with the same rigour, and we test that directly" ([Seekho SDE 2](https://to.indeed.com/aak8d4rrrgw9)).
  - HackerRank (an "AI fluency" section): "Deep, hands-on proficiency with AI-powered development tools (e.g., GitHub Copilot, Cursor, Claude Code) - you don't just use them, you've developed workflows and best practices around them" ([HackerRank](https://job-boards.greenhouse.io/hackerrank/jobs/7693789)).
  - Sarvam: "Daily, hands-on use of AI tools in your engineering workflow, with concrete examples of what you automated or sped up" ([Sarvam Model API](https://jobs.ashbyhq.com/sarvam/0371342b-5cb8-487b-9310-4d0eb5b37f47)).
  - Increff: "AI -native developer experience- familiarity with AI-assisted development tools" ([Increff](https://to.indeed.com/aaqhlhnbmf4s)).
  - Freshworks: "AI Tool Fluency: Exposure and experience working with or integrating AI tools" ([Freshworks](https://jobs.smartrecruiters.com/Freshworks/744000150608630-lead-software-engineer-full-stack)).
  - MongoDB: "Expertise integrating Large Language Models (LLMs) into the developer workflow to automate unit test generation" ([MongoDB SE3 Modernization](https://www.mongodb.com/careers/job/?gh_jid=8239047)).
  - Coinbase (generic, in every India posting sampled): "Utilizes generative AI responsibly, maintaining human oversight" ([Coinbase Security Platform](https://www.coinbase.com/careers/positions/8165441?gh_jid=8165441)).
- **Preferred-level AI-tool mentions:** "Comfort using AI-assisted engineering tools thoughtfully" ([MongoDB SE3 Martech](https://www.mongodb.com/careers/job/?gh_jid=8083366)); "Hands-on experience with GenAI-based coding tools" ([Adobe CS-I Python](https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist-I--Python-_R173660)); "Familiarity with the agentic AI tooling ecosystem (AI IDEs, CLIs, and assistants)" ([MongoDB AI Framework](https://www.mongodb.com/careers/job/?gh_jid=8127772)).
- **Responsibility-level (not a qualification):** "Apply AI-assisted and agentic development practices and tools to improve engineering productivity" ([MS IQ](https://apply.careers.microsoft.com/careers/job/1970393557047620)).
- **AI in "plain" Big Tech SDE-2 JDs:**
  - Google: "Experience integrating generative AI tools or Large Language Model (LLM) interfaces into workflows" is a **minimum** qualification for SE II, AI Security ([Google](https://to.indeed.com/aassmm9djyx9)).
  - Amazon TFS (opportunity, not a requirement): "the opportunity to work on the leading technologies like AI/ML, Gen-AI, RAG" ([Amazon TFS](https://www.amazon.jobs/en/jobs/10531789/software-development-engineer-ii-tfs)).
  - Generic Amazon SDE II templates (Tax, ACD) contain no AI language ([Amazon Tax](https://to.indeed.com/aa9yq7q8yb6x)).
- **"GenAI a plus" pattern:** "Experience with ML or LLM systems is a plus" ([Databricks AI](https://databricks.com/company/careers/open-positions/job?gh_jid=8924868002)); "Experience serving or integrating LLMs in production ... Bonus" ([Sarvam SDE2 API](https://to.indeed.com/aa779t9klyz7)); "Exposure to LLM serving infrastructure ... Good to Have" ([Triomics](https://to.indeed.com/aa2gdqzk8gr8)); "Experience or interest in driving agentic-AI projects" bonus ([CrowdStrike](https://to.indeed.com/aa4rvpnjssc9)).
- **MCP appears in 4 mid-level JDs:** Sarvam Full Stack ("MCP servers or clients"), InMobi ("Experience with Model Context Protocol (MCP)"), MongoDB AI Framework ("MCP servers, agent skills, or plugins"), Seekho ("increasingly by agents") ([Sarvam](https://jobs.ashbyhq.com/sarvam/fa96b55d-0c77-423d-8eef-f579c8496adb); [InMobi](https://job-boards.greenhouse.io/inmobi/jobs/8073988); [MongoDB](https://www.mongodb.com/careers/job/?gh_jid=8127772)).
- **Secondary corpus (156 India eng postings, all levels):** LLM/GenAI/agentic/RAG mentioned in 74 (47%). AI coding tools explicitly mentioned in 20 (13%), at HackerRank, MongoDB, Rubrik, Composio and Meesho, but 7 of the 20 are near-duplicate Rubrik postings. MongoDB's Salesforce/GTM roles name "Cursor, Claude Code, Agentforce, and GitHub Copilot"; a Meesho security architect role covers "guardrails for both human developers and AI coding agents". Source: ATS feeds (e.g. [MongoDB board](https://www.mongodb.com/careers/job/?gh_jid=8083366)).

### Inferences
- AI-coding-tool fluency has moved from "nice" to "baseline" at AI-native and Indian product employers, and Adobe now lists it as a must-have. Expect interviews to test it (Seekho says so outright). For a 2–5 YOE candidate, demonstrable workflows with Claude Code, Cursor or Copilot, plus judgment in reviewing AI output, are becoming a screening item.
- About half of plain SDE-2 JDs now involve building with LLMs (RAG, agents, LLM APIs, evals). Many are "AI platform" roles in disguise (Microsoft Foundry/IQ, Google Model Armor, Databricks AI, Sarvam APIs) whose core is still distributed systems.

### Gaps
- Explicit AI-tool counts are a lower bound for Big Tech. Amazon and Google templates are standardized and may not reflect team practice.

## Q12. Cross-category skill intersection and best backend language for an AI-leaning engineer

### Takeaway
The skills that intersect across all four categories are:
- one strong backend language
- distributed-systems fundamentals (idempotency, consistency, failure handling)
- design/DSA
- CI/CD + Kubernetes + observability ("own it in production")
- a relational database (Postgres) + Redis
- now, LLM integration and AI-tool fluency

For an AI-leaning engineer, **Python** gives the most optionality: it appears in 17 of 20 AI-product JDs, is the most-required language, and is the core language at AI-native startups. Pair it with **Java (Spring Boot)** for Big Tech and enterprise reach, or **Go** for platform/infra reach. TypeScript/Node gives the least backend optionality in this sample.

### Cited Findings
- **Present in all four category buckets (coded sample):** Python, Java, Kubernetes, Docker, CI/CD, observability, system design, DSA, Kafka, Redis, PostgreSQL, MongoDB, AI/LLM product work, AI coding tools.
- **Language overlap with AI-product JDs (20 JDs with any AI/LLM product work):** Python in 17, Java in 12, C# in 4 (all Microsoft), Go in 6, TypeScript in 2.
- **Python is the language of AI-platform roles:**
  - "3+ years of software engineering experience in C# and/or Python ... Experience building or integrating with LLM-based systems" ([MS Applied AI Engineer II](https://apply.careers.microsoft.com/careers/job/1970393557041515)).
  - "Python, SQL, TensorFlow/PyTorch ... LLM-powered applications" ([InMobi SDE II AI](https://job-boards.greenhouse.io/inmobi/jobs/8073988)).
  - "solid proficiency in Python and/or TypeScript" for AI framework integrations ([MongoDB](https://www.mongodb.com/careers/job/?gh_jid=8127772)).
  - "Developing and deploying GenAI/ML services" with "Significant experience in Python" ([Adobe CS-I Python](https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist-I--Python-_R173660)).
- **Java + Python hybrids put Java on the systems side and Python on the AI side:** Triomics ("Backend: Java / Spring Boot; AI Services: Python") ([Triomics](https://to.indeed.com/aa2gdqzk8gr8)); Cisco (Java Spring Boot + Python + LangGraph/RAG) ([Cisco](https://to.indeed.com/aatktq786h9k)).
- **Go is the "next" language for AI platforms at scale:** Sarvam's LLM API gateway is being rewritten from FastAPI to Go ([Sarvam SDE2 API](https://to.indeed.com/aa779t9klyz7)). Sarvam's GPU platform role wants "fluent in Kubernetes at the controller and internals level, comfortable in Go or Python" ([Sarvam Platform Engineer – AI Infrastructure](https://jobs.ashbyhq.com/sarvam/fcb15601-6440-41f7-aa79-b9992057a4b2), YOE not captured, not in the 41).
- **Java/Scala remains required for some AI platform backends:** "Strong experience with backend technical stacks such as Scala or Java" for the Databricks AI platform (traces, evals, LLM judges) ([Databricks AI](https://databricks.com/company/careers/open-positions/job?gh_jid=8924868002)).
- **TypeScript/Node:** TypeScript is mentioned in 4/41 JDs and Node.js in 3/41. Only one backend role requires Node (Transak) ([Transak](https://to.indeed.com/aazdfcfbyy6q)).

### Inferences
- **Ranking for maximum optionality (AI-leaning, India, 2–5 YOE), on this sample:**
  1. **Python.** It is the AI-product default and the most-required language; startups and Indian SaaS use it as their primary backend, and Big Tech AI teams name it.
  2. **Java.** It has the largest Big Tech and enterprise footprint and Spring Boot is a hard requirement wherever it is named, but it rarely leads AI-product JDs.
  3. **Go.** It is high-signal for platform, infra, security and high-throughput API gateways, including LLM gateways, and is concentrated at SaaS companies and startups.
  4. **TypeScript/Node.** It is mainly valuable as the frontend/BFF complement in full-stack AI products.
- **Practical portfolio:** "Python (FastAPI/async) + one of Java/Spring Boot or Go" plus Postgres/Redis, K8s/observability, an LLM integration (RAG/agents/streaming APIs, MCP), and demonstrable AI-coding-tool workflows. This covers the intersection of all four categories.
- Because 27% of JDs are language-agnostic (mostly Big Tech), Python is not a penalty for Big Tech interviews. DSA and design are the gate there.

### Gaps
- The optionality ranking is skewed by the missing Java/Go-heavy Indian unicorns (Q0). With Flipkart, Swiggy, PhonePe and Razorpay included, Java and Go would likely rank higher for Indian product companies.

## Q13. IT services firms vs product companies

### Takeaway
No IT-services JD could be read in full: Indeed detail calls were rate-limited, and the firms' boards were not reachable via public APIs. Only listing titles were observed, so IT services are excluded from all counts above. Titles suggest Java/Spring/microservices and "AI Platform/Applied AI" rebranding.

### Cited Findings
- **IT-services and consulting listing titles seen on Indeed (2026-11-27, titles only):**
  - Photon: "Java Developer", "Sr. Backend Dev – Java/Spring Boot" ([Photon listing](https://to.indeed.com/aarckgkh4gyc)).
  - UNISON Group: "Java Developer - Spring Boot | Microservices | Kafka / Solace" ([UNISON listing](https://to.indeed.com/aa6k79z7xrkv)).
  - Relevantz: "Java Full stack Developer" ([Relevantz](https://to.indeed.com/aa7z8tbds8w9)).
  - Accenture: "Cloud Platform Engineer", "AI / ML Engineer" ([Accenture](https://to.indeed.com/aavf8n4syx74)).
  - Capgemini: "AI Platform Engineer" ([Capgemini](https://to.indeed.com/aahccdxwtdy7)).
  - Infosys: "Azure Infrastructure Engineer" ([Infosys](https://to.indeed.com/aantwthqyj7t)).
  - Deloitte: "Applied AI Platforms Engineer II", "Applied AI Platform Engineer (SDET + PE)", "Applied AI Engineer Sales Force - Software Engineer II" ([Deloitte](https://to.indeed.com/aacflc8tbvqb)).
  - Kyndryl: "Modernization AI Engineer" ([Kyndryl](https://to.indeed.com/aagvk426zlyq)).
  - Ness Digital Engineering: "AI Full Stack Engineer" ([Ness](https://to.indeed.com/aa84s2z7h4dg)).
  - HCLTech: "Technical Specialist/Lead" ([HCLTech](https://to.indeed.com/aakvl9v4vx6d)).

### Inferences
- Among the roughly 14 IT-services titles seen, about half carry "AI" in the title. This suggests heavy AI rebranding at services firms, but without JD text skills cannot be compared with product companies.

### Gaps
- Full IT-services JDs (TCS, Infosys, Wipro, HCLTech, Accenture, Capgemini, Deloitte) are needed for a like-for-like comparison. Retry the Indeed `get_job_details` calls once the rate limit resets (the job IDs above are recorded in the Indeed search results).
