---
layout: page
title: Entropy and learnability
description: How does the entropy of a distribution relate to a language model's ability to learn from that distribution?
img: assets/img/long_range_bigrams_50_softmax.png
importance: 1
category: work
related_publications: true
---

## Introduction

Are statistical properties of sequential data, like entropy, necessarily predictive of a language model's ability to learn from that data? The entropy, or self-entropy of a random variable $X\sim p$ is defined as:

$$H(X) = -\sum_{x \in \mathcal{X}} p(x) \log p(x)$$

where $X$ is a random variable with support (possible outcomes) $\mathcal{X}$, and $p(x)$ is the probability of observing some particular outcome $x$.

Entropy can be thought of as a measure of how uncertain we are, on average, about the outcome of a random variable. In this sense, it is the expected value (the mean) of the surprisal $(-\log p(x))$ of the random variable - on average, how surprised are we by the outcome of the random variable?

The language modeling task seeks to minimize a related quantity called *cross-entropy*, which is defined as:

$$H(p, q) = -\sum_{x \in \mathcal{X}} p(x) \log q(x)$$

where $p$ is the true distribution of the data, and $q$ is the model's distribution over the data. The cross-entropy is a measure of how well the model's distribution $q$ matches the true distribution $p$.

A model that is optimized to convergence on the cross-entropy objective, in theory, will have:

$$p(x) = q(x) \forall x \in \mathcal{X}$$

In other words, the model's distribution over the data will match the true distribution of the data exactly. Then, we would expect the cross-entropy to reduce to the entropy of the true distribution:

$$H(p, q) = H(p, p) = H(X)$$

## Some experiments

Take a look at some plots I made [here](https://dan-the-meme-man.github.io/entropy-learnability/).
