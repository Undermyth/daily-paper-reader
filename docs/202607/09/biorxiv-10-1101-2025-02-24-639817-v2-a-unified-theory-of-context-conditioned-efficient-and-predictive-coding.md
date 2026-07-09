---
title: A unified theory of context-conditioned efficient and predictive coding
title_zh: 上下文条件化高效编码与预测编码的统一理论
authors: "Tavoni, G."
date: 2026-07-06
pdf: "https://www.biorxiv.org/content/10.1101/2025.02.24.639817v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 上下文条件下的高效与预测编码统一理论
tldr: 感觉处理受其他感官、动作和行为上下文影响。该研究统一了高效编码与预测编码理论，证明上下文条件下的高效编码等价于预测编码：上下文信号提供期望，局部神经元编码偏差，递归交互白化残差。该框架解释了跨模态抑制和多模态感受野等现象，为分布式神经系统的上下文依赖编码提供理论基石。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-001.webp\", \"caption\": \"\", \"page\": 6, \"index\": 1, \"width\": 981, \"height\": 426}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-002.webp\", \"caption\": \"\", \"page\": 6, \"index\": 2, \"width\": 983, \"height\": 434}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-003.webp\", \"caption\": \"\", \"page\": 15, \"index\": 3, \"width\": 2225, \"height\": 1653}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-004.webp\", \"caption\": \"\", \"page\": 15, \"index\": 4, \"width\": 2220, \"height\": 785}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-005.webp\", \"caption\": \"\", \"page\": 15, \"index\": 5, \"width\": 454, \"height\": 411}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-006.webp\", \"caption\": \"\", \"page\": 15, \"index\": 6, \"width\": 462, \"height\": 431}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-007.webp\", \"caption\": \"\", \"page\": 15, \"index\": 7, \"width\": 461, \"height\": 431}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-008.webp\", \"caption\": \"\", \"page\": 18, \"index\": 8, \"width\": 2166, \"height\": 1390}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-009.webp\", \"caption\": \"\", \"page\": 20, \"index\": 9, \"width\": 2115, \"height\": 1719}]"
motivation: 现有编码理论多假设单模态孤立处理，但现实中感觉输入受多模态上下文调控，缺乏统一理论解释这种现象。
method: 通过数学推导建立上下文条件高效编码与预测编码的等价性，将编码目标映射为可解释的神经算法（上下文期望、偏差编码、残差白化）。
result: 理论统一了跨模态抑制、多模态感受野等实验现象，并恢复经典单模态高效编码特例。
conclusion: 该框架揭示了分布式神经系统中上下文塑造局部表征的普适原理，为理解多模态整合和预测处理提供了统一计算基础。
---

## 摘要
感觉处理并非孤立发生：在给定感觉模态中，神经元所表征的内容受到来自其他感觉、动作和行为背景信号的塑造。这种背景依赖性给神经编码理论提出了一个根本问题：神经回路如何在利用大脑其他部位可用信息的同时高效编码其局部输入？本文提出了一种高效编码与预测编码的统一理论，展示了多模态背景信息如何优化局部感觉回路内的表征。我们通过解析证明，高效编码解决方案可映射为一种可解释的神经算法：背景信号为局部回路提供关于感觉输入的预期，局部神经元编码与这些预期的偏差，而循环交互对残差信号进行白化。这一结果确立了上下文条件化高效编码与预测编码之间的数学等价性，揭示了预测性计算可从由背景引导的高效输入压缩中涌现。所得框架既不同于单一模态内的经典冗余降低，也不同于层次贝叶斯推断。该理论解释并统一了多种实验现象，包括对预期输入的跨模态反应抑制，以及跨感觉运动、视听、视觉-嗅觉和听觉-体感回路的多模态感受野，同时将经典单模态编码效应作为极限情况恢复。通过将编码目标、回路机制和实验观测现象纳入单一分析框架，本研究为理解分布式神经系统如何利用背景塑造局部表征提供了原理性基础。

## Abstract
Sensory processing does not occur in isolation: what neurons represent in a given sensory modality is shaped by signals from other senses, actions, and behavioral context. This context dependence raises a fundamental question for theories of neural coding: how can circuits efficiently encode their local input while using information available elsewhere in the brain? Here we develop a unified theory of efficient and predictive coding that shows how multimodal contextual information can optimize representations within a local sensory circuit. We demonstrate analytically that the efficient-coding solution maps onto an interpretable neural algorithm: contextual signals provide expectations about the sensory input to the local circuit, local neurons encode deviations from those expectations, and recurrent interactions whiten the residual signals. This result establishes a mathematical equivalence between context-conditioned efficient coding and predictive coding, revealing that predictive computations can emerge from efficient input compression guided by context. The resulting framework is distinct from both classical redundancy reduction within a single modality and hierarchical Bayesian inference. The theory explains and unifies diverse experimental phenomena, including cross-modal suppression of responses to predicted inputs and multimodal receptive fields across sensorimotor, audiovisual, visual-olfactory, and auditory-somatosensory circuits, while recovering classical unimodal coding effects as limiting cases. By linking coding objectives, circuit mechanisms, and experimentally observed phenomena within a single analytical framework, this work provides a principled foundation for understanding how distributed neural systems use context to shape local representations.