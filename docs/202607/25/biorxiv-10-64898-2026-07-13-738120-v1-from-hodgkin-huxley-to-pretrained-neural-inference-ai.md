---
title: From Hodgkin-Huxley to Pretrained Neural Inference AI
title_zh: 从霍奇金-赫胥黎模型到预训练神经推理AI
authors: "Zhang, Y., Han, D., Lv, Z., Ren, F., Wang, Y., Yang, Y., Li, D., Gu, Y."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.13.738120v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 基于生物物理仿真的预训练神经网络用于神经活动推断
tldr: 高密度探针记录的神经元身份解析困难，传统方法依赖真实数据。本文通过生物物理模拟生成大规模合成数据，预训练神经网络实现零样本泛化，准确推断单神经元活动和细胞类型，并发现弱活跃神经元被常规方法掩盖，解决了小鼠V1眼优势长期争议。该工作确立模拟作为参考标准，弥合了理论与实验的鸿沟。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1821, \"height\": 1554, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1770, \"height\": 1611, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1786, \"height\": 1724, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1757, \"height\": 1478, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1790, \"height\": 1222, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1811, \"height\": 2222, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1756, \"height\": 1386, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1776, \"height\": 671, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1634, \"height\": 1139, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1498, \"height\": 1173, \"label\": \"Figure\"}]"
motivation: 高密度探针记录中单神经元身份是不适定逆问题，而生物物理模拟的效用尚不明确。
method: 仅用生物物理模拟生成的大规模合成数据预训练人工神经网络，实现零样本推理。
result: 跨脑区、范式、物种零样本泛化；揭示弱活跃神经元；解决眼优势争议。
conclusion: 生物物理模拟可作为参考标准，通过数据驱动推断连接理论与实验观察。
---

## 摘要
高密度探针可同时记录数千个神经元的活动，但解析单个神经元身份仍是一个不适定逆问题。尽管详细模拟能精确刻画生物物理正向过程，但其在解释脑信号方面的实用性仍不明确。本文表明，群体神经元电信号的生物物理模拟可作为理论与实验之间的有效桥梁。通过仅在大规模合成数据上预训练人工神经网络，我们展示了其在多个脑区、实验范式和物种中的鲁棒零样本泛化能力，从而无需接触真实数据即可精确推断单单元活动及细胞类型特性。此外，我们的框架发现了一类数量可观、功能活跃但通常被传统启发式方法系统性掩盖的弱活动神经元，解决了小鼠初级视皮层中眼优势长期存在的争议。这些发现确立了生物物理模拟作为参考标准，通过数据驱动推断弥合了理论理解与实验观察之间的鸿沟。

## Abstract
High-density probes record from thousands of neurons simultaneously, yet resolving single-neuron identity remains an ill-posed inverse problem. While detailed simulations precisely characterize the biophysical forward process, their utility for interpreting brain signal remains unclear. Here we show that biophysical simulations of population neuronal electrical signals serve as an effective bridge between theory and experiment. By pre-training artificial neural networks exclusively on large-scale synthetic data, we demonstrate robust zero-shot generalization across diverse brain regions, experimental paradigms and species, enabling the accurate inference of single-unit activities and cell-type properties without exposure to real data. Furthermore, uncovering a substantial population of functionally competent but weakly active neurons systematically obscured by conventional heuristics, our framework resolves a long-standing discrepancy regarding ocular dominance in mouse primary visual cortex. These findings establish biophysical simulations as a reference standard, bridging the gap between theoretical understanding and experimental observation through data-driven inference.