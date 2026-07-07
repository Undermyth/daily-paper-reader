---
title: Connectome-scale self-supervised representation learning reveals neuronal organization beyond canonical labels
title_zh: 连接组尺度自监督表示学习揭示超越经典标签的神经元组织
authors: "Shi, T., Chen, Y., Liu, C., Zhang, R."
date: 2026-07-04
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.30.735468v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 自监督连接组表示学习揭示神经元组织
tldr: 密集电子显微镜连接组提供突触分辨率的神经结构图，但缺乏可扩展的表示学习。本文提出自监督框架，使用分层图神经网络和骨架分解进行对比学习，并用坐标无关拓扑减少混淆。细粒度骨架保留更丰富身份信息，结构嵌入改善亚型区分，迭代多跳学习揭示半球连接偏侧化等高级组织。该框架实现了大规模密集连接组中神经元身份和连接组组织的可扩展发现。
source: biorxiv
selection_source: fresh_fetch
motivation: 密集连接组缺乏可扩展的表示学习方法，需整合结构和连接性信息进行无监督发现。
method: 提出自监督框架，采用分层图神经网络与骨架分解进行对比学习，并使用坐标无关拓扑减少噪声。
result: 细粒度骨架保留更丰富身份信息，结构嵌入改善亚型区分，多跳学习发现半球连接偏侧化等组织规律。
conclusion: 建立了可扩展的自监督框架，在大型密集连接组中成功实现了神经元身份和连接组组织的自动化发现。
---

## 摘要
密集电子显微镜连接组提供了神经元结构和连接的突触级图谱，但学习可扩展的表示以整合结构和连接，从而以最少的人为干预进行连接组发现仍然困难。本文提出了一种用于密集连接组中结构-连接表示学习的自监督框架。具有骨架分解的分层图神经网络能够对精细采样的 FlyWire 神经元骨架进行对比学习，表明精细骨架比粗粒度表示保留了更丰富的身份信息。无坐标拓扑减少了发育和几何混杂因素，改善了聚类和标签高效推理。然后，我们使用学习到的结构嵌入作为突触伙伴的连续描述符来构建结构驱动的连接表示，在没有预定义伙伴类型标签的情况下改善亚型区分。迭代多跳学习进一步揭示了高阶组织，包括半球连接偏侧化和连接定义的亚群。注意力分析将这些差异与特定的突触伙伴联系起来。总之，这些结果建立了一个自监督且可扩展的框架，用于在大规模密集连接组中发现神经元身份和连接组组织。

## Abstract
Dense electron-microscopy connectomes provide synaptic-resolution maps of neuronal structure and wiring, but learning scalable representations that integrate structure and connectivity for connectome discovery with minimal human intervention remains difficult. Here we present a self-supervised framework for structure-connectivity representation learning in dense connectomes. A hierarchical graph neural network with skeleton decomposition enables contrastive learning from finely sampled FlyWire neuronal skeletons, showing that fine skeletons preserve substantially richer identity information than coarse representations. Coordinate-free topology reduces developmental and geometric confounds, improving clustering and label-efficient inference. We then use learned structural embeddings as continuous descriptors of synaptic partners to construct structure-driven connectivity representations, improving subtype discrimination without predefined partner-type labels. Iterative multi-hop learning further reveals higher-order organization, including hemispheric connectivity lateralization and connectivity-defined subgroups. Attention analysis links these differences to specific synaptic partners. Together, these results establish a self-supervised and scalable framework for discovering neuronal identity and connectome organization in a large-scale dense connectome.