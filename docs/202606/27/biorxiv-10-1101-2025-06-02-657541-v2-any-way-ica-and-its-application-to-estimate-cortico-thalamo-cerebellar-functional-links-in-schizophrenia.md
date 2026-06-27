---
title: aNy-way ICA and its application to estimate cortico-thalamo-cerebellar functional links in schizophrenia
title_zh: 任意方式独立成分分析（aNy-way ICA）及其在精神分裂症皮层-丘脑-小脑功能连接估计中的应用
authors: "Duan, K., Silva, R. F., Rahaman, M. A., Fu, Z., Liu, J., Kochunov, P., van Erp, T. G. M., Shultz, S., Calhoun, V. D."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.1101/2025.06.02.657541v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 提出任意方式ICA估计精神分裂症脑功能连接
tldr: 多模态数据融合面临尺度与模型阶数差异问题。本文提出aNy-way ICA，通过IVA-G优化加载相关性并同时进行独立ICA，允许不同模态不同阶数。仿真表明其在噪声下准确识别源与加载，优于现有方法。应用于精神分裂症fMRI数据，发现皮层-丘脑-小脑回路功能连接异常，区分患者与对照，并与认知缺陷相关，揭示了“认知共济失调”的神经基础。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有融合方法要求源正交或相同阶数，无法有效处理多模态异质性。
method: 提出aNy-way ICA，结合IVA-G优化加载相关结构和独立ICA优化独立性，支持不同模态不同阶数。
result: 仿真中准确识别源和加载，噪声下优于其他方法；应用发现皮层-丘脑-小脑回路异常连接。
conclusion: 异常连接区分患者并关联认知缺陷，为精神分裂症的认知共济失调假说提供证据。
---

## 摘要
国际和国家生物库研究收集的多模态数据具有不同的尺度和模型阶数，并为疾病机制提供独特且互补的见解。我们提出了一种新颖、灵活且高效的数据融合方法——任意方式独立成分分析（aNy-way ICA）。aNy-way ICA通过高斯独立向量分析（IVA-G）优化连接组件的整个载荷相关结构，同时通过分离的ICA优化独立性，从而融合N维多模态或多域数据。该方法允许不同模态/域具有不同的模型阶数，并在任意数量的模态或域中检测多个连接源，且无需对源施加正交性约束。模拟结果表明，aNy-way ICA能够识别设计源和载荷以及真实的协方差模式，并且与其他方法相比，尤其在噪声条件下具有更高的准确性。将aNy-way ICA应用于精神分裂症4维多域fMRI数据融合，我们识别出一个皮层-丘脑-小脑回路，突显了高阶丘脑核团、视觉皮层、默认模式网络和小脑后叶之间的功能连接。这些功能连接在两个独立数据集中得到复制。高阶丘脑核团、视觉皮层和默认模式网络之间的连接能够区分精神分裂症患者与对照组，并且这种异常连接与发现和复制数据集中的多种认知缺陷相关，表明所识别的皮层-丘脑-小脑回路可能是精神分裂症中“认知共济失调”的基础。

## Abstract
Multimodal data collected by international and national biobanking efforts have distinct scales and model orders and provide unique and complementary insights into disease mechanisms. We propose a novel, flexible and efficient data fusion approach, aNy-way independent component analysis (aNy-way ICA). aNy-way ICA fuses N-way multimodal or multidomain data by optimizing the entire loading correlation structure of linked components via Gaussian independent vector analysis (IVA-G) and simultaneously optimizing independence via separate ICAs. This allows for distinct model orders for different modalities/domains and multiple linked sources detection across any number of modalities or domains without requiring orthogonality constraints on sources. Simulation results demonstrate that aNy-way ICA identifies the designed sources and loadings, as well as the true covariance patterns, with improved accuracy compared to other approaches, especially under noisy conditions. Applying aNy-way ICA to fuse 4D multi-domain fMRI data in schizophrenia, we identified a cortico-thalamo-cerebellar circuit, highlighting the functional linkages among higher order thalamic nuclei, the visual cortex, default mode network, and the posterior lobe of cerebellum. Their function links were replicated in two independent datasets. The connection among higher order thalamic nuclei, the visual cortex, and default mode network discriminates schizophrenia from controls and this aberrant connection is related to multiple cognitive deficits in both discovery and replication datasets, indicating the identified cortico-thalamo-cerebellar circuit may underlie "cognitive dysmetria" in schizophrenia.