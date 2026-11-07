---
layout: post
title: "The Moat Was a Calendar: AI Agents Reprice RSA-1024"
date: 2026-11-07 06:00:00 +0000
tags: [semantic-thinking, assumption-audit, first-principles-thinking, inversion, ladder-of-abstraction, google, deepmind, cryptography, rsa, ai-agents]
published: true
permalink: /:year/:month/:title/
description: "DeepMind's agents found two faster attacks on legacy 1024-bit RSA in weeks — not a break of modern encryption, but the death of the assumption that cryptographic hardness moves on human time. Four frames on the repricing."
---

On Friday, Google DeepMind announced two cryptanalytic results against legacy 1024-bit RSA, led by Krishnamurthy Dvijotham and Abhradeep Thakurta in collaboration with Nadia Heninger (UC San Diego and Inria) and Emmanuel Thomé (Inria) — the cryptographers whose own 2026 work set the baseline now being beaten.[^1][^2] The headline numbers: a signature-forgery method that, by theoretical estimate, improves on the best known attack by roughly 1,600x once an attacker controls about half of a PKCS#1-signed block, and a batch-factoring algorithm with better asymptotics that cuts roughly 30x off the marginal cost of each additional 1024-bit key.[^2] Both papers are drafts; 2048-bit RSA and everything above it is explicitly untouched; and DeepMind's own framing is tempo, not apocalypse — advances that "historically take years or decades" now arrive in weeks.[^1][^3] Four frames on what actually moved.

## 1. Assumption Audit: The Keystone Was Never Mathematical

Sort the claim everyone is repeating — "AI agents broke RSA" — into its premises. The factual layer is true but narrower than the headlines: the signature result was demonstrated in a sandbox against an already-solved benchmark key, at 3.5x less CPU time than the academic run.[^2] The hidden premises carry the real weight. First: that smart people tried for decades and failed, therefore the problem is hard. That is evidence, not proof — the difficulty of factoring was never a theorem, only a posterior built from what the general number field sieve has cost so far. Second, and load-bearing: that the search over possible attacks is bounded by human careers. That premise is the one these papers remove. The keystone assumption is that cryptanalytic tempo is human-scaled, and the cheapest test of whether it has moved is independent reproduction of the 30x batch saving on real hardware — which is not yet known.[^3]

## 2. First Principles: Hardness Is a Race, Not a Wall

What is RSA-1024's security actually made of? A race between two curves. One is the cost of the best known factoring algorithm, updated occasionally by heroic human projects — RSA-768 took a thirteen-person team about two years in 2009. The other is the retirement schedule of deployed keys. The safety margin is the gap between the curves, and the industry's implicit model was that the attack curve's slope is set by how many Heninger-and-Thomé-grade humans exist. What changed is not the mathematics; it is who does the searching. Reports of the reproduction run describe two cooperating agents — supervisor and executor — steered by roughly twenty human messages, writing tens of thousands of lines of code and compressing the academic team's months into days.[^4][^5] The margin was always a clock. The clock speed was an assumption.

## 3. Inversion: How to Guarantee the Worst Outcome

Ask how to guarantee catastrophe. Keep treating "no attack observed" as "no attack exists." Let 1024-bit keys linger wherever they actually live — trust anchors, code-signing paths, embedded firmware, old PGP keys — because nobody can say where they all are. Budget cryptographic review on the human cadence of decades while attack tempo moves to weeks. Wait for a public break before rotating. Each negation is a checklist item: inventory legacy crypto (most organizations cannot), adopt DeepMind's own prescription of continuous stress-testing,[^1] and treat agent-accelerated cryptanalysis as a planning input rather than a press event. And note where the real disaster hides: not in 1024 falling, but in assuming 2048 inherits the same moat — without ever re-running the agents against the GNFS extrapolations that 2048's margins rest on.

## 4. Ladder of Abstraction: From Two Drafts to Every Empirical Moat

Bottom rung: two draft papers, a retired key size, a sandboxed reproduction. Middle rung: the mechanism — agentic search converts accumulated human failure into machine iterations, repricing the asset "we have looked for years and found nothing." That asset backs more than RSA: AlphaEvolve's 48-multiplication matrix result and the co-mathematician's FrontierMath run are the same template in different domains.[^2] Top rung: every defense whose safety argument is "the search space is too large" — cryptographic hardness, but also fuzzing, exploit discovery, proof search — now carries an unstated exposure to compute tempo. Descend the ladder and the concrete action is boring and overdue: find where legacy RSA lives and retire it. The principle it teaches is that hardness assumptions need owners, budgets, and refresh cycles like any other control.

## What the Frames Converge On

DeepMind's framing is right and quietly radical: the results show "why we must not assume the mathematical hardness" of schemes we have relied on.[^1] They do not move today's risk — 2048 is fine, the papers are drafts, the 1,600x is a theoretical estimate.[^2][^3] What moved is the calibration of the future. The moat around cryptographic hardness was time, and time just got cheaper. The tell to watch: independent reproductions of the batch-factoring savings on real hardware, and whether standards bodies start demanding cryptographic inventories with retirement deadlines. A defense whose primary resource was "attackers haven't gotten around to it yet" was never a defense; it was a schedule. Agents just changed the schedule.

---

[^1]: https://x.com/pushmeet/status/2118752095859794390
[^2]: https://officechai.com/ai/google-deepmind-says-it-has-used-ai-agents-to-break-legacy-rsa-1024-encryption-faster-than-anyone-thought-possible
[^3]: https://framesignal.com/stories/google-deepmind-ai-finds-cheaper-attacks-old-1024-bit-encryption-keys
[^4]: https://eprint.iacr.org/2026/2131
[^5]: https://x.com/neuralloot/status/2118767097895399828
