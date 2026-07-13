---
title: A unified theory of context-conditioned efficient and predictive coding
title_zh: 统一理论下的情境条件性高效编码与预测编码
authors: "Tavoni, G."
date: 2026-07-06
pdf: "https://www.biorxiv.org/content/10.1101/2025.02.24.639817v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 统一的高效与预测编码理论，整合多模态上下文
tldr: 感觉处理受多模态上下文影响，但缺乏统一编码理论。本文提出一个统一框架，证明上下文条件高效编码等价于预测编码：上下文提供输入期望，局部神经元编码预测误差，循环连接白化残差。该理论统一了跨模态抑制和多模态感受野等实验现象，并恢复经典高效编码作为极限情况。为理解大脑如何利用上下文优化局部表示提供了数学基础。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1198, \"height\": 1457, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1358, \"height\": 1303, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1431, \"height\": 1571, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1493, \"height\": 977, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-02-24-639817-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1657, \"height\": 1220, \"label\": \"Figure\"}]"
motivation: 在感觉电路中，上下文信息如何优化局部表示缺乏统一理论。
method: 通过数学分析建立上下文条件高效编码和预测编码的等价性，推导出可解释的神经算法。
result: 揭示上下文信号提供期望、局部编码偏差、循环白化残差的机制，统一多种实验现象。
conclusion: 该理论连接了编码目标、电路机制和实验现象，为上下文依赖的神经编码提供了原则性框架。
---

## 摘要
感官处理并非孤立进行：在特定感官模态中，神经元所表征的内容受到来自其他感官、动作和行为情境信号的塑造。这种情境依赖性为神经编码理论提出了一个基本问题：电路如何在利用大脑其他部位可用信息的同时，高效编码其局部输入？在此，我们发展了一个高效编码与预测编码的统一理论，展示了多模态情境信息如何优化局部感觉电路内的表征。我们通过分析证明，高效编码解可映射到一种可解释的神经算法：情境信号提供关于局部电路感官输入的预期，局部神经元编码与这些预期的偏差，而递归交互则对残差信号进行白化。这一结果建立了情境条件性高效编码与预测编码之间的数学等价性，揭示了预测计算可从由情境引导的高效输入压缩中涌现。所得的框架既不同于单一模态内的经典冗余减少，也不同于分层贝叶斯推断。该理论解释并统一了多种实验现象，包括跨模态抑制对预测输入的响应，以及感觉运动、视听、视觉-嗅觉和听觉-体感电路中的多模态感受野，同时将经典单模态编码效应恢复为极限情况。通过在一个分析框架内连接编码目标、电路机制和实验观察到的现象，这项工作为理解分布式神经系统如何利用情境塑造局部表征提供了原则性基础。

## Abstract
Sensory processing does not occur in isolation: what neurons represent in a given sensory modality is shaped by signals from other senses, actions, and behavioral context. This context dependence raises a fundamental question for theories of neural coding: how can circuits efficiently encode their local input while using information available elsewhere in the brain? Here we develop a unified theory of efficient and predictive coding that shows how multimodal contextual information can optimize representations within a local sensory circuit. We demonstrate analytically that the efficient-coding solution maps onto an interpretable neural algorithm: contextual signals provide expectations about the sensory input to the local circuit, local neurons encode deviations from those expectations, and recurrent interactions whiten the residual signals. This result establishes a mathematical equivalence between context-conditioned efficient coding and predictive coding, revealing that predictive computations can emerge from efficient input compression guided by context. The resulting framework is distinct from both classical redundancy reduction within a single modality and hierarchical Bayesian inference. The theory explains and unifies diverse experimental phenomena, including cross-modal suppression of responses to predicted inputs and multimodal receptive fields across sensorimotor, audiovisual, visual-olfactory, and auditory-somatosensory circuits, while recovering classical unimodal coding effects as limiting cases. By linking coding objectives, circuit mechanisms, and experimentally observed phenomena within a single analytical framework, this work provides a principled foundation for understanding how distributed neural systems use context to shape local representations.