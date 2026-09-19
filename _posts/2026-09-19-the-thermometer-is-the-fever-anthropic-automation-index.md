---
layout: post
title: "The Thermometer Is the Fever: Anthropic Measures Its Own Handover"
date: 2026-09-19 12:00:00 +0000
tags: [semantic-thinking, first-principles-thinking, assumption-audit, nietzche-ladder, explanation-ladder, anthropic, claude, recursive-self-improvement, ai-safety, ai-governance, measurement]
published: true
permalink: /:year/:month/:title/
description: "Anthropic published an index of how much of its own R&D Claude performs — rated largely by Claude. Four recipes on a lab that built a gauge for its own replacement, and what a self-made ruler can and cannot do."
---

On Wednesday, Anthropic published three measurements meant to let the public track "the pace of AI development inside frontier labs."[^1] The headline instrument is the Anthropic R&D Automation Index: as of August 2026, Claude "leads" — completes most of a task end-to-end under supervision, Level 4 of 6 — 26% of the company's AI R&D work, up from under 1% in February. Over 90% of work now sits at or above "AI collaborates," and no measured subset runs fully autonomously. The surrounding numbers talk too: more than 80% of the code merged into Anthropic's codebase in May was written by Claude, and engineers merge roughly eight times more code per day than in 2024.[^2] The methodology is the twist — Claude agents read Slack to build the task tree, and an independent Claude judge assigns the automation ratings. The Associated Press rendered it without decoration: Claude is helping to build the next version of itself.[^3]

## First Principles — what the number is made of

Strip the framing and the index reduces to simple parts: R&D is person-time on tasks; the index is a person-time-weighted average of task-level automation ratings; the ratings come from a Claude judge reading Claude-gathered evidence, on Epoch AI's scale.[^4] What must be true is not controversial: machine labor is substituting for researcher labor in model-building, and it is now measured — under 1% to 26% in six months. What is merely customary is the reading of the act: a number published by a lab is conventionally called "transparency." Rebuild from fundamentals and this is instrumentation — a gauge built to make Dario Amodei's call to "pace the frontier" arguable in public rather than prophetic.[^5] The headline number is also the conservative one: it is the loudest fact on the page only if you ignore that AI is an active collaborator on over 90% of the work.

## Assumption Audit — the keystone under the index

The disclosure rests on a short register of load-bearing assumptions. Definitional: that Epoch's six levels cut research work at stable joints — Anthropic concedes "real room for disagreement" on where "collaborates" ends and "leads" begins, and its judge agreed exactly with staff raters 59% of the time while staff agreed exactly with each other just 35%.[^1] Fidelity: that the judge is not systematically generous to its own kind — partially answered by a blind staff cross-check in which model and human ratings landed within one level 97% of the time. Causal: that publication produces understanding, and understanding produces legitimate pacing decisions rather than calibrated complacency. Continuity: that a frozen basket of July 2026 tasks still represents the work — checked against task drift from February to July. The keystone is the definitional one: the AL3/AL4 boundary is precisely where the story lives, it is the softest line on the page, and the headline 26% inherits all of that softness. The cheapest test is the one Anthropic proposes but has not yet run: independent third-party evaluators with real access. Until then, 26% is a self-portrait — well-attested, but a self-portrait.

## Nietzsche Ladder — the ruler and the ruled

The Camel carries the inherited burden: lab self-reporting runs from safety frameworks through risk reports to last week's incident disclosures, and the operational weight behind this one is real — a billion agent decisions monitored in August, full coverage, roughly fifty escalations to humans per week.[^1] You have carried the tablets well; now ask who etched them. The Lion notes that the measured party wrote the scale, drew the basket, and defined the tripwire — "fully autonomous" — at which the world is supposed to become alarmed. The number arrives in the same weeks the labs petition Washington for coordinated slowdown while the president calls their warnings a hoax.[^6] Defining the threshold of public panic is a power that precedes any measurement. The Child answers without smashing the instrument: make the gauge adversarial — third-party judges inside the loop, published denominators, versioned baskets, rival labs' models reading the evidence. A number the public can audit is a beginning of governance. The alternative, unmeasured acceleration, serves nobody — including the labs asking to be paced.

## Explanation Ladder, compressed — from 26% to the pattern

High School: in February Claude did almost none of Anthropic's research; by August it led a quarter of it. College: the index is a person-time-weighted basket of roughly fifteen thousand tasks in a 542-node tree, each rated AL0–AL5 by a judge model.[^1] PhD: the reliability numbers are contested but checked — 59% exact agreement against humans who agree with each other 35% of the time; a frozen basket that can miss work migrating to new task types; a companion compute metric that measures spend, not effort. Philosopher: measurement precedes governance — nothing unmeasured has ever been paced — but the instrument's builder holds the strongest interest in its reading, and the category "full autonomy" is drawn by the party whose freedom it bounds. Gigabrain: we built a machine that reports, as a single number, how fast it is replacing the people who built it — and the astonishing part is not the 26. It is that the machine computed the number, about itself, using itself as the judge.

## Synthesis — the odometer and the handover

Read together, the frames converge: the index is simultaneously the first honest odometer on recursive self-improvement and a strategic artifact in the pacing fight. Three things decide which it becomes. Whether the third-party evaluator plan gets staffed, given access, and published. Whether a rival publishes comparable numbers — OpenAI's new automated "research intern" is offered in the same spirit, and Elon Musk says humans at xAI are "gradually getting less and less in the loop."[^7] And whether the metric ever gates a launch, or only decorates the debate. An index that never gates anything is a chart. But every instrument regime began with a first reading — and the fight worth having now is over who holds the gauge.

[^1]: https://www.anthropic.com/institute/measuring-pace-of-ai-development
[^2]: https://moroccoworldnews.com/2026/09/338870/anthropic-warns-ai-could-soon-start-building-its-own-successors
[^3]: https://techxplore.com/news/2026-09-anthropic-claude-version.html
[^4]: https://epochai.substack.com/p/toward-an-onet-for-ai-r-and-d
[^5]: https://darioamodei.com/post/we-must-pace-the-frontier
[^6]: https://www.nytimes.com/2026/09/18/us/politics/trump-ai-safety-anthropic-openai-china.html
[^7]: https://wtop.com/national/2026/09/will-ai-models-achieve-the-ability-to-improve-autonomously-leading-labs-say-the-scenario-is-near
