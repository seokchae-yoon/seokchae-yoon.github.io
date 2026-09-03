---
title: "Bayesian Model, Bayesian Estimation, Bayesian Learning Model"
date: 2026-09-03
permalink: /posts/2026/09/bayesian-model-estimation-learning-model/
excerpt: "Three phrases that get used almost interchangeably, and aren't. A map between them, with a coin and a new hire to make it concrete."
tags:
  - bayesian statistics
  - econometrics
---

"Bayesian" attaches itself to a lot of nouns: model, estimation, learning, network, inference. Three of these phrases in particular get used almost interchangeably, and shouldn't be. Before going deeper into any one of them, it's worth mapping out what each actually names, and worth making the map concrete rather than abstract.

## Bayesian model: the scaffolding

A **Bayesian model** is a structure, nothing more. You specify a prior $p(\theta)$ over some parameters and a likelihood $p(D \mid \theta)$ that says how probable the data would be under each value of $\theta$. That's the whole definition, before a single number gets computed. Bayesian linear regression, a Bayesian hierarchical model with varying intercepts across groups, a Bayesian neural network with a prior over its weights, these are all Bayesian models in exactly this sense: the word describes how the model is built, not what happens to it afterward.

To keep things concrete, take the simplest possible case and stay with it for a while. You have a coin, possibly unfair, and you want to know its bias $\theta$, the probability it lands heads. A natural prior is $\theta \sim \text{Beta}(1,1)$, which is just the uniform distribution on $[0,1]$: before flipping anything, every bias is equally plausible. The likelihood is Binomial: given $\theta$, the probability of seeing a particular sequence of heads and tails is what you'd expect from independent coin flips. Prior plus likelihood, full stop. Nothing has been estimated yet. This pairing alone is already a complete Bayesian model.

## Bayesian estimation: the computation, and why order doesn't matter

**Bayesian estimation** is what happens once data show up: the procedure that turns a Bayesian model plus observed data into a posterior, $p(\theta \mid D) \propto p(D\mid\theta)p(\theta)$. This can be done in one pass over a fixed dataset, or one observation at a time, folding each posterior back in as the next prior. It is tempting to call the first "just estimation" and the second "learning," but the coin makes it easy to see why that distinction doesn't hold up.

Flip the coin ten times and get 7 heads, 3 tails. Because Beta and Binomial are conjugate, the batch posterior has a closed form: $\text{Beta}(1+7,\,1+3) = \text{Beta}(8,4)$. Now do it one flip at a time instead. Say the sequence was H, H, T, H, T, H, H, T, H, H. Updating after every flip:

$$\text{Beta}(1,1) \to \text{Beta}(2,1) \to \text{Beta}(3,1) \to \text{Beta}(3,2) \to \text{Beta}(4,2) \to \text{Beta}(4,3) \to \text{Beta}(5,3) \to \text{Beta}(6,3) \to \text{Beta}(6,4) \to \text{Beta}(7,4) \to \text{Beta}(8,4)$$

Same endpoint, $\text{Beta}(8,4)$, reached ten small steps at a time instead of one big step. And it's not just this sequence: run the flips in a completely different order, three tails first and then seven heads straight through, and the running posterior visits a different path, $\text{Beta}(1,2) \to \text{Beta}(1,3) \to \text{Beta}(1,4) \to \text{Beta}(2,4) \to \cdots \to \text{Beta}(8,4)$, but arrives at exactly the same place. This is a direct consequence of Bayes' rule being associative and commutative under the usual i.i.d. assumption: the posterior only tracks the total count of heads and tails, not the order they arrived in or whether they were processed together or apart. Batch versus sequential is a computational choice, not a different kind of inference. Whichever way you run it, this is Bayesian estimation, and it's what most people mean when they say a model was "fit Bayesianly."

## Bayesian learning model: a different question, not a different computation

A **Bayesian learning model** is a different thing again, and the difference isn't about *how* the posterior is computed but about *what it's a posterior over*. The coin example, run either way, is still an analyst estimating a fixed, external, physical parameter chosen for a study. In the structural econometrics sense of the term, a learning model swaps that out entirely: the unknown quantity isn't a coin's bias sitting outside anyone's life, it's something an economic agent doesn't know about *themselves*.

Take a new hire at a firm. Call her true long-run productivity $\theta_i$. On day one, nobody knows $\theta_i$ exactly, not her manager, and often not even the analyst herself; ability of this kind rarely announces itself. Each quarter, a signal arrives: a performance review score, a count of completed projects, a client's feedback, something correlated with $\theta_i$ but contaminated by the ordinary noise of who happened to review her, which projects she happened to draw, whether the quarter was slow company-wide. Her manager, watching these signals accumulate, revises a belief about $\theta_i$ after each one. If that revision follows the same Bayes'-rule mechanics as the coin's posterior update, algebraically it can look identical: a prior belief, a noisy signal, an updated posterior belief that becomes the next prior. But the referent has completely changed. Nobody is running a designed experiment on an inert object. Someone's professional life is the thing generating the signals, and someone's belief about a person, sometimes that very person's belief about herself, is the thing being revised.

The same structure shows up anywhere the truth about something only reveals itself gradually, and where the person doing the learning is a participant rather than an outside observer: a firm inferring the real demand for a new product from early, noisy sales figures; a founder inferring their startup's actual viability from a handful of ambiguous early customers; a worker inferring, from a string of good and bad performance reviews, whether they're actually suited to the job. The researcher isn't the one doing the learning in any of these. The agent inside the model is, and the researcher's job is to estimate the parameters, the signal-to-noise ratio, the speed of updating, that govern that process.

## Where this leaves the three terms

Bayesian model is the scaffolding, prior plus likelihood, with no data touched yet. Bayesian estimation is the computation that scaffolding supports once data arrive, and as the coin showed, it genuinely doesn't care whether you run it in one shot or many; the posterior lands in the same place either way. Bayesian learning model is a specific application of both, one where the belief being formed and revised belongs to an agent embedded in the economics, not to the statistician standing outside it. [The next post](/posts/2026/09/bayesian-learning-model-noisy-signals/) takes that third one apart properly, starting from where it actually starts: not a coin, but a noisy signal, and someone who doesn't yet know the truth about themselves.
