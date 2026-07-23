---
title: From Hodgkin-Huxley to Pretrained Neural Inference AI
title_zh: 从Hodgkin-Huxley到预训练神经推理AI
authors: "Zhang, Y., Han, D., Lv, Z., Ren, F., Wang, Y., Yang, Y., Li, D., Gu, Y."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.13.738120v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 利用生物物理模拟预训练人工神经网络进行神经推断
tldr: 高密度探针记录大量神经元，但单神经元身份解析困难。本文利用生物物理模拟生成大规模合成数据，预训练神经网络实现零样本跨区域、跨物种泛化，无需真实数据即可准确推断单神经元活动和细胞类型。该方法还发现传统方法遗漏的弱活跃神经元，解决了小鼠初级视觉皮层眼优势的争议。模拟成为连接理论与实验的桥梁。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1821, \"height\": 1554, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1770, \"height\": 1611, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1786, \"height\": 1724, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1757, \"height\": 1478, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1790, \"height\": 1222, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1811, \"height\": 2222, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1756, \"height\": 1386, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1776, \"height\": 671, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1634, \"height\": 1139, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1498, \"height\": 1173, \"label\": \"Figure\"}]"
motivation: 现有方法难以从群体电信号解析单神经元身份，而生物物理模拟虽精确但未有效用于脑信号解读。
method: 基于霍奇金-赫胥黎模型生成大规模合成群体电信号数据，预训练神经网络进行零样本推理。
result: 网络零样本泛化至多脑区、范式和物种，准确推断单神经元活动并发现传统方法忽略的弱活跃神经元。
conclusion: 生物物理模拟可作为参考标准，通过数据驱动推理弥合理论与实验的鸿沟。
---

## 摘要
高密度探针可同时记录数千个神经元的信号，但解析单个神经元身份仍然是一个不适定逆问题。尽管详细的模拟能精确表征生物物理正向过程，但其在解释脑信号方面的效用仍不明确。在此，我们表明群体神经元电信号的生物物理模拟可充当理论与实验之间的有效桥梁。通过仅在大规模合成数据上预训练人工神经网络，我们展示了跨不同脑区、实验范式及物种的稳健零样本泛化能力，从而在未接触真实数据的情况下实现对单个单元活动和细胞类型特性的准确推断。此外，我们的框架揭示了一类数量可观的功能上胜任但弱活跃的神经元群体，这些神经元系统性地被传统启发式方法所掩盖，从而解决了关于小鼠初级视皮层眼优势的一个长期存在的矛盾。这些发现确立了生物物理模拟作为参考标准，通过数据驱动力推断弥合了理论理解与实验观察之间的差距。

## Abstract
High-density probes record from thousands of neurons simultaneously, yet resolving single-neuron identity remains an ill-posed inverse problem. While detailed simulations precisely characterize the biophysical forward process, their utility for interpreting brain signal remains unclear. Here we show that biophysical simulations of population neuronal electrical signals serve as an effective bridge between theory and experiment. By pre-training artificial neural networks exclusively on large-scale synthetic data, we demonstrate robust zero-shot generalization across diverse brain regions, experimental paradigms and species, enabling the accurate inference of single-unit activities and cell-type properties without exposure to real data. Furthermore, uncovering a substantial population of functionally competent but weakly active neurons systematically obscured by conventional heuristics, our framework resolves a long-standing discrepancy regarding ocular dominance in mouse primary visual cortex. These findings establish biophysical simulations as a reference standard, bridging the gap between theoretical understanding and experimental observation through data-driven inference.