---
title: "What Makes a New Deep Learning Model Paper Convincing, Part 2: Contribution, Evidence, and the Narrative"
date: 2026-09-17
permalink: /posts/2026/09/proving-it-and-telling-it/
excerpt: "Notes from reading 52 published deep-learning-model papers: how contribution claims get proven, not just asserted, and how gap, novelty, and contribution turn out to be one argument rather than three."
tags:
  - deep learning
  - research methodology
  - information systems
---

*Notes from reading 52 published deep-learning-model papers in ISR, MISQ, Marketing Science, and Management Science — Part 2 of 2*

In [Part 1](/posts/2026/09/what-a-new-deep-learning-model-actually-needs-to-justify-itself/), I walked through the first two of three connections that seemed to separate strong DL-model papers from weak ones: a motivation that names a specific failure rather than an absence, and a novelty claim that survives being asked "would this hold if you swapped out the deep learning component?" This post covers the third connection — how contribution claims get proven, not just asserted — and then zooms out to the harder question: how do all three pieces get woven into something that reads as one coherent argument rather than three separate, half-connected assertions?

## Claiming a Contribution Is Not the Same as Proving One

Here's a distinction that seems obvious in the abstract and turns out to be very easy to blur in practice: claiming a type of contribution, and actually furnishing the evidence that contribution requires, are two different acts, and a paper can do the first without doing the second.

Across the corpus, contribution claims clustered into recognizable types: the method or artifact itself; generalized design principles; theoretical contribution (extending, testing, or challenging an existing theory); domain insight; practical or economic value; generalizability; and societal value. None of these are illegitimate claims to make. The problem is what happens when the claim outruns the evidence — practical value claimed with no dollar figure or field data behind it, generalizability claimed off a single dataset with no transfer evidence, theoretical contribution claimed by citation alone with no extension or test of the theory.

## Practical Value Has to Be Counted, Not Asserted

The clearest positive case in the corpus is Yu and colleagues' (2024) *ISR* paper on fall prevention for senior care. The paper doesn't just say the HMM-GAN framework has practical value — it quantifies it: "through an in-depth case study, we demonstrate how the proposed framework can lead to significantly reduced potentially catastrophic falls by senior citizens and produce more than $33 million of economic benefits over competing models" (Yu, Chai, Samtani, Liu, & Chen, 2024). That number is doing real work in the paper. It converts "our model reduces false negatives" into a claim a hospital administrator or a health policymaker can actually act on. A practical-value claim without a figure like this is, structurally, an unfinished sentence.

## Interpretability Claims Need a Human in the Loop

A related pattern shows up around interpretability claims specifically. It's easy to claim a model is "interpretable" and stop there — show some attention weights, call it a day. Guo and colleagues' (2025) ICU length-of-stay paper goes further: it validates its explanations using "the conceptual evaluation property (Co-12) framework and a small-scale user study of ICU clinicians" (Guo, Bardhan, Ding, & Zhang, 2025). The interpretability claim isn't just asserted from the model's internals; it's checked against the actual people the interpretability is supposedly for. If your gap is "clinicians need to understand why," your evidence eventually has to include clinicians, not just SHAP values.

## Evidence Beyond the Performance Table

Here's a pattern that showed up so consistently it started to feel like an unwritten rule: every strongly-rated paper had at least one form of evidence *beyond* a benchmark comparison and ablation study. Not instead of those — in addition to them. Yu and colleagues' (2024) economic-value case study is one flavor of this. A different flavor shows up in Cont and colleagues' (2026) *Management Science* paper, TAIL-GAN: its central claim rests on a mathematical property — the joint elicitability of Value-at-Risk and Expected Shortfall — which the authors "exploit ... to design a Generative Adversarial Network that learns to simulate price scenarios preserving these tail risk features" (Cont, Cucuringu, Xu, & Zhang, 2026). The loss function isn't chosen because it happened to work in a grid search; it's chosen because it's provably tied to the statistical properties the paper cares about, and that theoretical grounding is itself a form of evidence a performance table alone couldn't provide.

A performance table, no matter how favorable, answers only one question: does this model predict better than the alternatives? It doesn't answer the questions a design-science reviewer actually cares about — does this matter to anyone, does it change a decision, does it hold up for a reason grounded in theory rather than luck. This is something I now plan for at the *research design* stage, not something I retrofit after the model is built, because a case study, a field partnership, or a theoretically grounded loss function usually needs to be built into the project from the start.

## Mechanism, Not Just Accusation, When You Claim Fairness or Bias Contributions

Fu and colleagues' (2022) *Management Science* paper, "'Un'Fair Machine Learning Algorithms," is a useful contrast case because it isn't a deep-learning-architecture paper at all — it's a theoretical argument about fairness-constrained algorithms — but it illustrates something that applies directly to any paper claiming a fairness or bias contribution. Rather than asserting that fairness constraints are good or bad in the abstract, the paper works out a specific mechanism: fair ML algorithms that require impact parity can, under specific and identifiable conditions, "make everyone worse off, including the very class they aim to protect," because firms facing a costly fairness constraint may rationally underinvest in improving their model's accuracy (Fu, Aseri, Singh, & Srinivasan, 2022). That's a theoretical contribution earning its keep: it doesn't just cite fairness theory, it derives a specific, falsifiable mechanism from it. If your paper claims a theoretical contribution around bias or fairness, the bar this sets is a mechanism, not an accusation.

## Matching Your Vocabulary — and Your Framing — to the Venue

One mismatch I saw repeatedly, and which is easy to miss when you're deep in your own draft, is contribution claims phrased in the wrong journal's dialect. ISR and MISQ favor a fairly distinct vocabulary — "IT artifact," "design principles," "situated implementation" — built on a citation lineage running through Hevner, Rai (2017), Gregor and Hevner (2013), and more recent typologies. Zhu and colleagues' (2026) RecAudit paper is a clean example of this vocabulary used correctly and specifically, not decoratively: the authors describe their contribution as "developing a privacy-preserving IT artifact that operationalizes regulatory requirements on data revocation and profiling in learning-based recommender systems" (Zhu, Yang, Fan, & Lian, 2026) — the artifact language is tied to a concrete regulatory requirement (GDPR's "right to be forgotten"), not floating free of the paper's actual content.

*Marketing Science* and *Management Science* speak differently — contributions are more often framed against two or three specific streams of prior literature, without needing the "IT artifact" vocabulary at all. Fu and colleagues' (2022) fairness paper, for instance, situates itself against the fair-ML literature and against the economics of algorithmic decision-making, with no design-science apparatus in sight, and reads as entirely appropriate for its venue because of that fit rather than in spite of it. When these get crossed — design-science language showing up in a paper with no challenge-to-artifact structure behind it, or a design-science venue paper with no such vocabulary at all — it reads as slightly off-key, even when the underlying research is sound.

## Zooming Out: Why This Is Really One Argument, Not Three

Writing all of this down forced me to notice something I hadn't fully articulated before: these three connections — gap, novelty, contribution — aren't three separate checklists to satisfy independently. They're links in a single chain, and the chain either holds together or it doesn't.

The chain runs like this: a specific number of named limitations in existing methods → an equal number of named design components that each address one limitation → a novelty claim that survives being asked whether the deep learning component is actually doing the work, or is just a replaceable part → a set of contribution claims whose evidence matches their type, laid out in an order that mirrors the paper's actual structure.

You can see the whole chain working end to end in a single paper. Zhu and colleagues' (2025) FDA 510(k) recall-prediction paper opens with a concrete stakes claim (device recalls causing "substantial patient harm" and financial strain), narrows to three named design challenges (predicate network structure, temporal patterns, citation dependencies), builds three correspondingly named components, and closes by tying the model's "insights into the performance variations across device categories" to "the literature on health information systems for societal good" — a contribution claim that follows directly from what the model was actually shown to do, rather than being bolted on at the end (Zhu, Sen, Everhart, & Karaca-Mandic, 2025). Every weak paper I read, by contrast, had a break somewhere in that chain — and the break is usually locatable in a specific, nameable way once you know to look for it: a claimed novelty in architecture with no theoretical account of why it needs that shape, a generalizability claim resting on adjectives instead of a transfer path, a contribution vocabulary borrowed from a different journal's conventions.

## How the Chain Should Show Up in the Writing Itself

This has practical consequences for how a paper — or really, any piece of design-oriented writing — should be built, sentence by sentence and section by section, not just conceptually.

The introduction should open by establishing why the problem matters, with the kind of concrete stakes Zhu and colleagues (2025) or Zhang and colleagues (2025) provide, rather than a general assertion. It should then name the limitations of existing approaches as a numbered list of specific failures, and introduce the proposed model with each of its components pre-mapped, even briefly, to the limitation it's meant to solve. Whatever order the contributions are previewed in at the end of the introduction should be the *exact same order* they reappear in at the end of the paper — this consistency check alone catches a surprising number of structural drifts that happen across multiple rounds of revision, where a limitation gets added late but the corresponding component never quite gets built, or a contribution gets reordered in the conclusion without anyone updating the introduction to match.

The method section should re-establish the challenge-to-component mapping explicitly, the way Zhu and colleagues (2025) do with their three named design challenges, rather than assuming the reader remembers the introduction's promise three sections later. Each component's subsection should explain *why* it needs to exist — the domain or theoretical reasoning, as in Zhang and colleagues' (2025) lexicon-to-attention pipeline — before it explains *what* it computationally does, and should close by explicitly naming which challenge it resolves.

The evaluation section should follow benchmarks and ablations with a clearly separated space for evidence beyond the performance table — an economic case study like Yu and colleagues' (2024), a user study like Guo and colleagues' (2025), or a theoretical property like Cont and colleagues' (2026) — not buried in a footnote or an appendix, but given its own visible section, because that's often exactly the evidence a reviewer is scanning for and won't credit if it's hard to find.

And the discussion should restate the contributions in the same order they were promised, using the vocabulary appropriate to the target venue — "IT artifact" framing tied to a concrete requirement, as in Zhu and colleagues (2026), if the venue is ISR or MISQ; a literature-positioning framing, as in Fu and colleagues (2022), if it's Marketing Science or Management Science — and should address the paper's own limitations honestly, including, if it's true, acknowledging that the novelty leans more on theory or formulation than on architecture. Papers that pre-empt this objection tend to read as more trustworthy than papers that let a reviewer discover it first.

## What Changed for Me

The biggest shift this exercise produced wasn't a new fact about deep learning. It was a change in what question I ask myself first when I have a new idea. I used to start with: is this model good? Now I start with: does the chain hold? Is the gap a specific failure or just an absence? Does the novelty survive the substitution test, or is it hiding somewhere else in the paper that the framing hasn't found yet? For every contribution I want to claim, do I actually know, right now, what evidence would prove it — a number like Yu and colleagues' (2024) $33 million, a user study like Guo and colleagues' (2025), a derived mechanism like Fu and colleagues' (2022) — and have I planned to collect that evidence, or am I hoping it'll show up later?

That's a much earlier and much cheaper place to find a paper's weaknesses than after a full draft, let alone after a rejection.

## The Checklist, Complete

Putting both posts together, here's the full checklist I now run against any new idea, and again against any finished draft:

1. Are the limitations of existing methods numbered (two to four), and is each one a specific, concrete failure rather than an absence?
2. Do challenges, components, and ablations line up one-to-one-to-one?
3. If the novelty is purely architectural, has it been reinforced with theory, problem formulation, or a training objective?
4. Does the model survive the substitution test — would the paper's conclusions hold if the deep learning component were swapped for a standard alternative?
5. Does the abstract's verb (develop/propose vs. apply/leverage) match what the method section actually does?
6. Is there at least one form of evidence beyond the performance table — a case study, a user study, an economic-value calculation, or a theoretical property?
7. Are contributions ordered method → design principles/theory → generalizability → practical/societal value, in vocabulary that matches the target venue?
8. For every claim of practical value, generalizability, or theoretical contribution, is there evidence actually planned — not just asserted?

This list came out of reading fifty-two other people's papers closely enough to see where they were strong and where they were quietly hoping nobody would ask the obvious question. The tool is useful, but the habit underneath it is the real point: stop asking whether the model is good, and start asking whether the chain — from failure, to design, to proof — actually holds all the way through.

## References

Cont, R., Cucuringu, M., Xu, R., & Zhang, C. (2026). TAIL-GAN: Learning to simulate tail risk scenarios. *Management Science, 72*(4), 2917–2936. https://doi.org/10.1287/mnsc.2023.00936

Fu, R., Aseri, M., Singh, P. V., & Srinivasan, K. (2022). "Un"fair machine learning algorithms. *Management Science, 68*(6), 4173–4195. https://doi.org/10.1287/mnsc.2021.4065

Guo, T., Bardhan, I. R., Ding, Y., & Zhang, S. (2025). An explainable artificial intelligence approach using graph learning to predict intensive care unit length of stay. *Information Systems Research, 36*(3), 1478–1501. https://doi.org/10.1287/isre.2023.0029

Yu, S., Chai, Y., Samtani, S., Liu, H., & Chen, H. (2024). Motion sensor-based fall prevention for senior care: A hidden Markov model with generative adversarial network approach. *Information Systems Research, 35*(1), 1–15. https://doi.org/10.1287/isre.2023.1203

Zhang, D., Zhou, L., Tao, J., Zhu, T., & Gao, G. (2025). KETCH: A knowledge-enhanced transformer-based approach to suicidal ideation detection from social media content. *Information Systems Research, 36*(1), 572–599. https://doi.org/10.1287/isre.2021.0619

Zhu, Y., Sen, S., Everhart, A., & Karaca-Mandic, P. (2025). A deep learning approach for predicting FDA's 510(k) medical device recalls using device citation relationships. *Information Systems Research*, Articles in Advance. https://doi.org/10.1287/isre.2024.1351

Zhu, Z., Yang, Y., Fan, Y., & Lian, D. (2026). Forget me if you can: Auditing user data revocation in recommendation systems. *Information Systems Research*, Articles in Advance. https://doi.org/10.1287/isre.2024.1179
