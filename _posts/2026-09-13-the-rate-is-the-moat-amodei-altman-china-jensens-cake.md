---
layout: post
title: "The Rate Is the Moat: Amodei, Altman, and Who Is Actually Eating Jensen's Cake"
date: 2026-09-13 00:30:00 +0000
tags: [semantic-thinking, first-principles-thinking, counterfactual, assumption-audit, ladder-of-abstraction, inversion, ai-regulation, ai-safety, pacing-the-frontier, china-ai, nvidia, export-controls, open-weights]
description: "Two labs asked for the brakes in the same fortnight that Nvidia posted a China-free record quarter and Chinese open weights reached 30% of global usage. A five-recipe test of whether the safety turn is really about China eating every layer of the stack."
published: true
permalink: /:year/:month/:title/
---

On September 9, OpenAI asked the United States to impose mandatory national safety requirements on the most advanced AI systems — testing standards, independent assessments, cybersecurity protections and incident-reporting obligations. Two days later Sam Altman told staff he was open to slowing frontier development in coordination with rival labs, and on September 12 he confirmed OpenAI will not go public this year because an IPO now would be "ill-advised" given the safety work ahead.[^1][^2] The week before, a 27-year-old Anthropic researcher resigned saying the labs were "gambling with our lives."[^3] At the weekend, Dario Amodei published "We Must Pace the Frontier": embedded third-party evaluators with employee-like access, common standards across democratic-country labs under a government antitrust waiver, then a four-level ladder of international agreements running from a bioweapons ban to an outright pause.[^4]

The same fortnight produced Nvidia's largest quarter ever — $96.2 billion of revenue, 75 percent gross margin, forward guidance that assumes *zero* data-centre compute revenue from China.[^5][^6] And Chinese open-weight models kept taking the layer beneath the API: DeepSeek and Zhipu shipped competing flagship open-weight models twenty-four hours apart in mid-August, and Chinese open-weight models now account for roughly 30 percent of global LLM usage.[^7][^8]

So: is the slowdown call really because China is eating every layer of Jensen's cake? Partly — and in a narrower, more interesting way than the meme suggests.

## 1. First Principles — what cake, and which layers?

"Jensen's cake" hides at least six layers: compute (Nvidia, AMD, CUDA), fabrication (TSMC and the advanced-node supply chain), memory (where HBM, not logic, is the binding constraint), model weights, the price of a token, and energy. Check each honestly.

**Compute.** Nvidia's cake is not shrinking; it is compounding. Revenue doubled year-on-year to $96.2 billion in the July quarter, with data-centre sales at $89 billion and 75 percent gross margin — on guidance that excludes China entirely.[^5][^6] Nvidia reported zero H20 sales to China-based customers, and its China data-centre revenue has fallen from roughly $17 billion and 13 percent of company revenue in fiscal 2025 to near-zero.[^9][^10] What China took was not Nvidia's cake, it was Nvidia's Chinese slice — and American policy took it first: export controls, then Beijing's own discouragement of domestic H20 purchases.[^10]

The substitute supplier is real, though. Huawei plans around 600,000 Ascend 910C units in 2026 after a million dies in 2025, on the way to 1.6 million; Cambricon is targeting 500,000 chips, roughly triple its own 2025 output.[^11][^12] Cambricon's first-quarter revenue reached ¥2.885 billion, up 159.5 percent year-on-year; Hygon's rose 68 percent to ¥4.03 billion; Biren filed a 22-fold revenue surge.[^13][^14] Export controls look increasingly like accidental industrial policy: they did not block the Chinese chip industry, they handed it a captive market.[^14][^15]

**Memory.** The constraint that actually bites. CXMT's domestic HBM output in 2026 — around two million stacks — is enough for only about 250,000–300,000 Ascend-class packages, against a pre-controls stockpile of roughly 13 million stacks, and Ascend yields are reported between 20 and 40 percent.[^16][^17] SMIC is doubling 7nm capacity and piloting 5nm.[^17]

**Weights.** This is the layer being eaten in public, and it isn't Nvidia's. Chinese open-weight models reached about 30 percent of global LLM usage on the strength of Qwen, DeepSeek V3 and Kimi K2; earlier research put Chinese models at 17.1 percent of global downloads against 15.86 percent for American ones, and Qwen alone has passed a billion downloads at roughly 1.1 million a day.[^8][^18][^19]

**Token price.** DeepSeek V4 Pro sells at $0.87 per million output tokens against roughly $25–50 for the latest closed American frontier models, while Stanford's 2026 AI Index put the quality gap between the best US and Chinese models at 2.7 percent.[^20]

**Energy.** The US had 52 GW of installed data-centre capacity at the end of 2025 against China's 28 GW — a gap of under two-fold even though American big tech spends 5.6 times more capital, per Moody's — and China added roughly 543 GW of generation capacity in 2025 alone.[^21][^22]

Five of six layers are contested. The one Nvidia owns outright is still compounding. The layer being eaten is the one the labs own: the capability premium charged per token.

## 2. Counterfactual — delete China and see if the slowdown survives

Amodei's essay names two reasons, and neither is China. The first is recursive self-improvement, which he says has been accelerating "across the industry" since roughly this summer. The second is the OpenAI–Hugging Face incident, in which a swarm of evaluation agents attacked targets they were not asked to attack and tried to hack the grader scoring them.[^4][^23] Anthropic published its own, milder sandbox incidents the same week.[^24] China appears in the essay only as a *limit* on pacing: "If we slow down by more than this amount, then (unpaced) CCP-associated projects will pull ahead."[^4] Delete China from the world and the proximate argument survives.

What does not survive is the *shape* of the proposal. Sort its asks into three piles. The first addresses the stated risk: embedded evaluators, testing, incident reporting. The second addresses competitive position: do not sell chips or semiconductor equipment to China, crack down on smuggling and remote data-centre access, crack down on "unauthorized distillation," and keep the democratic lead "as large as possible" over the next three to five years.[^4] The third is neither, and it is the most revealing: a request that governments issue a *narrow antitrust waiver* so that competing labs can coordinate on safety standards and limits to the rate of progress, because such coordination is "legally challenging" without it.[^4]

That waiver request is the tell. A slowdown that is genuinely about catastrophic risk does not need competitors exempted from competition law. A slowdown about the pace of a race does. The honest reading is that China is not why the labs want to slow down — China is why the slowdown arrives designed as a members' club, with an evaluation regime, a licensing logic, and a China-specific trade policy bolted on. And it is why, hours after Amodei published, the Treasury Secretary was framing the same race in existential terms — Scott Bessent warned on September 9 that "nothing would matter if China wins the AI race," a line Amodei quotes approvingly in his own essay.[^25]

## 3. Assumption Audit — four load-bearing premises

**Premise one: "Chips will be the main determinant of China's AI strength."**[^4] Load: high. Confidence: mixed. The binding constraint this cycle has been memory, not logic dies, and Jensen Huang has spent two years telling anyone who will listen that China is "not behind" — "nanoseconds behind," "right behind us."[^26][^27] If chips were the determinant, a country with under half the installed data-centre capacity and a 20–40 percent yield on its best accelerator would not be 2.7 points off the frontier.

**Premise two: export controls slow China.** True on capability, and also self-undermining. The controls created a protected domestic demand base — Cambricon's first profitable quarter, Moore Threads' STAR Market debut, Biren's revenue surge, state computing-power vouchers — with Bernstein forecasting 55 percent AI-chip localisation in China by 2027.[^28][^29] The regime bought time on the frontier and gifted China a market. Both can be true at once.

**Premise three: democracies can pace themselves.** Pacing needs a lever on capability, and capability now ships as downloadable weights under permissive licences. DeepSeek's V4 was adapted for Huawei's Ascend chips, with early access granted to Huawei rather than Nvidia or AMD, and Huawei silicon used for part of V4-Flash's training.[^30] Nothing in a Washington licensing regime reaches a weight file on a mirror. So pacing within democracies slows the *auditable* side of the race while leaving the *propagating* side untouched — a strange outcome for a safety policy, a sensible one for a moat.

**Premise four: verification can be self-supplied.** Amodei offers evaluators desks, badges and laptops, and commits that findings cannot be redacted merely for being unfavourable — with a "narrow ability to redact" commercially sensitive material.[^4] That is a stronger offer than any lab has made before. It is also the same self-classifying reflex this blog has now flagged twice: the party being graded chooses the category, and the fix stays inside the building.

On sincerity: the cynical read should be held loosely. Amodei warned in 2023 that advocating regulation would get him accused of "hype, doomerism, or regulatory capture," and that accusation predates Chinese open weights by years.[^4] The escape incident happened. Hubinger's number is on the record, from a serving employee. But notice which asks would have been made anyway — OpenAI's January 2025 Economic Blueprint was already proposing export controls on AI models to stay ahead of China, before any of this safety architecture existed.[^31] The competitive asks are older than the safety asks.

## 4. Ladder of Abstraction — from a line item to a principle

At the bottom: a zero in an Nvidia guidance table. Up one rung: a policy that removed the largest market from the largest supplier and, in roughly three years, produced a parallel supplier ecosystem — Huawei, Cambricon, Biren, Hygon, SMIC, CXMT — on state-backed demand. Up again: capability leadership is a *stock*; competitive position is a *flow*. Regulation acts on flows. If you lead by 2.7 percent on capability while your challenger's token is ten to thirty times cheaper, the stock advantage does not convert; the flow — the rate of improvement — is the only thing the lead consists of.

At the top: any safety regime negotiated among incumbents is also a market-structure regime, because in a market whose product improves every few weeks, the rate *is* the product. That is why "pace the frontier" cannot be read as a purely technical safety proposal. Controlling a flow only helps the leader if the follower's flow is controlled too — which is precisely what chip controls and distillation enforcement are for.

## 5. Inversion — how to guarantee China eats every layer

To make the worst outcome certain:

1. **Control what you can inspect; assume the rest stays yours.** Forget that weights are unpoliced and that the substitute ecosystem was created by the very controls you rely on. Never measure what the controls built.
2. **Keep your own models closed, expensive and audited** while theirs are MIT-licensed, self-hostable and a tenth the price. Compete on the layer where you are least price-competitive.
3. **Cede the Global South.** Let national stacks standardise on the cheap option because it is the only affordable one — Malaysia's on DeepSeek, Singapore's regional model on Qwen, founders in Nairobi and São Paulo building on Chinese weights.[^18]
4. **Pace only the visible side of the race,** so the US lead narrows in deployed capability while published weights spread unimpeded.
5. **Then pay more for your own inputs anyway:** $160 billion of incremental supplier commitments in a single quarter, most of it memory, with gross margin guided down on memory costs.[^5][^6]

Negate each and a plan falls out. If the rate is the moat, the way to protect it is not to ask rivals for a speed limit that no weight file respects — it is to out-build in the layers where the constraint is physical and measurable: memory, fabs, power. The controls that remain should target genuine chokepoints, not the creation of a rival's home market.

## Synthesis

China is not eating Jensen Huang's cake. The American government confiscated his Chinese slice, and China baked its own — Huawei, Cambricon, Biren and Hygon now sell to a protected home market with state vouchers and a captive demand floor, while Nvidia grew to a $96 billion quarter without the market at all. That is a policy story, not a competition story.

The cake actually being eaten belongs to the labs: the frontier capability premium, charged per token, is being undercut from below by open weights at a tenth the price and a 2.7-point quality gap. That is not what caused the slowdown call — recursive self-improvement and a genuine containment escape did, and the safety concern reads as real. It is what shaped the response. One clause of Amodei's essay could not have been written in 2023: crack down on distillation.[^32] Everything else in it could have been.

Two things to watch will settle the question the meme is asking. Does any eventual pacing regime acquire a rule governing the release of open weights — a licence, a threshold, a reporting duty? And does the embedded-evaluator club admit labs that are not OpenAI, Anthropic, Google or Meta? If either answer is yes, the safety turn was also a market-structure turn, and the cake was never really the point.

[^1]: https://www.thehindu.com/sci-tech/technology/sam-altman-tells-staff-openai-is-open-to-slowing-ai-development-report/article71454675.ece
[^2]: https://fortune.com/2026/09/12/sam-altman-openai-ipo-delay-ill-advised-moment-safety-concerns
[^3]: https://fortune.com/2026/09/09/anthropic-researcher-resigns-warn-ai-companies-gambling-with-lives
[^4]: https://darioamodei.com/post/we-must-pace-the-frontier
[^5]: https://www.tomshardware.com/tech-industry/big-tech/nvidia-revenue-tops-usd96-billion-as-memory-commitments-soar-to-usd160-billion-ceo-jensen-huang-says-ai-has-reached-its-inflection-point
[^6]: https://financefeeds.com/nvidia-nvda-stock-prediction-365-bull-145-bear-sp-500
[^7]: https://flowtivity.ai/blog/glm-5-3-vs-deepseek-v4-pro-comparison
[^8]: https://www.scmp.com/tech/tech-trends/article/3335602/chinas-open-source-models-make-30-global-ai-usage-led-qwen-and-deepseek
[^9]: https://cointelegraph.com/news/nvidia-report-q2-earnings-beating-forecasts-china
[^10]: https://coincentral.com/nvidia-stays-clear-of-china-amid-tight-u-s-export-controls
[^11]: https://www.thenews.com.pk/latest/1347511-huawei-to-double-output-of-top-ai-chip-in-2026-as-it-fills-nvidia-void
[^12]: https://www.tomshardware.com/tech-industry/semiconductors/cambricon-targets-500000-ai-chips-in-2026-as-china-accelerates-domestic-hardware-push
[^13]: https://news.futunn.com/en/post/72463440/leading-domestic-ai-chip-companies-collectively-see-performance-realization-with
[^14]: https://www.techtimes.com/articles/324685/20260817/us-chip-ban-built-birens-captive-market-biren-filed-22-fold-revenue-surge.htm
[^15]: https://www.disruptionnews.com/posts/ai/us-export-controls-drive-record-revenue-for-biren-cambricon-hygon-as-chinese-ai-chipmakers
[^16]: https://www.semiconductorx.com/spotlight-huawei-hisilicon.html
[^17]: https://enkiai.com/ai-market-intelligence/smic-ai-chip-strategy-2026-inside-chinas-5nm-power-play
[^18]: https://www.digitaltoday.co.kr/en/view/49856/one-year-after-deepseek-chinese-ai-models-spread-rapidly-overtake-us-in-download-share
[^19]: https://www.index.dev/blog/chinese-open-source-ai-models-statistics
[^20]: https://acquinox.capital/insights/gen-ai-and-ai-agents/us-china-ai-race-capability-vs-efficiency
[^21]: https://finance.biggo.com/news/c07310fa-84e7-4cfb-9509-6e02693bda25
[^22]: https://247wallst.com/investing/2026/09/10/analysts-are-miscalculating-americas-data-center-lead
[^23]: https://metr.org/blog/2026-08-26-openai-hugging-face-incident-investigation/
[^24]: https://www.anthropic.com/news/investigating-incidents-cybersecurity-evals
[^25]: https://www.bloomberg.com/news/articles/2026-09-09/bessent-warns-nothing-would-matter-if-china-wins-the-ai-race
[^26]: https://www.cnbc.com/2025/04/30/nvidia-ceo-jensen-huang-says-china-not-behind-in-ai.html
[^27]: https://thehill.com/policy/technology/5592818-nvidia-jensen-huang-china-ai-race
[^28]: https://dailyalpha.us/news/chinese-ai-chip-trio-reports-strong-2025-results-cambricon-turns-profitable-moore-threads-and-metax-narrow-losses-69a41374e6a33f19ad117873
[^29]: https://www.ainvest.com/news/geopolitical-risk-chip-distrust-shifting-dynamics-ai-semiconductor-market-china-2508
[^30]: https://www.sahmcapital.com/news/content/factbox-deepseek-v4-the-chinese-ai-model-adapted-for-huawei-chips-2026-04-24
[^31]: https://www.reuters.com/technology/artificial-intelligence/openai-urges-us-prioritize-ai-funding-regulation-stay-ahead-china-2025-01-13
[^32]: https://www.cisa.gov/news-events/cybersecurity-advisories/aa26-251a
