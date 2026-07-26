---
title: Improved inference of latent neural states from calcium imaging data
title_zh: 从钙成像数据改进潜在神经状态的推断
authors: "Keeley, S., Zoltowski, D. M., Charles, A., Pillow, J. W."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.17.682993v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 钙成像数据的潜在神经状态推断
tldr: 钙成像数据分析常采用去卷积或高斯假设，但精度有限。本文在HMM、GPFA和动态系统中引入泊松发放与自回归钙动力学观测模型，直接建模荧光信号。在生物物理仿真和实验数据上，该方法改善了潜在状态推断和模型拟合。该模型可广泛用于群体钙成像数据的潜在结构分析。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1012, \"height\": 371, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1486, \"height\": 486, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1457, \"height\": 713, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1482, \"height\": 539, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1480, \"height\": 512, \"label\": \"Figure\"}]"
motivation: 现有钙成像数据建模方法不准确，缺乏直接从荧光信号推断潜在状态的概率模型。
method: 在HMM、GPFA和动态系统中增加泊松发放与自回归钙动力学的观测模型，实现端到端推断。
result: 在仿真和实验数据上，新模型比传统去卷积方法更准确地恢复了潜在神经状态和动态结构。
conclusion: 提出的观测模型提升了钙成像群体记录中潜在变量分析的准确性和可靠性。
---

## 摘要
钙成像是记录神经群体活动的标准方法，因为它能够同时记录数百到数千个个体体细胞信号。因此，钙成像记录是群体水平潜在变量分析的主要候选对象，例如使用高斯过程因子分析、隐马尔可夫模型和潜在动力系统等模型。然而，这些模型主要是针对放电活动的电生理测量而开发和优化的。为了将这些模型应用于钙成像记录的钙信号，通常会对每个神经元的荧光时间序列进行解卷积以近似放电事件，或在高斯观察假设下直接分析。前一种方法虽然能够直接应用为放电数据开发的潜在变量方法，但受限于从钙成像中估计放电的不精确性。此外，孤立的放电在荧光信号中可能无法检测到，从而增加了额外的不确定性。将观察到的荧光与潜在变量直接联系的更直接模型可以解释这些不确定性来源。在此，我们开发了准确且易处理的模型，用于从钙成像数据描述神经群体活动的潜在结构。我们提出用包含潜在泊松放电和自回归钙动力学的钙成像观察模型来增强HMM、GPFA和动力系统模型。重要的是，该模型既更灵活，又与拟合神经动力学潜在模型的标准方法直接兼容。我们证明，使用这种更准确的钙成像观测模型可以改进对使用最先进生物物理模拟生成的钙成像观察以及在实验环境中记录的成像数据的潜在变量推断和模型拟合。我们期望所开发的方法能够广泛应用于群体钙成像数据的多种不同分析。

## Abstract
Calcium imaging (CI) is a standard method for recording neural population activity, as it enables simultaneous recording of hundreds-to-thousands of individual somatic signals. Accordingly, CI recordings are prime candidates for population-level latent variable analyses, for example, using models such as Gaussian Process Factor Analysis (GPFA), hidden Markov models (HMMs), and latent dynamical systems. However, these models have been primarily developed and fine-tuned for electrophysiological measurements of spiking activity. To adapt these models for use with the calcium signals recorded with CI, per-neuron fluorescence time-traces are typically either de-convolved to approximate spiking events or analyzed directly under Gaussian observation assumptions. The former approach, while enabling the direct application of latent variable methods developed for spiking data, suffers from the imprecise nature of spike estimation from CI. Moreover, isolated spikes can be undetectable in the fluorescence signal, creating additional uncertainty. A more direct model linking observed fluorescence to latent variables would account for these sources of uncertainty. Here, we develop accurate and tractable models for characterizing the latent structure of neural population activity from CI data. We propose to augment HMM, GPFA, and dynamical systems models with a CI observation model that consists of latent Poisson spiking and autoregressive calcium dynamics. Importantly, this model is both more flexible and directly compatible with standard methods for fitting latent models of neural dynamics. We demonstrate that using this more accurate CI observation model improves latent variable inference and model fitting on both CI observations generated using state-of-the-art biophysical simulations and imaging data recorded in an experimental setting. We expect the developed methods to be widely applicable to many different analyses of population CI data.