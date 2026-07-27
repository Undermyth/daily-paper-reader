---
title: From Hodgkin-Huxley to Pretrained Neural Inference AI
title_zh: 从Hodgkin-Huxley到预训练的神经推理AI
authors: "Zhang, Y., Han, D., Lv, Z., Ren, F., Wang, Y., Yang, Y., Li, D., Gu, Y."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.13.738120v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 计算神经科学中的预训练神经推断
tldr: 高密度探针记录带来单神经元身份辨识难题。研究者利用生物物理模拟生成大规模合成数据，预训练神经网络实现零样本泛化，准确推断单单元活动。该方法还发现了被传统方法遮蔽的弱活跃神经元群，解释了小鼠视觉皮层眼优势矛盾。这确立了模拟数据作为参考标准，桥接理论与实验。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1821, \"height\": 1554, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1770, \"height\": 1611, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1786, \"height\": 1724, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1757, \"height\": 1478, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1790, \"height\": 1222, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1811, \"height\": 2222, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1756, \"height\": 1386, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1776, \"height\": 671, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1634, \"height\": 1139, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1498, \"height\": 1173, \"label\": \"Figure\"}]"
motivation: 解决高密度探针数据中单神经元身份辨识的逆问题，弥合理论与实验的鸿沟。
method: 基于生物物理模拟生成大规模合成数据，预训练人工神经网络进行零样本推断。
result: 实现跨区域、物种的零样本泛化，推断单单元活动；发现被遮蔽的弱活跃神经元群，解决眼优势矛盾。
conclusion: 生物物理模拟可作为参考标准，通过数据驱动推理有效连接理论与实验。
---

## 摘要
高密度探针同时记录数千个神经元的活动，但解析单个神经元的身份仍然是一个不适定的逆问题。虽然详细的模拟精确刻画了生物物理的正向过程，但其在解释脑信号方面的效用仍不明确。在此，我们展示了种群神经元电信号的生物物理模拟可作为理论与实验之间的有效桥梁。通过在大规模合成数据上专门预训练人工神经网络，我们证明了在无需接触真实数据的情况下，该网络能够在不同脑区、实验范式和物种间实现稳健的零样本泛化，从而准确推断单单位活动和细胞类型特性。此外，我们的框架揭示了一类功能健全但活动较弱的神经元群体，这些神经元被传统启发式方法系统地掩盖，从而解决了小鼠初级视觉皮层中关于眼优势的长期争议。这些发现将生物物理模拟确立为参考标准，通过数据驱动的推断弥合了理论理解与实验观察之间的鸿沟。

## Abstract
High-density probes record from thousands of neurons simultaneously, yet resolving single-neuron identity remains an ill-posed inverse problem. While detailed simulations precisely characterize the biophysical forward process, their utility for interpreting brain signal remains unclear. Here we show that biophysical simulations of population neuronal electrical signals serve as an effective bridge between theory and experiment. By pre-training artificial neural networks exclusively on large-scale synthetic data, we demonstrate robust zero-shot generalization across diverse brain regions, experimental paradigms and species, enabling the accurate inference of single-unit activities and cell-type properties without exposure to real data. Furthermore, uncovering a substantial population of functionally competent but weakly active neurons systematically obscured by conventional heuristics, our framework resolves a long-standing discrepancy regarding ocular dominance in mouse primary visual cortex. These findings establish biophysical simulations as a reference standard, bridging the gap between theoretical understanding and experimental observation through data-driven inference.