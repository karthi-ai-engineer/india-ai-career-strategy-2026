# Win India's applied-AI hiring market with focus

For an engineer who reaches two years of experience around November 2027, the best target in India is the **Applied AI / GenAI / Agentic AI Engineer** role. Run it alongside a narrower but more distinctive **AI Forward Deployed Engineer (FDE)** lane, and keep Big Tech SDE-2 as a stretch lane for its higher pay ceiling, not as the main bet. AI/ML postings on Naukri grew **20–49% year on year in every 2026 release**, while IT/software services fell 4% (Sep 2026). LinkedIn ranks AI Engineer the **#1 fastest-growing job in Bengaluru and Hyderabad** for 2026. India FDE postings grew about **19-fold** in a year, but the whole India FDE market is **only hundreds of openings, and the median posting asks for at least about five years of experience**, so FDE cannot carry a job search on its own. Two hand-coded samples of 2026 India job descriptions (49 AI/FDE and 41 SDE-2, so 90 in total) point to one portable core: Python, agents with tool calling, RAG, evals and production observability on one cloud. A Tokyo AI Engineer/FDE already has part of that core. The real constraints are three: DSA and system-design interview fluency; the 3–5-year minimum experience most job descriptions state; and getting hired at the SDE-2/L4 level rather than L3. That level difference roughly **doubles total compensation** (Google India median L3 ₹38.9L vs L4 ₹66.5L). Realistic outcomes at about 2 years' experience are **₹20–50 LPA** at AI startups, unicorns and GCCs, and **₹40–70 LPA** at Big Tech or top SaaS if hired at L4. FDE pay data is thin: Glassdoor's Bengaluru FDE average rests on about 9 reports. The plan below therefore sets out one clean stack, three portfolio projects that each report evaluation metrics, a 6–8-month part-time interview build, and two application waves. Wave 1 runs Oct 2027–Feb 2028 and targets employers whose minimum is 2–3 years or less. Wave 2 runs May–Sep 2028 and targets the 3+-year SDE-2 band.

## 1. Executive summary: AI engineering is the volume play, FDE the premium lane, level the pay lever

The Indian market of late 2026 rewards a narrow, deep profile over a broad one. Demand is growing fastest for engineers who have shipped LLM systems to real users. Generic coding roles and certificate-level AI skills are oversupplied. NASSCOM counts **more than 2 million people "upskilled in AI"** ([NASSCOM Strategic Review, 24 Feb 2026](https://d3r3sr3o54kk15.cloudfront.net/s3fs-public/media_pdf/India%E2%80%99s%20tech%20industry%20continues%20to%20redefine%20AI-led%20transformation,%20efficiency%20and%20skilling--%20Nasscom%20Annual%20Strategic%20Review%202026.pdf)). Yet TeamLease finds **one qualified engineer for every 10 open GenAI roles** ([Deccan Herald / TeamLease Digital, Aug 2025](https://www.deccanherald.com/technology/artificial-intelligence/ai-boom-1-qualified-engineer-for-every-10-open-genai-roles-says-teamlease-report-3701061)). Taken together, the shortage is of people with production AI experience, not of people with AI credentials. This candidate already sits on the short side of that gap. What remains is to prove it in the formats Indian hiring loops use, and to time applications to the experience minimums that job descriptions state.

| Decision | Recommendation | Confidence | Anchor evidence |
|---|---|---|---|
| Primary role | Applied AI / GenAI / Agentic AI Engineer at product companies, tech-first GCCs and funded AI startups | High | 21,534 India "AI engineer" listings on Glassdoor (Oct 2026); LinkedIn #2 nationally, #1 in Bengaluru and Hyderabad (Jan 2026) |
| Co-primary lane | AI FDE at Big Tech GenAI teams and AI-native companies, filtered by stated minimum experience | Medium-high | India FDE postings up ~19x YoY (Jun 2026), but 138 roles at 84 companies with a median minimum of ~5 years (12 Oct 2026) |
| Stretch lane | SDE-2 on AI-platform teams at Big Tech/top SaaS (Google SWE II/III, Microsoft Applied AI Engineer II, Amazon SDE II) | Medium | Highest pay ceiling (₹63–70L median at L4/SDE II), but loops with 2–3 DSA rounds and real down-levelling risk |
| Safety lane | Founding/early FDE and AI Engineer roles at Indian AI startups and services AI practices | High | Postings open to 1–2 years exist (Gushwork, Isomorph, Nanonets 2+, Infosys 2–5) at ₹7–30L |
| Primary stack | Python (async/FastAPI) + LLM application core (agents/tool calling/MCP, RAG, evals, observability) + Postgres/pgvector + Docker/CI + one cloud; TypeScript at working level | High | Python in 78% of AI/FDE JDs; agents 76%, RAG 63%, evals 63%; the same core appears in every company category |
| Biggest gap to close | DSA (LeetCode medium in ~30 min, in Python), LLD machine coding, HLD + LLM system design | High | 1–3 DSA rounds remain standard at Big Tech and Indian product companies even for AI-flavoured roles |
| Pay lever | Get levelled at L4 / SDE II / IC2 rather than L3 / SDE I | High | L3→L4 median roughly doubles TC at Google, Amazon, Uber and CRED (Levels.fyi, Nov 2026) |
| City order | Bengaluru → Hyderabad → Delhi NCR/Mumbai (for FDE) → Pune → Chennai | High | Bengaluru holds ~80% of sampled AI JDs and 176 of 503 Glassdoor FDE listings; highest pay medians |
| Timing | Wave 1 Oct 2027–Feb 2028 (≤2–3-year minimums); Wave 2 May–Sep 2028 (3+-year SDE-2 band) | Medium | "3+ years" is the most common SDE-2 minimum (20 of 38 JDs); AI JD minimums cluster at 2–5 years |

### Evidence labels used throughout

Every material claim carries a source and date. Where the distinction matters, claims are labelled as **[V] verified/reported fact** (a dated source states it), **[E] estimate** (a calculation or analyst judgement from cited data), or **[F] forecast** (a projection by a named source, or explicit scenario speculation). Compensation figures are additionally marked as *reported* (Levels.fyi, AmbitionBox, Glassdoor, posted bands) or *estimated*. Levels.fyi medians are self-reported and skew toward higher earners at product companies. Indeed's India software engineer average base salary is only **₹8.86 LPA (n=16.8k)** ([Indeed India](https://in.indeed.com/career/software-engineer/salaries)), against a Levels.fyi India median total comp of **₹30.8L (n=20,834)** ([Levels.fyi, Nov 2026](https://www.levels.fyi/t/software-engineer/locations/india)).

### Data conflicts and gaps register

The research base is broad, but several of its pillars are thin or contradictory. The table below lists every conflict that could change a decision, and how this report handles it.

| Issue | What conflicts or is missing | How this report treats it |
|---|---|---|
| Naukri October 2026 | CareerIndia reports white-collar +14% and AI/ML +32% ([4 Nov 2026](https://www.careerindia.com/news/india-job-market-2026-ai-ml-hiring-surge-october-report-011-68141.html)). The Naukri blog page titled for October shows +2% and +20%, identical to September ([Naukri blog](https://www.naukri.com/blog/naukri-jobspeak-october-2026-white-collar-hiring-ai-ml-growth/)). The page returned HTTP 403, so it could not be checked. | Uses the full-year range (+20–49%) rather than any single month |
| Naukri vs foundit direction | Naukri shows Aug 2026 hiring +14% YoY; foundit shows overall −10% (Aug) and −12% (Jul) | Treats overall hiring as flat; only the AI/ML growth signal is consistent across platforms |
| Glassdoor ML engineer counts | 20,621 on glassdoor.co.in (Nov 2026) vs 63,012 on glassdoor.com (Sep 2026) | Uses counts only for order of magnitude |
| FDE growth rate | Indeed: ~19x YoY (Jun 2026), 16x (Jul), 6x (Aug). NewsBytes: +130% YoY to Jul 2026 | Uses the Indeed series and stresses that growth is slowing |
| FDE India volume | Glassdoor ~100–570 depending on filter (Oct 2026); Masai 138 roles at 84 companies (12 Oct 2026); Neurapath 71 open (Nov 2026) | Treats it as a market of "hundreds" |
| FDE pay | Indeed average base ~₹12 LPA; Glassdoor Bengaluru ~₹17 LPA from ~9 reports; posted bands ₹15–45L; Cartesia ₹70–90L comes from an aggregator only. No Levels.fyi Palantir India data | Treats FDE pay as "track the employer's SDE ladder" (estimate) |
| Levels.fyi skew | Self-reported, product-company-heavy, medians only, no sample size per level; "last updated" may be the render date | Uses it for relative level comparisons only, not as offer predictions |
| JD sample sizes | 49 AI/FDE + 41 SDE JDs, each coded by a single person. Bengaluru (~80%) and Google (8 JDs) are over-represented; IT services and Java-heavy Indian unicorns are under-represented; Indeed rate-limited full-JD fetches | Treats percentages as directional; category columns move 6–20 points per JD |
| Amazon India investment | "$75B total planned" (Dec 2025) vs "$48B for 2026–2030" (Jun 2026) | Quotes each with its own framing |
| GCC count | 2,117 (Zinnov-NASSCOM FY26) vs 1,700+ (government) vs 2,554 (GCCPROs, Nov 2026) | Uses 2,117 as the methodological anchor |
| Neysa round | $600M equity + $600M debt vs "$1.2B Series B" | Cites as "$600M+" |
| Japan experience value | No source quantifies how Indian employers value Japan-based experience, relocation, or JPY-anchored offers | All Japan-framing advice is labelled [E] |
| Referrals, ATS, keyword-stuffing | No sourced India data | Advice labelled [E] |
| MLOps/AI infra and Solutions Engineer counts | No clean India posting counts or level-wise pay | Flagged in each table |

## 2. Indian technology job market overview: a two-speed market where AI grows 20–30% and generic software stalls

India's tech labour market in 2026 is growing slowly in aggregate but splitting sharply underneath. NASSCOM puts FY26 industry revenue at about **$315B (+6.1%)** with headcount up only **2.3%, about 135,000 net jobs**, to roughly 5.95M people ([NASSCOM SR, 24 Feb 2026](https://d3r3sr3o54kk15.cloudfront.net/s3fs-public/media_pdf/India%E2%80%99s%20tech%20industry%20continues%20to%20redefine%20AI-led%20transformation,%20efficiency%20and%20skilling--%20Nasscom%20Annual%20Strategic%20Review%202026.pdf)). Within that slow aggregate, AI/ML postings have grown 20–49% a year in every Naukri release of 2026, while plain software and services postings went flat or negative. Indeed recorded a **12.3% fall in software development postings in the three months to ~May 2026**, although software still accounts for about one in five Indeed India postings ([People Matters / Indeed, 2026](https://www.peoplematters.in/news/recruiting-and-onboarding/software-job-postings-fall-123percent-as-ai-reshapes-tech-hiring-in-india-indeed-50486)). The implication for this candidate is direct. A profile read as "generic software engineer" competes in a shrinking pool. A profile read as "production AI engineer" competes in the one segment where demand is growing faster than qualified supply.

### Demand indicators

| Indicator | Latest value | Date | Label | Source |
|---|---|---|---|---|
| Naukri AI/ML postings YoY | +34% (Jan), +49% (Feb), +22% (May), +25% (Jun), +31% (Aug), +20% (Sep), +32% or +20% (Oct, conflicting) | Jan–Nov 2026 | V | [Naukri Feb](https://www.naukri.com/blog/naukri-jobspeak-it-hiring-shows-meaningful-recovery-and-ai-momentum-continues-white-collar-market-posts-12-yoy-growth-in-february-2026/); [Naukri Aug](https://www.naukri.com/blog/naukri-jobspeak-white-collar-hiring-grows-14-in-aug-fresher-hiring-ai-roles-lead/); [The People's Board, Sep](https://www.thepeoplesboard.com/news/ai-ml-hiring-20-september-naukri-jobspeak-2026/); [CareerIndia, Oct](https://www.careerindia.com/news/india-job-market-2026-ai-ml-hiring-surge-october-report-011-68141.html) |
| Indian MNCs' AI/ML hiring vs foreign MNCs | +82% vs +43% YoY | Feb 2026 | V | [Naukri Feb 2026](https://www.naukri.com/blog/naukri-jobspeak-it-hiring-shows-meaningful-recovery-and-ai-momentum-continues-white-collar-market-posts-12-yoy-growth-in-february-2026/) |
| IT/software services postings | −4% YoY (Sep); software/QA +1% (Oct) | Sep–Oct 2026 | V | [The People's Board](https://www.thepeoplesboard.com/news/ai-ml-hiring-20-september-naukri-jobspeak-2026/); [CareerIndia](https://www.careerindia.com/news/india-job-market-2026-ai-ml-hiring-surge-october-report-011-68141.html) |
| GCC postings | +18% YoY | Oct 2026 | V | [CareerIndia](https://www.careerindia.com/news/india-job-market-2026-ai-ml-hiring-surge-october-report-011-68141.html) |
| AI roles posted (foundit) | 290,256 in 2025; +32% forecast for 2026 (~3.8 lakh) | 2025 / F | V / F | [Storyboard18](https://www.storyboard18.com/how-it-works/ai-roles-cross-2-9-lakh-in-2025-hiring-seen-up-32-in-2026-87532.htm) |
| LinkedIn Jobs on the Rise | #1 Prompt Engineer, #2 AI Engineer nationally; AI Engineer #1 in Bengaluru and Hyderabad | Jan 2026 | V | [Business Standard](https://www.business-standard.com/industry/news/majority-of-indian-professionals-feel-unprepared-to-find-new-job-linkedin-126010800504_1.html); [Deccan Chronicle](https://www.deccanchronicle.com/jobs-and-education/ai-engineer-is-fastest-growing-job-role-in-hyderabad-linkedin-2026-report-1931848) |
| GCCs in India | 2,117 GCCs, $98.4B market; 1,200+ with AI/ML capabilities | Jul 2026 | V | [Zinnov-NASSCOM](https://zinnov.com/centers-of-excellence/zinnov-nasscom-india-gcc-landscape-2026-report/); [YourStory, May 2026](https://yourstory.com/enterprise-story/2026/05/gccs-number-touch-2117-in-india-revenue-just-short-of-100-billion) |
| New GCC roles needing AI skills | ~65% | Sep 2026 | V | [ANSR via GlobeNewswire, 24 Sep 2026](https://www.globenewswire.com/news-release/2026/09/24/3368576/0/en/new-ansr-report-finds-ai-skills-driving-gcc-hiring-in-india.html) |
| Big Tech India | ~33,000 added in 2025 (+18%); ~4,200 open roles, ~15% entry-level, ~half in AI/ML, cloud, cyber | 9 Feb 2026 | V | [Rest of World](https://restofworld.org/2026/h1b-visa-impact-india-tech-hiring-faamng/) |
| IT services top 5 net hiring | +13,918 in Q2 FY27 (TCS +4,258; Infosys +4,480; HCLTech +6,450) | Jul–Sep 2026 | V | [Lapaas Voice](https://lapaasvoice.com/tcs-infosys-hcltech-wipro-and-tech-mahindra-add-13918-employees-in-q2-fy27) |
| Firms reporting fewer entry-level hires | 55% (vs 25% mid-career, 14% senior), survey of 651 firms (attributed variously to ICRIER or Nomura) | 2026 | V, attribution unclear | [International News and Views](https://www.internationalnewsandviews.com/ai-jobs-india-fresher-hiring-world-bank-report-410814-2/) |
| Indian tech funding | $10.3B Jan–Sep 2026 (+7%), but rounds −38%; AI $1.6B (+96%), 75% to infrastructure | 21 Sep 2026 | V | [YourStory/Tracxn](https://yourstory.com/2026/09/indias-tech-cos-raise-usd-103b-in-2026-tracxn-report); [People Matters/Tracxn](https://www.peoplematters.in/news/ai-and-emerging-tech/india-ai-funding-nearly-doubles-to-usd-16-billion-in-jan-sept-2026-tracxn-53503) |
| Enterprise agent adoption | 40% of large organisations scaling AI agents vs 27% a year earlier (definitions differ) | 2026 | V | [McKinsey State of AI 2026](https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai) |

### Where the demand comes from

Four engines drive the growth, and they differ in how durable they are. **GCCs** are the most durable. They have grown from about 1,700 to 2,117 in roughly two years ([Zinnov-NASSCOM, Jul 2026](https://zinnov.com/centers-of-excellence/zinnov-nasscom-india-gcc-landscape-2026-report/)). They face a **~40% AI skills gap** and are building talent internally ([Business Today, 15 Jul 2026](https://www.businesstoday.in/amp/jobs/story/indias-gccs-face-a-40-ai-skills-gap-why-theyre-building-talent-from-within-instead-of-just-hiring-543090-2026-07-15)). Even so, Zinnov-NASSCOM rates **0% of Indian GCCs "AI-native"** ([AIM](https://analyticsindiamag.com/gcc/worlds-largest-ai-hiring-hub-yet-no-gcc-in-india-is-actually-ai-native)). That gap is a structural opening for engineers who can lead AI transformation work. **Big Tech** is pouring capital into India:

- Google: $15B for the Visakhapatnam AI hub, 2026–2030 ([Google India blog, 14 Oct 2025](https://blog.google/intl/en-in/company-news/our-first-ai-hub-in-india-powered-by-a-15-billion-investment/)).
- Microsoft: $17.5B over 2026–2029 ([Microsoft Source Asia, 9 Dec 2025](https://news.microsoft.com/source/asia/2025/12/09/microsoft-invests-us17.5-billion-in-india-to-drive-ai-diffusion-at-population-scale/)).
- Amazon: $35B by 2030, plus $13B more for AI infrastructure added in June 2026 ([TechCrunch, 25 Jun 2026](https://techcrunch.com/2026/06/25/amazon-ups-india-bet-with-fresh-13b-ai-infrastructure-investment/)).

Much of that capex is data-centre spending. It therefore signals demand for cloud-AI customer and solutions engineering more than raw SWE headcount [E]. **IT services** are hiring again at the margin, with about +14,000 net at the top five in Q2 FY27. However, Aon projects tech consulting and services pay rises of only **6.6%**, the lowest of any sector ([Business Today / Aon](https://www.businesstoday.in/latest/corporate/story/salary-hikes-in-india-likely-to-be-around-9-in-2026-aon-497149-2025-10-07)). **Startups** are well funded in total but concentrated in a few names. Deal count fell 38%. October 2026 funding dropped about **61% YoY with no $100M+ rounds** ([NewsBytes / Entrackr](https://www.newsbytesapp.com/news/business/october-2026-indian-startup-funding-down-475-to-678-million/tldr)). So startup hiring will come from a small set of well-capitalised companies.

US policy adds a tailwind for India-based roles. The **$100,000 fee on new H-1B petitions** (Sep 2025) applies only to new petitions ([The Register, 22 Sep 2025](https://www.theregister.com/2025/09/22/h1b_visa_changes/)). Forrester expects more offshoring to India by IT vendors and GCCs as a result ([Forrester](https://www.forrester.com/blogs/the-long-term-impact-of-the-100000-h-1b-fee-higher-it-service-prices-and-more-offshore)). For a candidate moving to India rather than the US, this is a net positive. More senior AI work is likely to be built in India rather than relocated away from it [E].

### City comparison

| City | AI/ML postings YoY (Naukri, Oct 2026) | Levels.fyi SWE median TC | AI/FDE employers seen in 2026 JDs | Priority |
|---|---|---|---|---|
| Bengaluru | +12% | ₹37.1L (n=11,405) | Google Cloud/YouTube FDE, Meta FDE, Apple, Cisco, Databricks, Sarvam, Rubrik, Rippling, Anthropic, Whatfix, HackerRank, Nanonets, Glean, most YC India AI startups; 176 of 503 Glassdoor India FDE listings (Oct 2026) | 1 |
| Hyderabad | +15% (fastest) | ₹31.6L (n=2,985) | Microsoft Core AI / Applied AI Engineer II / IQ, Amazon SDE II, Google SWE II Cloud, ServiceNow (largest engineering site globally), Salesforce CoE, Optum, UST | 2 |
| Delhi NCR | +13% | ~₹21.4L (2025 heatmap average) | MongoDB (Gurugram FDE and SE3), DevRev FDE, Cursor FDE (New Delhi), OpenAI (New Delhi), Adobe (Noida), Eternal (Gurugram), Google Cloud FDE (Gurugram option) | 3 |
| Mumbai | +12% | just under ₹20L (2025 heatmap average) | Google Cloud GenAI FDE (Mumbai option), Databricks, Cursor, DevRev, Neysa, Yotta, Anthropic Applied AI Architect, OpenAI (announced) | 3 (for FDE) |
| Pune | +14% | ₹21.1L (n=1,748) | Google SWE II AI Security (Model Armor), NVIDIA, Snowflake CoE, CrowdStrike, Mastercard | 4 |
| Chennai | +11% | ₹18.1L (n=995) | Freshworks, Walmart Global Tech, Sei AI, Ampera, Zoho, Uniphore | 5 |

Sources: city growth from [CareerIndia, 4 Nov 2026](https://www.careerindia.com/news/india-job-market-2026-ai-ml-hiring-surge-october-report-011-68141.html). Medians from [Levels.fyi Bengaluru](https://www.levels.fyi/t/software-engineer/locations/greater-bengaluru), [Hyderabad](https://www.levels.fyi/t/software-engineer/locations/hyderabad-ind), [Pune](https://www.levels.fyi/t/software-engineer/locations/pune-ind) and [Chennai](https://www.levels.fyi/t/software-engineer/locations/chennai-ind) (viewed 26–27 Nov 2026). Delhi NCR and Mumbai figures are from the [2025 Levels.fyi heatmap via Storyboard18](https://www.storyboard18.com/amp/how-it-works/bengaluru-software-engineers-earn-nearly-4x-more-than-those-in-ahmedabad-report-83862.htm). FDE counts are from [Glassdoor, Oct 2026](https://www.glassdoor.co.in/Job/bengaluru-forward-deployed-engineers-jobs-SRCH_IL.0,9_IC2940587_KO10,36.htm). City pay gaps mostly reflect **which employers are in each city, not differences in pay for the same company and level**. A Google L4 offer in Pune is not a ₹21L offer [E].

## 3. Target role analysis and ranking: AI Engineer wins on volume, FDE on differentiation

Indian 2026 job descriptions separate the role families more clearly than the titles suggest:

- **AI Engineer / GenAI / Agentic** roles build LLM applications: RAG, agents, evals and managed AI services.
- **ML Engineer** roles lean toward model training, classical ML and data pipelines.
- **SDE-with-AI** roles are standard SDE-ladder jobs on LLM-adjacent systems. Examples are Amazon's "SDE, Alexa LLM Inference, Capacity & Efficiency" (24 Nov 2026) and CrowdStrike's "AI Powered SRE" (23 Oct 2026) ([Indeed](https://to.indeed.com/aapxpcklhd6n); [Indeed](https://to.indeed.com/aal9kvgbqqbp)).
- **FDE** roles alternate between embedded customer work and core product engineering. Pragmatic Engineer describes FDEs as contributing more to the core product than solutions engineers do ([Pragmatic Engineer](https://newsletter.pragmaticengineer.com/p/forward-deployed-engineers)).

### Role market facts

| Role family | Demand signal (dated) | Companies seen hiring in India (2026) | Pay at ~2 YOE (reported unless marked) | Core skills | Typical stack |
|---|---|---|---|---|---|
| **SDE-2 / Backend / Platform** (incl. AI-platform SDE) | Software/QA +1% YoY (Oct 2026); Indeed software development postings −12.3% (3 months to ~May 2026); 66% of sampled SDE-2 JDs mention AI/LLM work or AI coding tools (Nov 2026) | Google, Microsoft, Amazon, Adobe, Databricks, MongoDB, Rubrik, Rippling, CrowdStrike, Wayfair, Mastercard, Sarvam, Increff, HackerRank, Zeta | Big Tech L4/SDE II ₹63–70L TC; unicorn SDE2 ₹36–46L TC (Levels.fyi, Nov 2026); generic SDE-2 ₹20–35 LPA at ~4 years ([UnboxCareer](https://unboxcareer.com/blog/salary-sde2-india-2026-companies-comparison)) | DSA, LLD/HLD, distributed systems, production ownership | Python/Java/Go, Spring Boot, Postgres/Redis, Kubernetes, Kafka, CI/CD |
| **Applied AI / GenAI / Agentic AI Engineer** | 21,534 India "AI engineer" listings ([Glassdoor, Oct 2026](https://www.glassdoor.co.in/Job/india-ai-engineer-jobs-SRCH_IL.0,5_IN115_KO6,17.htm)); LinkedIn #2 rising job (Jan 2026) | Cisco, Microsoft, Google, Fractal, Sarvam, Groww, Razorpay, Whatfix, 100ms, Infer, Vahan, Walmart GT, Amex, Visa, Infosys, Wipro | Posted bands ₹20–50L at funded startups (100ms at 2 YOE, Infer at 3 YOE); GenAI Engineer median fixed pay ₹13.2 LPA at 0–2 YOE in GCCs ([TeamLease, Oct 2026](https://cxotoday.com/others/teamlease-digital-44-of-indian-gccs-own-full-platforms-ai-outcomes-as-compensation-tops-₹108-6-lpa/)); ₹8–15 LPA at 2–4 YOE ([Instahyre](https://resources.instahyre.com/blog/ai-engineer-salary-in-india/)) | Agents and tool calling, RAG, evals, observability, cloud deployment | Python, LangGraph/ADK, pgvector or another vector DB, FastAPI, multi-provider LLM APIs |
| **ML Engineer** (training-heavy) | Glassdoor 20,621 (.co.in, Nov 2026) vs 63,012 (.com, Sep 2026), a conflict | Uber, Adobe, Google (separate L4 MLE track), UST, Optum | Levels.fyi ML/AI SWE median ₹29.0L across all levels (n=1,297), *below* the overall SWE median of ₹30.8L ([Levels.fyi, Nov 2026](https://www.levels.fyi/t/software-engineer/focus/ml-ai/locations/india)) | Modelling, training, data pipelines | PyTorch, Hugging Face, Spark, MLOps tooling |
| **MLOps / LLMOps / AI Infra / Inference** | No clean India count (gap). Infrastructure took 75% of Indian AI funding in Jan–Sep 2026 (Tracxn) | NVIDIA, Sarvam (Platform – AI Infrastructure), Razorpay (LLM gateway), E2E Networks, Neysa, Simplismart, TrueFoundry, Amazon (Alexa LLM inference) | No level-wise India data (gap); TeamLease reports >18% annual raises for GenAI and MLOps staff ([Deccan Herald, Aug 2025](https://www.deccanherald.com/technology/artificial-intelligence/ai-boom-1-qualified-engineer-for-every-10-open-genai-roles-says-teamlease-report-3701061)) | Kubernetes internals, GPU serving, inference optimisation, cost engineering | Go/Python/C++, vLLM, Triton, TensorRT, Kubernetes |
| **FDE / AI FDE** | ~19x YoY (Jun 2026), ~16x (Jul), ~6x (Aug) ([People Matters / Indeed, 15 Oct 2026](https://www.peoplematters.in/news/workforce-planning/demand-for-forward-deployed-engineers-jumps-19-fold-in-india-report-52770)); 503 India listings ([Glassdoor, Oct 2026](https://www.glassdoor.com/Job/india-forward-deployed-engineer-jobs-SRCH_IL.0,5_IN115_KO6,31.htm)); 138 roles at 84 companies, only 6 entry-level, median minimum ~5 years ([Masai, 12 Oct 2026](https://www.masaischool.com/blog/forward-deployed-engineer-jobs-in-india/)) | Google Cloud, YouTube, Meta, Apple, Cisco, Databricks, Cursor, DevRev, HackerRank, MongoDB, ServiceNow, Whatfix, Nanonets, Gushwork, Cekura, NTT DATA, Accenture, Wipro | Indeed average base ~₹12 LPA (range ₹9–16) ([Masai citing Indeed](https://www.masaischool.com/blog/forward-deployed-engineer-jobs-in-india/)); posted bands ₹15–30L (Cekura), ₹15–23L (Weekday client, 2+ YOE), ₹30–45L (HackerRank, 3+ YOE) | Customer discovery, agents/RAG/evals, cloud architecture, integrations, full-stack delivery | Python + TypeScript, a hyperscaler AI platform (Vertex/ADK, Bedrock, Azure OpenAI), Terraform |
| **Solutions / Customer Engineer / Applied AI Architect** | No clean count (gap). OpenAI and Anthropic India roles are mostly Applied AI Architect/Engineer, about 6–7 openings each (late 2026) | OpenAI, Anthropic (Bengaluru, 10+ YOE), Databricks Specialist SA (5+), ServiceNow "AI Engineer – Sr Solution Consultant", Freshworks Lead Solution Engineer, Snowflake | Levels.fyi Solution Architect median ₹45.9L, n=334, mostly mid/senior ([Levels.fyi, Nov 2026](https://www.levels.fyi/t/solution-architect/locations/india)) | Pre-sales, demos, architecture, stakeholder management | Platform-specific |
| **Emerging titles** (Agent Engineer, Evals Engineer, Agent Reliability, Deployment Strategist, AI Security) | Tens of postings, often 3–7 years | Sarvam Agent Engineer (3+), Brillio AI Agent Evaluation (5–7), Emergent AI Agent Reliability, Sarvam and ElevenLabs Deployment Strategist, Google SWE II AI Security (Model Armor, 1 yr) | AI Evals band of ₹10–40 LPA from a blog estimate only (gap) | Evals, regression testing, guardrails, red-teaming | Python, Langfuse/LangSmith, Ragas/DeepEval |

### Role assessment and ranking

The two notes that produced role rankings disagree. One ranks FDE first on fit. This report ranks Applied AI Engineer first, for two reasons. First, the AI Engineer pool is roughly **40x larger** than the FDE pool (21,534 vs 503 Glassdoor listings, Oct 2026) [E]. Second, the FDE pool skews senior: of 138 tracked roles, only 6 were entry-level and the median minimum was about 5 years (Masai, 12 Oct 2026). A 2-YOE candidate who targets only FDE titles can apply to perhaps a few dozen realistic openings in a given quarter [E]. The fix is to market one identity, "AI Engineer who deploys with customers", that qualifies for both titles.

| Rank | Role | Interview difficulty [E] | Competition [E] | 2-year outlook [F] | Progression | Fit for this profile |
|---|---|---|---|---|---|---|
| **1** | Applied AI / GenAI / Agentic AI Engineer (product, tech-first GCC, funded AI startup) | 6–7 | High and rising at the low end; thin at the production level (1 qualified per 10 open GenAI roles) | Strong. The title absorbs SDE demand and blurs into "software engineer" by 2028 | Senior → Staff AI Engineer → AI platform lead | Very high: a direct continuation of current work |
| **2** | AI FDE (Big Tech GenAI teams, AI-native SaaS) | 7–9 (Big Tech, labs), 6–7 (startups) | Small qualified pool; Indeed India's MD says candidates still find the role confusing ([Deccan Chronicle](https://www.deccanchronicle.com/amp/nation/in-other-news/demand-for-forward-deployed-engineers-jumps-19-fold-in-india-report-1995773)) | Growth slows from 19x but stays high; partly merges into Applied AI and Solutions titles | Senior/Staff FDE → Solutions Architect / Applied AI Architect / FDE manager / founder | Very high on skills; limited by ~5-year median minimums |
| **3** | SDE-2 on AI-platform teams (Google SWE II/III, Microsoft Applied AI Engineer II, Amazon SDE II, Databricks, Rubrik) | 8–9 | Very large applicant pool; only ~15% of Big Tech India openings are entry-level | Flat volume; AI skills become the default expectation | SDE-3 → Staff/Principal | Medium-high; gated on DSA/LLD |
| **4** | Founding / early FDE or AI Engineer at Indian AI startups | 5–6 | Moderate | Volatile; funding is concentrated | Broad ownership → lead → founder | High fit; lower pay, higher risk |
| **5** | Solutions / Customer Engineer / Applied AI Solutions Architect | 6–7 | Moderate | Grows with lab and SaaS go-to-market teams in India | SA → Principal SA | Medium; risk of drifting into pre-sales |
| **6** | MLOps / LLMOps / AI Infra / Inference | 8 | Small pool, high bar | Rising in 2027–28 as compute comes online [F] | Infra/platform lead | Medium-low now; a good pivot after 2028 |
| **7** | ML Engineer (classical / training) | 7–8 | Moderate | Stable | Senior MLE → Staff | Medium-low; needs modelling depth not shown in current work |
| **8** | Emerging titles (Evals, Agent Reliability, Context Engineer) | 6–7 | Few postings | Absorbed into AI Engineer JDs | — | Low as target titles; high as skills to feature |

## 4. Comprehensive company landscape: hyperscaler FDE teams, SaaS AI platforms and agentic unicorns

The company universe divides into four categories with different hiring rules:

- **Big Tech and product MNCs** pay the most at L4 and post the most India FDE roles. Their minimum experience ranges from 1 to 8 years, depending on the team.
- **Enterprise SaaS and GCCs** run real AI platform work in India (ServiceNow Hyderabad, SAP's Joule, Databricks R&D). Pay ranges from top of market (Databricks, Rubrik) to middling (SAP, Snowflake, Oracle).
- **Indian product companies** are now shipping named agentic architectures. Swiggy has MCP servers with 66 tools. Razorpay's Agent Studio is built on the Claude Agent SDK. Groww is hiring AI Engineer II/III for MCP tooling.
- **AI-native startups** are covered in Section 5.

In the tables, the "Evidence" column marks hiring evidence as **V** (a dated posting or announcement is cited), **S** (taken from search snippets or aggregator pages that were not opened in full) or **I** (inferred from investment or general presence). Careers URLs marked "seen" appeared in sourced results. URLs marked "std" are the company's standard careers domain and were not fetched.

### Category A: Big Tech and product MNCs

| Company | Domain / HQ | India locations | Stage | Relevant India roles (dated) | Stack signal from JDs | Comp at ~2 YOE (Levels.fyi median TC, Nov 2026) | Evidence | Why target | Careers URL |
|---|---|---|---|---|---|---|---|---|---|
| **Google / Google Cloud** | Search, cloud, AI; Mountain View | Bengaluru, Hyderabad, Pune, Gurugram, Mumbai | Public; $15B Vizag AI hub (14 Oct 2025) | GenAI FDE (8 yrs, 2 Nov 2026); **FDE V Data Cloud (2-yr minimum, 4 Nov 2026)**; YouTube FDE (4 yrs, 13 Nov 2026); **SWE II Cloud (1 yr, Hyderabad, 23 Nov 2026)**; **SWE II AI Security / Model Armor (1 yr, Pune, 24 Nov 2026)**; SWE III Full Stack Cloud AI (2 yrs) | Language any-of (Python/Java/C++); DSA as a minimum qualification; GCP, Vertex, ADK; Terraform for agent infrastructure (GECX FDE) | L3 ₹38.9L; **L4 ₹66.5L** | V ([Indeed](https://to.indeed.com/aasc8sxtn2sh); [Indeed](https://to.indeed.com/aa9bklnrtcsn); [Indeed](https://to.indeed.com/aassmm9djyx9)) | Largest verified India FDE employer; unusually low 1–2-year minimums on SWE II/III | careers.google.com (std) |
| **Microsoft** | Cloud, software; Redmond | Hyderabad, Bengaluru, Noida | Public; $17.5B for 2026–29 | **Applied AI Engineer II (3 yrs, Hyderabad, 19 Oct 2026)**; SWE II Core AI – Foundry Agentic Core Services (3 yrs); SWE II Data Security (4); SWE II Microsoft IQ (5) | C# and/or Python; Azure OpenAI, AKS, Cosmos DB for RAG; DSA + system design | 61 ₹41.9L; 62 ₹65.1L | V ([Microsoft careers](https://apply.careers.microsoft.com/careers/job/1970393557041515)) | Hyderabad AI-platform hub; 3-year minimum reachable in Wave 2 | apply.careers.microsoft.com (seen) |
| **Amazon / AWS** | E-commerce, cloud; Seattle | Hyderabad, Bengaluru, Chennai | Public; $35B by 2030 + $13B AI infrastructure (Jun 2026) | SDE II (3 yrs + 2 yrs design, multiple, Sep–Nov 2026); SDE Alexa LLM Inference (24 Nov 2026) | Language-agnostic; AWS Lambda, DynamoDB, Step Functions, CDK | SDE I ₹28.9L; **SDE II ₹63.2L** | V ([amazon.jobs](https://www.amazon.jobs/en/jobs/10611676/software-development-engineer-ii-icon)) | Large SDE II pool; Leadership Principles loop; down-levelling risk | amazon.jobs (seen) |
| **Meta** | Social, AI; Menlo Park | Bengaluru | Public; India AI hiring expansion reported May 2026 | **FDE, Enterprise AI (Bangalore), 13 Nov 2026** | AI-enabled coding round in its loop (since Oct 2025) | Not fetched | V ([Indeed](https://to.indeed.com/aa8s9lp8m2q4)) | New India FDE team; rare Meta India engineering openings | metacareers.com (std) |
| **Apple** | Consumer tech; Cupertino | Bengaluru | Public | FDE – GSSM Solutions (4 Nov 2026); Senior Applied AI Engineer (8 yrs) | DSA, distributed systems (Kafka/Spark/Flink), MCP preferred | Not fetched | V ([Indeed](https://to.indeed.com/aaldxr64qjd8)) | FDE title in India; senior-skewed | jobs.apple.com/en-in (std) |
| **Cisco** | Networking, security; San Jose | Bengaluru | Public | **AI Engineer, CloudX (3 yrs, 24 Nov 2026)**; SWE (AI & Full-Stack) (5, or 3 with an MS); FDE and Senior FDE (14 Oct 2026) | Java Spring Boot + Python; LangGraph / Bedrock / OpenAI or Anthropic SDKs; **builds MCP servers**; Snowflake, Airflow; Weaviate | Cisco is the top payer for India Solution Architects (₹78.3L, all levels) | V ([Indeed](https://to.indeed.com/aabtcp7sghz9)) | Near-perfect JD match for the target stack | jobs.cisco.com (std) |
| **NVIDIA** | AI compute; Santa Clara | Bengaluru, Pune, Hyderabad + 3 cities | Public; ~760k sq ft Bengaluru lease (2026) | Senior System SWE – Local AI (5, Pune); Senior AI/ML SWE Enterprise Agentic (6); Senior MLOps (8) | C++, vLLM, llama.cpp, TensorRT, Triton, NIM, CUDA | IC2 ₹34.2L; IC3 ₹64.6L | V ([AnitaB](https://jobs.anitab.org/companies/nvidia/jobs/87547967-senior-system-software-engineer-local-ai)) | Only for an inference/infra pivot | nvidia.com/careers (std) |
| **Adobe** | Creative/document SaaS; San Jose | Noida, Bengaluru | Public; ~8,000 India staff | Computer Scientist-I Python GenAI (5, 17 Nov 2026); MLE Agentic Marketing (5); Firefly FDE manager and "FDE – Full Stack AI" listings | Java/Spring Boot, Python; **AI-assisted engineering a must-have**; SFT/DPO preferred | P20 ₹35.3L; P30 ₹54.6L | V/S ([Adobe Workday](https://adobe.wd5.myworkdayjobs.com/external_experienced/job/Noida/Computer-Scientist-I--Python-_R173660)) | GenAI services team in India; FDE track forming | adobe.com/careers.html (seen) |
| **LinkedIn** | Professional network (Microsoft); Sunnyvale | Bengaluru | Subsidiary; largest R&D hub outside Silicon Valley (Jul 2026) | ML, ML infrastructure, agentic hiring products (2025 postings, mostly Staff) | Not verified | IC1 ₹46.8L; **IC2 ₹62.6L** | S ([YourStory, Jul 2026](https://yourstory.com/enterprise-story/2026/07/india-global-products-shaping-how-they-evolve-linkedin-malai-lakshmanan)) | Highest IC2 pay among the MNCs fetched | careers.linkedin.com (std) |
| **Uber** | Mobility/delivery; San Francisco | Bengaluru, Hyderabad | Public; two campuses for ~9,600 people due by end-2027 (14 May 2026) | Senior MLE (5, or 2 with MS/PhD) | Not verified | L3 ₹34.4L; **L4 ₹70.3L** | V/I ([TechCrunch](https://techcrunch.com/2026/05/14/uber-to-open-2-campuses-in-india-to-support-product-development-operations/)) | Campus timing matches a 2028 start | uber.com/careers (std) |
| **Salesforce** | CRM / Agentforce; San Francisco | Hyderabad, Bengaluru (+4 cities) | Public; 14,000+ India staff (Nov 2025) | Agentforce FDE title exists (India location unconfirmed) | Not verified | MTS ₹48.9L | V/I ([Salesforce India](https://www.salesforce.com/in/news/press-releases/2025/11/25/agentic-enterprise-salesforce-india-transformation/)) | Hyderabad CoE builds products end to end | careers.salesforce.com (std) |
| **Atlassian** | Collaboration SaaS; Sydney | Bengaluru (remote-first) | Public | Senior FDE, AI (5 + 3 in AI; removed Feb 2026); in-band SWE postings need 8+ yrs | Kotlin/Java | P30 ₹43.8L; **P40 ₹69.6L** | V ([Built In](https://builtin.com/job/senior-forward-deployed-engineer-ai-remote/7303438)) | Top pay; few in-band openings in Nov 2026 | atlassian.com/company/careers (std) |
| **Intuit** | Fintech/tax SaaS; Mountain View | Bengaluru IDC | Public; "one of the core teams for GenOS is here in India" (Nov 2025) | Staff SWE Gen AI / AI/ML (senior) | GenOS, AWS CDK | SE1 ₹31.2L; **SE2 ₹46.6L** | S ([YourStory, Nov 2025](https://yourstory.com/enterprise-story/2025/11/india-development-centre-play-key-role-frontier-ai-intuit-chief-ai-officer)) | GenAI platform ownership in India | jobs.intuit.com (seen) |
| **Oracle (OCI)** | Database, cloud; Austin | Bengaluru, Hyderabad, Noida | Public; new Mumbai/Hyderabad DCs | AI Developer – Cloud Operations (14 Feb 2026) | OCI | IC-2 ₹27.6L | S ([AnitaB](https://jobs.anitab.org/companies/oracle-2-2edaf908-7a2f-4ec2-a440-aed90715dc36/jobs/67749507-ai-developer-cloud-operations)) | A stepping-stone pay band | oracle.com/in/careers (seen) |

### Category B: enterprise SaaS, infrastructure, AI labs and GCCs

| Company | Domain / HQ | India locations | Stage / India scale | Relevant India roles (dated) | Stack signal | Comp at ~2 YOE | Evidence | Why target | Careers URL |
|---|---|---|---|---|---|---|---|---|---|
| **Databricks** | Data/AI platform; San Francisco | Bengaluru (R&D), Mumbai, Delhi | Private; $250M over 3 years, ~1,000 staff, +100 R&D engineers (Mar 2026) | 5 India FDE roles incl. Senior FDE (6+, Oct 2026); SE Infrastructure (3–5, 30 Sep 2026); Sr SE Agentic Full Stack (5); Specialist SA AI/ML (5) | Scala/Java; Python + React; Terraform; HF/LangChain/DSPy for FDE | **L3 ₹68.5L; L4 ₹1.00Cr** | V ([Databricks](https://databricks.com/company/careers/open-positions/job?gh_jid=8829029002); [Masai, 30 Oct 2026](https://www.masaischool.com/blog/forward-deployed-engineer-jobs-in-india/)) | Top pay; India R&D growing; FDE track | databricks.com/company/careers (seen) |
| **ServiceNow** | Workflow / AI agents; Santa Clara | Hyderabad (largest engineering site globally), Bengaluru | Public; ~6,000 India engineers, 25% CAGR (2026, conflicting) | **Forward Deployed Software Engineer – Gen AI**; AI Engineer – Sr Solution Consultant; Sr SWE Java/JS/LLM | Java, JavaScript, LLMs, RAG, Now Platform | IC2 ₹41.6L (cached values conflict: ₹49.7–62.5L) | S ([Built In](https://builtin.com/job/forward-deployed-software-engineer-gen-ai/8672327); [Entrepreneur India](https://india.entrepreneur.com/growth-strategies/several-tailwinds-powering-servicenow-indias-growth/493894)) | Best-documented MNC FDE hiring plan for India in 2026 | careers.servicenow.com/locations/apj/india/ (seen) |
| **SAP Labs India** | ERP / Joule; Walldorf | Bengaluru (2 campuses), others | 17,300+ India staff; second campus Aug 2025 | Joule agentic engineering (team-level) | BTP (not verified) | T2 ₹24.7L; T3 ₹45.2L | V ([SAP News, Aug 2025](https://news.sap.com/2025/08/sap-labs-india-bengaluru-second-campus/)) | Agentic AI copilot built largely in India | jobs.sap.com (std) |
| **MongoDB** | Developer data platform; New York | Gurugram, Bengaluru | Public; new Gurugram engineering org (2025) | FDE Industry Solutions (5+, 28 Oct 2026); **SE3 AI Framework Integrations (3+, Gurugram)** | Java/Go, Spring Boot, Python/TS for AI frameworks, MCP servers/agent skills | Not fetched | V ([MongoDB](https://www.mongodb.com/careers/job/?gh_jid=8127772)) | NCR's best AI-framework role | mongodb.com/careers/locations/gurugram (seen) |
| **Rubrik** | Data security; Palo Alto | Bengaluru, Pune | Public | **SE Cloud Native Protection (2 yrs, 11 Nov 2026)**; SE IAM (Go); Sr AI Engineer Enterprise Agentic (7+) | Go | **L3 ₹68.7L; L4 ₹97.8L** | V ([Rubrik](https://www.rubrik.com/company/careers/departments/job.8327940?gh_jid=8327940)) | Rare 2-year minimum at top-tier pay | rubrik.com/company/careers (seen) |
| **Rippling** | HR/IT SaaS; San Francisco | Bengaluru | Private; ~2,500 India staff; AI lab and plan for 5,000 (Sep 2026, headline only) | SE II App Components (3, 12 Nov 2026) | Python + Go, Django, Kafka, Flink, React | L5 ₹45.5L; L6 ₹67.2L | V/S ([Indeed](https://to.indeed.com/aak7rvqqbt9x); [Rippling blog](https://www.rippling.com/blog/rippling-expands-india-office)) | #1 India payer on the Levels.fyi leaderboard | rippling.com/careers (std) |
| **Glean** | Enterprise AI search/agents; Palo Alto | Bengaluru | Private; ~450+ India staff | SWE – Machine Learning (India); backend | Not verified | Levels.fyi leaderboard #4 (L2 $120,483) | S ([Built In](https://builtin.com/job/software-engineer-machine-learning-india/3746516)) | AI-native product with Indian engineering ownership | job-boards.greenhouse.io/gleanwork (seen) |
| **Snowflake** | Data cloud; Bozeman | Pune CoE, Bengaluru | 700+ India target (2025) | India listings mostly Solution Engineer / FDE / support | — | IC2 ₹27.7L | S ([Business Today, Sep 2025](https://www.businesstoday.in/technology/news/story/ai-will-enhance-work-not-replace-it-snowflake-to-hire-700-in-india-by-2025-says-vijayant-rai-492594-2025-09-04)) | FDE/SE entry; lower pay | careers.snowflake.com/us/en/pune (seen) |
| **Stripe** | Payments infrastructure | Bengaluru | Private | All 4 Bengaluru SWE postings need 7–8+ yrs (Nov 2026) | gRPC, GraphQL, K8s | L1 ₹56.9L; L2 ₹1.00Cr | V ([Stripe](https://stripe.com/jobs/search?gh_jid=7618977)) | Out of band until ~2029 | stripe.com/jobs (seen) |
| **OpenAI** | Frontier AI; San Francisco | New Delhi; Mumbai/Bengaluru announced | Private; India entity Aug 2025 | Applied AI Engineer / Applied AI Architect (Delhi, Mumbai); no India FDE title | — | n/a | V ([AIM](https://analyticsindiamag.com/ai-news/openai-is-hiring-ai-engineers-in-delhi-mumbai/)) | Dream stretch for 2028+ | openai.com/careers (seen) |
| **Anthropic** | Frontier AI; San Francisco | Bengaluru (opened 16 Feb 2026) | Private; second Asian office after Tokyo | Applied AI Architect, Beneficial Deployment (Bengaluru, 24 Nov 2026); Bengaluru architect role asks for 10+ yrs | — | n/a | V ([Anthropic](https://www.anthropic.com/news/bengaluru-office-partnerships-across-india); [Indeed](https://to.indeed.com/aadsxd4xtysy)) | Tokyo–Bengaluru link makes Japan deployment experience relevant [E] | anthropic.com/careers (std) |
| **Walmart Global Tech** | Retail GCC | Bengaluru, Chennai, Gurugram | CTO: headcount "roughly the same" (Jan 2026) | SE II (3, 25 Jun 2026); Senior SWE agentic full-stack (5) | Agentic full-stack | P3 ₹33.9L | V ([AnitaB](https://jobs.anitab.org/companies/walmart/jobs/84130611-ind-software-engineer-ii)) | GCC AI mandate; the change is in the mix of roles, not net growth | careers.walmart.com (std) |
| **JPMorgan Chase** | Banking GCC | Bengaluru, Hyderabad, Mumbai | ~55,000 India staff; ~1,000 tech hires (~Jul 2026) | AI data pipelines, cloud, cyber | — | Not fetched | V ([Business Standard](https://www.business-standard.com/world-news/jpmorgan-plans-1-000-india-gcc-hires-despite-ai-driven-workforce-cuts-126072300511_1.html)) | Stable GCC demand; BFSI domain | careers.jpmorgan.com (std) |
| **Goldman Sachs** | Banking GCC | Bengaluru, Hyderabad | — | — | — | Analyst ₹33.0L; Associate ₹39.5L | V (pay only) | Mid-band GCC benchmark | goldmansachs.com/careers (std) |
| **American Express** | Payments GCC | Bengaluru | — | AI Engineer III (LLM and agentic features) | — | Not fetched | S ([eFinancialCareers](https://www.efinancialcareers.com/jobs-India-Bangalore-AI_Engineer_III.id24734078)) | GCC GenAI role | americanexpress.com/careers (std) |
| **Visa** | Payments | Bengaluru | ~2,600 global cuts, Bengaluru among the hubs hit (Aug 2026) | Lead AI Engineer (agentic), Sr MLE (MLOps) | — | Not fetched | S ([Business Today, 6 Aug 2026](https://businesstoday.in/latest/corporate/story/visas-ai-layoffs-hit-india-hard-why-even-top-performers-may-no-longer-be-safe-at-work-547578-2026-08-06)) | Example of GCCs swapping generalist roles for AI roles | visa.co.in/en_in/jobs (seen) |
| CrowdStrike / Wayfair / Mastercard / Coinbase | Security / e-commerce / fintech | Pune, Bengaluru, Remote-India | — | Backend Engineer II Go+Kafka (4); Engineer III AI-Powered SRE; SE II Java (3–5); SE II backend; SE Security Platform (3) | Go, Kafka (CrowdStrike); Java (Wayfair) | Not fetched | V ([Indeed](https://to.indeed.com/aa4rvpnjssc9); [Indeed](https://to.indeed.com/aacqzg6fh9zl); [Coinbase](https://www.coinbase.com/careers/positions/8165441?gh_jid=8165441)) | Fallback for SDE-2 platform roles | Company ATS |

### Category C: Indian product companies and unicorns

| Company | Domain | HQ / India | Stage (dated) | GenAI work and roles | Stack signal | Comp at 2–4 YOE | Evidence | Why target | Careers URL |
|---|---|---|---|---|---|---|---|---|---|
| **Razorpay** | Payments | Bengaluru | Private, IPO track | **Agent Studio on the Claude Agent SDK (12 Mar 2026)**; agentic payments with NPCI/OpenAI; Lead AI Engineer for the LLM gateway (5–8, removed Apr 2026); AI Builder roles | Go or Python; Kubernetes; Prometheus/OTel; LiteLLM, Portkey, Langfuse; token economics | SE ₹21.2L, SSE ₹40.7L (Levels.fyi); AmbitionBox SDE-2 figures conflict (₹24–37L vs ₹30–55L) | V ([Razorpay newsroom](https://razorpay.com/newsroom/razorpay-launches-the-worlds-first-ai-native-agent-studio-for-payments-at-ftx26-powered-by-anthropics-claude/)) | Named internal LLM platform team; agentic payments | razorpay.com/jobs (std); [Greenhouse](https://job-boards.greenhouse.io/razorpaysoftwareprivatelimited/jobs/4681550005) (seen) |
| **Swiggy** | Food / quick commerce | Bengaluru | Listed | **4 MCP servers, 66 tools for ChatGPT/Claude/Gemini ordering (Jan 2026)**; Hermes text-to-SQL V3 | MCP, LLM + SQL warehouse | L7 ₹38.3L | V ([Inc42](https://inc42.com/buzz/how-swiggy-is-using-ai-agents-to-take-commerce-beyond-its-app/); [InfoQ, Jan 2026](https://infoq.com/news/2026/01/swiggy-hermes-conversational-ai)) | Agentic commerce in production; but its public board showed no SDE roles on 27 Nov 2026 | careers.swiggy.com (std) |
| **Flipkart** | E-commerce (Walmart) | Bengaluru | Pre-IPO, IPO paused | Agentic e-commerce platform; 250+ models; SLAP assistant; "AI writes 40% of code" (Jul 2026) | Custom LLMs + frontier models | SDE2 ₹36.0L | V ([NewsBytes](https://www.newsbytesapp.com/news/science/flipkart-says-ai-now-writes-40-of-its-code/story)) | Scale; machine-coding-heavy loop | flipkartcareers.com (std) |
| **Groww** | Brokerage | Bengaluru | Listed Nov 2025 | **AI Engineer II (MCPs/tools for financial-data agents) and AI Engineer III (agentic systems + compliance guardrails), tagged 2–5 YOE (2026)** | MCP, agents, guardrails | Glassdoor SDE median ₹17L (self-reported, undated) | V ([Greenhouse](https://job-boards.eu.greenhouse.io/groww/jobs/4528373101)) | Best Indian-unicorn match at 2 YOE | job-boards.eu.greenhouse.io/groww (seen) |
| **Eternal (Zomato/Blinkit) + Nugget** | Food, quick commerce; AI support | Gurugram | Listed; OpenAI partnership (Feb 2026) | Nugget spun out as an enterprise AI support business (15M+ interactions/month) | OpenAI | Not fetched | V ([Inc42](https://inc42.com/features/eternals-enterprise-ai-turn-why-the-zomato-parent-spun-out-nugget/)) | Nugget is a natural FDE-style employer [E] | zomato.com/careers (std) |
| **PhonePe** | Payments | Bengaluru | IPO paused; targets Feb–Mar 2027 | OpenAI partnership; no AI posting found | — | SE2 ₹46.2L (Levels.fyi); old AmbitionBox ₹69–77L (Apr 2023) | V ([Inc42](https://inc42.com/buzz/with-upi-mdr-clarity-phonepe-eyes-ipo-by-march-2027/)) | High SDE-2 pay; listing timing affects equity | phonepe.com/careers (std) |
| **CRED** | Fintech | Bengaluru | Late-stage | No 2026 AI posting; Anthropic partner (Feb 2026) | — | L3 ₹29.4L; **L4 ₹63.6L** | V (pay) | Top Indian unicorn pay at L4 | cred.club/careers (std) |
| **Freshworks** | CX/ITSM SaaS | Chennai, Hyderabad, Bengaluru | NASDAQ; **11% layoff plan (Q1 2026)** | Freddy agentic layer, AI Agent Studio, MCP Gateway; Lead Solution Engineer (Aug 2026) | MCP Gateway | All-level median ~₹33.7L (Feb 2026) | V ([Inc42](https://inc42.com/buzz/freshworks-posts-4-8-mn-loss-in-q1-2026-to-lay-off-11-workforce/)) | Agent platform work; layoff risk | freshworks.com/company/careers (std) |
| **Jio / Reliance Intelligence** | Telecom, AI | Navi Mumbai, Bengaluru, Hyderabad | Jio IPO in preparation | Hiring AI/ML engineers for Indic LLMs; invited "cracked engineers" to pitch directly (Feb 2026) | JioBrain platform | Not fetched | V ([Digit](https://www.digit.in/news/general/india-ai-impact-summit-reliance-jio-fast-tracks-ai-hiring-chief-ai-scientist-invites-direct-pitches-at-the-mega-event.html)) | Direct-pitch hiring channel | careers.jio.com (std) |
| **Zoho** | SaaS | Chennai | Bootstrapped | Zia LLM (1.3B–7B), Agent Studio, MCP server (Jul 2025) | In-house LLM on NVIDIA | Not fetched | V ([BusinessWire](https://www.businesswire.com/news/home/20250717118204/en/)) | Own-model company; no 2026 hiring data | zoho.com/careers (std) |
| **Whatfix** | Digital adoption SaaS | Bengaluru | Late-stage | **FDE-AI (3–7, 16 Nov 2026)**; 3 AI agents; targets 25% of ARR from AI | LLM APIs, retrieval, agents, evals, **coding agents + spec-driven development as must-haves** | Not fetched | V ([Indeed](https://to.indeed.com/aazjxf46s9zc)) | Archetypal Indian-product FDE JD | whatfix.com/careers (std) |
| **HackerRank** | Developer hiring SaaS | Bengaluru | Late-stage | **FDE (₹30–45L posted, 3+)**; Senior Backend Engineer (3–6) | Kafka/RabbitMQ, Postgres; "AI fluency" section | ₹30–45L posted (FDE) | V ([YC](https://www.ycombinator.com/companies/hackerrank/jobs/6yUyOZa-forward-deployed-engineer)) | Rare disclosed FDE band | job-boards.greenhouse.io/hackerrank (seen) |
| **DevRev** | AI-native CRM/support | Bengaluru, NCR, Mumbai, Chennai | Private | FDE (5+, 3 Sep 2026); Forward Deployed Architect | — | Not fetched | V ([Greenhouse](https://job-boards.greenhouse.io/devrev/jobs/6174459004)) | Explicit FDE career track | job-boards.greenhouse.io/devrev (seen) |
| **Meesho / Zepto / Zerodha / Postman / BrowserStack / InMobi** | Various | Bengaluru, Mumbai | Meesho listed Dec 2025; Zepto IPO expected Feb–May 2027; InMobi IPO talks | BrowserStack AI testing agents + MCP server (Jun 2025); InMobi SDE II – AI (3–5, Jul 2026); Postman Senior Applied AI (5) | InMobi: Python, PyTorch, vector DBs, MCP | Meesho SE II ₹40.1L; Zerodha mostly cash | V/S ([InMobi](https://job-boards.greenhouse.io/inmobi/jobs/8073988)) | Opportunistic | Company sites (std) |
| Increff / Zeta / Seekho / Triomics / 100ms | Retail SaaS / banking tech / edtech / health | Bengaluru | Growth stage | **Increff SDE-II (2–4)**; **Zeta SRE II (2)**; Seekho SDE 2 (coding agents "baseline, not a perk"); Triomics SDE2 (3–5); **100ms AI Engineer – AI Agents (2–5, ₹20–50L)** | Java/Spring (Increff, Triomics); K8s/Envoy (Zeta); Django (Seekho) | 100ms ₹20–50L posted | V ([Indeed](https://to.indeed.com/aaqhlhnbmf4s); [Lever](https://jobs.lever.co/zeta/f827a249-2537-4f7f-aade-25b829fc13f2); [Accel](https://jobs.accel.com/companies/100ms-2/jobs/64657380-ai-engineer-ai-agents-healthcare)) | Minimums of 2 years | Company ATS (seen) |
| Krutrim / Dream11 | Ola AI cloud / fantasy gaming | Bengaluru / Mumbai | Krutrim: three layoff rounds, ~150 staff left (2026); Dream11: real-money gaming ban risk | — | — | — | V ([YourStory, Jul 2026](https://yourstory.com/2026/07/krutrim-lays-off-nearly-half-workforce)) | **Avoid** | — |

A sampling caveat matters for Category C. On 27 Nov 2026, several prominent unicorns showed almost no public mid-level backend hiring:

- Razorpay's Greenhouse board listed 2 engineering roles out of 23 postings.
- Meesho's board listed only EM and Security roles.
- Swiggy's board showed no SDE roles.
- CRED listed one engineering-titled role.

Source: the SDE JD-sampling note, observed 27 Nov 2026 ([Razorpay board](https://job-boards.greenhouse.io/razorpaysoftwareprivatelimited/jobs/4712147005)). Two readings follow. Indian unicorn hiring in late 2026 is selective and often runs through referrals or targeted AI teams rather than broad SDE-2 requisitions. And a candidate should not plan a search around their public job boards [E].

## 5. Emerging startup and industry landscape: concentrated capital, voice and agent platforms, and an infrastructure wave

Indian AI startup funding nearly doubled in 2026, but it is very concentrated, and that shapes where startup jobs will be. Tracxn counts **~$1.6B of AI funding in Jan–Sep 2026 (+96%)**, the highest nine-month total since 2019. **Neysa alone was 37% of it.** Infrastructure took **75% ($1.2B over 19 rounds)**. Application-layer funding fell 27% and vertical AI fell 87% ([People Matters / Tracxn](https://www.peoplematters.in/news/ai-and-emerging-tech/india-ai-funding-nearly-doubles-to-usd-16-billion-in-jan-sept-2026-tracxn-53503)). Inc42 tracks a different universe and gets similar momentum: **$676M across 57 deals in H1 2026** (over 4x YoY) and **$438M in Q3** (+265%) ([Inc42 H1](https://inc42.com/features/indian-ai-startup-funding-soars-over-4x-yoy-in-h1-2026-but-is-it-enough-to-compete-globally/); [Inc42 Q3](https://inc42.com/features/indian-ai-startup-funding-surges-265-yoy-in-q3-will-momentum-continue/)). The caution flags are equally clear. AIM reports that most startups were "starving" outside two big deals. **63% of surveyed investors** think AI valuations are above comfortable levels ([AIM](https://analyticsindiamag.com/ai-startups/indias-ai-funding-boom-in-h1-2026-left-most-startups-starving/)). Krutrim went from ~550 to ~150 staff, and Yellow.ai cut ~30% before announcing a SPAC. For a candidate, this means startup offers need runway diligence. The well-funded names are a short list.

### Category D: AI-native and deep-tech startups worth tracking

| Company | Domain | HQ / India | Latest round (dated) | Roles and hiring evidence | Comp signal | Why target / risk | Careers |
|---|---|---|---|---|---|---|---|
| **Sarvam AI** | Indic foundation models, agents | Bengaluru | Series B first close $234M led by HCLTech (Jun 2026); IndiaAI Mission's first pick; Sarvam 30B/105B open-sourced | Applied AI Engineer – Sarvam Agents (3–5; MCP servers at scale, hybrid search + reranking, evals; closed); Agent Engineer (3+; "shipped work matters more than years"); SDE2 API Platform (3; FastAPI → Go rewrite); Deployment Strategist; FDE (closed) | Anecdotal ₹84 LPA ML offer (single source) | India's flagship sovereign-AI company; loop reportedly has no LeetCode round | [Ashby](https://jobs.ashbyhq.com/sarvam/fa96b55d-0c77-423d-8eef-f579c8496adb) (seen) |
| **Emergent** | AI app builder ("vibe coding") | Bengaluru + SF | $130M Series C at $1.5B (15 Jul 2026) | No specific posting found | — | Fastest-growing Indian AI unicorn | — |
| **Neysa** | AI cloud / GPU | Mumbai | $600M+ (Feb 2026; amount disputed) | Not checked | — | Infra/MLOps track | — |
| **Simplismart** | Inference platform | Bengaluru | $14M Series B with NVIDIA, Accel (Oct 2026) | Not checked | — | Inference optimisation | — |
| **Portkey** | AI gateway / LLMOps | Bengaluru | $15M Series A, Elevation (20 Feb 2026) | Scaling go-to-market (solutions roles inferred) | — | Sits in the AI-engineer tooling layer | — |
| **TrueFoundry** | MLOps / LLM deployment | Bengaluru + SF | $19M, Intel Capital (Feb 2025) | **FDE – GTM** | — | Explicit FDE role | [Wellfound](https://wellfound.com/jobs/4520954-forward-deployed-engineer-gtm) (seen) |
| **Composio** | Agent tool integrations | Bengaluru + SF | $25M Series A, Lightspeed (2025) | Mentions AI coding tools in postings | — | Agent infrastructure | — |
| **Bolna** | Voice AI orchestration | Bengaluru | $6.3M seed, General Catalyst (20 Jan 2026), to expand **engineering and deployment teams** | FDE – Business | — | Direct FDE fit; voice AI is crowded | YC jobs (std) |
| **Smallest.ai / Gnani.ai** | Voice models | Bengaluru | $13M Series A (Jul/Aug 2026) / ~₹68 Cr (Mar 2026; IndiaAI pick) | Not checked | — | Voice-agent deployments | — |
| **Cekura (YC F24)** | Voice/chat agent testing | Bengaluru | YC | **FDE ₹15–30L**; MTS AI/SWE $40–60K | Posted | Evals-centred FDE | [WaaS](https://www.workatastartup.com/jobs/84800) (seen) |
| **Infer (YC S21)** | Insurance voice agents | Bengaluru | YC | **Applied AI Engineer ₹20–50L, 3+**; owns LLM-as-judge evals; DSPy/GEPA | Posted | Evals-heavy applied AI | [YC](https://www.ycombinator.com/companies/infer/jobs/1DhbYdF-applied-ai-engineer) (seen) |
| **Vahan (YC S19)** | Blue-collar hiring, voice | Bengaluru | YC | Lead AI Engineer ₹30–60L (5+); "golden set and regression gate" on every change | Posted | Benchmark for eval discipline | [YC](https://www.ycombinator.com/companies/vahan/jobs/7zvIddz-lead-ai-engineer) (seen) |
| **Nanonets** | Document AI / agents | Bengaluru | Not checked | **FDE, 2+ YOE** (Mar and Aug 2026) | — | FDE at exactly this experience level | [Accel](https://jobs.accel.com/companies/nanonets/jobs/71054302-forward-deployed-engineer) (seen) |
| **Ema** | Agentic "AI employee" | California + Bengaluru | $77M Series B, Creaegis (23 Sep 2026) | Go-to-market expansion (solutions/FDE inferred) | — | Enterprise agents | ema.co/careers (std) |
| **Yellow.ai** | Agentic CX | Bengaluru | $550M Nasdaq SPAC announced 3 Aug 2026; ~30% layoffs ~Dec 2025 | — | — | Post-SPAC risk | yellow.ai/careers (std) |
| **Atlan** | Data/AI governance, "context layer" | Singapore / India | $105M Series C (May 2024) | Context Engineering Studio (2026) | — | Context engineering | atlan.com/careers (std) |
| **Lyzr / Lab0 / Redapto** | Enterprise agent frameworks; "agents that run implementations" | Bengaluru | Lyzr $8M Series A (Oct 2025); Lab0 YC P26 (10 people) | Lab0 Founding Engineer (3; USD 30–60K + equity) | Posted | FDE-as-a-product companies | [YC](https://www.ycombinator.com/companies/lab0/jobs/hlPvGkT-founding-engineer) (seen) |
| **Cursor (India)** | AI coding | Bengaluru, New Delhi, Mumbai | US-funded | **FDE India, no experience minimum listed (28 Sep 2026)**; strong Python/TypeScript | — | Dream-tier FDE | cursor.com/careers (std) |
| **Cartesia** | Voice AI | Bengaluru | US-funded | FDE, 4+ yrs, ₹70–90L (aggregator only, unverified) | Unverified | Top-of-band FDE | — |
| Gushwork / Isomorph AI / Tsenta / Sei AI / workwise | SMB agents / founding roles | Bengaluru, Chennai | Seed–YC | Gushwork FDE (1–2); Isomorph (~2, 24 Nov 2026); Tsenta (3, ₹12–48L); Sei AI LLM Engineer (4, ₹20–50L + equity); workwise AI Engineer (3–5, ₹20–30L) | Posted | Safety tier, open at 1–3 years | [Lever](https://jobs.lever.co/gushwork/bf544796-090e-47fd-b05d-79b0b5339f92); [Wellfound](https://wellfound.com/jobs/5137295-founding-engineer-builder-experience-clone) (seen) |
| **E2E Networks / Yotta** | GPU cloud | Delhi/Chennai; Navi Mumbai | E2E ₹420.51 Cr raise; Yotta $150M at ~$3.9B | E2E Accelerated Computing Engineer (2–4, Chennai) | — | Compute-layer MLOps | [E2E](https://e2enetworks.com/careers/jobs/accelerated-computing-engineer) (seen) |

### Startup domains ranked by 2026–28 hiring potential

| Rank | Domain | Evidence (dated) | Hiring outlook for AI engineers [F] | Fit |
|---|---|---|---|---|
| 1 | Enterprise agents and "services-as-software" (sold to GCCs, BFSI, global SaaS) | 40% of large firms scaling agents (McKinsey 2026); Ema $77M (Sep 2026); Razorpay Agent Studio; Lab0, Lyzr | Highest and most durable | Very high |
| 2 | AI infrastructure, inference, sovereign cloud | 75% of AI funding (Tracxn, Jan–Sep 2026); Neysa, Yotta, E2E, Simplismart; IndiaAI 38,000+ GPUs onboarded (Feb 2026) ([PIB](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2227612&reg=3&lang=2)) | Rising in 2027–28 [F]; niche but well paid | Medium (pivot) |
| 3 | Voice AI for BFSI, collections and CX | Bolna, Ringg ($10M extension led by Peak XV, Aug 2026), Smallest, Gnani; described as crowded ([TechCrunch, 25 Aug 2026](https://techcrunch.com/2026/08/25/indias-ringg-gets-backing-from-peak-xv-as-it-pushes-voice-ai-past-the-phone-call)) | High volume, consolidation risk | High (FDE) |
| 4 | Fintech AI (regulated, data-rich) | Razorpay, Groww, PhonePe, Super.money agents (Sep 2026) | Steady | High |
| 5 | AI developer tooling / LLMOps | Portkey, TrueFoundry, Composio, Emergent, Cursor India | Selective, high pay | High |
| 6 | Indic LLMs | Sarvam, Soket, Gnani, BharatGen; 20 model proposals under IndiaAI (~Jul 2026) | A small number of elite roles | Medium |
| 7 | Defence tech and semiconductors | Defence tech funding a record $247M (2025); 12 ISM projects worth ₹1.64 lakh crore | Small software headcount | Low |

## 6. Actual job description analysis: 90 India JDs converge on agents, RAG and evals on top of production basics

Two independent samples were hand-coded from India-located postings viewed on **27 Nov 2026**:

- **Sample A:** 49 AI/GenAI/LLM, ML, MLOps, AI-infra and FDE/solutions JDs. 31 were still live; 18 had closed, most of them posted in 2026.
- **Sample B:** 41 SDE-2-equivalent backend, full-stack, platform and AI-platform JDs.

Sources were the Indeed connector, company ATS boards (Greenhouse, Ashby, Lever, Workday, amazon.jobs, Microsoft careers), YC/Wellfound, VC job boards and Cutshort. Both samples have a single coder and known skews. Sample A over-represents Google (8 JDs) and Bengaluru (~80%). Sample B over-represents MNCs (29 of 41) and misses the Java/Go-heavy unicorns (Flipkart, Swiggy, PhonePe, Razorpay backend). Both under-represent IT services, because Indeed rate-limited full-JD fetches after 14–20 calls. Within a category, one JD moves the percentage by 6–20 points. Read every figure below as directional. As a robustness check, the live-only Sample A subset (n=31) gives almost the same headline rates: Python 77%, agents 74%, RAG 68%, evals 65%.

| Sample | n | Category mix | Role mix | Stated minimum YOE |
|---|---|---|---|---|
| A: AI / FDE | 49 | Big Tech 16, Enterprise SaaS/GCC 7, Indian product 5, funded AI startup 5, early-stage 9, IT services 7 | AI/GenAI engineer 28, FDE/solutions 15, AI infra 3, MLOps 1, classic MLE 2 | 80% of the 45 stating a minimum set it at 2–5 yrs; most common is 4–5 (21 JDs) |
| B: SDE-2 / platform | 41 | Big Tech 13, SaaS/MNC 16, Indian product 6, India startups 6 | Backend, full-stack, platform/SRE, AI platform | Most common is "3+" (20 of 38); range 1+ (Google SWE II) to 5+ |

### 6.1 AI and FDE JDs: frequency by company category (Sample A, any mention)

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

### 6.2 SDE-2 JDs: frequency by company category (Sample B, any mention)

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

### 6.3 Mandatory versus preferred

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

### 6.4 Cross-category intersection

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

### 6.5 Experience floors: the binding constraint at 2 YOE

Counting the stated minimums gives a decisive result [E]. In Sample A, only **8 of 45 JDs (18%) set a minimum of 2 years or less**, and **18 of 45 (40%) set one of 3 years or less**. In Sample B the figures are **5 of 38 (13%)** at 2 years or less and **25 of 38 (66%)** at 3 years or less. Median minimums by category in Sample A are 5 years at Big Tech, Enterprise/GCC and services, 4 at Indian product companies, and 3 at AI startups and early-stage companies. These floors bend in practice:

- One LeetCode poster at 2 YOE reports an Amazon SDE-2 loop ([LeetCode](https://leetcode.com/discuss/post/7027366/amazon-sde-2-interview-experience-2yoe-h-ynf0/)).
- Sarvam's Agent Engineer JD says shipped work "matters more than years" ([Sarvam careers](https://www.sarvam.ai/careers/jobs/36f89b00-2010-4d23-aae3-17a2f53d9eaa)).
- Many startup "Senior" titles accept 3–5 years.

Even so, the numbers explain why this report splits applications into two waves. A move from 2 to 3 years of experience roughly **triples to quintuples the number of reachable JDs** in the SDE-2 band.

## 7. Technology stack demand matrix: what each role family actually asks for

The matrix combines both samples. It shows any-mention and mandatory rates, where each technology concentrates, and which role families need it most. "—" means no meaningful signal in that sample.

| Technology | AI/FDE any (n=49) | AI/FDE mandatory | SDE-2 any (n=41) | SDE-2 required | Concentrates at | Needed most by |
|---|---|---|---|---|---|---|
| Python | 78% | 73% | 63% | 37% | Everywhere; 100% of AI-startup and services AI JDs | All AI roles, AI-platform SDE |
| Agents / tool calling | 76% / 33% | 47% / 22% | 49% (any LLM work) | 20% | Enterprise/GCC, Indian product, AI startups | AI Eng, FDE |
| RAG | 63% | 43% | (inside LLM work) | — | AI startups, services, Big Tech | AI Eng, FDE |
| Evals | 63% | 37% | — | — | AI startups (100%), early-stage (78%) | AI Eng, FDE, emerging evals roles |
| Observability (general) | 47% | 14% | 37% | 22% | Product companies; FDE 67% | FDE, AI Eng, SRE |
| Cloud (any) | 51% | 41% | AWS 32 / Azure 27 / GCP 24% | low | Big Tech, services, FDE (73%) | FDE, AI Eng |
| LLM framework (any) | 53% | 29% | 7% (3 JDs) | — | Services (86%) | AI Eng (services), FDE |
| LangGraph / LangChain | 31% / 37% | 16% / 22% | — | — | Services, Big Tech (LangGraph 38%) | AI Eng |
| Vector DB | 39% | 22% | 2% | — | AI startups, services | AI Eng |
| TypeScript / JS | 33% | 22% | 10% / 15% | 2% | Early-stage, enterprise, FDE | FDE, founding roles |
| System design | 27% | 18% | 41% | 37% | Indian product (60% in A) | SDE-2, AI Eng |
| DSA | 16% | 12% | 32% | 29% | Big Tech, GCC | SDE-2, Big Tech AI Eng |
| Distributed systems | 14% | 8% | 39% | 15% | Big Tech, Indian product platform | SDE-2, AI platform, infra |
| Kubernetes | 20% | 10% | 41% | 15% | India startups (67% in B), services | Platform, AI infra, SDE |
| Docker | 22% | 10% | 32% | 12% | Services (71% in A) | All (baseline) |
| CI/CD | 29% | 14% | 41% | 22% | Services, SaaS | All (baseline) |
| PostgreSQL | 4% | 2% | 22% | 17% | India startups (67% in B) | AI-platform SDE, startup AI Eng |
| Redis | 2% | 2% | 20% | 10% | India startups | AI-platform SDE |
| Java (+ Spring Boot) | 16% | 10% | 61% (15%) | 24% (15%) | Big Tech (85% in B), enterprise | SDE-2 at Big Tech/GCC |
| Go | 16% | 12% | 34% | 15% | SaaS, startups, LLM gateways | Platform, AI infra |
| MCP | 18% | 4% | 10% | — | Big Tech (38% in A) | AI Eng, FDE, AI platform |
| Fine-tuning / post-training | 24% | 16% | — | — | Enterprise ML (57%), AI startups (60%) | MLE, AI startups |
| AI coding tools | 10% | 8% | 32% | 22% | Indian product, startups, Adobe | All engineering roles |
| Guardrails | 18% | 14% | — | — | Services, enterprise | AI Eng (BFSI, enterprise) |
| Context engineering / memory | 12% | 10% | — | — | Indian product, AI startups | AI Eng |
| Voice / ASR / TTS | 14% | 2% | — | — | AI startups, early-stage | Voice-agent FDE/AI Eng |
| LLM observability tools | 10% | 2% | — | — | AI startups | AI Eng, LLMOps |
| Kafka | 10% | 2% | 22% | 5% | SaaS, India startups | SDE-2, data platform |
| PyTorch / Hugging Face | 16% / 10% | 14% / 8% | (InMobi, Adobe) | — | Enterprise ML | MLE |
| vLLM / Triton / TensorRT / CUDA | 6% / 2% / 2% / — | — | — | — | NVIDIA, inference startups | AI infra only |
| Terraform | 4% | 2% | 10% | 7% | Google FDE GECX, Databricks, Zeta | Platform, hyperscaler FDE |
| React | — | — | 12% | 5% | Rippling, Databricks agentic full-stack | Full-stack AI products |
| Spark / Airflow / Snowflake | 12% / 4% / 4% | — | — | — | Cisco, Wayfair | Data/MLE |
| CrewAI / AutoGen / Semantic Kernel / DSPy / A2A | 10% / 6% / 4% / 4% / 2% | 0–2% | — | — | Preferred-only | None as a gate |

Source: both JD registers, viewed 27 Nov 2026. Each register's appendix lists every JD with its URL; representative links are cited in Section 6.

## 8. Technology priority ranking: seven skills to master, a long tail to ignore

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

## 9. Compensation benchmark report: at ~2 YOE the level you land at outweighs your title or city

Three facts organise the compensation picture.

1. **Employer tier and level dominate.** At Levels.fyi medians, moving from L3 to L4 (or SDE I to SDE II) roughly doubles total compensation: Google ₹38.9L → ₹66.5L, Amazon ₹28.9L → ₹63.2L, Uber ₹34.4L → ₹70.3L, CRED ₹29.4L → ₹63.6L ([Levels.fyi company pages, viewed 26–27 Nov 2026](https://www.levels.fyi/companies/google/salaries/software-engineer/locations/india)).
2. **The "AI premium" is real but conditional.** The Levels.fyi ML/AI median (₹29.0L, n=1,297) is slightly *below* the all-SWE median (₹30.8L) because of a mix effect. TeamLease's GCC data shows **GenAI Engineers at 0–2 YOE earning ₹13.2 LPA median fixed pay, about 22% more than Data Scientists (₹10.8L) and 29% more than Data Engineers (₹10.2L)** ([TeamLease Digital, Oct 2026](https://cxotoday.com/others/teamlease-digital-44-of-indian-gccs-own-full-platforms-ai-outcomes-as-compensation-tops-₹108-6-lpa/)). foundit finds AI-skill salaries up ~23% since 2024 while legacy IT pay stagnated ([Free Press Journal, Sep 2026](https://www.freepressjournal.in/business/ai-job-salaries-jump-23-since-2024-as-legacy-tech-pay-declines-report)).
3. **FDE pay data is the weakest in the set.** No Levels.fyi Palantir India data exists. The Glassdoor Bengaluru FDE average (~₹17L, range ₹11–36L) rests on about 9 data points ([fdeindia.live / Taggd compilation](https://taggd.in/blogs/forward-deployed-engineers/)).

### 9.1 By company category at ~2 YOE

| Category | Company / level likely at ~2 YOE (inferred mapping) | Reported median TC (₹ L) | Estimated base share [E] | Reported or estimated |
|---|---|---|---|---|
| Top-tier infra/fintech MNC | Databricks L3 68.5 / L4 100; Rubrik L3 68.7 / L4 97.8; Stripe L1 56.9 / L2 100 | **57–100** | ~55–65% | Reported (Levels.fyi) |
| Big Tech at L4 / SDE II / IC2 | Google L4 66.5; Amazon SDE II 63.2; Uber L4 70.3; Atlassian P40 69.6; LinkedIn IC2 62.6 | **63–70** | ~55–65%; one Google L4 split: base ₹40.8L of ~₹69.8L average (search summary, unverified) | Reported |
| Big Tech if levelled one step lower | Google L3 38.9; Amazon SDE I 28.9; Uber L3 34.4; Atlassian P30 43.8; LinkedIn IC1 46.8 | **29–47** | ~60–70% | Reported |
| Big Tech / MNC lower bands | Microsoft 61 41.9 / 62 65.1; Adobe P20 35.3 / P30 54.6; NVIDIA IC2 34.2; Salesforce MTS 48.9; Intuit SE2 46.6; ServiceNow IC2 41.6 | **34–55** | ~60–75% | Reported |
| Mid-tier enterprise SaaS | SAP T2 24.7 / T3 45.2; Oracle IC-2 27.6; Snowflake IC2 27.7 | **25–28** (45 at the next level) | ~70–85% | Reported |
| High-pay Indian / India-centred | CRED L4 63.6; PhonePe SE2 46.2; Rippling L5 45.5 | **45–64** | ~65–80% | Reported |
| Indian unicorns | Flipkart SDE2 36.0; Swiggy L7 38.3; Meesho SE II 40.1; Razorpay SE 21.2 → SSE 40.7 | **21–41** | ~70–85% | Reported |
| Bank/retail GCCs | Goldman Analyst 33.0 / Associate 39.5; Walmart P3 33.9 | **33–40** | ~75–90% | Reported. The AIM all-level GCC median is ₹18.4 LPA ([AIM](https://analyticsindiamag.com/ai-highlights/global-capability-centers-gccs-salary-trends-in-india-2026)) |
| Funded AI startups (posted bands) | 100ms AI Engineer (2 YOE) ₹20–50L; Infer (3) ₹20–50L; Sei AI (4) ₹20–50L + equity; Tsenta (3) ₹12–48L; workwise (3) ₹20–30L | **20–50** | ~85–100% cash + ESOP | Reported (posted) |
| Early-stage FDE / generalist | Zirodigital ₹7L (0–2); Weekday client FDE ₹15–23L (2+); Cekura FDE ₹15–30L | **7–30** | ~90–100% | Reported (posted) |
| IT services | Mass-market software engineer base ~₹8.9 LPA (Indeed); tech-services increments 6.6% (Aon 2026) | **well below 15** | ~95% | Reported (aggregate) |

Base-share estimates are an analyst inference, built from three inputs: the single Google L4 split, Zerodha's all-cash structure on the Levels.fyi leaderboard (19 Nov 2026), and the common pattern that RSUs make up a larger share at US MNCs. Levels.fyi did not provide base/stock/bonus splits for India levels in this research.

### 9.2 By role at ~2 YOE

| Role | Best-supported range | Top-of-band signal | Evidence quality |
|---|---|---|---|
| SDE-2 (Big Tech / top SaaS) | ₹63–70L TC at L4; ₹29–47L if levelled L3 | Databricks/Rubrik L4 ~₹1 Cr | Medium-high (Levels.fyi, self-reported) |
| SDE-2 (unicorn / GCC) | ₹33–46L TC | CRED L4 ₹63.6L | Medium |
| Applied AI / GenAI Engineer | ₹20–50L at funded startups (posted); ₹13.2L median fixed at GCC entry (0–2 YOE); Big Tech AI Engineers sit on SDE ladders [E] | Lead roles ₹30–60L (Vahan, 5 YOE) | Medium-low (posted bands, n=10 salary-listed JDs) |
| FDE / AI FDE | ₹12L average base (Indeed, ₹9–16L); ₹15–45L posted at 2–3+ YOE; Big Tech FDE likely tracks the SDE ladder [E] | HackerRank ₹30–45L (3+); Cartesia ₹70–90L (4+, unverified) | **Low** (Glassdoor n≈9; no Levels.fyi data) |
| Solutions Architect / Customer Engineer | Levels.fyi median ₹45.9L (n=334, mostly mid/senior) | Cisco ₹78.3L, AWS ₹74.0L (all levels) | Medium for mid/senior; no 2-YOE split |
| ML Engineer | ₹18–30L at 3–5 YOE (aggregator); Levels.fyi ML/AI median ₹29.0L (all levels) | GenAI/LLM +25–40% vs generalist ML (Instahyre via InterviewBit) | Low-medium; sources conflict |
| MLOps / AI infra | No India level data | >18% annual raises (TeamLease, Aug 2025) | **Gap** |

### 9.3 By city

| City | Levels.fyi SWE median TC | P75 / P90 | Read-across |
|---|---|---|---|
| Bengaluru | **₹37.1L** (n=11,405) | ₹57.7L / ₹79.6L | Top payers are concentrated here (Broadcom, Airbnb, Rippling, Rubrik, Stripe) |
| Hyderabad | ₹31.6L (n=2,985) | ₹50.2L / ₹70.1L | Microsoft, Amazon, Google, ServiceNow |
| Delhi NCR | ~₹21.4L (2025 heatmap average) | — | City page not found; small sample |
| Pune | ₹21.1L (n=1,748) | ₹32.8L / ₹47.8L | More services and GCC-heavy |
| Mumbai | just under ₹20L (2025 heatmap average) | — | City page not found |
| Chennai | ₹18.1L (n=995) | ₹29.6L / ₹46.4L | Lowest median of the six |

Other city indices disagree. Hyring ranks Gurugram highest, at ₹10.8–11.9L on a mass-market base. Futurense indexes Hyderabad at 115–130 against a national 100 ([Hyring](https://hyring.com/blog/software-engineer-salary-india/); [Futurense](https://futurense.com/blog/software-developer-salary-in-india)). The consistent reading is that city medians mostly reflect employer mix. Same-company, same-level pay across cities was not available [gap].

### 9.4 Hikes, switching and the Japan question

In-place increments are about **9.0% in 2026, with 9.1% projected for 2027**. Attrition rose to 18% ([Aon, 2026](https://www.aon.com/apac/in-the-press/asia-newsroom/2026/aon-study-finds-salaries-in-india-projected-to-fise-9-1-in-2027-employers-balance-growth-and-cost-pressures)). Switch expectations cluster at 21–40%: 27% of respondents expect 21–30% and 23% expect 31–40% ([Business Today / foundit, 23 Jul 2026](https://www.businesstoday.in/jobs/story/almost-everyone-is-looking-to-switch-jobs-but-only-if-employers-meet-this-pay-demand-544684-2026-07-23)). Michael Page reports switch hikes **up to 30%** in AI fields ([Outlook Business](https://www.outlookbusiness.com/corporate/ai-ev-chip-roles-command-30-pay-hikes-three-times-market-average)). One more data point argues against relying on raises at the current employer: a Blind survey (Oct 2026, seen only in a search snippet) found that 35% of India-based tech workers got no hike or a pay cut ([Blind](https://www.teamblind.com/blog/1-in-3-indian-tech-workers-got-no-hike-or-a-pay-cut-this-year/)).

The most important unknown is how an Indian recruiter will anchor an offer for someone coming from Tokyo. **No source quantified this.** Indian offers are usually anchored to current CTC. A Japanese salary converted at nominal FX could either help or hurt, depending on the band. The safe tactic [E] is to never lead with the converted current salary. Anchor instead on the target company's level band, as Levels.fyi medians show, and on a competing Indian offer. Negotiate the **level** first and the number second.

## 10. 2026–2028 industry forecast: production AI skills earn a premium in every scenario

No institution has published an India tech-hiring forecast for 2027–2028. The scenarios below are therefore **analyst constructions [F]** built on dated anchors:

- Headcount +2.3% in FY26 (NASSCOM, Feb 2026).
- AI/ML postings +20–49% through 2026 (Naukri), with foundit forecasting +32% for 2026.
- 2,117 GCCs (Zinnov-NASSCOM, Jul 2026).
- 40% of large firms scaling agents, up from 27% (McKinsey 2026).
- India FDE postings slowing from 19x to 6x YoY between June and August 2026 (Indeed).
- Tech funding +7% while deal count fell 38% (Tracxn, Sep 2026).

Projected supply is the backdrop. Deloitte-NASSCOM projects India's AI talent pool to grow past 1.25M by 2027 ([Deloitte, Aug 2024](https://www.deloitte.com/in/en/about/press-room/bridging-the-ai-talent-gap-to-boost-indias-tech-and-economic-impact-deloitte-nasscom-report.html)). Bain sees 2.3M+ AI openings by 2027 against a pool of ~1.2M ([Gulf News](https://gulfnews.com/world/asia/india/indias-ai-sector-poised-to-surpass-23-million-job-openings-by-2027-1.500056470)). Business Standard reads the Deloitte 1.25M figure as demand rather than supply, so even that anchor is contested. The scenario probabilities are subjective.

| Dimension | Conservative (~25%) | Expected (~55%) | Optimistic (~20%) |
|---|---|---|---|
| Triggers | US recession or tariff shock; AI capex pullback and "ROI disappointment"; GPU and power delays in India; IT clients cut discretionary spend | Steady enterprise agent adoption; continued GCC expansion; H-1B costs keep pushing work to India | Agent adoption spreads to mid-market companies; GCC setups accelerate; Vizag and IndiaAI compute arrive on schedule; application-layer AI funding recovers |
| Tech headcount growth | 0–1% a year; more middle-management cuts at IT services | +2–4% a year | +5–6% a year |
| AI/ML postings growth | ~5–10% a year, concentrated in GCCs and Big Tech | ~15–25% a year; AI skills spread into most SDE JDs | 30%+ a year, sustained |
| GCCs by 2028 | ~2,250–2,350 | ~2,400–2,600 | 2,700+, with the first AI-native GCCs |
| FDE / applied-AI roles | Startup FDE titles shrink; the work moves into Big Tech and services AI practices | Grow from hundreds to low thousands of openings; the title partly merges into "Applied AI Engineer" and "AI Solutions Engineer" | Become a mainstream track, including India-based roles serving US/EU clients at global-band pay |
| Startups | Voice and wrapper startups fail; consolidation | A few well-capitalised winners hire; most stay small | One or two Indic/voice winners hire hundreds each; a distinct MLOps market emerges |
| Junior / generic SDE | Hit hardest | Flat volume at a higher bar (AI-tool fluency, projects) | Recovers only in AI-augmented roles |
| Pay | Flat for production-AI seniors; cuts elsewhere | GenAI premium holds (TeamLease projects senior GenAI pay rising from ₹28L in FY25 to ₹33.5L in FY27) | Premium widens; global bands spread |
| **Implication for this candidate** | Prioritise Big Tech/GCC AI roles; avoid seed-stage offers without 24+ months of runway | Plan as written: AI Engineer + FDE lanes, Wave 1 and 2 | Push for FDE / global-facing roles and higher levels; consider a labs Applied AI role by late 2028 |

Four conclusions hold in all three scenarios, and they are the basis for the strategy. **Production AI skills earn a premium. Generic junior coding and "prompt engineer" titles are oversupplied. GCCs and Big Tech India are a steadier demand base than startups. And H-1B costs favour roles based in India over relocation to the US.**

### Rising, oversaturating, commoditising and premium

| Category | 2026–28 call [F] | Evidence anchor (dated) |
|---|---|---|
| **Rising roles** | Applied AI / agent engineer; AI platform engineer (LLM gateways, eval infrastructure, agent runtimes); FDE / deployment engineer (growing, but the title normalises); LLMOps / inference / GPU platform (2027–28 wave); AI security and governance engineer | Agents 76% of AI JDs; Razorpay LLM gateway, Sarvam API platform; FDE growth slowing to 6x; IndiaAI 38,000+ GPUs (Feb 2026); Google SWE II AI Security / Model Armor (Pune, 24 Nov 2026) |
| **Oversaturating roles** | Generic "prompt engineer"; junior generic SDE and manual QA; dashboard data analysts; IT-services bench roles | Prompt-engineer titles absorbed into AI Engineer roles (MentorCruise / LetsDataScience, 2026); 55% of firms cut entry-level hiring; data & analytics was the posting category that mentioned AI most (38.6%, Indeed Sep 2025) ([Indeed Hiring Lab](https://hiringlab.indeed.com/?p=20708)) |
| **Commoditising skills** | Basic "chat with PDF" RAG; LangChain tutorial apps; prompt crafting; GenAI certificates; framework name lists | 2M+ upskilled (NASSCOM); vertical/application AI funding −87% / −27% in 2026, a sign that thin wrappers struggle (Tracxn) |
| **Premium skills** | Production agent engineering (tools, state, guardrails); evals and observability; inference and cost engineering; AI security; customer-facing deployment; domain + AI (BFSI, insurance, healthcare); distributed systems combined with AI-assisted coding | Evals in 63% of AI JDs, 100% at AI startups; salary-listed JDs with a ₹48L+ upper bound cluster on agent + eval ownership, voice and fine-tuning; GCC GenAI premium of 30–40% (EY / TeamLease) |
| **Startup domains** | Enterprise agents > AI infrastructure > voice AI > fintech AI > AI dev tooling > Indic LLMs > defence/semiconductors | Section 5 ranking |

## 11. Role difficulty and competition analysis: frontier labs and Big Tech SDE-2 are hardest, AI-native startups most accessible

The scores are **analyst estimates [E]** on a 1–10 scale for a ~2-YOE candidate. They are anchored to the interview evidence in Section 16 (round structures from LeetCode, Glassdoor and prep-site reports, 2025–2026), the JD minimums in Section 6.5, and the competition signals in Sections 2–3. No survey measures interview difficulty or applicant volume in India directly. The interview research rated individual loops as follows: Google L4 8–9, Databricks 8–9, Atlassian P40 7–8, Palantir FDSE 7–8, Amazon SDE-2 7, Flipkart SDE-2 7, Razorpay/Swiggy 6–7, OpenAI/Anthropic FDE/Applied AI 9–10, Sarvam ML/inference 8–9, Sarvam agent/applied 6–7.

| Role archetype (example employers) | Technical | Interview | DSA | System design | AI/ML depth | Project expectations | Competition | Experience expectations | Reachable at ~2 YOE? |
|---|---|---|---|---|---|---|---|---|---|
| Big Tech SDE-2 (Google L4, Amazon SDE II, Microsoft 61–62) | 8 | 8–9 | 9 | 7 | 3 | 5 | 9 | 7 | Stretch; risk of down-levelling to L3 |
| Indian unicorn SDE-2 (Flipkart, Swiggy, Razorpay, Groww) | 7 | 7 | 7 | 8 (LLD knockout) | 2 | 5 | 8 | 6 | Possible with LLD prep |
| Tech-first MNC AI Engineer (Cisco AI Engineer, Microsoft Applied AI Engineer II, Google Cloud AI Engineer) | 7 | 7–8 | 6 | 7 | 6 | 7 | 7 | 7 (3+) | Wave 2 |
| AI-native startup AI Engineer (Sarvam Agent Engineer, Infer, 100ms, Whatfix) | 7 | 6–7 | 3 | 6 | 7 | 9 | 6 | 4 | **Yes; best ratio of fit to bar** |
| Bank/retail GCC GenAI Engineer (Walmart GT, Amex, JPMorgan) | 6 | 6 | 5 | 5 | 5 | 5 | 6 | 6 | Yes |
| Big Tech GenAI FDE (Google Cloud, YouTube, Meta, Cisco) | 8 | 8 | 6 | 7 | 6 | 7 | 6 | 8 (2–8; varies by level) | Selective (Google FDE V Data Cloud: 2 yrs) |
| SaaS / AI-native FDE (HackerRank, DevRev, Whatfix, Databricks, ServiceNow) | 7 | 7 | 4 | 6 | 6 | 8 | 5 | 7 | Wave 2 |
| Early-stage FDE (Nanonets, Gushwork, Cekura, Isomorph) | 5 | 5 | 3 | 4 | 5 | 7 | 5 | 3 | **Yes (safety)** |
| Frontier-lab Applied AI (OpenAI, Anthropic India) | 9 | 9–10 | 6 | 9 | 8 | 9 | 10 | 10 (10+ for Bengaluru architect) | No (revisit after 2028) |
| ML Engineer (Google MLE, Uber, Adobe) | 8 | 8 | 7 | 7 | 9 | 7 | 7 | 7 | Unlikely without training depth |
| MLOps / AI infra / inference (NVIDIA, Sarvam Platform, E2E Networks) | 8–9 | 8 | 5 | 8 | 7 | 7 | 4 | 7 (E2E: 2–4) | Pivot lane only |
| Emerging titles (Agent Engineer, Evals Engineer) | 7 | 7 | 3 | 6 | 7 | 8 | 4 | 6 (3–7) | Wave 2 |
| IT services GenAI engineer (Infosys, Wipro, Accenture, NTT DATA) | 5 | 4–5 | 3 | 3 | 5 | 4 | 7 | 4–5 (Infosys: 2–5) | Yes, but low pay |

The competitive structure explains the strategy [E]. Big Tech SDE-2 has the largest pool of well-prepared rivals: India's DSA-prep culture, and only ~15% of Big Tech openings being entry-level ([Rest of World, Feb 2026](https://restofworld.org/2026/h1b-visa-impact-india-tech-hiring-faamng/)). This candidate's AI experience barely helps in those loops. In AI-native and FDE loops, the competition falls sharply. Those loops reward shipped systems, eval stories and customer conversations ([techinterview.org, Jul 2026](https://www.techinterview.org/post/3233476824/ai-engineer-interview-rag-agents-evals/)), which most certificate-holders cannot show. The best expected value is to compete where the bar measures what the candidate already does, and to put enough DSA practice in to clear the one coding round that remains in those loops.

## 12. Recommended career direction: market one identity, run four lanes

**Positioning.** Market one identity: *"AI Engineer who ships production agents with evals, and deploys them with enterprise customers."* One sentence covers both the AI Engineer title (volume) and the FDE title (premium). It is truthful for a Tokyo AI Engineer/FDE and matches the cross-category core in Section 6.4. On the resume, use a title such as "AI Engineer (Forward Deployed)" or "Applied AI Engineer". Do not alternate between titles.

| Rank | Lane | Search titles | Share of applications [E] | Apply window | Target employers (examples) | Expected TC at ~2–3 YOE |
|---|---|---|---|---|---|---|
| 1 | **A. Applied / Agentic AI Engineer** (product, tech-first GCC, funded startup) | AI Engineer, Applied AI Engineer, GenAI Engineer, Agentic AI Engineer, Agent Engineer, LLM Engineer | ~45% | Wave 1 (startups, ≤3-yr minimums) + Wave 2 (MNCs at 3+) | Cisco, Microsoft Applied AI, Groww, Razorpay AI, Sarvam, Whatfix, 100ms, Infer, Walmart GT, Amex, Glean | ₹25–50L; ₹40–65L at MNCs |
| 2 | **B. AI FDE** | Forward Deployed Engineer, AI FDE, Deployment Engineer, Applied AI Engineer (labs) | ~25% | Wave 1 for postings at ≤2–3 yrs (Google FDE V Data Cloud, Cursor, Nanonets); Wave 2 for 3–5 | Google Cloud, YouTube, Meta, Cisco, Cursor, HackerRank, DevRev, ServiceNow, Databricks, MongoDB, Adobe | ₹30–45L startups/SaaS; Big Tech on its SDE ladder |
| 3 | **C. AI-platform SDE-2** (stretch, for the pay ceiling) | Software Engineer II/III (AI), SDE II, Applied AI Engineer II | ~15% | Wave 1 for Google SWE II/III (1–2 yr minimums) and Rubrik (2); Wave 2 for Amazon/Microsoft (3+) | Google, Microsoft, Amazon, Rubrik, Databricks, LinkedIn, Rippling, MongoDB | ₹63–70L at L4; ₹29–47L if levelled L3 |
| 4 | **D. Safety lane** | Founding Engineer, FDE, GenAI Engineer | ~15% | Wave 1 | Nanonets, Gushwork, Cekura, Isomorph, Infosys, Wipro, NTT DATA, Fractal | ₹15–30L |

**Cities.** Lead with **Bengaluru**, which has the densest FDE and AI listings and the highest medians. Add **Hyderabad**, the fastest-growing city for AI/ML (+15%, Oct 2026), home to Microsoft's AI platform teams, Amazon and ServiceNow's largest engineering site. Accept **Delhi NCR or Mumbai** for FDE roles (MongoDB, DevRev, Cursor, OpenAI, Google Cloud FDE location options). Treat **Pune** as role-specific (Google Model Armor, NVIDIA, Snowflake). Treat **Chennai** as the lowest priority on pay, unless the employer is a top payer.

**What not to do.** Drifting into pre-sales-only "solutions" roles trades production-engineering credibility for quota exposure. DataCamp argues that it is easier for an engineer to add customer skills than for a solutions engineer to add production-engineering skills ([DataCamp](https://www.datacamp.com/blog/what-is-forward-deployed-engineer)). Classical ML Engineer roles expect training depth that applied work rarely builds. IT-services GenAI roles pay a fraction of product bands, and Aon projects their increments at 6.6%. Keep them as a safety net, not a destination. Seed-stage offers without at least 24 months of runway carry real risk in a market where October 2026 funding fell ~61% YoY.

**Decision gates [E].** By **month 9 (Aug 2027)**, if LeetCode mediums are not solved in about 30 minutes at least 70% of the time, shrink Lane C to Google-only and move its share into Lane A. If by **month 14 (Jan 2028)** Wave 1 has produced no offer at ₹30L+ in TC, stay in Tokyo and accumulate experience. That keeps Wave 2's 3-year-minimum pool open, rather than accepting a down-levelled offer, because the level gap compounds at every later raise.

## 13. Primary technology stack: Python-first production LLM systems, nothing more

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

### Skills inventory: have, strengthen, acquire

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

## 14. Company target list: 11 dream, 18 target and 10 safety employers, sequenced by experience minimums

Tiers combine three things: pay and brand (Section 9), fit with the stack (Section 13), and **reachability at the stated minimum experience** (Section 6.5). "Wave" says when to apply. W1 = Oct 2027–Feb 2028 at ~2 YOE. W2 = May–Sep 2028 at ~2.5–3 YOE. URL status: **seen** means the URL appeared in sourced results. **std** means the standard careers domain, which was not fetched in this research and should be confirmed before use.

### Dream tier (high pay or brand, competitive)

| Company | Role to target | City | Stated minimum seen (date) | Wave | Comp signal at ~2–3 YOE | Careers URL | Status |
|---|---|---|---|---|---|---|---|
| Google / Google Cloud | FDE V GenAI (Data Cloud); SWE II/III Cloud AI / AI Security | Bengaluru, Hyderabad, Pune | 1–2 yrs (Nov 2026) | W1 | L4 ₹66.5L (L3 ₹38.9L) | https://careers.google.com | std |
| Databricks | AI Engineer – FDE; SE (Infra/AI) | Bengaluru, Mumbai, Delhi | 3–5; FDE "extensive" (2026) | W2 | L3 ₹68.5L; L4 ₹1.00Cr | https://databricks.com/company/careers | seen |
| Rubrik | Software Engineer (Cloud Native Protection) | Bengaluru, Pune | 2 yrs (11 Nov 2026) | W1 | L3 ₹68.7L | https://www.rubrik.com/company/careers | seen |
| LinkedIn | SWE (AI/ML, agentic hiring products) | Bengaluru | Mostly Staff in 2025 postings | W2 | IC2 ₹62.6L | https://careers.linkedin.com | std |
| Rippling | Software Engineer II (AI lab) | Bengaluru | 3 yrs (12 Nov 2026) | W2 | L5 ₹45.5L; L6 ₹67.2L | https://www.rippling.com/careers | std |
| Microsoft | Applied AI Engineer II; SWE II Core AI (Foundry Agentic) | Hyderabad, Bengaluru, Noida | 3 yrs (Oct–Nov 2026) | W2 | 61 ₹41.9L; 62 ₹65.1L | https://apply.careers.microsoft.com | seen |
| Meta | Forward Deployed Engineer, Enterprise AI | Bengaluru | Not captured (13 Nov 2026) | W1/W2 | Not fetched | https://www.metacareers.com | std |
| Cursor | Forward Deployed Engineer (India) | Bengaluru, New Delhi, Mumbai | None stated (28 Sep 2026) | W1 | Not disclosed | https://cursor.com/careers | std |
| Glean | SWE – Machine Learning / Backend | Bengaluru | Not captured | W2 | Leaderboard #4 (L2) | https://job-boards.greenhouse.io/gleanwork | seen |
| Sarvam AI | Agent Engineer; Applied AI Engineer (Sarvam Agents); SDE2 API Platform | Bengaluru | 3+ ("shipped work matters more than years") | W1 | Anecdotal ML offer ₹84L (single source) | https://jobs.ashbyhq.com/sarvam | seen |
| Atlassian | FDE, AI; P40 SWE | Bengaluru (remote-first) | 5+ for FDE (Feb 2026); SWE 8+ (Nov 2026) | W2 (watch) | P40 ₹69.6L | https://www.atlassian.com/company/careers | std |
| *Beyond the window* | OpenAI / Anthropic Applied AI Engineer or Architect | Delhi, Mumbai, Bengaluru | Anthropic Bengaluru architect 10+ (24 Nov 2026) | 2029+ | n/a | https://openai.com/careers ; https://www.anthropic.com/careers | seen / std |

### Target tier (strong fit, realistic)

| Company | Role to target | City | Stated minimum seen (date) | Wave | Comp signal | Careers URL | Status |
|---|---|---|---|---|---|---|---|
| Cisco | AI Engineer (CloudX); FDE | Bengaluru | 3 yrs (24 Nov 2026) | W2 (W1 if flexible) | SA top payer ₹78.3L (all levels) | https://jobs.cisco.com | std |
| ServiceNow | Forward Deployed Software Engineer – Gen AI | Hyderabad | Not captured (2026) | W1/W2 | IC2 ₹41.6L | https://careers.servicenow.com/locations/apj/india/ | seen |
| Adobe | Computer Scientist-I (GenAI); Firefly FDE | Noida, Bengaluru | 4–5 (Nov 2026) | W2 | P20 ₹35.3L; P30 ₹54.6L | https://www.adobe.com/careers.html | seen |
| Intuit | GenOS / AI engineering | Bengaluru | Mostly Staff in postings seen | W2 | SE2 ₹46.6L | https://jobs.intuit.com | seen |
| Salesforce | Agentforce engineering / FDE | Hyderabad, Bengaluru | Not captured | W2 | MTS ₹48.9L | https://careers.salesforce.com | std |
| MongoDB | SE3 AI Framework Integrations; FDE | Gurugram | 3+ (SE3); 5+ (FDE) | W2 | Not fetched | https://www.mongodb.com/careers/locations/gurugram | seen |
| Uber | SWE / ML on India product teams | Bengaluru, Hyderabad | Varies | W2 | L4 ₹70.3L | https://www.uber.com/careers | std |
| Amazon | SDE II (AI/LLM teams, e.g. Alexa LLM inference) | Hyderabad, Bengaluru | 3 + 2 design (Sep–Nov 2026) | W2 | SDE II ₹63.2L | https://www.amazon.jobs | seen |
| Whatfix | Forward Deployed Engineer – AI | Bengaluru | 3 (16 Nov 2026) | W1/W2 | Not disclosed | https://whatfix.com/careers | std |
| HackerRank | Forward Deployed Engineer | Bengaluru | 3+ | W2 | ₹30–45L posted | https://job-boards.greenhouse.io/hackerrank | seen |
| DevRev | Forward Deployed Engineer | Bengaluru, NCR, Mumbai, Chennai | 5+ (3 Sep 2026) | W2 (stretch) | Not disclosed | https://job-boards.greenhouse.io/devrev | seen |
| Razorpay | AI platform / AI Builder roles | Bengaluru | Lead role 5–8 | W2 | SSE ₹40.7L | https://razorpay.com/jobs | std |
| Groww | AI Engineer II / III | Bengaluru | 2–5 (2026) | **W1** | Not fetched | https://job-boards.eu.greenhouse.io/groww | seen |
| Walmart Global Tech | Software Engineer II (agentic) | Bengaluru, Chennai | 3 (Jun 2026) | W1/W2 | P3 ₹33.9L | https://careers.walmart.com | std |
| American Express / JPMorgan | AI Engineer III / AI data pipelines | Bengaluru, Hyderabad, Mumbai | Not captured | W2 | Not fetched | https://www.americanexpress.com/en-us/careers/ ; https://careers.jpmorgan.com | std |
| CRED / PhonePe / Swiggy / Flipkart | SDE-2 / AI teams (often through referrals) | Bengaluru | Boards thin (Nov 2026) | W2 | CRED L4 ₹63.6L; PhonePe SE2 ₹46.2L; Flipkart SDE2 ₹36.0L | cred.club/careers; phonepe.com/careers; careers.swiggy.com; flipkartcareers.com | std |
| 100ms | AI Engineer – AI Agents | Bengaluru | 2–5 | **W1** | ₹20–50L posted | https://jobs.lever.co/100ms | seen |
| Infer (YC) | Applied AI Engineer | Bengaluru | 3 | W1 | ₹20–50L posted | https://www.ycombinator.com/companies/infer/jobs | seen |

### Safety tier (accessible at 1–2 YOE)

| Company | Role | City | Stated minimum seen | Comp signal | Careers URL | Status |
|---|---|---|---|---|---|---|
| Nanonets | Forward Deployed Engineer | Bengaluru | 2+ (Mar/Aug 2026) | Not disclosed | https://jobs.accel.com/companies/nanonets/jobs/71054302-forward-deployed-engineer | seen |
| Cekura (YC) | Forward Deployed Engineer | Bengaluru | Not stated | ₹15–30L | https://www.workatastartup.com/jobs/84800 | seen |
| Gushwork | Forward Deployed Engineer | Bengaluru | 1–2 (Nov 2026) | Not disclosed | https://jobs.lever.co/gushwork | seen |
| Isomorph AI | Founding Engineer / FDE | Bengaluru | ~2 (24 Nov 2026) | Not disclosed | https://wellfound.com/jobs/5137295-founding-engineer-builder-experience-clone | seen |
| workwise / Tsenta / Sei AI | AI Engineer / Founding Engineer / LLM Engineer | Bengaluru, Chennai | 3–4 | ₹12–50L posted | Cutshort / YC / Wellfound pages (Section 5) | seen |
| Infosys | Gen AI, LLM Engineer | Bengaluru | 2–5 (~4 Nov 2026) | Services band | https://www.bayt.com/en/india/jobs/gen-ai-llm-engineer-75383098/ | seen |
| Wipro | Generative AI Engineer / Gen AI Engineer Lead (FDE) | Bengaluru, Pune, Chennai, Hyderabad | 3–5 / 5+ | Services band | https://careers.wipro.com | seen |
| NTT DATA / Accenture / GlobalLogic | Forward Deployed Engineer | Bengaluru | Not captured (Oct 2026) | Services band | https://careers-inc.nttdata.com | seen |
| Increff / Zeta | SDE-II (2–4) / SRE II (2) | Bengaluru | 2 | Not disclosed | https://jobs.lever.co/zeta | seen |
| E2E Networks | Accelerated Computing Engineer (MLOps pivot) | Chennai | 2–4 | Not disclosed | https://www.e2enetworks.com/careers/jobs/all | seen |

**Watchlist (well funded, roles unverified):** Emergent, Portkey, Composio, TrueFoundry (FDE – GTM seen), Simplismart, Ema, Bolna (expanding deployment teams), Nugget (Eternal spin-out), Reliance Intelligence (direct-pitch hiring), Lab0, and the YC India jobs board (https://www.ycombinator.com/jobs/location/india, seen). Japan-linked employers in India (for example Rakuten, Sony and Mercari, as named in the company research) were **not researched**. They are worth checking directly, because Japanese-client experience could be valued unusually highly there [E, gap].

## 15. 6/12/24-month learning roadmap: three portfolio projects, a 6–8-month interview build, two application waves

**Assumptions.** Today is 27 Nov 2026 and the candidate has ~1 YOE. ~2 YOE arrives around Nov 2027, and the window closes Nov 2028 at ~3 YOE. Full-time employment leaves about **10–12 hours a week** for preparation. That is the planning figure the interview research uses. Under it, NeetCode 150 takes ~2–3 months part-time ([Educative](https://www.educative.io/blog/neetcode-roadmap)). Mid-level engineers are typically ready 1–2 months into serious preparation, and serious preparation overall runs 3–4 months ([techinterview.org](https://www.techinterview.org/post/3233474686/interview-prep-timeline-by-level/)). Big Tech SDE-2 readiness (DSA + LLD + HLD) is estimated at **~6–8 months part-time** [E]. Applied-AI/FDE readiness for someone already doing the work is about **2–3 months** of turning experience into interview stories [E]. The first and most valuable input to the plan is the **day job**: every month, log shipped features with metrics (latency, eval scores, cost per request, adoption, customers onboarded). These become resume bullets and deep-dive stories.

### Phase plan

| Phase | Dates | Weekly split [E] | Technical priorities | Projects | DSA / design | Career actions | Exit criteria |
|---|---|---|---|---|---|---|---|
| **0–6 months: foundation and proof** | Dec 2026 – May 2027 | DSA 4h · project 5h · reading 1–2h · writing 1h | Eval engineering (metrics, judge calibration, CI gates); Postgres + pgvector, hybrid search; async FastAPI; Langfuse tracing; Docker + CI | **P1** shipped; P2 started | NeetCode patterns: arrays/hashing → two pointers/sliding window → stacks → binary search → linked lists → trees → heaps (~120 problems) | Skills self-audit; check notice terms and bonus/vesting dates in Tokyo; build a list of 40 target companies; publish post #1 (eval methodology) | P1 public with an eval report; ~120 problems; reliably solve easy/medium |
| **6–12 months: depth, design and launch** | Jun – Nov 2027 | DSA 3h · design 3h · project 4h · career 1–2h | MCP server authoring with OAuth; LangGraph agent patterns; TypeScript (MCP, UI); Redis, queues, SSE; Kubernetes basics; LLM cost engineering | **P2** shipped; **P3** shipped | Graphs, DP, intervals, tries (~250 total incl. company-tagged); **LLD**: 10–15 timed 90-min problems over 4–6 weeks; **HLD**: 6–8 weeks of fundamentals + 8 classic prompts + 6 LLM system-design prompts | Resume + LinkedIn final (Aug–Sep); post #2; referral outreach to 20–30 contacts (Sep); **Wave 1 applications from Oct 2027**; 6+ mock interviews | LC medium in ~30 min on ≥70% of attempts; 3 projects; first recruiter screens booked |
| **12–24 months: convert, then compound** | Dec 2027 – Nov 2028 | Interviews first; 4–6h maintenance otherwise | One specialisation chosen by target employer: voice agents, inference/LLMOps, or BFSI-domain agents | Optional **P4** (specialisation) | Company-specific drills before each loop; mock bar-raiser/values rounds | Wave 1 loops Dec 2027–Mar 2028; negotiate level; resign on notice; if no qualifying offer, Wave 2 May–Sep 2028 | Signed offer at L4/SDE-II-equivalent or ₹30L+ TC; start date within the window |

### Portfolio projects and the topics each covers

| # | Project | Topics covered | JD / interview evidence it answers | Deliverables | Build time [E] |
|---|---|---|---|---|---|
| **P1** | **Bilingual (Japanese/English) enterprise-document RAG with a published eval set** | Structure-aware chunking; embeddings; Postgres + pgvector hybrid (BM25 + vector) search; reranking; citations; a 50–100-question golden set; recall@5, MRR, faithfulness; LLM-as-judge calibrated against human labels; CI regression gate; Langfuse traces; FastAPI; Docker; cloud deploy | Sarvam must-haves ("chunking, embeddings, hybrid search, reranking, vector databases"); workwise "RAG … with source references"; the take-home "Q&A over 50 docs, 20-question eval set, recall@5 and faithfulness" ([techinterview.org](https://www.techinterview.org/post/3233476824/ai-engineer-interview-rag-agents-evals/)) | Repo, README with an architecture diagram and eval table, chunking/reranker ablation, live demo, blog post | 8–10 weeks |
| **P2** | **Governed MCP tool server + LangGraph agent for a realistic business workflow** (e.g. ticketing/CRM sandbox) | MCP server in TypeScript with OAuth and scoped tools; tool calling; structured outputs; step and spend caps; human approval for unsafe actions; trajectory/agent evals; tracing; latency budget; a minimal Next.js UI | Cisco: "MCP servers and tool integrations that give AI agents secure, governed access"; Google/YouTube FDE: "MCP servers … evaluation pipelines and observability"; Swiggy and Groww MCPs; agent design prompts on tool-call caps and an 800 ms latency target | Repo, threat model, eval report, demo video | 8–10 weeks |
| **P3** | **LLM gateway / agent platform service** | Multi-provider routing and fallbacks; Redis caching and rate limiting; per-tenant cost attribution; idempotent retries; SSE streaming with backpressure; OpenTelemetry traces; Kubernetes deploy; load test; an RFC-style design doc | Razorpay AI Inference Platform ("shared routing, observability, caching, per-team spend attribution"); Sarvam SDE2 API Platform (SSE, Postgres/Redis, Kubernetes); Portkey/LiteLLM patterns | Repo, design doc, load-test results, cost dashboard | 6–8 weeks |
| P4 (optional) | **Specialisation**: (a) voice agent with latency and quality evals; (b) LoRA fine-tune vs prompting on tool-use accuracy; or (c) vLLM serving benchmark | ASR/TTS or LoRA/SFT or batching/KV cache/quantisation | Salary-listed JDs with a ₹48L+ upper bound cluster on voice and fine-tuning; NVIDIA/inference JDs | One write-up with numbers | 4–6 weeks |

Each repo's README must contain five things: the problem, the architecture, a results table with eval metrics, the cost/latency profile, and a "what broke and what I changed" section. That last section answers the "shipped … long enough for it to break" test that Vahan states outright. No source quantifies how much GitHub, blogs or Kaggle move Indian recruiter screens [gap]. The case for public, eval-instrumented projects rests on how take-homes and project deep-dives are structured, not on screening data.

### Resume and LinkedIn positioning

The narrative is one sentence repeated everywhere: **"I ship production LLM agents with evals, and deploy them with enterprise customers."**

| Element | Recommendation [E] |
|---|---|
| Headline | "AI Engineer (Forward Deployed) · Production LLM agents, RAG & evals · Python/TypeScript · Relocating to Bengaluru, available in 30 days" (adjust to the actual notice period) |
| Format | One page at ~2 YOE; summary of 2 lines; 4–6 impact bullets per role in the format *action → system → metric*; 3 projects; one skills line (Section 13) |
| Metrics to surface | Eval-score deltas, latency, cost per request, adoption or users, number of enterprise deployments, time to production, incidents resolved |
| Japan experience | Present it as **enterprise deployment under demanding customer standards**: Japanese enterprise clients, quality bar, security/governance reviews, bilingual delivery if applicable. Present it as ownership of the customer relationship, not as an "onsite/offshore" arrangement. Anthropic's Bengaluru office is its second in Asia after Tokyo ([CNBC, 8 Oct 2025](https://www.cnbc.com/2025/10/08/anthropic-to-open-first-india-office-in-2026.html)), and global employers serving APAC accounts are the natural audience. No source measures how Indian employers value Japan experience, so test the framing in early recruiter calls |
| Anti-stuffing rules | No framework lists (CrewAI/AutoGen/DSPy/LlamaIndex); one cloud; one vector store; no certificate section; every skill on the line must appear in a bullet or project |
| LinkedIn | Turn on "Open to work" (recruiters only) from Aug 2027; set locations to Bengaluru, Hyderabad and NCR; pin P1–P3; post the eval and FDE write-ups |

### Application strategy

| Lever | Evidence | Tactic [E] |
|---|---|---|
| **Timing waves** | Minimums: 13–18% of JDs accept ≤2 yrs, 40–66% accept ≤3 yrs (Section 6.5) | W1 (Oct 2027–Feb 2028): Google SWE II/III and FDE V, Rubrik, Groww, 100ms, Sarvam, Cursor, Whatfix, startups, safety tier. W2 (May–Sep 2028): Microsoft, Amazon, Cisco, Databricks, MongoDB, HackerRank, Rippling |
| **Notice periods** | Indian notice runs ~15 days (startups) to 90 days (large firms); ~1 in 3 IT roles has 90 days; recruiters increasingly filter on notice length ([Instahyre](https://resources.instahyre.com/blog/notice-period-in-india/); [AIM](https://analyticsindiamag.com/ai-features/report-notice-periods-in-india-it); [The People's Board, Jul 2026](https://www.thepeoplesboard.com/hr-voices/the-90-day-notice-period-debate-is-it-hurting-indian-tech-hiring/)) | A Japanese contract often allows ~1 month (unverified; check yours). That beats most Indian rivals on 60–90 days, so state "available in ~30 days" up front |
| **Referrals** | No India conversion data [gap]; several unicorn boards were nearly empty on 27 Nov 2026 | Treat referrals as the main channel for CRED/PhonePe/Swiggy/Flipkart/Razorpay; build 20–30 warm contacts by Sep 2027 (ex-colleagues, alumni, Tokyo–India AI community, authors of the JDs' engineering blogs) |
| **Channels** | Postings came from company ATS boards (Greenhouse, Ashby, Lever, Workday), VC/accelerator boards (Accel, Khosla, General Catalyst, YC), Indeed, Wellfound and Cutshort | Daily alerts on ATS/VC boards for "Forward Deployed", "Applied AI", "Agent Engineer" in target cities; use Reliance Intelligence's direct-pitch channel |
| **Levelling** | L3→L4 roughly doubles TC; one Amazon "SDE-2 loop, offered SDE-1" report exists ([LeetCode](https://leetcode.com/discuss/post/6657524/offer-amazon-india-sde-2-loop-offered-sd-yn0n/)) | Ask for the level before the loop; prepare SDE-2-grade design answers; walk away from L3 at Big Tech if a startup offers ₹40L+ with real scope |
| **Offer anchoring** | Offers anchor to current CTC; Japan-to-India anchoring is unresearched | Anchor on Levels.fyi level bands and competing offers, not on the converted JPY salary |
| **Equity timing** | PhonePe targets listing Feb–Mar 2027; Zepto Feb–May 2027 ([Inc42](https://inc42.com/buzz/with-upi-mdr-clarity-phonepe-eyes-ipo-by-march-2027/); [YourStory, Jul 2026](https://yourstory.com/2026/07/zepto-rs-1000-cr-pre-ipo-round-prepublic-listing-delayed)) | A 2028 join likely gets RSUs priced at public valuations; value them as cash-like, not as lottery tickets |
| **Buyouts** | Example: ~₹3.75L to buy out 90 days on a ₹15 LPA salary; needs the current employer's consent | Mostly relevant for Indian rivals; check Tokyo bonus and vesting dates before resigning |

## 16. Interview preparation strategy: clear one coding bar, win on eval stories and customer rounds

India loops fall into four archetypes, and preparation should match the target lane rather than covering everything equally.

| Archetype | Typical rounds (reported) | DSA level | Design | AI-specific rounds | Behavioural | AI-tool policy | Sources |
|---|---|---|---|---|---|---|---|
| **Big Tech SDE-2** (Google L4, Amazon SDE II) | Google: recruiter → DSA screen → 2–3 DSA → Googleyness. Amazon: OA (2 DSA + work-style) → DSA+LP → LLD+LP → HLD+LP → Bar Raiser | Medium–hard; graphs, trees, DFS with optimisation follow-ups | Amazon has separate LLD and HLD rounds | Rare; a separate Google MLE track exists | Amazon LPs in every round; Googleyness | Google: AI use "will not work" in online rounds | [LeetCode Amazon](https://leetcode.com/discuss/post/7132680/amazon-sde-2-bangalore-onsite-interview-pr26m/); [LeetCode Google](https://leetcode.com/discuss/post/7240829/) |
| **Indian product / SaaS SDE-2** (Flipkart, Swiggy, Razorpay, Atlassian P40, Groww) | DSA → **90-min machine coding (knockout)** → HLD → HM/values | Medium (occasionally hard) | LLD: Splitwise, parking lot, food ordering, booking, rating system, Snake; HLD: notifications, scheduler with retries, subscriptions, quick commerce | Rare | Atlassian values round is "the most difficult round" for some | Mostly prohibited | [LeetCode Flipkart](https://leetcode.com/discuss/post/6933851/flipkart-sde-2-interview-experience-2025-gcq9/); [Glassdoor Razorpay](https://www.glassdoor.com/Interview/Razorpay-Interview-E1146550-RVW86702348.htm); [LeetCode Atlassian](https://leetcode.com/discuss/post/7070747/) |
| **Applied AI / LLM engineer** (product, AI startups) | 4–5 rounds; only one looks like classic algorithms; debugging an integration or a looping agent; RAG/agent system design; eval design; project deep dive; 2–4 h take-home | Medium, one round | LLM system design: support assistant "and how you'd know it helps"; eval + serving around a model you don't control; agent tracing and cost caps; chunking and choice of k; inference batching on one GPU | **Evals are often the "weed-out" round** | STAR on ambiguity and execution | Live rounds mostly prohibit AI; take-homes may allow it with disclosure; Meta has an AI-enabled coding round (since Oct 2025) | [techinterview.org, Jul 2026](https://www.techinterview.org/post/3233476824/ai-engineer-interview-rag-agents-evals/); [Maven / Hamel Husain](https://maven.com/p/07e7c7/cracking-the-ai-evals-interview); [Hello Interview](https://www.hellointerview.com/blog/meta-ai-enabled-coding) |
| **FDE / Applied AI (customer-facing)** | Palantir-style: recruiter ("why us") → live coding → decomposition, learning (extend an unfamiliar codebase), re-engineering (find planted bugs), coding → HM. Labs: take-home, CodeSignal, system design, **customer-conversation simulation** | Practical DS&A (maps, strings), rarely graphs | Decomposition of vague prompts into data/schema/API plans | Customer simulation "quietly rejects a large share" of those who passed coding | 15–20 min embedded in most rounds | Palantir prohibits AI throughout | [aced.io Palantir FDE](https://www.aced.io/guides/palantir-forward-deployed-engineer-interview); [Exponent OpenAI FDE](https://www.tryexponent.com/guides/openai-forward-deployed-engineer-interview); [Educative Anthropic](https://www.educative.io/courses/forward-deployed-engineer/interview-guide-anthropic-applied-ai-engineers) |

Sarvam reportedly runs a hands-on build (a ~2.5-hour voice activity detector) and a fundamentals round, with **no LeetCode round**. That evidence comes from a single source ([techinterview.org, Nov 2026](https://www.techinterview.org/post/3233477952/sarvam-ai-interview-guide/)).

### Preparation plan by round type

| Round type | Standard to reach | Method and materials | When |
|---|---|---|---|
| **DSA** | LeetCode medium in ~30 min; 15–20 core patterns (hashing, two pointers/sliding window, BFS/DFS, heaps, binary search, intervals, basic DP); hard-level only for Google/Databricks | NeetCode 150 (2–3 months part-time), then ~250–300 total incl. company-tagged; solve in Python; review weekly | Months 0–12, then maintenance |
| **LLD / machine coding** | Runnable, extensible, SOLID code in 90 min with every requirement covered | 10–15 timed problems from the known set; record "requirement gaps", the cited rejection reason | Months 7–10 |
| **HLD** | Moderate depth at SDE-2: classic product designs plus fintech/infra prompts | *Designing Data-Intensive Applications* and Alex Xu Vols 1–2 (widely used; not verified as a ranking); practise notification service, scheduler, rate limiter, payments subscriptions | Months 7–11 |
| **LLM system design** | Defend chunking, retrieval, k, reranking, eval plan, cost/latency, failure modes, guardrails, prompt injection, multi-tenant isolation | Use P1–P3 as worked answers; Chip Huyen's *AI Engineering* (community-cited); six practice prompts from the table above | Months 6–12 |
| **Eval take-home / eval round** | Explain recall@k, precision@k, MRR/nDCG, faithfulness vs relevance; judge biases (length, position, self-preference); calibrating judges to human labels | P1 is the rehearsal; Hamel Husain's free evals lesson; time-box practice runs at 2–4 hours | Months 3–12 |
| **Project deep dive** | 30–45 min on one system: goals, design, alternatives rejected, eval evidence, what broke, impact | Write two deep-dive docs: one day-job system (sanitised), one portfolio project | Months 9–11 |
| **FDE decomposition / learning / customer simulation** | Turn a vague business problem into a scoped, buildable plan; navigate an unfamiliar codebase by asking questions | Practise with prompts like "sync two employee record systems"; role-play discovery calls drawn from Tokyo client experience | Months 9–12 |
| **Behavioural** | 8–10 STAR stories covering ambiguity, conflict, failure, customer escalation, ownership, influence; mapped to Amazon LPs, Atlassian values and Googleyness | Story bank with metrics; a specific "why this company" for each target (Palantir and Atlassian reject generic answers) | Months 10–12 |
| **AI-assisted coding** | Use the assistant to verify, not to think; review AI output critically | Practise the Meta-style format: bug fix → 120+ line implementation → optimisation | Before any Meta loop |

## 17. Final action plan: what to do this month, this quarter, and at each gate

| When | Action | Output / KPI |
|---|---|---|
| **Next 30 days (Dec 2026)** | Self-audit against the Section 13 inventory; read the Tokyo employment contract for notice period, bonus and vesting dates; choose the one cloud; start NeetCode (arrays, hashing, two pointers); open the P1 repo; start a monthly "work wins" log with metrics; build a target sheet of the Section 14 companies with alerts | Audit done; contract facts known; 20 problems; P1 skeleton; 40-company sheet |
| **Days 31–90 (Jan–Feb 2027)** | Build P1's golden set and retrieval pipeline; run the first eval and ablation; publish post #1 on eval methodology | P1 v1 with an eval table; ~60 problems; one public post |
| **Months 4–6 (Mar–May 2027)** | Finish P1 (CI regression gate, tracing, deployment); start P2 (MCP server + OAuth); read DDIA chapters 1–9 | P1 complete; ~120 problems |
| **Months 7–9 (Jun–Aug 2027)** | Ship P2; LLD drills; HLD study; first mock interviews; **gate 1:** LC medium in ~30 min on ≥70% of attempts? If not, narrow Lane C to Google-only | P2 complete; 6 LLD problems; gate decision |
| **Months 10–12 (Sep–Nov 2027)** | Ship P3; finalise resume and LinkedIn; contact 20–30 referrers; **launch Wave 1 (from Oct 2027)** to W1 employers; 6+ mocks incl. one FDE-style decomposition | P3 complete; ~250 problems; 15–25 applications; first screens |
| **Months 13–16 (Dec 2027–Mar 2028)** | Run Wave 1 loops; negotiate level first; **gate 2:** offer at L4/SDE-II-equivalent or ≥₹30L TC with real AI scope? If yes, resign on notice. If no, keep the Tokyo role | Offer decision |
| **Months 17–21 (Apr–Aug 2028)** | If still searching: pick the specialisation that fits the employers that rejected or shortlisted you (voice, inference/LLMOps or BFSI agents) and ship P4; **launch Wave 2 (May–Sep 2028)** to 3+-year-minimum employers | P4; 20–30 Wave 2 applications |
| **Months 22–24 (Sep–Nov 2028)** | Close and join; plan the first 90 days in India around owning one production AI system with measurable outcomes | Start date within the window |

The biggest lesson from this research is that the candidate's constraint is **proof and timing, not missing skills**. The market wants exactly what a Tokyo AI Engineer/FDE does: agents, RAG and evals shipped to enterprise users. But most Indian JDs set minimums the candidate will not meet until 2028, and the best-paying loops still filter on DSA and design. Two cheap moves therefore give the most leverage: apply in two waves timed to those experience minimums, and treat getting levelled at L4 as the main compensation decision. Expensive breadth, such as more frameworks, more clouds or certificates, does little. The second lesson is that an **eval-instrumented track record is the scarcest asset in the market**. India has 2M+ people "upskilled in AI" but roughly one qualified engineer per ten GenAI openings. The engineer who can show "here is my golden set, here is how I calibrated the judge, here is the regression that the gate caught" stands out in every lane. Three things should be re-checked before Wave 1, because the evidence was weakest on them: FDE pay at Big Tech, how recruiters read Japan experience, and current minimums at the dream-tier employers. Each can be resolved cheaply in the first few recruiter conversations.
