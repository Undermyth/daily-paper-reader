---
title: Improved inference of latent neural states from calcium imaging data
title_zh: 改进的钙成像数据中潜在神经状态推断方法
authors: "Keeley, S., Zoltowski, D. M., Charles, A., Pillow, J. W."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.17.682993v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 改进钙成像数据的潜在状态推断方法
tldr: 钙成像记录的神经群体活动缺乏适配的潜在变量模型。现有方法通过去卷积估计尖峰或使用高斯观测假设，精度不足。本文提出在HMM、GPFA和动态系统中加入包含泊松尖峰和自回归钙动力学的观测模型。在模拟和实验数据上，该方法改进了潜在变量推断和模型拟合，有望广泛用于群体钙成像数据分析。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1012, \"height\": 371, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1486, \"height\": 486, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1457, \"height\": 713, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1482, \"height\": 539, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1480, \"height\": 512, \"label\": \"Figure\"}]"
motivation: 现有潜在变量模型主要针对尖峰活动设计，直接用于钙成像数据时精度低，需要更精确的观测模型。
method: 在HMM、GPFA和动态系统模型中融入包含泊松尖峰和自回归钙动力学的钙成像观测模型。
result: 在生物物理模拟和实验数据上，该方法提升了潜在状态推断和模型拟合的准确性。
conclusion: 提出的钙成像观测模型可广泛用于群体钙成像数据的潜在变量分析。
---

## 摘要
钙成像（CI）是记录神经群体活动的标准方法，因为它能同时记录数百到数千个独立胞体信号。因此，CI记录是群体水平潜在变量分析的理想候选，例如使用高斯过程因子分析（GPFA）、隐马尔可夫模型（HMM）和潜在动力系统等模型。然而，这些模型主要针对电生理尖峰活动测量而开发和优化。为了将这些模型应用于CI记录的钙信号，通常需要对每个神经元的荧光时间序列进行去卷积以近似尖峰事件，或者在高斯观测假设下直接分析。前一种方法虽然能够直接应用为尖峰数据开发的潜在变量方法，但受到从CI估计尖峰的不精确性的影响。此外，孤立的尖峰在荧光信号中可能无法检测，带来额外的不确定性。一个更直接的将观测荧光与潜在变量联系起来的模型将考虑这些不确定性来源。在此，我们开发了准确且易于处理的模型，用于从CI数据中表征神经群体活动的潜在结构。我们提出在HMM、GPFA和动力系统模型中增加一个CI观测模型，该模型由潜在泊松尖峰和自回归钙动力学组成。重要的是，该模型既更灵活，又与拟合神经动力学潜在模型的标准方法直接兼容。我们证明，使用这种更准确的CI观测模型，能够改善对使用最先进生物物理模拟生成的CI观测以及实验环境下记录的成像数据的潜在变量推断和模型拟合。我们期望所开发的方法能够广泛应用于群体CI数据的多种不同分析。

## Abstract
Calcium imaging (CI) is a standard method for recording neural population activity, as it enables simultaneous recording of hundreds-to-thousands of individual somatic signals. Accordingly, CI recordings are prime candidates for population-level latent variable analyses, for example, using models such as Gaussian Process Factor Analysis (GPFA), hidden Markov models (HMMs), and latent dynamical systems. However, these models have been primarily developed and fine-tuned for electrophysiological measurements of spiking activity. To adapt these models for use with the calcium signals recorded with CI, per-neuron fluorescence time-traces are typically either de-convolved to approximate spiking events or analyzed directly under Gaussian observation assumptions. The former approach, while enabling the direct application of latent variable methods developed for spiking data, suffers from the imprecise nature of spike estimation from CI. Moreover, isolated spikes can be undetectable in the fluorescence signal, creating additional uncertainty. A more direct model linking observed fluorescence to latent variables would account for these sources of uncertainty. Here, we develop accurate and tractable models for characterizing the latent structure of neural population activity from CI data. We propose to augment HMM, GPFA, and dynamical systems models with a CI observation model that consists of latent Poisson spiking and autoregressive calcium dynamics. Importantly, this model is both more flexible and directly compatible with standard methods for fitting latent models of neural dynamics. We demonstrate that using this more accurate CI observation model improves latent variable inference and model fitting on both CI observations generated using state-of-the-art biophysical simulations and imaging data recorded in an experimental setting. We expect the developed methods to be widely applicable to many different analyses of population CI data.