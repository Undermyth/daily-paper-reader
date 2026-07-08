---
title: A unified theory of context-conditioned efficient and predictive coding
title_zh: 上下文条件下的高效与预测编码的统一理论
authors: "Tavoni, G."
date: 2026-07-06
pdf: "https://www.biorxiv.org/content/10.1101/2025.02.24.639817v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 计算神经科学中高效与预测编码的统一理论。
tldr: 感官处理离不开跨模态情境，但高效编码理论如何融入情境信息？本文构建了情境依赖高效编码与预测编码的统一理论框架。通过数学推导证明，情境提供对感官输入的期望，局部神经元编码预测误差，递归连接用于白化残差信号，实现输入的高效压缩。该理论统一解释了传感器、视听、视觉-嗅觉和听觉-体感等回路中的跨模态抑制与多模态感受野，经典单模态冗余减少作为其特例。与分层贝叶斯推断不同，该框架具有明确的编码优化目标，为理解分布式系统如何利用情境塑造局部表征提供了第一性原理基础，同时弥合了编码理论与实验现象之间的鸿沟。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有编码理论（单模态冗余减少、分层贝叶斯）未纳入跨模态情境信息，无法解释实际的跨模态抑制等实验现象。
method: 通过数学推导建立情境依赖高效编码与预测编码的等价性，证明情境提供期望、局部编码偏差、递归交互白化残差是最优解。
result: 该框架统一解释了传感器、视听、视觉-嗅觉等回路中的跨模态抑制和多模态感受野，经典单模态编码作为特例出现。
conclusion: 该理论首次将编码目标、电路机制和实验现象统一在一个分析框架内，为情境依赖的神经编码提供了原则性基础。
---

## 摘要
感觉处理并非孤立发生：神经元在某一感觉模态中表征的内容受到来自其他感官、动作和行为背景的信号塑造。这种上下文依赖性对神经编码理论提出了一个基本问题：神经回路如何在利用大脑其他地方可用信息的同时高效地编码其局部输入？在此，我们发展了一个高效编码与预测编码的统一理论，展示了多模态上下文信息如何优化局部感觉回路内的表征。我们通过分析表明，高效编码的解映射到一个可解释的神经算法：上下文信号为局部回路提供关于感觉输入的预期，局部神经元编码与这些预期的偏差，而递归交互则对残差信号进行白化。这一结果建立了上下文条件下高效编码与预测编码之间的数学等价性，揭示了预测计算可以从由上下文引导的高效输入压缩中涌现。由此产生的框架既不同于单一模态内的经典冗余减少，也不同于层级贝叶斯推断。该理论解释并统一了多样的实验现象，包括跨模态抑制对预期输入的反应，以及感觉运动、视听、视觉-嗅觉和听觉-躯体感觉回路中的多模态感受野，同时将经典单模态编码效应作为极限情况恢复。通过将编码目标、回路机制和实验观察到的现象统一在一个分析框架内，这项工作为理解分布式神经系统如何利用上下文塑造局部表征提供了原则性基础。

## Abstract
Sensory processing does not occur in isolation: what neurons represent in a given sensory modality is shaped by signals from other senses, actions, and behavioral context. This context dependence raises a fundamental question for theories of neural coding: how can circuits efficiently encode their local input while using information available elsewhere in the brain? Here we develop a unified theory of efficient and predictive coding that shows how multimodal contextual information can optimize representations within a local sensory circuit. We demonstrate analytically that the efficient-coding solution maps onto an interpretable neural algorithm: contextual signals provide expectations about the sensory input to the local circuit, local neurons encode deviations from those expectations, and recurrent interactions whiten the residual signals. This result establishes a mathematical equivalence between context-conditioned efficient coding and predictive coding, revealing that predictive computations can emerge from efficient input compression guided by context. The resulting framework is distinct from both classical redundancy reduction within a single modality and hierarchical Bayesian inference. The theory explains and unifies diverse experimental phenomena, including cross-modal suppression of responses to predicted inputs and multimodal receptive fields across sensorimotor, audiovisual, visual-olfactory, and auditory-somatosensory circuits, while recovering classical unimodal coding effects as limiting cases. By linking coding objectives, circuit mechanisms, and experimentally observed phenomena within a single analytical framework, this work provides a principled foundation for understanding how distributed neural systems use context to shape local representations.