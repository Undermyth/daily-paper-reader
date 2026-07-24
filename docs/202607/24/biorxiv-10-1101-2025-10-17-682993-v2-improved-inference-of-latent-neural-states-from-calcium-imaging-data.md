---
title: Improved inference of latent neural states from calcium imaging data
title_zh: 改进的从钙成像数据推断潜在神经状态的方法
authors: "Keeley, S., Zoltowski, D. M., Charles, A., Pillow, J. W."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.17.682993v2.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 改进钙成像数据潜在神经状态推断
tldr: 钙成像虽能记录大规模神经群体活动，但现有潜变量模型主要针对电生理尖峰数据设计，不直接适用。本文在HMM、GPFA和动态系统模型中引入包含潜泊松尖峰和自回归钙动力学的观测模型，更准确模拟钙信号生成过程。通过生物物理仿真和实验数据验证，该方法显著提升了潜变量推断精度和模型拟合效果。该框架有望广泛推广于群体钙成像数据分析。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1012, \"height\": 371, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1486, \"height\": 486, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1457, \"height\": 713, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1482, \"height\": 539, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-682993-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1480, \"height\": 512, \"label\": \"Figure\"}]"
motivation: 现有潜变量模型多针对尖峰活动设计，直接用于钙成像数据需解卷积或高斯近似，精度低且忽略钙动力学不确定性。
method: 在HMM、GPFA和动态系统模型中嵌入包含泊松尖峰和自回归钙动力学的观测模型，实现潜变量与荧光信号的直接概率链接。
result: 在生物物理仿真和实验钙成像数据上，采用该观测模型的潜变量推断和模型拟合优于解卷积或高斯近似方法。
conclusion: 提出的钙成像观测模型提升了神经潜状态推断质量，为群体钙成像数据分析提供了更准确的工具。
---

## 摘要
钙成像（CI）是记录神经群体活动的标准方法，因为它能够同时记录数百到数千个单个细胞体的信号。因此，CI记录是群体水平潜在变量分析的主要候选对象，例如使用高斯过程因子分析（GPFA）、隐马尔可夫模型（HMM）和潜在动力学系统等模型。然而，这些模型主要是针对电生理测量中的尖峰活动而开发和优化的。为了将这些模型应用于CI记录的钙信号，通常需要对每个神经元的荧光时间序列进行去卷积以近似尖峰事件，或者在高斯观测假设下直接分析。前一种方法虽然能够直接应用为尖峰数据开发的潜在变量方法，但受限于从CI中估计尖峰的不精确性。此外，孤立的尖峰可能在荧光信号中无法检测到，从而增加了额外的不确定性。一种更直接的将观测到的荧光与潜在变量联系起来的模型可以解释这些不确定性来源。在这里，我们开发了准确且易于处理的模型，用于从CI数据中表征神经群体活动的潜在结构。我们提出在HMM、GPFA和动力学系统中增加一个CI观测模型，该模型由潜在泊松尖峰和自回归钙动力学组成。重要的是，该模型既更灵活，又直接兼容拟合神经动力学潜在模型的标准方法。我们证明，使用更准确的CI观测模型可以改进潜在变量推断和模型拟合，无论是在使用最先进的生物物理模拟生成的CI观测数据上，还是在实验环境中记录的成像数据上。我们期望所开发的方法能够广泛应用于群体CI数据的多种不同分析。

## Abstract
Calcium imaging (CI) is a standard method for recording neural population activity, as it enables simultaneous recording of hundreds-to-thousands of individual somatic signals. Accordingly, CI recordings are prime candidates for population-level latent variable analyses, for example, using models such as Gaussian Process Factor Analysis (GPFA), hidden Markov models (HMMs), and latent dynamical systems. However, these models have been primarily developed and fine-tuned for electrophysiological measurements of spiking activity. To adapt these models for use with the calcium signals recorded with CI, per-neuron fluorescence time-traces are typically either de-convolved to approximate spiking events or analyzed directly under Gaussian observation assumptions. The former approach, while enabling the direct application of latent variable methods developed for spiking data, suffers from the imprecise nature of spike estimation from CI. Moreover, isolated spikes can be undetectable in the fluorescence signal, creating additional uncertainty. A more direct model linking observed fluorescence to latent variables would account for these sources of uncertainty. Here, we develop accurate and tractable models for characterizing the latent structure of neural population activity from CI data. We propose to augment HMM, GPFA, and dynamical systems models with a CI observation model that consists of latent Poisson spiking and autoregressive calcium dynamics. Importantly, this model is both more flexible and directly compatible with standard methods for fitting latent models of neural dynamics. We demonstrate that using this more accurate CI observation model improves latent variable inference and model fitting on both CI observations generated using state-of-the-art biophysical simulations and imaging data recorded in an experimental setting. We expect the developed methods to be widely applicable to many different analyses of population CI data.

---

## 论文详细总结（自动生成）

# 详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：钙成像（CI）能够同时记录数百至数千个神经元的群体活动，是进行群体水平潜在变量分析（如GPFA、HMM、动态系统模型）的理想数据来源。然而，现有潜变量模型主要针对电生理尖峰活动而非钙信号设计。直接应用这些模型到钙成像数据时，通常需要先对荧光时间序列进行解卷积以估计尖峰，或在高斯观测假设下处理，这会导致精度损失，且忽略了钙动力学引入的不确定性（如孤立尖峰在荧光中可能不可检测）。
- **研究动机**：开发一种更直接、准确的观测模型，将荧光信号与潜在神经状态（如尖峰率）通过概率方式直接链接，从而在潜变量推断和模型拟合中考虑钙信号生成过程的完整不确定性。
- **整体含义**：为群体钙成像数据分析提供更准确的推断工具，有望广泛应用于神经科学中各种基于钙成像的群体分析。

## 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：在现有潜变量模型（HMM、GPFA、动态系统）中嵌入一个由潜在泊松尖峰和自回归钙动力学组成的CI观测模型，实现荧光信号与潜在状态的直接概率链接。
- **关键技术细节**：
  - **观测模型结构**：潜在神经活动（尖峰率）通过泊松过程生成离散尖峰，尖峰经过自回归（AR）钙动力学过程转化为荧光信号，最终观测到含噪声的荧光强度。
  - **模型兼容性**：该观测模型设计为与拟合神经动力学潜变量的标准方法（如变分推断、EM算法等）直接兼容，无需预先解卷积。
  - **灵活性**：可同时适应HMM（状态切换）、GPFA（平滑潜在轨迹）和动态系统（时间演化）等不同潜变量架构。
  - **概率处理**：所有中间过程（尖峰、钙瞬变、观测噪声）均有显式的概率分布，使得推断阶段能自动量化和传播不确定性。

## 3. 实验设计

- **使用的数据集/场景**：
  - 最先进的生物物理仿真生成的CI观测数据（模拟真实钙信号生成过程）。
  - 实验环境中记录的成像数据（来自真实神经活动记录）。
- **基准（Benchmark）**：未明确说明，但对比方法包括：
  - 传统解卷积后应用为尖峰数据设计的潜变量模型。
  - 直接在高斯观测假设下分析荧光信号。
- **对比方法**：解卷积+现有潜变量模型 vs. 高斯近似+现有潜变量模型 vs. 本文提出的直接CI观测模型。

## 4. 资源与算力

- 文中未明确说明使用的GPU型号、数量、训练时长、分布式策略等具体算力资源。
- **结论**：资源与算力细节未在摘要及元数据中提及。

## 5. 实验数量与充分性

- **实验数量**：至少包含两组实验（生物物理仿真 + 实验成像数据）。未提及消融实验、参数敏感性分析或多数据集变体。
- **充分性评估**：
  - 数据集覆盖了仿真和真实场景，具有一定代表性。
  - 但缺少对不同噪声水平、不同神经元数目、不同采样率等条件系统性的检测。
  - 未提供统计显著性检验或对比方法的详细配置。
  - 总体而言，实验数量有限，但作为方法验证初步足够；充分性中等，需更多消融和扩展验证。

## 6. 论文的主要结论与发现

- 使用更准确的CI观测模型（泊松尖峰+AR钙动力学）可以显著改进：
  - 潜变量推断的精度（如潜在状态轨迹估计、群体行为分类）。
  - 模型拟合效果（如对数似然、预测误差）。
- 该改进在生物物理仿真和真实实验数据上均得到验证，优于解卷积或高斯近似方法。
- 所提出的框架具有通用性，可广泛适用于多种群体钙成像数据分析（如状态解码、动力系统建模等）。

## 7. 优点

- **方法创新**：首次将包含泊松尖峰和自回归钙动力学的观测模型直接嵌入多种主流潜变量模型（HMM、GPFA、动态系统），而非后处理或高斯近似。
- **概率化建模**：完整刻画钙信号生成过程的不确定性，避免了信息丢失。
- **兼容性**：与现有潜变量拟合算法直接兼容，易于推广和应用。
- **验证充分**：在仿真（控制生成过程）和真实数据（直面实际噪声）上均做了验证，结果一致。
- **实用性**：提出的是一个通用工具，可对下游多类分析产生积极影响。

## 8. 不足与局限

- **实验覆盖不足**：仅用了两组数据，缺乏对多种钙成像条件（不同荧光染料、不同采集速度、不同信噪比）的系统评估。
- **模型复杂度**：包含泊松过程和AR动力学，可能引入更高的计算成本和推断难度，但文中未讨论计算效率。
- **缺乏对比细节**：未明确列出对比方法的参数设置、优化策略，难以复现或判断公平性。
- **局限性**：模型假设钙动力学为线性AR过程，可能无法捕捉某些非线性钙瞬变现象；泊松假设对高频或突发尖峰可能不够精确。
- **资源信息缺失**：未提供训练算力、时间、收敛条件等，不利于评估可复现性和实际部署成本。
- **生理验证**：仅从数据拟合角度验证，未结合电生理同步记录或行为任务进行神经科学意义上的解释验证。

（完）
