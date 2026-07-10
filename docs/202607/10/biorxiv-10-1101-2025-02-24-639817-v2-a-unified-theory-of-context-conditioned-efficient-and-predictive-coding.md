---
title: A unified theory of context-conditioned efficient and predictive coding
title_zh: 上下文条件的高效与预测编码的统一理论
authors: "Tavoni, G."
date: 2026-07-06
pdf: "https://www.biorxiv.org/content/10.1101/2025.02.24.639817v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 上下文条件下的高效与预测编码统一理论
tldr: 感觉处理受多模态语境影响，但缺乏统一理论。本文提出上下文条件化高效编码理论，数学证明其与预测编码等价。语境提供输入期望，局部神经元编码偏差，循环相互作用白化残差信号。该框架统一解释了跨模态抑制和多模态感受野等现象，为分布式神经系统如何利用语境优化局部表征提供了原理性基础。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1198, \"height\": 1457, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1358, \"height\": 1303, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1431, \"height\": 1571, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1493, \"height\": 977, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1657, \"height\": 1220, \"label\": \"Figure\"}]"
motivation: 现有编码理论未考虑多模态语境影响，需要统一解释跨模态交互的神经机制。
method: 通过数学推导建立上下文条件化高效编码与预测编码的等价性，提出局部电路利用语境期望编码预测误差并白化残差。
result: 该理论统一解释了跨模态抑制、多模态感受野等现象，并恢复经典单模态编码作为特例。
conclusion: 为理解分布式神经系统中语境如何塑造局部表征提供了统一理论框架。
---

## 摘要
感觉处理并非孤立发生：神经元在特定感觉模态中所代表的内容，受其他感官、动作和行为背景信号的塑造。这种背景依赖性对神经编码理论提出了一个基本问题：电路如何高效地编码其局部输入，同时利用大脑其他部位可用的信息？在这里，我们发展了一个统一的高效和预测编码理论，展示了多模态背景信息如何优化局部感觉电路内的表征。我们分析性地证明，高效编码解决方案映射到一个可解释的神经算法：背景信号为局部电路提供关于感觉输入的期望，局部神经元编码与这些期望的偏差，而循环相互作用对残差信号进行白化。这一结果建立了上下文条件高效编码与预测编码之间的数学等价性，揭示预测计算可以从由背景引导的高效输入压缩中涌现。由此产生的框架既不同于单一模态内的经典冗余减少，也不同于分层贝叶斯推理。该理论解释并统一了多种实验现象，包括对预测输入的跨模态反应抑制以及跨感觉运动、视听、视觉-嗅觉和听觉-体感电路的多模态感受野，同时将经典的单模态编码效应作为极限情况恢复。通过在一个单一的分析框架内将编码目标、电路机制和实验观察到的现象联系起来，这项工作为理解分布式神经系统如何利用背景塑造局部表征提供了原则性的基础。

## Abstract
Sensory processing does not occur in isolation: what neurons represent in a given sensory modality is shaped by signals from other senses, actions, and behavioral context. This context dependence raises a fundamental question for theories of neural coding: how can circuits efficiently encode their local input while using information available elsewhere in the brain? Here we develop a unified theory of efficient and predictive coding that shows how multimodal contextual information can optimize representations within a local sensory circuit. We demonstrate analytically that the efficient-coding solution maps onto an interpretable neural algorithm: contextual signals provide expectations about the sensory input to the local circuit, local neurons encode deviations from those expectations, and recurrent interactions whiten the residual signals. This result establishes a mathematical equivalence between context-conditioned efficient coding and predictive coding, revealing that predictive computations can emerge from efficient input compression guided by context. The resulting framework is distinct from both classical redundancy reduction within a single modality and hierarchical Bayesian inference. The theory explains and unifies diverse experimental phenomena, including cross-modal suppression of responses to predicted inputs and multimodal receptive fields across sensorimotor, audiovisual, visual-olfactory, and auditory-somatosensory circuits, while recovering classical unimodal coding effects as limiting cases. By linking coding objectives, circuit mechanisms, and experimentally observed phenomena within a single analytical framework, this work provides a principled foundation for understanding how distributed neural systems use context to shape local representations.