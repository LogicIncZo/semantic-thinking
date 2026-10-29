---
layout: post
title: "The Competitor Is the Creditor: OpenAI, Google's TPUs, and the Compute Estate That Owns Itself"
date: 2026-10-29 06:30:00 +0000
tags: [semantic-thinking, first-principles-thinking, nietzche-ladder, inversion, analogy-transfer, google, openai, nvidia, anthropic, tpu, ai-compute]
published: true
description: "OpenAI plans to buy Google's chips, Oracle will rent them out, and Broadcom is financing Anthropic's ~$400B TPU bet. Four frames on the week the escape from Nvidia turned into a round trip."
permalink: /:year/:month/:title/
---

On Tuesday, October 28, [The Information and Bloomberg reported](https://www.bloomberg.com/news/articles/2026-10-28/openai-plans-to-buy-google-s-chips-as-part-of-its-ai-build-out) that OpenAI — the single most valuable customer Nvidia has — plans to buy Google's tensor processing units. Terms are unknown; both companies declined to comment. But OpenAI has already posted a job listing for an engineer to lead optimization of its frontier models on TPUs, for training and inference both — [not a test drive, a team](https://michaelparekh.substack.com/p/ai-googles-tpu-moment-with-openai). The report landed inside a 48-hour pileup. The day before, [Oracle became the first hyperscaler outside Google to offer TPUs](https://www.oracle.com/news/announcement/ai-world-oracle-brings-google-tpus-to-oracle-cloud-infrastructure-2026-10-27/) — the 8t for training, the 8i for inference — starting 2027. The same day, Broadcom arranged [$63 billion in financing through a special purpose vehicle](https://biz.heraldcorp.com/article/10917707) to fund Anthropic's purchases of the TPUs it co-designs with Google. And Anthropic's S-1, filed this week, itemized roughly [$400 billion of Google-linked compute commitments](https://michaelparekh.substack.com/p/ai-googles-tpu-moment-with-openai) — $161.2 billion in five-year TPU leases through Broadcom, $114.5 billion with Google Cloud, and $125–150 billion in estimated TPU spend for 2028–2031 — about half its ~$800 billion total. Alphabet then reported Q3 on Wednesday: [Cloud revenue up 103% to $30.7 billion](https://9to5google.com/2026/10/28/alphabet-q3-2026-earnings/), [capex of $51.4 billion for the quarter, negative free cash flow](https://www.cnbc.com/2026/10/28/alphabet-googl-earnings-q3-2026.html) — and the stock fell more than 10% anyway. Run it through four frames.

## 1. First-Principles Decomposition: A Token Has a Bill of Materials

**Problem.** Why would Nvidia's biggest customer buy its rival's chip?

**Assumptions to question.** The default read — "OpenAI is diversifying supply" — treats compute as one commodity and chips as interchangeable insurance. It also treats the chip vendor's margin as invisible.

**First principles.** Strip it down. What a frontier lab actually buys is not chips; it is served tokens — intelligence delivered at the lowest cost per token, per watt, per second of latency. From there: (1) training is a spike; inference is an annuity, and the industry's volume is moving to the annuity. (2) The chip vendor's gross margin is a tax on every token served — and that tax is the largest renegotiable line in the bill of materials. (3) The real moat is software, not silicon: CUDA. (4) Purpose-built silicon trades generality for unit economics — a TPU does less, so it can cost less per token.

**Rebuilt answer.** A multi-chip strategy is not supply security; it is arbitrage against the margin tax, plus leverage in every future negotiation. That is why the most quietly radical item this week is not the purchase plan but OpenAI's floated release of [internal tooling for running models across many kinds of chips](https://www.theinformation.com/newsletters/ai-infrastructure/openai-release-internal-tool-weaken-nvidias-software-advantage) — aimed not at Nvidia's silicon but at its software lock. When the biggest customer attacks the lock rather than the chips, it is repricing the token, not shopping for hardware.

**Difference from the default.** "Nvidia faces competition" is the headline. The fundamentals say something narrower and bigger: the bill of materials for machine intelligence is being renegotiated, and chips are becoming lease terms on rentable cognition.

**Practical next step.** Watch cost-per-token at listed prices — not TOPS, not deal headlines.

## 2. Nietzsche Ladder: Camel, Lion, Child

**Camel.** Carry the inherited account first, because it is heavy and honestly held. Diversification is prudence. "The next generation of AI will require a diverse range of compute," said [Amin Vahdat, Google's chief technologist for AI and infrastructure](https://www.techtarget.com/news/openais-reported-google-tpu-deal-tests-ai-chip-economics/873139), announcing TPU availability beyond Google's own cloud. The numbers carry the burden: TD Cowen estimates TPUs bring Google [$9.4 billion in the second half of 2026, growing to a $138 billion business by 2028](https://michaelparekh.substack.com/p/ai-googles-tpu-moment-with-openai). Meta rents them; [Apple and Citadel Securities buy capacity](https://michaelparekh.substack.com/p/ai-googles-tpu-moment-with-openai). Hedging concentration risk in the most capital-intensive supply chain on earth is not a sin.

**Lion (responding to Camel).** You have carried the burden well — now ask who wrote the tablets. "Diversification" is the word creditors use. Look at the structure under the story: Nvidia invests [$3 billion in Meta's equity offering](https://michaelparekh.substack.com/p/ai-googles-tpu-moment-with-openai) — while Meta rents Google's TPUs. Nvidia extends [$105 billion in credit support to an OpenAI datacenter built entirely on Nvidia chips](https://biz.heraldcorp.com/article/10917707). Broadcom finances Anthropic's purchase of Broadcom's own co-designed accelerators through an SPV. Google sells chips to labs it competes with in models; OpenAI serves its models through Google's cloud. Every buyer is a shareholder; every rival is a creditor. This is not a market of competitors — it is a keiretsu with a product roadmap. The stated frame is rivalry; the realized structure is mutual capture, in which nobody can afford for anybody to fail.

**Child (responding to Lion).** Your No is necessary, but it is not yet creation. If every lab holds every vendor and every vendor holds every lab, then the fiction the industry still maintains — my chips versus your chips, my cloud versus yours — can finally be dropped for what already exists: one interconnected compute estate, wearing competing logos. The child's move is to make it official and honest: a public obligations graph, the way an S-1 itemizes debts — who has committed what to whom, netted and published. OpenAI's hinted cross-chip software layer points the same direction: if interoperability is inevitable, ship it as a commons instead of a hostage. The playful version is also the sober one — intelligence as a utility does not need rival gods, it needs a clearinghouse.

## 3. Inversion: How to Guarantee the Buildout Breaks

**Goal.** A compute expansion that survives a demand wobble.

**Inverted question.** How would you guarantee it collapses?

**Failure modes.** (1) Finance the buyers: lend customers the money to purchase your product, via SPVs and equity stakes. (2) Out-commit revenue: sign take-or-pay obligations that dwarf income — Anthropic's ~$800 billion in commitments against $16.3 billion of first-half revenue; Alphabet spending $51.4 billion a quarter into negative free cash flow, [long-term debt up from $21.6 billion to $125.1 billion in a year](https://eu.36kr.com/en/p/4046614272119681). (3) Correlate everyone's balance sheet with everyone else's revenue, so one default cascades. (4) Concentrate the payback in inference demand that is still mostly projected. (5) Assume the demand curve stays vertical through 2030.

**Guards.** Net the obligations publicly, so exposure is known before it is fatal. Contract for capacity, not chips — chips depreciate, contracts can be restructured. Keep at least one major balance sheet unlevered. Count vendor equity stakes as what they are — financing with extra steps — against real demand, not as evidence of it.

**The plan, stated forward.** Diversification that reduces correlated obligations is resilience. Diversification that multiplies them is synchronization gear. The TPU moment is simultaneously the hedge and the amplifier of the fragility it hedges against.

## 4. Analogy Transfer: Vendor Financing Has a Track Record

**Structural form.** A dominant supplier taxes an industry; buyers seek alternatives; suppliers and buyers blur through financing until the tax, the product, and the credit become one instrument.

**Structural twins.**

| Domain | Their version of the problem | Their mechanism |
|---|---|---|
| Telecom, 1996–2001 | Lucent and Nortel financed carriers' equipment purchases | Vendor credit converts customers into leveraged demand; ends in write-downs when end-demand stalls |
| Keiretsu Japan | Cross-shareholding among suppliers and customers | Interlocking absorbs shocks — until it transmits them, synchronized, as in the 1990s |
| Airlines vs Boeing/Airbus | Duopoly buyers hedge across two airframers | Financing stays separate from hardware; the duopoly persists but nobody owns the airline's debt |

**Candidate transfers.** Broadcom's SPV is textbook telecom-style vendor financing — the track record says the mechanism survives growth and fails on demand stalls, and Nvidia's equity stakes are the same instrument wearing an equity hat. The keiretsu predicts today's resilience and tomorrow's synchronized bust. The airline model is the counter-design: keep the silicon merchant and the financing neutral.

**Disanalogy check.** Telecom vendors financed customers who were not their competitors; here Google sells chips to model rivals and Nvidia holds stakes in the customers its chips power — the loop is tighter, which strengthens the analogy rather than breaking it. One real break: chips depreciate on a two-year cycle where planes fly for twenty-five years, so any reckoning arrives faster. The analogy survives, with a shorter fuse.

## What the Frames Converge On

Not one frame turned on whether OpenAI's purchase closes, or how large it is. All four agree the event is structural: the AI compute buildout has matured from a market into a web of mutual obligations, and the word of the week — diversification — names the stated motive, not the realized mechanism. Two testables to watch. First, whether OpenAI actually ships the cross-chip software layer: that would convert CUDA's moat into a public utility and tell us whether the token's bill of materials gets renegotiated for everyone or only for the biggest buyer. Second, whether anyone publishes the obligations graph in netted form: Anthropic's S-1 offered the first honest line items, and Alphabet's negative free cash flow the first honest cash confession. The TPU was the quiet part of Google's stack. This week it got loud — and turned out to be wired to everything.
