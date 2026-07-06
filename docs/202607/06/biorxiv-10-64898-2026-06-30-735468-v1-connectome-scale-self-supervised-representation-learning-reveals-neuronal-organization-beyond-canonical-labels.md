---
title: Connectome-scale self-supervised representation learning reveals neuronal organization beyond canonical labels
title_zh: 连接组尺度的自监督表示学习揭示超越规范标签的神经元组织
authors: "Shi, T., Chen, Y., Liu, C., Zhang, R."
date: 2026-07-04
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.30.735468v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 连接组尺度自监督表征学习与图神经网络
tldr: 密集电子显微镜连接组提供了突触分辨率的神经元结构图谱，但如何学习整合结构与连接的可扩展表示以进行无监督发现仍是挑战。本文提出一种自监督框架，利用分层图神经网络和骨架分解进行对比学习，在FlyWire连接组上验证了细骨架保留更丰富的身份信息，并通过坐标无关拓扑减少混淆。结构-连接表示改善了亚型区分，多跳学习揭示了半球连接偏侧化等高阶组织，证明了该框架在大规模连接组中自动化发现神经元身份和组织的有效性。
source: biorxiv
selection_source: fresh_fetch
motivation: 在密集连接组中学习整合结构与连接的可扩展表示，以减少人工干预并发现神经元组织。
method: 提出自监督框架，用分层图神经网络结合骨架分解进行对比学习，并利用结构嵌入构建连接表示。
result: 细骨架保留更丰富神经元身份信息，结构-连接表示改善亚型区分，多跳学习揭示半球偏侧化等组织。
conclusion: 该框架可自监督地在大规模密集连接组中发现神经元身份和组织结构。
---

## 摘要
密集电子显微镜连接组提供了神经元结构和突触连接的突触级图谱，但学习可扩展的表示来整合结构和连接性以进行最小人工干预的连接组发现仍然困难。本文提出了一个在密集连接组中进行结构-连接性表示学习的自监督框架。具有骨架分解的分层图神经网络能够从精细采样的FlyWire神经元骨架中进行对比学习，表明精细骨架比粗糙表示保留了更丰富的身份信息。无坐标拓扑减少了发育和几何混淆，改进了聚类和标签高效推断。然后，我们使用学习到的结构嵌入作为突触伙伴的连续描述符来构建结构驱动的连接性表示，在没有预定义伙伴类型标签的情况下改进了亚型区分。迭代多跳学习进一步揭示了更高阶的组织，包括半球连接侧化和连接性定义的子组。注意力分析将这些差异与特定的突触伙伴联系起来。总之，这些结果建立了一个自监督且可扩展的框架，用于在大规模密集连接组中发现神经元身份和连接组组织。

## Abstract
Dense electron-microscopy connectomes provide synaptic-resolution maps of neuronal structure and wiring, but learning scalable representations that integrate structure and connectivity for connectome discovery with minimal human intervention remains difficult. Here we present a self-supervised framework for structure-connectivity representation learning in dense connectomes. A hierarchical graph neural network with skeleton decomposition enables contrastive learning from finely sampled FlyWire neuronal skeletons, showing that fine skeletons preserve substantially richer identity information than coarse representations. Coordinate-free topology reduces developmental and geometric confounds, improving clustering and label-efficient inference. We then use learned structural embeddings as continuous descriptors of synaptic partners to construct structure-driven connectivity representations, improving subtype discrimination without predefined partner-type labels. Iterative multi-hop learning further reveals higher-order organization, including hemispheric connectivity lateralization and connectivity-defined subgroups. Attention analysis links these differences to specific synaptic partners. Together, these results establish a self-supervised and scalable framework for discovering neuronal identity and connectome organization in a large-scale dense connectome.