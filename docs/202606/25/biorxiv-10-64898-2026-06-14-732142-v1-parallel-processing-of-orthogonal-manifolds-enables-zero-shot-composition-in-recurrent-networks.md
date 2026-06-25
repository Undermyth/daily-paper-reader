---
title: Parallel processing of orthogonal manifolds enables zero-shot composition in recurrent networks
title_zh: 正交流形的并行处理使循环网络中的零样本组合成为可能
authors: "Osako, Y., Arango, A., Asabuki, T."
date: 2026-06-17
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.14.732142v1.full.pdf"
tags: ["query:la"]
score: 7.0
evidence: 递归网络中利用可塑性规则实现零样本组合
tldr: 动物能灵活组合习得行为而无需联合训练，但其计算机制尚不明确。本研究通过局部预测可塑性规则训练循环网络发现，独立学习的反馈向量将不同计算嵌入可分离动态子空间，使新输入组合能零样本并行激活这些组件并生成复合输出；而对齐反馈向量或BPTT训练虽能实现单任务学习，却无法支持并行组合。该结果揭示了反馈几何是结构循环动态以实现未来组合复用的关键原则。
source: biorxiv
selection_source: fresh_fetch
motivation: 探索循环网络如何通过反馈几何实现零样本并行组合，分离任务获取与未来可重用性的学习机制。
method: 采用局部预测可塑性规则训练循环网络，对比独立与对齐反馈向量以及BPTT训练，分析并行组合能力。
result: 独立反馈向量使学习嵌入可分离子空间，支持零样本组合；对齐反馈向量或BPTT则无法实现。
conclusion: 反馈几何是结构化循环动态以支持组合复用的计算原则，可解释运动皮层中的相加姿势几何。
---

## 摘要
动物能够灵活地将学到的行为组合成新的动作，而无需练习这些组合，然而，使独立习得的计算能够并行表达的机制仍不清楚。在此，我们表明学习期间的反馈几何结构决定了循环动态是否可以通过零样本并行组合进行重组。使用由局部预测可塑性规则训练的循环网络，我们发现不同的反馈向量将独立学习的计算嵌入到可分离的动态子空间中，从而允许新的输入组合共同激活这些组件并生成复合输出，而无需联合训练。相比之下，对齐的反馈向量以及通过时间反向传播训练的网络，表现出准确的单任务性能，但未能支持并行组合，这表明任务获取和未来可重用性是学习的可分离属性。组合输入引发了一个单一的复合群体轨迹，其在反馈形状任务子空间上的投影恢复了独立学习的组件动态。同样的原理重现了在运动皮层中观察到的加性伸臂-姿势几何结构，并推广到更高维度的运动基元。这些结果将反馈几何结构确定为一种计算原理，学习系统通过该原理组织循环动态以实现未来的组合重用。

## Abstract
Animals flexibly combine learned behaviors into novel actions without practicing their combinations, yet the computational mechanisms that enable independently acquired computations to be expressed in parallel remain unclear. Here we show that feedback geometry during learning determines whether recurrent dynamics can be recombined through zero-shot parallel composition. Using recurrent networks trained by a local predictive plasticity rule, we found that distinct feedback vectors embed independently learned computations in separable dynamical subspaces, allowing novel input combinations to co-activate these components and generate composite outputs without joint training. In contrast, aligned feedback vectors, as well as networks trained by backpropagation through time, exhibited accurate single-task performance but failed to support parallel composition, demonstrating that task acquisition and future reusability are dissociable properties of learning. A combined input evoked a single composite population trajectory, whose projections onto feedback-shaped task subspaces recovered the independently learned component dynamics. The same principle reproduced additive reach-posture geometry observed in motor cortex and generalized to higher-dimensional movement primitives. These results identify feedback geometry as a computational principle by which learning systems structure recurrent dynamics for future compositional reuse.