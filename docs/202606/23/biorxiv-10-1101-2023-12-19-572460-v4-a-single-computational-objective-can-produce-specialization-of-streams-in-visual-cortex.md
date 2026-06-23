---
title: A single computational objective can produce specialization of streams in visual cortex
title_zh: 一个单一的计算目标可以产生视觉皮层中通路的分化
authors: "Finzi, D., Margalit, E., Kay, K., Yamins, D. L. K., Grill-Spector, K."
date: 2026-06-20
pdf: "https://www.biorxiv.org/content/10.1101/2023.12.19.572460v4.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 使用计算模型（TDANN）证明单个自监督目标可以产生视觉皮层流的分化
tldr: 视觉皮层组织成背侧、外侧和腹侧流，传统观点认为这些流分别支持不同视觉行为。本研究通过比较自监督地形深度人工神经网络（TDANN）与任务专用模型，发现TDANN更好匹配fMRI数据，并再现了跨流的空间分离和功能分化。这一结果挑战了行为驱动的流分化假说，表明单一的学习目标（局部空间约束下的通用视觉表示）即可解释流组织的出现。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究视觉皮层功能流是否真正源于支持不同行为的需求，还是可由单一学习原则解释。
method: 使用自监督地形深度人工神经网络（TDANN）与任务专用DANN模型，对比其与大规模fMRI数据的匹配度。
result: TDANN比任务专用模型更准确预测脑反应，并复现了视觉流的空间分离与功能分化。
conclusion: 视觉流组织可能并非为不同行为独立进化，而是源于在局部空间约束下学习通用视觉表示的单一目标。
---

## 摘要
人类视觉皮层被组织成背侧、外侧和腹侧通路。一个长期存在的假说认为，通路的功能组织是为了支持不同的视觉行为。在这里，我们比较基于神经网络的计算机模型与大规模fMRI数据集，以探究视觉通路出现的原因。我们发现，一个自监督的拓扑深度人工神经网络（TDANN），它鼓励相邻单元做出相似响应，比专门为通路特定视觉行为训练的DANN模型更好地捕捉了大脑反应，以及通路间的空间分离和功能分化。这些发现挑战了主流观点，即通路是分别为了支持不同行为而演化，反而暗示功能组织可能源于一个单一原则：在局部空间约束下学习普遍有用的视觉表征。

## Abstract
Human visual cortex is organized into dorsal, lateral, and ventral streams. A long-standing hypothesis is that the functional organization into streams emerged to support distinct visual behaviors. Here, we compare neural network-based computational models against a massive fMRI dataset to investigate why visual streams emerge. We find that a self-supervised Topographic Deep Artificial Neural Network (TDANN), which encourages nearby units to respond similarly, better captures brain responses, as well as spatial segregation and functional differentiation across streams, than DANN models trained for stream-specific visual behaviors. These findings challenge the prevailing view that streams evolved to separately support different behaviors and suggest instead the possibility that functional organization can arise from a single principle: learning generally useful visual representations subject to local spatial constraints.