[Index](../INDEX.md) | [Next](../02%20Indian%20Tech%20Job%20Market%20Overview/02%20Indian%20Tech%20Job%20Market%20Overview.md)

# 1. Executive summary: AI engineering is the volume play, FDE the premium lane, level the pay lever

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

## Evidence labels used throughout

Every material claim carries a source and date. Where the distinction matters, claims are labelled as **[V] verified/reported fact** (a dated source states it), **[E] estimate** (a calculation or analyst judgement from cited data), or **[F] forecast** (a projection by a named source, or explicit scenario speculation). Compensation figures are additionally marked as *reported* (Levels.fyi, AmbitionBox, Glassdoor, posted bands) or *estimated*. Levels.fyi medians are self-reported and skew toward higher earners at product companies. Indeed's India software engineer average base salary is only **₹8.86 LPA (n=16.8k)** ([Indeed India](https://in.indeed.com/career/software-engineer/salaries)), against a Levels.fyi India median total comp of **₹30.8L (n=20,834)** ([Levels.fyi, Nov 2026](https://www.levels.fyi/t/software-engineer/locations/india)).

## Data conflicts and gaps register

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

---
[Index](../INDEX.md) | [Next](../02%20Indian%20Tech%20Job%20Market%20Overview/02%20Indian%20Tech%20Job%20Market%20Overview.md)
