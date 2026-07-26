---
title: From Hodgkin-Huxley to Pretrained Neural Inference AI
title_zh: 从霍奇金-赫胥黎到预训练神经推理AI
authors: "Zhang, Y., Han, D., Lv, Z., Ren, F., Wang, Y., Yang, Y., Li, D., Gu, Y."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.13.738120v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 使用生物物理模拟预训练神经网络的计算神经科学方法
tldr: 高密度探针记录海量神经元信号，但单神经元识别仍为病态逆问题。本研究以Hodgkin-Huxley模型为基础，生成大规模生物物理合成数据，预训练神经网络实现零样本泛化，跨脑区、物种准确推断单神经元活动与细胞类型。该方法揭示了被传统启发式规则掩盖的大量功能性弱活跃神经元，并解决了小鼠初级视皮层眼优势的长期争议。该工作确立了生物物理模拟作为参考标准，通过数据驱动推理弥合理论与实验鸿沟。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1821, \"height\": 1554, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1770, \"height\": 1611, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1786, \"height\": 1724, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1757, \"height\": 1478, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1790, \"height\": 1222, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1811, \"height\": 2222, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1756, \"height\": 1386, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1776, \"height\": 671, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1634, \"height\": 1139, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738120-v1/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1498, \"height\": 1173, \"label\": \"Figure\"}]"
motivation: 单神经元身份解析是逆问题，传统方法依赖经验规则，存在偏差且泛化差，需更优理论指导的推理方案。
method: 基于Hodgkin-Huxley模型生成大规模群体电信号合成数据，预训练神经网络进行零样本推断，仅用合成数据学习映射。
result: 实现零样本泛化至多脑区、物种与实验范式，准确推断单神经元活动与细胞类型；发现被传统方法遗漏的弱活跃神经元，解决眼优势争议。
conclusion: 生物物理模拟作为参考标准，结合数据驱动推理，有效连接理论与实验，为神经数据分析提供新范式。
---

## 摘要
高密度探针同时记录数千个神经元，但解析单个神经元身份仍然是一个不适定的逆问题。虽然详细模拟精确描述了生物物理正向过程，但其对解读脑信号的效用仍不明确。在这里，我们展示了群体神经元电信号的生物物理模拟作为理论与实验之间的有效桥梁。通过仅在大型合成数据上预训练人工神经网络，我们展示了跨不同脑区、实验范式和物种的鲁棒零样本泛化能力，从而无需接触真实数据即可准确推断单单元活动和细胞类型特性。此外，我们的框架揭示了大量功能完备但弱活跃的神经元被传统启发式方法系统性掩盖，解决了关于小鼠初级视觉皮层眼优势的长期争议。这些发现确立了生物物理模拟作为参考标准，通过数据驱动推断弥合理论理解与实验观察之间的差距。

## Abstract
High-density probes record from thousands of neurons simultaneously, yet resolving single-neuron identity remains an ill-posed inverse problem. While detailed simulations precisely characterize the biophysical forward process, their utility for interpreting brain signal remains unclear. Here we show that biophysical simulations of population neuronal electrical signals serve as an effective bridge between theory and experiment. By pre-training artificial neural networks exclusively on large-scale synthetic data, we demonstrate robust zero-shot generalization across diverse brain regions, experimental paradigms and species, enabling the accurate inference of single-unit activities and cell-type properties without exposure to real data. Furthermore, uncovering a substantial population of functionally competent but weakly active neurons systematically obscured by conventional heuristics, our framework resolves a long-standing discrepancy regarding ocular dominance in mouse primary visual cortex. These findings establish biophysical simulations as a reference standard, bridging the gap between theoretical understanding and experimental observation through data-driven inference.