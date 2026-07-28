---
title: Improved inference of latent neural states from calcium imaging data
title_zh: 从钙成像数据推断潜在神经状态的改进方法
authors: "Keeley, S., Zoltowski, D. M., Charles, A., Pillow, J. W."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.17.682993v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 从钙成像推断潜在神经状态
tldr: 钙成像记录神经群体活动，但现有潜变量模型多针对电生理尖峰信号设计。本文提出将隐层泊松尖峰活动和自回归钙动力学整合到HMM、GPFA和动态系统模型中，构建更准确的钙成像观测模型。通过生物物理仿真和实验数据验证，该方法能改进潜状态推断和模型拟合。预期广泛适用于群体钙成像数据分析。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1012, \"height\": 371, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1486, \"height\": 486, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1457, \"height\": 713, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1482, \"height\": 539, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1480, \"height\": 512, \"label\": \"Figure\"}]"
motivation: 现有潜变量模型不适合钙成像荧光信号，直接反卷积或高斯假设导致精度不足。
method: 在HMM、GPFA和动态系统中嵌入泊松尖峰和自回归钙动力学观测模型。
result: 在仿真和实际数据上，新观测模型提升了潜变量推断和模型拟合性能。
conclusion: 该方法为钙成像群体数据分析提供了更准确灵活的潜变量建模方案。
---

## 摘要
钙成像（CI）是记录神经群体活动的标准方法，因为它能够同时记录数百到数千个单独的胞体信号。因此，CI记录是群体水平潜在变量分析的主要候选对象，例如使用高斯过程因子分析（GPFA）、隐马尔可夫模型（HMM）和潜在动态系统等模型。然而，这些模型主要是针对电生理测量的锋电位活动进行开发和调优的。为了使这些模型适用于CI记录的钙信号，通常需要对每个神经元的荧光时间序列进行去卷积以近似锋电位事件，或在高斯观测假设下直接分析。前一种方法虽然可以直接应用为锋电位数据开发的潜在变量方法，但受限于从CI估计锋电位的不精确性。此外，孤立的锋电位在荧光信号中可能无法检测到，从而增加了额外的不确定性。将观测到的荧光与潜在变量直接联系的模型可以解释这些不确定性来源。在此，我们开发了准确且易处理的模型，用于从CI数据表征神经群体活动的潜在结构。我们提出用包含潜在泊松发放和自回归钙动力学的CI观测模型来增强HMM、GPFA和动态系统模型。重要的是，该模型既更灵活，又直接兼容拟合神经动力学潜在模型的标准方法。我们证明，使用这种更准确的CI观测模型可以改进潜在变量推断和模型拟合，无论是在使用先进生物物理模拟生成的CI观测数据上，还是在实验环境下记录的成像数据上。我们期望所开发的方法能广泛适用于群体CI数据的多种不同分析。

## Abstract
Calcium imaging (CI) is a standard method for recording neural population activity, as it enables simultaneous recording of hundreds-to-thousands of individual somatic signals. Accordingly, CI recordings are prime candidates for population-level latent variable analyses, for example, using models such as Gaussian Process Factor Analysis (GPFA), hidden Markov models (HMMs), and latent dynamical systems. However, these models have been primarily developed and fine-tuned for electrophysiological measurements of spiking activity. To adapt these models for use with the calcium signals recorded with CI, per-neuron fluorescence time-traces are typically either de-convolved to approximate spiking events or analyzed directly under Gaussian observation assumptions. The former approach, while enabling the direct application of latent variable methods developed for spiking data, suffers from the imprecise nature of spike estimation from CI. Moreover, isolated spikes can be undetectable in the fluorescence signal, creating additional uncertainty. A more direct model linking observed fluorescence to latent variables would account for these sources of uncertainty. Here, we develop accurate and tractable models for characterizing the latent structure of neural population activity from CI data. We propose to augment HMM, GPFA, and dynamical systems models with a CI observation model that consists of latent Poisson spiking and autoregressive calcium dynamics. Importantly, this model is both more flexible and directly compatible with standard methods for fitting latent models of neural dynamics. We demonstrate that using this more accurate CI observation model improves latent variable inference and model fitting on both CI observations generated using state-of-the-art biophysical simulations and imaging data recorded in an experimental setting. We expect the developed methods to be widely applicable to many different analyses of population CI data.