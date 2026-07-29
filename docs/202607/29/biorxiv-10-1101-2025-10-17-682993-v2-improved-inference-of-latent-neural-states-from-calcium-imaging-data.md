---
title: Improved inference of latent neural states from calcium imaging data
title_zh: 改进的钙成像数据神经潜在状态推断
authors: "Keeley, S., Zoltowski, D. M., Charles, A., Pillow, J. W."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.17.682993v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 改进钙成像数据的潜在神经状态推断
tldr: 钙成像数据分析常使用潜在变量模型，但传统方法或对荧光去卷积、或采用高斯观测假设，导致不精确。本文在HMM、GPFA及动态系统模型中引入更符合生理的观测模型，即通过泊松发放和自回归钙动力学直接连接荧光与潜在状态。该方法在生物物理仿真和实验数据上均提升了潜在变量推断和模型拟合的准确性。此工作为群体钙成像数据提供了更可靠的潜在结构分析工具。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1012, \"height\": 371, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1486, \"height\": 486, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1457, \"height\": 713, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1482, \"height\": 539, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1480, \"height\": 512, \"label\": \"Figure\"}]"
motivation: 现有潜在变量模型处理钙成像数据时，观测假设不准确，影响推断精度，亟需直接建模荧光信号与潜在神经活动的关系。
method: 在HMM、GPFA及动态系统模型中嵌入泊松发放-自回归钙动力学观测模型，实现端到端的潜在状态推断。
result: 在生物物理仿真和实验钙成像数据上，该方法相比传统去卷积或高斯假设方法，显著改进了潜在状态和动力学参数的估计。
conclusion: 该模型更灵活且准确，可广泛适用于群体钙成像数据的潜在变量分析。
---

## 摘要
钙成像是记录神经群体活动的标准方法，因为它能够同时记录数百到数千个个体体细胞信号。因此，钙成像记录是群体水平潜在变量分析的主要候选对象，例如使用高斯过程因子分析（GPFA）、隐马尔可夫模型（HMMs）和潜在动态系统等模型。然而，这些模型主要是为电生理测量中的脉冲活动开发和优化的。为了将这些模型应用于钙成像记录的钙信号，通常要么对每个神经元的荧光时间序列进行反卷积以近似脉冲事件，要么在高斯观测假设下直接分析。前一种方法虽然能够直接应用为脉冲数据开发的潜在变量方法，但受限于钙成像中脉冲估计的不精确性。此外，孤立的脉冲在荧光信号中可能无法检测到，从而增加了额外的不确定性。将观测到的荧光与潜在变量直接关联的更直接模型能够解释这些不确定性来源。在这里，我们开发了准确且易于处理的模型，用于从钙成像数据中表征神经群体活动的潜在结构。我们提出通过一个由潜在泊松脉冲和自回归钙动力学组成的钙成像观测模型来增强HMM、GPFA和动态系统模型。重要的是，该模型既更灵活，又与拟合神经动态潜在模型的标准方法直接兼容。我们证明，使用这种更准确的钙成像观测模型改进了潜在变量推断和模型拟合，无论是在使用最先进的生物物理模拟生成的钙成像观测数据上，还是在实验环境中记录的成像数据上。我们期望所开发的方法能够广泛适用于群体钙成像数据的多种不同分析。

## Abstract
Calcium imaging (CI) is a standard method for recording neural population activity, as it enables simultaneous recording of hundreds-to-thousands of individual somatic signals. Accordingly, CI recordings are prime candidates for population-level latent variable analyses, for example, using models such as Gaussian Process Factor Analysis (GPFA), hidden Markov models (HMMs), and latent dynamical systems. However, these models have been primarily developed and fine-tuned for electrophysiological measurements of spiking activity. To adapt these models for use with the calcium signals recorded with CI, per-neuron fluorescence time-traces are typically either de-convolved to approximate spiking events or analyzed directly under Gaussian observation assumptions. The former approach, while enabling the direct application of latent variable methods developed for spiking data, suffers from the imprecise nature of spike estimation from CI. Moreover, isolated spikes can be undetectable in the fluorescence signal, creating additional uncertainty. A more direct model linking observed fluorescence to latent variables would account for these sources of uncertainty. Here, we develop accurate and tractable models for characterizing the latent structure of neural population activity from CI data. We propose to augment HMM, GPFA, and dynamical systems models with a CI observation model that consists of latent Poisson spiking and autoregressive calcium dynamics. Importantly, this model is both more flexible and directly compatible with standard methods for fitting latent models of neural dynamics. We demonstrate that using this more accurate CI observation model improves latent variable inference and model fitting on both CI observations generated using state-of-the-art biophysical simulations and imaging data recorded in an experimental setting. We expect the developed methods to be widely applicable to many different analyses of population CI data.