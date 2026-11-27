---
layout: post
title: "The Algorithm Is a Rumor: Aaronson's 'Bombshells,' the Labs' Silence, and Who Holds a Broken RSA"
date: 2026-11-27 12:30:00 +0000
permalink: /:year/:month/:title/
description: "Scott Aaronson says he has heard 'many, many rumors' that OpenAI or Anthropic are sitting on a polynomial-time factoring algorithm — a result that would break RSA — and neither lab has said a word. Four frames on a break that exists publicly only as a rumor."
tags: [semantic-thinking, assumption-audit, first-principles-thinking, analogy-transfer, inversion, openai, anthropic, cryptography, rsa, scott-aaronson, factoring, p-vs-np]
published: true
---

Late on November 24, Scott Aaronson — UT Austin complexity theorist, former OpenAI alignment researcher — answered a reader on his blog: "I've now heard many, many rumors that one or both labs are sitting on Factoring in P. I don't know how much to credit this."[^1] Andrew Curran, who says the rumor has run about ten days, adds the parallel-labs logic: "if one has it, they probably both do. This would crack RSA."[^2] Two days later Nature quoted his escalation — "I'm virtually certain, from multiple reliable sources, that the AI labs are now sitting on one or more bombshells" — alongside his own caveat: until he sees details, "I feel much, much less confident about the specific nature of those bombshells."[^3] The rumored object: a polynomial-time algorithm for integer factoring — the assumption RSA's padlocks are built on — whispers extend to "more-advanced technologies" — the post-quantum schemes.[^3] The Times reported mathematicians who "fear discoveries are being hushed up."[^4] Neither OpenAI nor Anthropic has said a word.[^5] Four frames on a break that exists, publicly, only as a rumor.

## 1. Assumption Audit: What "Sitting On" Actually Claims

The phrase packs premises:

| # | Assumption | Category | Load | Confidence | Testability |
|---|---|---|---|---|---|
| 1 | A factoring-in-P algorithm exists at one or both labs | Factual | Breaks everything | Low — no artifact, no statement | Cheap — publication |
| 2 | "Sitting on" means deliberate withholding, not unfinished verification | Causal | Shapes the secrecy story | Unknown | Moderate — a dated statement |
| 3 | The algorithm is practical at deployed key sizes | Capability | High for impact; irrelevant to the math | Low — polynomial time is not automatically practical | Expensive |
| 4 | Aaronson's sources are reliable | People | Breaks the news value | His own hedge concedes the gap | Only in hindsight |
| 5 | The rumor's spread is harmless until confirmed | Continuity | Degrades | Already falsified — in most copies "the caveat had fallen off" | Done |

The keystone is #1, and note what the autumn's verified results do to it: OpenAI and Anthropic both posted VP ≠ VNP proofs on November 23 — an algebraic cousin of P vs NP, i.e., evidence *for* hardness elsewhere — and Nature reports most researchers think the encryption rumors are unlikely to be confirmed.[^3][^6] The rumor thrives not because evidence points at it but because this industry has demonstrated it *can* hold results back.

## 2. First Principles: What a Withheld Algorithm Is Worth

Strip the case to fundamentals. A zero-day's value survives secrecy because the vulnerable code is specific and expensive to rediscover. A mathematical algorithm is the opposite artifact: the discovery process — an agentic search over proof space, run on rented compute — is repeatable by anyone with similar compute. DeepMind's agents already compressed cryptanalytic months into days against RSA-1024.[^7] The fundamentals then invert the secrecy logic: the same search re-run finds the same algorithm; the holder's advantage is bounded by time-to-rediscovery; the migration RSA's fall demands — rotating keys, re-signing code, retiring embedded firmware — takes years and can only begin on signal. A rational holder of a civilizational lockpick discloses on a coordinated calendar. The rumor describes the opposite: an open-ended hold.

## 3. Analogy Transfer: The Equities Process Nobody Built

The structural twin exists. When a government agency discovers a zero-day in widely deployed software, it faces the same choice — use, withhold, disclose — and the US formalized it as the Vulnerabilities Equities Process, a charter that is "biased toward responsibly disclosing" but has no hard rules, thin oversight, and a demonstrated failure mode: the NSA's retained Windows exploit escaped into WannaCry.[^8][^9] The transferable mechanism: a pre-committed charter, a default toward disclosure for anything touching civilian infrastructure, a decision clock. Translated to labs: a published cryptographic-equities policy before the next rumor, with artifact release to a trusted third-party set on a timeline. Disanalogy check: a zero-day is patchable; factoring-in-P is a mathematical truth with no patch — only a years-long migration. That strengthens the disclosure case: the only remediation is the slow one.

## 4. Inversion: How to Guarantee the Worst Outcome

Goal: minimize harm if the rumor is true. Invert it. (1) Say nothing and let the rumor metabolize into fact-free certainty — the Aaronson comment reached 3.4 million views within a day, caveats stripped.[^2] (2) Disclose a capability claim with no artifact — panic without verification, the mirror of last week's artifact-without-readers.[^10] (3) Let rumor-management substitute for a migration plan: no cryptographic inventory, no agility standard, no post-quantum deadline pulled forward. (4) Let each lab hoard privately, so rediscovery races an unknown clock instead of a coordinated one. The negations are cheap: a dated confirmed/denied/incomplete statement, an artifact to vetted referees, a standards-body bulletin. The context makes the silence stranger: OpenAI's October release dumped 722 manuscripts in a day — disclosure as volume — while its Yang-Mills proof sits vaulted behind "shepherds" — disclosure as favor.[^11] And 575 physicists, Witten and Maldacena among them, signed a statement insisting AI-produced results "should be released openly and in full": a result only one company can read is an announcement, not science.[^12]

## What the Frames Converge On

The story is not factoring; it is the absence of any institution for holding a discovery the world must act on before it can verify. Automated discovery makes the breakthrough cheap and the disclosure channel scarce, and the rumor is the market's guess at what a sealed vault contains. Whatever the vault holds, the week proved silence is now load-bearing infrastructure — and nobody is maintaining it. Watch for three tells: a lab statement naming what exists, an artifact released to trusted referees, or a standards body moving post-quantum timelines. If the rumor dies quietly, that is the darker outcome: the indefinite hold becomes a permanent genre, and every future "many, many rumors" gets priced in as normal.

---
[^1]: https://scottaaronson.blog/?p=10379
[^2]: https://x.com/kimmonismus/status/2125602411540566221
[^3]: https://www.nature.com/articles/d41586-026-03875-6
[^4]: https://www.thetimes.com/uk/technology-uk/article/ai-making-online-security-useless-smr73d3n8
[^5]: https://clashreport.com/world/articles/aaronson-rumors-ai-labs-factoring-rsa-0s2ejunl8kx
[^6]: https://github.com/anthropics/formal-math/blob/main/vp-vnp/README.md
[^7]: https://logicinczo.github.io/semantic-thinking/2026/11/the-moat-was-a-calendar-deepmind-rsa-1024/
[^8]: https://www.belfercenter.org/publication/governments-role-vulnerability-disclosure-creating-permanent-and-accountable
[^9]: https://georgetownsecuritystudiesreview.org/2019/05/28/vulnerabilities-equities-process-revisited
[^10]: https://logicinczo.github.io/semantic-thinking/2026/11/the-proof-outgrew-the-prover/
[^11]: https://aiweekly.co/node/17268
[^12]: https://www.facebook.com/ayushphy/posts/575-theoretical-physicists-have-signed-a-short-statement-asking-ai-companies-to-/1815329623930253
