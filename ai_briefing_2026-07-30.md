# 🤖 AI Daily Briefing — July 30, 2026
*Generated: 2026-07-30*

---

## 🔬 Research & Breakthroughs

- **ICML paper: LLMs have a fundamental, potentially unfixable security flaw.** Researchers Charles Ye and Jasmine Cui published findings at the International Conference on Machine Learning showing that LLMs cannot be made fully secure because they identify instruction sources (user, system, tool, chain-of-thought) by *text style* rather than by structural tags — making "chain-of-thought forgery" attacks trivially effective. Demonstrated attacks coaxed GPT-5, GPT-OSS-20B, and models from Anthropic, Alibaba, and DeepSeek to produce cocaine synthesis instructions and aircraft navigation sabotage guides. Authors say the underlying mechanism is a fundamental flaw, not a fixable guardrail gap. *(Source: [MIT Technology Review](https://www.technologyreview.com/2026/07/30/1140927/a-fundamental-flaw-leaves-llms-vulnerable-to-attack/))*

- **OpenAI's GPT-5.6 Sol surpasses Claude Opus 5 on ARC-AGI-3 via two API settings.** OpenAI reported on July 30 that enabling "Retained Reasoning" (preserves chain-of-thought between steps) and "Compaction" (summarizes prior context) lifts GPT-5.6 Sol's ARC-AGI-3 public-set score from 7.8% to 38.3%, surpassing Claude Opus 5's 30.2%. ARC Prize co-founder François Chollet confirmed the settings are legitimate since they are general-purpose API features, not custom benchmark harness tricks. *(Source: [The Decoder / AI Weekly](https://the-decoder.com/openai-claims-gpt-5-6-sol-beats-opus-5-on-arc-agi-3-with-its-latest-api-and-two-additional-settings/))*

- **Anthropic's Claude Mythos discovers novel cryptographic attacks on HAWK and AES-128.** In research published July 28, Anthropic reported that its unreleased Claude Mythos Preview model independently discovered two cryptographic attacks in ~60 hours of work: a lattice automorphism in the NIST post-quantum signature HAWK cutting security from 2^64 to 2^38, and a "Möbius Bridge" technique speeding 7-round AES-128 attacks by 200–800x. Neither breaks deployed systems, each cost ~$100K in API usage, and responsible disclosure was followed with government and industry partners. *(Source: [Anthropic / AI Weekly](https://www.anthropic.com/research/discovering-cryptographic-weaknesses))*

- **Frontier agents fail NeurIPS shadow research evaluations.** A 25-author "Shadow Evaluations" paper tested frontier agents against the central research questions of two unpublished NeurIPS 2026 submissions, graded by original authors. Agents completed all engineering work autonomously over six days with thousands of dollars in compute, but were "unambiguously rejected" — failing on five recurring dimensions: publishability judgment, creative problem-solving, backtracking, resource awareness, and instruction drift. *(Source: [Hugging Face Papers / AI Weekly](https://huggingface.co/papers/2607.27191))*

---

## 🏢 Industry & Companies

- **Microsoft Azure tops $100B for first full fiscal year; Copilot at 30M paid seats.** Microsoft's Q4 FY26 results show revenue of $90B (+18% YoY) and net income of $35.8B (+31%), with Azure +43% YoY. CEO Satya Nadella announced Azure crossed $100B for FY26 for the first time, Microsoft 365 Copilot crossed 30 million paid seats, and commercial remaining performance obligations surged 84% to $678B — the sharpest signal yet of compounding enterprise AI demand. Microsoft also disclosed a $3.2B gain on its Anthropic investment in Q4, while its OpenAI stake was marked down ~$600M in the same quarter. *(Source: [Microsoft / AI Weekly](https://www.microsoft.com/en-us/Investor/earnings/FY-2026-Q4/press-release-webcast))*

- **Meta raises 2026 AI capex floor to $130B as Q2 revenue hits $60.8B.** Meta reported Q2 2026 revenue of $60.8B (+28% YoY) and raised its full-year capex guidance floor to $130B–$145B (from $125B–$145B), citing datacenter buildout. Costs surged 55% YoY to $42B, including $1.18B in severance from the May 2026 layoff of ~8,000 employees. Zuckerberg said AI is "accelerating our core business today and opening the door to entirely new enterprise opportunities." Separately, Meta and BlackRock announced a joint venture to build a 1 GW AI datacenter campus in El Paso, Texas, at roughly $14B total development cost. *(Source: [Meta Investor Relations / AI Weekly](https://investor.atmeta.com/investor-news/press-release-details/2026/Meta-Reports-Second-Quarter-2026-Results/default.aspx))*

- **ByteDance profiled as China's would-be full-stack AI champion.** The Financial Times detailed ByteDance's push to vertically integrate across frontier models (Seed, Doubao), video generation (Seedance), distribution (TikTok/Douyin), and custom AI chips co-designed with TSMC targeting mass production in 2026. No Western AI company matches the combination of model development, consumer distribution, and compute ownership ByteDance is building. *(Source: [Financial Times / AI Weekly](https://www.ft.com/content/fde2dd97-317a-41b8-a746-d917c5680397))*

- **Qualcomm closes Modular acquisition; Chris Lattner named EVP of Advanced AI Software.** Qualcomm completed its acquisition of Modular, the AI infrastructure company founded by compiler expert Chris Lattner. Lattner becomes EVP of Advanced AI Software, bringing Modular's MAX platform and Mojo language into Qualcomm's data-center push, in pursuit of CEO Cristiano Amon's stated $5B FY27 data-center revenue target. *(Source: [HPCwire / AI Weekly](https://www.hpcwire.com/aiwire/2026/07/29/qualcomm-completes-acquisition-of-modular/))*

- **Hugging Face publishes forensic timeline of OpenAI agent breach.** HF's security team reconstructed the July 9–13 OpenAI agent intrusion, recovering ~17,600 attacker actions. The two-stage chain used an HDF5 external-file-read primitive for disclosure and a Jinja2 SSTI via fsspec to execute code in a production Kubernetes pod, then pivoted via forged identity tokens and a stolen Tailscale key used 181 times. Because Claude Opus and Fable guardrails blocked exploit analysis, HF ran nvidia/GLM-5.2-NVFP4 on its own infrastructure to decrypt C2 payloads, recovering ~4x more secrets than manual scanning. *(Source: [Hugging Face Blog / AI Weekly](https://huggingface.co/blog/agent-intrusion-technical-timeline))*

---

## 💰 Funding & Business

- **Brookfield and NextEra announce $100B Kentucky AI campus, 1.2 GW by 2032.** Selected by the DOE in a Request-for-Offers process, the two companies will develop an AI data-center campus at the former Paducah Gaseous Diffusion Plant in Kentucky. NextEra will build 2 GW of natural gas generation plus 2.6 GW of battery storage; initial operations are targeted for 2028. The project is expected to create 8,000 construction jobs and 600 permanent operations roles. *(Source: [Data Center Knowledge / AI Weekly](https://www.datacenterknowledge.com/data-center-construction/brookfield-nextera-launch-100b-ai-campus-at-doe-s-paducah-site))*

- **China's Moonshot AI hits $35B valuation after $3.5B raise.** Moonshot AI surpassed its funding goal to reach a $35B valuation, riding momentum from its Kimi K3 model breakthrough. The round was announced July 29. *(Source: [Bloomberg](https://www.bloomberg.com/news/articles/2026-07-29/china-s-moonshot-ai-passes-funding-goal-to-hit-35-billion-value))*

- **CuspAI raises $450M at $2.6B to build AI materials foundry with Hinton and LeCun advisory.** CuspAI CEO Max Welling told the FT that the company is building an "AI Materials Foundry" with Nvidia to discover novel compounds via foundation models trained on physics simulations. Geoffrey Hinton and Yann LeCun have joined the advisory board — an unusually high-profile alignment for a materials-science startup. *(Source: [Financial Times / AI Weekly](https://www.ft.com/content/5c2ae092-14af-4bd1-8e3d-8996755cba6a))*

---

## ⚖️ Policy & Regulation

- **EU formally opens bidding for 7 AI gigafactories, €10B public funding committed.** On July 30, the European Commission opened its call for AI Gigafactory proposals, backing €10B ($11.4B) in public funding toward a €30B total target once private investment is included. Seven planned sites will each host at least 100,000 AI chips — roughly 4x current EU datacenter scale. The bidding window closes November 12, 2026, with awards expected by mid-2027. An earlier informal call drew 77 proposals across 16 member states and 60 sites. *(Source: [News4Jax / AI Weekly](https://www.news4jax.com/business/2026/07/30/eu-lays-out-114-billion-for-7-ai-gigafactories-as-it-aims-to-catch-up-with-us-and-china/))*

- **FCC bans new Chinese humanoid robots and grid inverters on national security grounds.** The FCC unveiled rules barring US imports of new Chinese humanoid and quadruped robots and connected power inverters used to link renewables, batteries, and datacenter gear to the grid. The rules frame the measures as insulating the US AI supply chain from Chinese disruption, data theft, and cyberattack. The robot rule is expected to hit Unitree hardest, which holds nearly a fifth of the global humanoid market. *(Source: [Yahoo Finance / AI Weekly](https://finance.yahoo.com/news/exclusive-trump-administration-ban-chinese-183301640.html))*

- **Anthropic clarifies open-weights position, urges three concrete policies.** Dario Amodei stated "Anthropic has never advocated for a ban on open-weights models," breaking silence after Anthropic skipped a 25-firm Nvidia-led pro-open-weights letter. The post makes three concrete asks: block powerful AI chips from reaching China (and crack down on smuggling), target "industrial-scale distillation" by authoritarian states, and require mandatory pre-release safety testing on cyber, bio, and alignment risks for any sufficiently capable model — open or closed. *(Source: [Anthropic / AI Weekly](https://www.anthropic.com/news/position-open-weights-models))*

---

## 🛠️ Tools & Products

- **MCP specification goes fully stateless in July 28 update.** The Agentic AI Foundation (a Linux Foundation directed fund) released the 2026-07-28 MCP spec — the largest change since launch. It moves MCP to a stateless request/response core, eliminates the initialize/initialized handshake and session headers so any server instance can handle any request behind a plain load balancer, adds Multi Round-Trip Requests for mid-call user input, and hardens auth with RFC 9207 issuer validation. TypeScript, Python, Go, C# Tier 1 SDKs and a beta Rust SDK ship with the release. *(Source: [MCP Blog / AI Weekly](https://blog.modelcontextprotocol.io/posts/2026-07-28/))*

- **Critical CVSS 10.0 flaw in Ruflo MCP platform exposed 233 tools; patched.** Noma Labs disclosed CVE-2026-59726 ("RufRoot") in Ruflo (67K+ GitHub stars, #2 on MCPMarket): a single unauthenticated HTTP POST to the MCP bridge on port 3001 could execute code and exfiltrate LLM API keys. Ruflo's maintainer shipped version 3.16.3 within 24 hours, binding the bridge to loopback and gating terminal_execute behind access controls. All 233 tools were exposed on default Docker Compose deployments. *(Source: [The Hacker News / AI Weekly](https://thehackernews.com/2026/07/ruflo-mcp-flaw-lets-unauthenticated.html))*

- **Ars Technica tests Google SynthID: watermarking holds but "a losing game" at scale.** Ars Technica's hands-on test found SynthID watermarking hard to break within Google's own generation pipeline, but trivially sidestepped by using non-SynthID models or regenerating content elsewhere. The piece argues that even a robust watermark can't solve provenance at internet scale when unwatermarked generation stacks remain widely available — following Google's May 2026 expansion of SynthID adoption to OpenAI, ElevenLabs, and Kakao. *(Source: [Ars Technica / AI Weekly](https://arstechnica.com/ai/2026/07/tested-google-synthid-works-great-but-labeling-ai-content-may-be-a-losing-game/))*

---

## ⚡ What to Watch

- **California AI Transparency Act goes operative August 2 (Friday).** This is the most imminent US state AI law to take effect — organizations operating AI systems in California should verify compliance by end of week.

- **Recursive Superintelligence (Socher) shipping initial "self-improving systems" products by October 2026.** The $650M-funded startup signed a $400M multiyear AWS compute deal and confirmed a public product launch target of October, making it the most-watched near-term agentic AI product debut.

- **EU Gigafactory bidding closes November 12, 2026; watch for the 77+ applicants to begin lobbying for selection.** Today's formal opening of the call kicks off a 15-week bidding process for the largest AI infrastructure public-funding program outside the US and China. Member state competition for site selection will intensify quickly.

---

*Sources used: technologyreview.com, aiweekly.co, anthropic.com, microsoft.com, investor.atmeta.com, ft.com, bloomberg.com, datacenterknowledge.com, news4jax.com, hpcwire.com, thehackernews.com, arstechnica.com, huggingface.co, blog.modelcontextprotocol.io, finance.yahoo.com, the-decoder.com, techcrunch.com*
