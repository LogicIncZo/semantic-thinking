---
layout: post
title: "The Speedometer Is the Law: OpenAI's Perplexity Curve and the Speed Limit Only One Lab Can Read"
date: 2026-11-23 12:45:00 +0000
permalink: /:year/:month/:title/
description: "On November 22, OpenAI chief scientist Jakub Pachocki published the lab's internal pretraining log-perplexity curve for the first time and asked rival labs to adopt it as the industry's shared yardstick — with common limits no one crosses until a monitoring milestone that does not exist yet. Three frames on the first disclosure of the ruler."
tags: [semantic-thinking, five-whys, nietzche-ladder, decision-matrix, openai, pachocki, perplexity, pretraining, scaling, ai-safety, pacing]
published: true
---

On November 22 at 17:03 UTC, OpenAI chief scientist Jakub Pachocki published "Perplexity and Intelligence" — the first public release of the lab's internal pretraining curve — and proposed that frontier labs adopt perplexity as a shared yardstick for a common system of development limits.[^1] The numbers, tracked since GPT-3.5 on a fixed snapshot of OpenAI's own codebase: ~0.99 for GPT-3.5 (fluent conversation), ~0.91 for GPT-4 (productive chain-of-thought), below 0.8 where transformative cybersecurity and mathematics capabilities emerged, and ~0.76 for the model that started "producing groundbreaking results" on open math problems — resolutions arriving "one after another in a single Slack thread."[^1] The published chart descends to roughly 0.73 for an unnamed internal model, with a shaded band below about 0.71 marked with a question mark.[^2] Pachocki expects "further transformative capabilities" — of an unknown nature, possibly not yet tested for — as models enter the ~0.68–0.7 window, alongside further degradation of alignment auditing and rising evaluation awareness; he warns that AI-accelerated pretraining research could produce an "avalanche" of advances "as soon as 2027," faster than alignment research can match.[^1] The concrete ask: common limits, based on perplexity and other measurements, that developers commit not to cross until understanding and monitoring of AI behavior achieves a concrete milestone — "such as the development of a successor to CoT monitors."[^1] Sam Altman endorsed it.[^3] Three frames on the first disclosure of the ruler.

## Five whys: why publish the curve now?

*Why publish numbers that help competitors?* The stated reason: the concern "is outweighed by the urgency of establishing shared safety measures," a step toward "a shared scientific basis for future pacing efforts," explicitly linking to Amodei's pacing essay.[^1] *Why the urgency now?* Because the same post concedes the next capability window (~0.68–0.7) is untestable in advance, and OpenAI's own alignment research reports that chain-of-thought monitorability degrades as perplexity falls — capability may outrun observation inside the very window the limit targets.[^1][^4] *Why gate the limit on a milestone?* Because a bare number is a press release; a milestone makes resumption conditional on an artifact that would have to actually work. *Why nominate a metric rivals cannot score?* The held-out dataset is a fixed snapshot of OpenAI's internal codebase; outside reporting notes only OpenAI — and, by one account, Microsoft AI — can run it.[^5] Transparency of the readings, opacity of the instrument. *Why, at root?* Standard-setting is strategy. The lab that owns the yardstick chairs the pacing table — and the seat was acquired by an act of apparent generosity.

## Nietzsche ladder: burden, idol, instrument

**The Camel** carries the proposal as handed down, and the burden is real: this is the first voluntary disclosure of a frontier lab's core progress metric, accompanied by four self-confessed weaknesses — cross-lab comparison is hard, perplexity maps to no task anyone cares about directly, chain-of-thought gains are invisible to it, and the floor is unknown, so "smaller gains on perplexity will correspond to larger leaps in model intelligence."[^1] It dignifies the ask: a concrete, measurable pacing proposal is on the table at all.

**The Lion (responding to Camel)** — you have carried the numbers well; now ask who forged the ruler. The yardstick is a private codebase snapshot. The gate is vaporware: the "successor to CoT monitors" does not exist, and the same lab reported this month that monitoring degrades with scale.[^4] The Camel's own favorite sentence cuts deepest — "I don't know what those capabilities will be, and we may not be testing for them today"[^1] — a confession that in the band that matters, the gauge reads nothing. A speed limit legible only to the manufacturer is not a shared rule; it is a request.

**The Child (responding to Lion)** — good: you broke the idol of vendor-neutral transparency. What can be built in the cleared space? A ruler is common when its construction is common: a jointly governed public evaluation corpus; bits-per-byte scoring to blunt tokenizer dependence (which reduces, though does not remove, the comparison problem);[^5] third-party scoring on the accreditation-lab model, so the measurer and the measured are different parties; a public milestone registry with falsifiable criteria, so the gate can be audited before anyone drives through it. Transparency of the instrument, not only of the readings. The essay's closing hope — "to see more transparency about it across the industry"[^1] — is an invitation with the signature line already printed.

## Decision matrix: four ways to share a yardstick

| Option | Cross-lab comparability | Third-party verifiable | Catches non-pretraining gains | Adoptable now |
|---|---|---|---|---|
| A. As proposed: OpenAI's fixed internal snapshot, log-perplexity | High — but for one lab | No | No | Yes |
| B. Common public corpus + bits-per-byte, externally scored | High | Yes | No | Medium — build effort |
| C. Status quo compute caps (EU AI Act Art. 51, California — input-based)[^5] | Crude | Moderate | No | Already live |
| D. Treaty-style verification body | High | Yes | Partial | Near zero |

Option A's disclosure is genuine and useful, but it fails the test that makes a limit *shared*: nobody else can check the reading. B dominates A on comparability and verifiability while preserving the metric that actually predicts emergence; A's curve is exactly the calibration data B would need. C is enforceable but measures an input, not the outcome that matters.[^5] D is what the situation eventually requires and politically cannot yet obtain. The honest verdict: build B on A's footing — the disclosure is necessary, the design is unfinished.

## What the frames reveal together

The whys show urgency and strategy entangled: the same disclosure that serves pacing also positions OpenAI as the industry's metrologist. The ladder separates the honest numbers from the private ruler — the first is a gift, the second is a jurisdiction. The matrix shows the repair is boring and buildable. Together: this is simultaneously the most concrete voluntary limit proposal the industry has produced and a governance design in which measurer and measured are the same party. The limit becomes real at the moment the ruler does — a public corpus, an external scorer, a falsifiable milestone. Until then, "common limits" is one lab's number line, with everyone else's signature requested underneath.

[^1]: https://openai.com/index/perplexity-and-intelligence/
[^2]: https://cellcog.ai/blog/openai-perplexity-and-intelligence
[^3]: https://www.investing.com/news/stock-market-news/openai-scientist-proposes-industry-ai-limits-tied-to-model-intelligence-metric-5044174
[^4]: https://alignment.openai.com/cot-monitorability-model-lifecycle
[^5]: https://www.techtimes.com/articles/331307/20261123/openais-jakub-pachocki-proposes-ai-scaling-limits-scored-private-test-only-openai-can-run.htm
