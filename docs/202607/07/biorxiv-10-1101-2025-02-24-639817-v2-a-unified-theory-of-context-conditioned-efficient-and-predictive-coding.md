---
title: A unified theory of context-conditioned efficient and predictive coding
title_zh: 上下文条件化的高效编码与预测编码的统一理论
authors: "Tavoni, G."
date: 2026-07-06
pdf: "https://www.biorxiv.org/content/10.1101/2025.02.24.639817v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 上下文条件的高效与预测编码统一理论
tldr: 感官处理受行为上下文和多模态信号影响，但现有理论缺乏统一框架。本研究提出一个统一理论，证明上下文条件的高效编码与预测编码在数学上等价，推导出可解释的神经算法：上下文提供期望，局部神经元编码偏差，循环交互白化残差信号。该理论统一解释了跨模态抑制、多模态感受野等实验现象，并恢复经典单模态编码效应。
source: biorxiv
selection_source: fresh_fetch
motivation: 感官处理依赖于上下文，但缺乏统一理论解释上下文如何优化局部神经编码。
method: 通过数学分析，建立上下文条件高效编码与预测编码的等价性，推导出局部回路算法。
result: 上下文提供期望，局部神经元编码预测偏差，循环连接白化残差信号，实现高效压缩。
conclusion: 该理论统一解释跨模态抑制和多模态感受野等现象，为分布式神经系统的上下文编码提供原理基础。
---

## 摘要
感觉处理并非孤立发生：在某种感觉模态中，神经元所表征的内容受到来自其他感官、动作和行为背景的信号塑造。这种上下文依赖性对神经编码理论提出了一个基本问题：电路如何利用大脑其他区域可用的信息来高效编码其局部输入？在这里，我们发展了一个高效编码与预测编码的统一理论，展示了多模态上下文信息如何在局部感觉电路中优化表征。我们通过分析证明，高效编码的解映射到一个可解释的神经算法：上下文信号为局部电路提供关于感觉输入的期望，局部神经元编码与这些期望的偏差，而循环交互则对残差信号进行白化。这一结果建立了上下文条件化的高效编码与预测编码之间的数学等价性，揭示了预测计算可以从由上下文引导的高效输入压缩中涌现。由此产生的框架既不同于单模态内的经典冗余减少，也不同于层级贝叶斯推理。该理论解释并统一了多种实验现象，包括对预测输入响应的跨模态抑制以及感觉运动、视听、视觉-嗅觉和听觉-体感回路中的多模态感受野，同时将经典的单模态编码效应恢复为极限情况。通过在一个统一的分析框架内连接编码目标、电路机制和实验观察到的现象，这项工作为理解分布式神经系统如何利用上下文塑造局部表征提供了原理性基础。

## Abstract
Sensory processing does not occur in isolation: what neurons represent in a given sensory modality is shaped by signals from other senses, actions, and behavioral context. This context dependence raises a fundamental question for theories of neural coding: how can circuits efficiently encode their local input while using information available elsewhere in the brain? Here we develop a unified theory of efficient and predictive coding that shows how multimodal contextual information can optimize representations within a local sensory circuit. We demonstrate analytically that the efficient-coding solution maps onto an interpretable neural algorithm: contextual signals provide expectations about the sensory input to the local circuit, local neurons encode deviations from those expectations, and recurrent interactions whiten the residual signals. This result establishes a mathematical equivalence between context-conditioned efficient coding and predictive coding, revealing that predictive computations can emerge from efficient input compression guided by context. The resulting framework is distinct from both classical redundancy reduction within a single modality and hierarchical Bayesian inference. The theory explains and unifies diverse experimental phenomena, including cross-modal suppression of responses to predicted inputs and multimodal receptive fields across sensorimotor, audiovisual, visual-olfactory, and auditory-somatosensory circuits, while recovering classical unimodal coding effects as limiting cases. By linking coding objectives, circuit mechanisms, and experimentally observed phenomena within a single analytical framework, this work provides a principled foundation for understanding how distributed neural systems use context to shape local representations.