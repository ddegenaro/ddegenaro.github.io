---
layout: page
title: FLASH-MAX
description: A quick overview of the FLASH-MAX project, accepted as a Spotlight Poster at NeurIPS 2026.
img: assets/img/flashmax.png
importance: 1
category: work
---

## TL;DR

We developed a shallow neural network technique for solving partial differential equations (PDEs) with constant coefficients. We've applied it extensively to Maxwell's equations, which describe the electromagnetic interaction in physics. It works really well; it's faster, cheaper, and needs way less data than any other method of solving these PDEs!

## Abstract from our paper

We introduce FLASH-MAX, a shallow, exact-by-construction neural network architecture for predicting homogeneous electromagnetic fields from sparse pointwise observations. Each hidden neuron represents a separate exact solution to Maxwell’s equations, so that the network satisfies the governing equations symbolically by construction and can be trained end-to-end from sparse data within seconds. We prove a universal approximation result showing that this exact model class remains universal on arbitrary domains. FLASH-MAX reaches sub-1% relative validation error from about 1K sparse pointwise observations in seconds, all while maintaining a zero PDE residual, and keeps single-digit errors even for only 100 observations sampled from 3D space. These results suggest that moving governing structure from the loss into the hypothesis class can dramatically improve the trade-off between precision and optimization speed in scientific machine learning.

## Project Page

See more at [https://ddegenaro.github.io/flash-max/](https://ddegenaro.github.io/flash-max/)!
