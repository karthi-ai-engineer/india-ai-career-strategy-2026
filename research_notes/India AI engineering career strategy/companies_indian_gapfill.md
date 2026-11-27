# Indian Product Companies and AI/Deep-Tech Startups: Gap-Fill Target List (for a ~2-YOE AI Engineer / FDE, joining 2027–28)

Research date: 27 Nov 2026. Method: about 27 WebSearch/WebFetch calls. Most facts come from search-result summaries of news and company pages. Pages were not fetched one by one unless noted, so treat the figures as "verified at headline level". **[V]** means a cited source states it. **[I]** means my inference. Careers URLs marked **[I]** are the standard company careers paths and were not fetched in this session.

---

## Q1. Indian product companies and unicorns: what are their GenAI engineering teams and initiatives, and are they hiring?

### Takeaway
Six companies have the clearest, citable GenAI or agentic engineering work going into 2027: Flipkart (agentic e-commerce platform, SLAP/Flippi, 250+ models), Swiggy (MCP servers for ChatGPT/Claude/Gemini, Hermes text-to-SQL), Eternal (OpenAI partnership, Nugget spun out as enterprise AI), Razorpay (Agent Studio on the Claude Agent SDK, agentic payments with NPCI/OpenAI), Freshworks (Freddy agentic layer, Agent Studio, MCP Gateway) and Jio/Reliance Intelligence (JioBrain, direct AI hiring). Groww has the most concrete 2–5 YOE "AI Engineer" postings found. Two caveats: Freshworks cut about 11% of staff in Q1 2026, and the PhonePe and Zepto IPOs slipped to early 2027.

### Cited Findings

#### Deep-dive rows (priority companies)

**Flipkart** (e-commerce, Walmart-owned; Bengaluru; pre-IPO)
- Stage: Angel One (Apr 2026) describes Flipkart "shifting from strategy to execution ahead of IPO", moving to an AI-first architecture with LLMs and agentic frameworks [V] — [Angel One](https://www.angelone.in/news/unlisted-companies/flipkart-accelerates-ai-transformation-as-it-shifts-from-strategy-to-execution-ahead-of-ipo)
- GenAI: CPTO Balaji Thiagarajan (Jul 2026 report) says Flipkart is building an "agentic e-commerce platform" on frontier plus proprietary models, a "mixture of experts... many... models we build ourselves". Headline: AI now writes 40% of its code [V, secondary] — [NewsBytes](https://www.newsbytesapp.com/news/science/flipkart-says-ai-now-writes-40-of-its-code/story); 250+ models and custom LLMs — [Apparel Resources](https://apparelresources.com/business-news/retail/flipkart-accelerates-ai-strategy-250-models-custom-llms/)
- Flippi, the 2023 GenAI shopping assistant, is being revamped as "SLAP", a standalone conversational shopping assistant (Jan 2026 reporting) [V] — [NewsBytes](https://www.newsbytesapp.com/news/science/flipkart-s-ai-shopping-assistant-slap-to-launch-next-week/story); [Apparel Resources](https://apparelresources.com/technology-news/retail-tech/flipkart-roll-standalone-conversational-ai-shopping-assistant/)
- Super.money (Flipkart fintech) is launching AI agents that shop for users. Exec says 30–40% of revenue could come from agentic use cases by 2030 (Sep 2026) [V] — [NewsBytes](https://www.newsbytesapp.com/news/science/flipkart-s-super-money-lets-ai-agents-shop-for-you/story)
- Acquired a majority stake in Minivet AI (GenAI catalogue-to-video) [V] — [Inc42](https://inc42.com/buzz/flipkart-to-acquire-majority-stake-in-ai-startup-minivet/)
- AI-led product discovery beyond keyword search — [Inc42](https://inc42.com/buzz/how-flipkart-is-using-ai-to-move-beyond-keyword-led-product-discovery/); GenAI Q&A with Mayur Datar — [Flipkart Stories](https://stories.flipkart.com/gen-ai-indian-ecommerce-mayur-datar)
- Careers: https://www.flipkartcareers.com [I]

**Swiggy** (food, quick commerce; Bengaluru; listed on NSE/BSE since Nov 2024 [I, background])
- Agentic commerce: four MCP servers with 66 tools across Food, Instamart and Dineout, so users can order inside ChatGPT, Claude and Gemini. Includes model-switching and agent access controls. Launched late Jan 2026 [V] — [Inc42](https://inc42.com/buzz/how-swiggy-is-using-ai-agents-to-take-commerce-beyond-its-app/); [YourStory, Jan 2026](https://yourstory.com/2026/01/swiggy-lets-users-order-through-chatgpt-claude-gemini); [Swiggy corporate](https://www.swiggy.com/corporate/?p=16731)
- Internal GenAI: Hermes, a Slack-native text-to-SQL "conversational AI data analyst", now at V3 with multi-turn memory; the original was built on GPT-3.5 variants [V] — [InfoQ, Jan 2026](https://infoq.com/news/2026/01/swiggy-hermes-conversational-ai); [ZenML LLMOps DB](https://zenml.io/llmops-database/evolution-of-hermes-v3-building-a-conversational-ai-data-analyst)
- Tech stack evidence: Slack + LLM + SQL warehouse (Hermes); MCP servers [V, per above]
- Careers: https://careers.swiggy.com [I]

**Eternal (Zomato, Blinkit, District, Hyperpure)** (Gurugram; listed)
- Strategic collaboration with OpenAI across Zomato, Blinkit, District, Hyperpure and Nugget (Feb 2026), later reported as expanded to partner apps and internal systems [V] — [AIM](https://analyticsindiamag.com/ai-news/eternal-collaborates-with-openai-to-deploy-ai-on-zomato-blinkit-platforms); [Outlook Business](https://www.outlookbusiness.com/news/eternal-openai-partner-to-build-indias-first-ai-native-commerce-ecosystem)
- Nugget is an AI-native no-code support platform handling more than 15M interactions/month, launched Feb 2025 out of Zomato Labs. It has since been spun out into a separate entity as an enterprise AI business; FY26 turnover ₹7.6 Cr [V] — [Inc42](https://inc42.com/features/eternals-enterprise-ai-turn-why-the-zomato-parent-spun-out-nugget/); [YourStory, Feb 2025](https://yourstory.com/2025/02/autonomous-customer-support-zomato-launches-ai-powered-nugget)
- Q1 FY27 consolidated profit ₹92 Cr [V] — [Inc42](https://inc42.com/buzz/eternal-q1-profit-rises-3x-yoy-to-%E2%82%B992-cr-but-declines-47-sequentially/)
- [I] Nugget, as a spun-out enterprise AI company, is a natural FDE-style target: customer-facing agent deployments.
- Careers: https://www.zomato.com/careers ; Blinkit: https://blinkit.com/careers [I]

**PhonePe** (payments/fintech, Walmart-backed; Bengaluru; pre-IPO)
- Got SEBI approval after a confidential filing (Jan–Feb 2026) and targeted a $9–10.5B valuation (Mar 2026). Paused in Mar 2026 on market volatility; Inc42 says it now eyes a listing by Feb–Mar 2027 [V] — [Business Standard](https://www.business-standard.com/markets/ipo/phonepe-gets-sebi-approval-for-ipo-listing-drhp-size-126012000783_1.html); [NST/Reuters](https://www.nst.com.my/amp/business/corporate/2026/03/1389733/walmart-backed-phonepe-targets-us105bil-valuation-india-ipo); [Inc42](https://inc42.com/buzz/with-upi-mdr-clarity-phonepe-eyes-ipo-by-march-2027/)
- AI: lists an OpenAI partnership among its key partnerships (2025) [V] — [Inc42](https://inc42.com/?p=540483). Sameer Nigam at TechSparks Oct 2026: "build like Google or Amazon" — [YourStory](https://yourstory.com/2026/10/govern-yourself-like-hdfc-or-sbi-build-like-google-or-amazon)
- Gap: I found no PhonePe engineering-blog GenAI evidence in this session.
- Careers: https://www.phonepe.com/careers/ [I]

**Razorpay** (payments; Bengaluru; private, IPO-track)
- Agent Studio launched 12 Mar 2026 at FTX'26. It is a B2B agent marketplace and builder for payments and business banking, built on Anthropic's Claude Agent SDK. Pre-built agents handle disputes, failed-payment recovery and cash-flow forecasting. Integrations include Shopify, Shiprocket, WhatsApp, ElevenLabs, Slack, Tally and QuickBooks [V] — [Razorpay newsroom](https://razorpay.com/newsroom/razorpay-launches-the-worlds-first-ai-native-agent-studio-for-payments-at-ftx26-powered-by-anthropics-claude/); [Business Standard](https://www.business-standard.com/finance/news/razorpay-launches-ai-agent-studio-anthropic-claude-payments-126031200388_1.html)
- Agentic Experience Platform and Agentic Dashboard (natural-language merchant ops) [V] — [The Paypers](https://thepaypers.com/payments/news/razorpay-launches-ai-agent-studio-and-agentic-experience-platform); engineering/product blog: [Agent Studio guardrails](https://razorpay.com/blog/razorpay-agent-studio-principles-guardrails-and-merchant-control/), [Agentic platform](https://razorpay.com/blog/razorpay-agentic-platform/)
- Agentic payments pilot with NPCI and OpenAI at GFF 2025 [V] — [AIM](https://analyticsindiamag.com/ai-news/razorpay-launches-ai-native-agent-studio-to-automate-payments)
- Tech stack: Claude Agent SDK, MCP-style integrations [V]
- Careers: https://razorpay.com/jobs/ [I]

**Freshworks** (CX/ITSM SaaS; Chennai roots, engineering in Hyderabad, Bengaluru and Chennai; NASDAQ: FRSH)
- Freddy AI was rebuilt as a cross-suite agentic layer. AI Agent Studio is in Freshservice, and the May 2026 launch covers IT, HR and CX agents [V] — [Freshworks press release](https://www.freshworks.com/pressrelease/freshworks-unveils-ai-agent-studio-in-freshservice-to-unlock-service-transformation-that-drives-compounding-business-growth/); [Product launch May 2026](https://www.freshworks.com/product-launches/?tactic_id=6778534); [ComputerWeekly, Refresh 2026](https://www.computerweekly.com/feature/Freshworks-Refresh-2026-pivot-to-AI-driven-employee-experience)
- Per the company, its engineering team and AI Center of Excellence are in Hyderabad and Bengaluru; the CEO cited about 3,800 India employees (Jan 2025) [V, possibly dated] — [YourStory](https://yourstory.com/2025/01/india-engineering-talent-software-freshworks-ceo-dennis-woodside)
- **Negative signal:** Q1 2026 net loss of $4.8M and a plan to lay off 11% of staff (~500) [V headline] — [Inc42](https://inc42.com/buzz/freshworks-posts-4-8-mn-loss-in-q1-2026-to-lay-off-11-workforce/)
- Role evidence: "Lead – Solution Engineer" (Bengaluru, Aug 2026) to build agentic workflows in Agent Studio and connect Freshservice via MCP Gateway [V] — [Accel jobs board](https://jobs.accel.com/companies/freshworks/jobs/91173536-lead-solution-engineer). [I] This is FDE-adjacent, but "Lead" implies seniority above 2 YOE.
- Careers: https://www.freshworks.com/company/careers/ [I]

**Zoho** (SaaS; Chennai/Tenkasi; bootstrapped, private)
- Zia LLM is proprietary, trained in-house on NVIDIA infrastructure, in 1.3B, 2.6B and 7B sizes. Announced 17 Jul 2025 with prebuilt agents, a no-code Agent Studio, an MCP server and a marketplace. The roadmap adds a reasoning model and more speech-to-text languages [V] — [BusinessWire](https://www.businesswire.com/news/home/20250717118204/en/); [Futurum](https://futurumgroup.com/insights/zoho-unveils-zia-llm-no%E2%80%91code-agent-studio-and-open-agent-interoperability/); [YourStory](https://yourstory.com/ai-story/zoho-zia-llm-enterprise-ai-capabilities-sridhar-mani-vembu)
- Gap: no 2026 AI-hiring evidence found; I could not confirm whether the reasoning model shipped.
- Careers: https://www.zoho.com/careers/ [I]

**Jio Platforms / Reliance Intelligence** (telecom/AI; Navi Mumbai, Bengaluru, Hyderabad [I]; Jio IPO in preparation)
- Reliance Intelligence is the AI subsidiary led by Chief AI Scientist Gaurav Aggarwal. It is hiring AI/ML engineers for Indic LLMs, training pipelines, distributed systems, model optimisation and product incubation (ET via TelecomTalk; the year of the "Dec 16" report is unclear) [V] — [TelecomTalk](https://telecomtalk.info/reliance-operationalises-ai-arm-reliance-intelligence-hiring/1002658/)
- India AI Impact Summit (Feb 2026): Aggarwal invited "cracked engineers" to pitch directly for fast-track hiring [V] — [Digit](https://www.digit.in/news/general/india-ai-impact-summit-reliance-jio-fast-tracks-ai-hiring-chief-ai-scientist-invites-direct-pitches-at-the-mega-event.html); [OneIndia](https://www.oneindia.com/india/reliance-jio-s-chief-ai-scientist-invites-cracked-engineers-at-ai-impact-summit-2026-7999727.html)
- JioBrain is the in-house AI/ML platform for network ops and customer engagement. The pre-IPO prospectus reportedly shows 84% of service requests resolved via self-service or AI-assisted flows in the quarter to 30 Jun 2026 [V, Hindi secondary] — [Angel One](https://www.angelone.in/news/hindi/ipos/how-jiobrain-is-helping-jio-build-an-ai-native-digital-business-ahead-of-ipo)
- Partnerships with Google and Meta for India's AI backbone (Aug 2025) [V] — [TechCrunch](https://techcrunch.com/2025/08/29/billionaire-ambani-taps-google-meta-to-build-indias-ai-backbone)
- Careers: https://careers.jio.com [I]

**Groww** (brokerage/fintech; Bengaluru; listed Nov 2025 [V, per Inc42 IPO class coverage])
- Several AI engineering postings in 2026. AI Engineer II (Jan 2026) builds MCPs and tools so agents can work with financial data. AI Engineer III builds agentic systems and compliance guardrails for 50M+ users. Others: an AI/ML Architect role and an AI Engineer Intern (RAG/LLMs, Noida). Aggregators tag the AI Engineer roles at 2–5 YOE [V] — [Greenhouse](https://job-boards.eu.greenhouse.io/groww/jobs/4528373101); [foundit](https://www.foundit.in/job/ai-engineer-iii-groww-bengaluru-bangalore-54400869); [getmereferred (2–5 yrs)](https://getmereferred.com/job-listing/ai-engineer-2-groww-bengaluru-2-to-5-years-experience-5c9972a7-c747-4db5-9230-ef30d744835f)
- Comp: Glassdoor median SDE total pay ₹17L/yr, self-reported, undated snapshot [V] — [Glassdoor](https://www.glassdoor.co.in/Jobs/Groww-Jobs-E2549469.htm)
- Careers: https://groww.in/careers (Greenhouse board verified above)

#### Lower-priority rows (one verified line each)
| Company | Verified line (date, source) | Careers URL |
|---|---|---|
| Zepto | Got SEBI observation in May 2026, then paused its IPO in Jul 2026 for a ~₹1,000 Cr pre-IPO round. IPO now expected Feb–May 2027. Proceeds are partly earmarked for AI/ML and cloud. Valuation figures conflict ($4.5B vs $7B) — [YourStory Jul 2026](https://yourstory.com/2026/07/zepto-rs-1000-cr-pre-ipo-round-prepublic-listing-delayed); [Business Today Jun 2026](https://www.businesstoday.in/amp/latest/corporate/story/inside-zeptos-1bn-ipo-revenue-surge-mounting-losses-cac-pressures-ed-cloud-535709-2026-06-09) | zepto.com/careers [I] |
| BrowserStack | Launched BrowserStack AI with 5 testing agents (20+ planned) and an MCP server for Copilot, Cursor and Claude (30 Jun 2025) — [BrowserStack press](https://www.browserstack.com/press/browserstack-launches-suite-of-ai-agents-to-redefine-software-quality-at-scale) | browserstack.com/careers [I] |
| InMobi / Glance | Tracker lists 100 India layoffs on 20 Mar 2026 (unconfirmed by company). $100M debt from MARS Growth. Bankers reportedly lined up for a ~$1B IPO (Jul 2026). Glance has 50M+ DAU — [AIM / tracker summary](https://analyticsindiamag.com/ai-news-updates/inmobi-joins-the-list-of-companies-on-a-firing-spree); [Outlook Business](https://www.outlookbusiness.com/news/inmobi-secures-100-million-from-mars-growth-capital-for-ai-focused-acquisitions-and-strategic-growth) | inmobi.com/company/careers [I] |
| Darwinbox | Launched "Darwinbox Cortex", an AI-native HCM rebuild (4 Aug 2026), and moved to co-CEOs (20 Jul 2026). Single secondary roundup, verify — [upgrowth.in](https://upgrowth.in/growth-moves/saas/) | darwinbox.com/careers [I] |
| Whatfix | 3 AI agents (Authoring, Insights, Guidance) on ScreenSense (Sep 2025). Targets 25% of ARR from AI products — [YourStory](https://yourstory.com/ai-story/whatfix-aims-25-revenue-from-ai-products-launches-ai-agents-saas) | whatfix.com/careers [I] |
| MoEngage | Acquired Aampe for per-user AI decisioning (date not given; single secondary source) — [upgrowth.in](https://upgrowth.in/growth-moves/saas/) | moengage.com/careers [I] |
| Innovaccer | CEO announced fresh AI-driven layoffs (May 2026) [V headline] — [American Bazaar](https://americanbazaaronline.com/2026/05/17/indian-national-innovaccer-ceo-announces-fresh-ai-driven-layoffs-across-startup-480960/) | innovaccer.com/careers [I] |
| Urban Company / Ather / PhysicsWallah | All three listed in 2025 (UC at ~60% premium; PW at ₹145 vs ₹109 issue). No AI-company positioning found — [Business Standard Dec 2025](https://www.business-standard.com/amp/markets/news/urban-company-slides-6pc-physicswallah-dips-2pc-heres-why-stocks-fell-125121500184_1.html); [YourStory IPO class 2025](https://yourstory.com/2025/11/the-ipo-class-of-2025-how-new-age-startups-minted-billionaires-and-vc-windfalls) | urbancompany.com/careers; atherenergy.com/careers; pw.live/careers [I] |
| Chargebee, CleverTap, Juspay, ShareChat, Navi, Upstox | **Not researched in this session** (budget). No verified 2025–26 AI facts gathered | chargebee.com/careers; clevertap.com/careers; juspay.io/careers; sharechat.com/careers; navi.com/careers; upstox.com/careers [I] |

### Inferences
- [I] The strongest "real GenAI engineering team" signals are product launches with named architectures: Swiggy MCP (66 tools), Razorpay Agent Studio (Claude Agent SDK), Flipkart's agentic platform and 250+ models, Freshworks Agent Studio/MCP Gateway, and Zoho's own LLM. These are integration-heavy agent platforms, which is the FDE/AI-engineer skill profile: tool/MCP design, guardrails, evals.
- [I] IPO timing matters for a 2027–28 join. PhonePe (Feb–Mar 2027 target), Zepto (Feb–May 2027), Jio, InMobi and Flipkart are all pre-IPO. Joining after listing means ESOPs/RSUs priced at public valuations.
- [I] Layoff-plus-AI-pivot is a recurring 2026 pattern (Freshworks −11%, Innovaccer, InMobi, Yellow.ai). Headcount is moving toward smaller AI-skilled teams, which helps candidates with agent-engineering skills but makes net hiring volumes uncertain.

### Gaps
- No PhonePe, Zomato or Flipkart engineering-blog posts were fetched. Tech stacks are inferred from news, not blogs.
- Chargebee, CleverTap, Juspay, ShareChat, Navi and Upstox were not researched.
- Zoho 2026 AI hiring and Zia reasoning-model release status are unverified.
- Careers URLs are mostly unverified [I].

---

## Q2. AI and deep-tech startups (India-based or India-engineering-heavy): stage, AI focus, hiring

### Takeaway
Ema (Series B, $77M, Sep 2026; Bengaluru office) and Yellow.ai (Nasdaq SPAC at $550M, announced Aug 2026, plus the Feb 2026 Nexus launch, after ~30% layoffs) are the most notable priority names. Atlan has had no new round since its 2024 Series C ($105M at $750M), but has strong 2026 "context engineering for agents" product momentum. I found no Observe.AI news after 2022 funding. Bolna (YC, $6.3M seed led by General Catalyst, Jan 2026) is explicitly expanding engineering and deployment teams, a direct FDE fit.

### Cited Findings

**Ema** (agentic "AI employee" platform; HQ California, offices in Bengaluru, London, Vancouver)
- $77M Series B led by Creaegis (Bengaluru) with Accel, S32 and Prosus, announced 23 Sep 2026. Total about $138–140M; valuation more than 4x the 2024 round, figure undisclosed. Funds go to GTM and APAC/EMEA expansion [V] — [TechCrunch](https://techcrunch.com/2026/09/23/ema-raises-77m-as-ai-starts-eating-into-enterprise-software-and-services/); [YourStory](https://yourstory.com/2026/09/enterprise-ai-startup-ema-raises-series-b-round-led-by-creaegis); [Inc42](https://inc42.com/buzz/ema-raises-77-mn-to-scale-its-universal-ai-employee-platform-globally/)
- Conflict: DealStreetAsia calls Ema "Bengaluru-based"; others say California HQ — [DealStreetAsia](https://dealstreetasia.com/stories/ai-ema-creaegis-496087)
- [I] GTM-led spend suggests solution/forward-deployed roles. Not verified by a posting.
- Careers: ema.co/careers [I]

**Yellow.ai** (conversational/agentic CX; Bengaluru and San Mateo [I])
- To go public via a $550M merger with Bluerock Acquisition Corp (Nasdaq: "YAI"), announced 3 Aug 2026, expected to close H2 2026 [V] — [PR Newswire](https://www.prnewswire.com/in/news-releases/yellowai-a-global-leader-in-enterprise-agentic-ai-to-go-public-via-550-million-merger-with-bluerock-acquisition-corp-302841119.html); [HPCwire](https://www.hpcwire.com/aiwire/2026/08/03/yellow-ai-to-go-public-via-550m-merger-with-bluerock-acquisition-corp/)
- Nexus, the "Universal Agentic Interface", launched 4 Feb 2026 [V] — [PR Newswire](https://tools.prnewswire.com/en-us/live/20823/release/20260204EN77518)
- Laid off 100+ (~30% of workforce), dated around Dec 2025; smaller round in Aug 2025 [V] — [Inc42](https://inc42.com/buzz/exclusive-yellow-ai-lays-off-over-100-employees-amid-automation-push)
- Careers: yellow.ai/careers [I]. Gap: SPAC close status as of Nov 2026 not confirmed.

**Atlan** (data/AI governance, "context layer for agents"; Singapore HQ per CB Insights, large India team [I])
- Latest confirmed round: $105M Series C led by GIC and Meritech at a $750M valuation (May 2024); total over $200M. No 2026 round found [V] — [Atlan](https://atlan.com/atlan-raises-105m-funding/); [TechCrunch](https://techcrunch.com/2024/05/08/atlan-scores-105m-for-data-control-plane-just-as-llms-increase-importance-of-data)
- 2026 product: Context Engineering Studio and Context Lakehouse ("8B reads in 90 days"). Claims a 5x accuracy gain at Workday and Fox. 400+ enterprise customers (Aug 2026). AIBoomi 2026 Scale-up of the Year [V, company-sourced] — [AI Engineer org page](https://www.ai.engineer/orgs/atlan); [Atlan about](https://atlan.com/about/)
- Careers: atlan.com/careers [I]

**Observe.AI** (contact-centre AI; HQ Redwood City/SF Bay Area, Bengaluru engineering)
- Last confirmed round is a $125M Series C led by SoftBank VF2 (Apr 2022), total $213M. No 2026 funding or layoff news found [V] — [TechCrunch 2022](https://techcrunch.com/2022/04/12/observe-ai-raises-125m-adding-zoom-as-an-investor-to-supercharge-the-contact-center-market); [Sacra](https://sacra.com/c/observe-ai/)
- Careers: observe.ai/careers [I]. Gap: no 2026 signal at all.

**Lower-priority startups**
| Company | Verified line (date, source) | Careers URL |
|---|---|---|
| Gupshup | Raised $60M+ equity and debt (Globespan, EvolutionX) in Jul 2025; unicorn status in question. Multiple layoff rounds in 2024–25. AI is 25–30% of revenue — [TechCrunch Jul 2025](https://techcrunch.com/2025/07/22/gupshup-raises-60m-in-equity-and-debt-leaves-unicorn-status-hanging); [Inc42 AI rebuild](https://inc42.com/features/gupshup-ai-rebuild-can-it-stay-ahead-of-the-platforms-it-runs-on/) | gupshup.io/careers [I] |
| Haptik (Jio-backed) | No 2026 funding or layoff news verified. Reports of 2025 "silent layoffs" exist only on a vendor-review site (unverified) — [CB Insights](https://www.cbinsights.com/company/haptik) | haptik.ai/careers [I] |
| SpotDraft (legal CLM AI; Bengaluru/NY) | $8M Series B extension from Qualcomm Ventures for on-device AI (Jan 2026), after a $54M Series B (Feb 2025) — [YourStory Jan 2026](https://yourstory.com/2026/01/spotdraft-funding-qualcomm-ventures-extended-series-b-round-on-device-ai-legal-workflows) | spotdraft.com/careers [I] |
| E2E Networks (NSE-listed GPU cloud; Delhi/Chennai) | Raised ₹420.51 Cr preferential issue for GPUs. Building a Blackwell cluster on its TIR platform. Hiring "Accelerated Computing Engineer" (2–4 YOE, GPU ops/MLOps, Chennai) — [E2E careers](https://e2enetworks.com/careers/jobs/accelerated-computing-engineer); [AIM](https://analyticsindiamag.com/ai-news-updates/ai-hyperscaler-e2e-networks-secures-inr-420-51-crores-to-expand-cloud-infrastructure/) | https://www.e2enetworks.com/careers/jobs/all [V] |
| Yotta (Hiranandani; Navi Mumbai) | Raised $150M at a ₹37,000 Cr (~$3.9B) valuation. ~50% of business from GPUs — [Inc42](https://inc42.com/features/how-yotta-is-building-its-ai-infra-playbook-to-serve-global-enterprises/) | yotta.com/careers [I] |
| Rocket.new (vibe-coding app builder; Surat/Palo Alto) | $15M seed led by Salesforce Ventures and Accel (22 Sep 2025); 400K users, $4.5M ARR — [TechCrunch](https://techcrunch.com/2025/09/22/rocket-new-one-of-indias-first-vibe-coding-startups-snags-15m-from-accel-salesforce-ventures) | rocket.new/careers [I] |
| Bolna (voice AI orchestration; Bengaluru; YC) | $6.3M seed led by General Catalyst (20 Jan 2026); funds to expand **engineering and deployment teams** — [TechCrunch](https://techcrunch.com/2026/01/20/bolna-nabs-6-3-million-from-general-catalyst-for-its-india-focused-voice-orchestration-platform/); [Bolna press](https://www.bolna.ai/newsroom/bolna-bags-63-million-seed-funding-led-by-general-catalyst-to-build-indias-voice-ai-platform) | ycombinator.com/companies/bolna-ai/jobs [I] |
| Ultrahuman (wearables/health AI; Bengaluru) | ~₹400 Cr Series C (Mar 2026), then $70M from Qualcomm Ventures, Alpha Wave and others (Sep 2026; one source says $60M) for sensing, AI and health-algorithm R&D — [YourStory Sep 2026](https://yourstory.com/2026/09/funding-ultrahuman-70m-qualcomm-ventures-alpha-wave-others) | ultrahuman.com/careers [I] |
| CynLr (robotic vision; Bengaluru) | Latest found: $10M Series A (Nov 2024), total $15.2M. No 2026 round found — [CB Insights](https://www.cbinsights.com/company/cynlr/financials) | cynlr.com/careers [I] |
| Ati Motors (industrial AMRs; Bengaluru) | $20M Series B co-led by Walden Catalyst and NGP (~2025); total $37M+ — [Inc42](https://inc42.com/buzz/ati-motors-nets-20-mn-to-power-industrial-automation-with-ai) | atimotors.com/careers [I] |
| Levo.ai | **No results found** in two searches; unverified | — |

### Inferences
- [I] For FDE specifically, the best startup fits are voice-agent and CX-agent companies with enterprise deployments: Bolna (explicit deployment-team expansion), Yellow.ai (post-SPAC), Ema (GTM expansion) and Nugget (Eternal spin-out). Their customers need on-site integration engineers.
- [I] Compute-layer players (E2E, Yotta) hire GPU/MLOps infra engineers at 2–4 YOE. That is a different track from application-layer AI engineering.

### Gaps
- No 2026 signals for Observe.AI, CynLr, Ati Motors or Haptik.
- Levo.ai could not be identified.
- No comp data was gathered for any of these startups.

---

## Q3. India-based YC W25/S25/W26 (and later) AI startups

### Takeaway
YC's India-AI directory (fetched 27 Nov 2026) lists 8 Bengaluru companies from 2025–26 batches. Most have 3–10 people, so hiring is sparse. Bolna (21) and Adalat AI (80, nonprofit) are the larger ones. The page shows no hiring flags.

### Cited Findings
- From the YC India AI directory [V] — [YC](https://www.ycombinator.com/companies/industry/ai/india):
  - Adalat AI — F2026, Bengaluru, 80 people, legal/GovTech NLP (nonprofit; [AIM](https://analyticsindiamag.com/ai-news/indian-legal-tech-nonprofit-adalat-ai-joins-y-combinators-fall-2026-batch/))
  - RouterPlus — F2026, 3, marketplace that matches teams to AI inference models and providers
  - Waybill — S2026, 3, hardware procurement automation
  - Lab0 — P2026, 10, agentic systems to speed enterprise software implementations (**FDE-like**)
  - Ressl AI — W2026, 3, platform to train, benchmark and deploy autonomous agents in business systems
  - Efficient Computation Inc. — F2025, 4, pretraining research and RL environments for science
  - Redapto — F2025, 7, specialized AI agents running operations end to end
  - Bolna AI — F2025, 21, voice AI orchestration
- Third-party count: 137 YC companies in Bengaluru, 94 active (9 Nov 2026) [V, non-official] — [Crustdata](https://crustdata.com/tools/yc-companies/location/bengaluru)
- YC jobs board for India SWE roles: https://www.ycombinator.com/jobs/role/software-engineer/india [V URL]

### Inferences
- [I] The directory filter ("AI" + "India") misses India-founded YC companies registered with US HQs. The real number of India-engineering YC AI startups is larger.
- [I] Lab0 and Redapto ("agents that run implementations/operations") are effectively FDE-as-a-product companies. They are worth tracking for 2027 hiring once they raise.

### Gaps
- Hiring status per company is not shown on the directory. No W25 or S25 India entries appeared under this filter; they may sit under other tags or US HQs.

---

## Q4. Compensation (2–4 YOE) and hiring evidence

### Takeaway
I gathered only limited comp data in this session. Freshworks SWE India median total comp is about ₹33.7L/yr (levels.fyi, Feb 2026 snapshot; entry level about ₹13.1L). The Groww SDE median is ₹17L (Glassdoor, self-reported). Most other comp cells are gaps.

### Cited Findings
- Freshworks SWE (India) on levels.fyi: range ~₹13.1L (entry) to ~₹1.03Cr (senior staff); median ~₹33.7L. That is the Feb 2026 snapshot; earlier snapshots show ₹28.7L (Jun 2025) and ₹35.8L (Jan 2025) [V] — [levels.fyi](https://www.levels.fyi/companies/freshworks/salaries/software-engineer)
- Groww SDE median total pay ₹17L/yr, Glassdoor self-reported [V] — [Glassdoor](https://www.glassdoor.co.in/Jobs/Groww-Jobs-E2549469.htm)
- Postings in the 2–4 YOE band that were verified: Groww AI Engineer II/III (tagged 2–5 yrs on aggregators) — [getmereferred](https://getmereferred.com/job-listing/ai-engineer-3-groww-bengaluru-2-to-5-years-experience-bf819164-6b0f-4a5c-8bea-43fd6e43c59e); E2E Networks Accelerated Computing Engineer (2–4 yrs) — [E2E](https://e2enetworks.com/careers/jobs/accelerated-computing-engineer)

### Inferences
- [I] A median of about ₹34L across all Freshworks SWE levels suggests SDE-II (2–4 YOE) sits below the median, roughly ₹20–30L. This is an inference, not read from level rows.

### Gaps
- No levels.fyi or AmbitionBox 2–4 YOE figures were collected for Zoho, Jio/Reliance Intelligence, Atlan, Observe.AI, Ema, Yellow.ai, Zepto, Groww (levels.fyi), BrowserStack, InMobi or the startups. The tool-call budget ran out, so these need a dedicated comp pass.
- AmbitionBox was not queried at all.
