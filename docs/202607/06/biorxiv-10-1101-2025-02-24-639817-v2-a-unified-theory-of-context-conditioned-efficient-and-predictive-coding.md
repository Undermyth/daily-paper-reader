---
title: A unified theory of context-conditioned efficient and predictive coding
title_zh: 上下文条件化高效编码与预测编码的统一理论
authors: "Tavoni, G."
date: 2026-07-06
pdf: "https://www.biorxiv.org/content/10.1101/2025.02.24.639817v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 上下文条件下高效与预测编码的统一理论
tldr: 感官处理受上下文强烈影响，但缺乏统一理论。本文提出一个理论框架，证明上下文条件下的高效编码与预测编码数学等价，即局部神经元编码输入与上下文预期之间的残差，并通过循环交互白化残差信号。该框架统一解释了跨模态抑制和多模态感受野等多种实验现象，并将经典单模态高效编码作为极限情况。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有编码理论无法解释上下文如何塑造感官表征，需要统一框架连接编码目标、电路机制和实验现象。
method: 通过理论分析建立上下文条件下的高效编码与预测编码的数学等价性，推导出可解释的神经算法。
result: 该理论统一了跨模态抑制、多模态感受野等实验现象，并恢复经典单模态编码效应。
conclusion: 提供了原则性基础，理解分布式神经系统中上下文如何优化局部表征。
---

## 摘要
感觉处理并非孤立发生：在给定感觉模态中，神经元所表征的内容受到来自其他感觉、动作和行为背景信号的影响。这种上下文依赖性对神经编码理论提出了一个基本问题：电路如何在利用大脑其他信息的同时，高效地编码其局部输入？在此，我们发展了一个统一的效率和预测编码理论，展示了多模态上下文信息如何优化局部感觉电路内的表征。我们分析表明，高效编码解决方案可映射为一个可解释的神经算法：上下文信号提供对局部电路感觉输入的预期，局部神经元编码与这些预期的偏差，而循环交互则对残余信号进行白化。这一结果建立了上下文条件化高效编码与预测编码之间的数学等价性，揭示了预测计算可以从上下文引导的高效输入压缩中涌现。由此产生的框架既不同于单一模态内的经典冗余减少，也不同于分层贝叶斯推理。该理论解释并统一了多样化的实验现象，包括对预测输入反应的跨模态抑制，以及跨感觉运动、视听、视觉-嗅觉和听觉-体感回路的多模态感受野，同时将经典单模态编码效应恢复为极限情况。通过将编码目标、回路机制和实验观察现象联系在一个统一的分析框架内，这项工作为理解分布式神经系统如何利用上下文塑造局部表征提供了原则性基础。

## Abstract
Sensory processing does not occur in isolation: what neurons represent in a given sensory modality is shaped by signals from other senses, actions, and behavioral context. This context dependence raises a fundamental question for theories of neural coding: how can circuits efficiently encode their local input while using information available elsewhere in the brain? Here we develop a unified theory of efficient and predictive coding that shows how multimodal contextual information can optimize representations within a local sensory circuit. We demonstrate analytically that the efficient-coding solution maps onto an interpretable neural algorithm: contextual signals provide expectations about the sensory input to the local circuit, local neurons encode deviations from those expectations, and recurrent interactions whiten the residual signals. This result establishes a mathematical equivalence between context-conditioned efficient coding and predictive coding, revealing that predictive computations can emerge from efficient input compression guided by context. The resulting framework is distinct from both classical redundancy reduction within a single modality and hierarchical Bayesian inference. The theory explains and unifies diverse experimental phenomena, including cross-modal suppression of responses to predicted inputs and multimodal receptive fields across sensorimotor, audiovisual, visual-olfactory, and auditory-somatosensory circuits, while recovering classical unimodal coding effects as limiting cases. By linking coding objectives, circuit mechanisms, and experimentally observed phenomena within a single analytical framework, this work provides a principled foundation for understanding how distributed neural systems use context to shape local representations.