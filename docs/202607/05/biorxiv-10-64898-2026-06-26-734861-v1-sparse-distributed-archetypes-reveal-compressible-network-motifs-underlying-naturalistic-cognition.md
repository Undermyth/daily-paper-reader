---
title: Sparse Distributed Archetypes Reveal Compressible Network Motifs Underlying Naturalistic Cognition
title_zh: 稀疏分布的原型揭示自然主义认知下的可压缩网络基序
authors: "Owen, L. L. W., Stone, E., Shepherd, A."
date: 2026-06-28
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.26.734861v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 自然认知脑网络基序的计算分析
tldr: 自然主义认知源于多尺度脑系统的协调交互，但高维神经活动中的认知信息难以刻画。本研究将多被试原型分析（MS-AA）应用于叙事聆听、打乱语音和静息态fMRI数据，发现原型表示保留了条件相关结构且信息高度可压缩。少量原型（约5-15个）即可恢复大部分解码性能，这些原型并非孤立脑网络，而是默认模式与额顶系统等高级联合系统的分布式混合。结果揭示了认知状态区分的关键稀疏网络基序，为研究认知脑状态的压缩性与多尺度组织提供了框架。
source: biorxiv
selection_source: fresh_fetch
motivation: 自然主义认知中脑活动的多尺度组织难以表征，需压缩高维神经活动以揭示认知相关的结构。
method: 对fMRI数据应用空间与时间多被试原型分析，通过解码、聚类和网络过度表示分析评估原型信息。
result: "解码性能按完整叙事>打乱语音>静息态递减；5-15个原型捕获大部分信息；默认模式与额顶网络过度表示。"
conclusion: MS-AA揭示了分布式稀疏原型作为认知状态区分的可压缩基序，强调了高级联合系统的关键作用。
---

## 摘要
自然主义认知源于跨多个表征尺度的分布式脑系统之间的协调交互。由于认知相关信息嵌入在高维神经活动中，描述这一组织仍然具有挑战性。本文将对完整叙事聆听、单词打乱音频和静息状态下收集的自然主义fMRI数据应用多被试原型分析（MS-AA）[1]，以研究条件相关信息如何在原型表征中分布。

我们考察了MS-AA的空间和时间形式，作为自然主义脑活动的互补视角。在各项分析中，解码性能始终遵循完整>打乱>静息的层级，表明原型表征保留了有意义的条件相关结构。Top-m解码分析进一步揭示，这些信息高度可压缩：相对较小的原型子集经常恢复全模型解码性能的显著部分。

空间AA表现出一种稳定的稀疏解码机制，该机制在多个表征尺度上持续存在。在广泛匹配的成分比率范围内，大约5-15个原型始终捕获了不成比例的条件相关信息。这些相同的稀疏子集还将受试者组织成与条件对齐的聚类，其强度超过随机原型子集的预期，最强的联合解码-聚类效应在中间表征区间（K≈50-88）内反复出现。

网络过度表征分析表明，信息丰富的原型并非孤立的典型网络，而是交互系统的分布式混合。在表现最优的解码-聚类配置中，默认模式和额顶系统相对于网络大小始终过度表征，而视觉和边缘系统则表征不足。这些发现共同表明，对区分认知状态最具信息量的原型基序是稀疏的、分布式的子网络，富含高阶关联系统。更广泛地说，结果证明MS-AA为研究认知脑状态的可压缩性、几何结构和多尺度组织提供了有用框架。

## Abstract
Naturalistic cognition emerges from coordinated interactions among distributed brain systems operating across multiple representational scales. Characterizing this organization remains challenging because cognitively relevant information is embedded within high-dimensional neural activity. Here, we apply Multisubject Archetypal Analysis (MS-AA) [1] to naturalistic fMRI data collected during intact narrative listening, word-scrambled audio, and rest to investigate how condition-relevant information is distributed across archetypal representations.

We examine both spatial and temporal formulations of MS-AA as complementary views of naturalistic brain activity. Across analyses, decoding performance consistently followed the hierarchy intact > word-scrambled > rest, indicating that archetypal representations preserve meaningful condition-related structure. Top-m decoding analyses further revealed that this information is highly compressible: relatively small subsets of archetypes frequently recovered substantial fractions of full-model decoding performance.

Spatial AA exhibited a stable sparse-decoding regime that persisted across representational scales. Across a broad range of matched component ratios, approximately 5-15 archetypes consistently captured disproportionate amounts of condition-relevant information. These same sparse subsets also organized subjects into condition-aligned clusters more strongly than expected from random archetype subsets, with the strongest joint decoding-clustering effects occurring repeatedly within an intermediate representational regime (K {approx}50 - 88).

Network over-representation analyses revealed that informative archetypes were not isolated canonical networks but distributed mixtures of interacting systems. Across the highest-performing decoding- clustering configurations, default mode and frontoparietal systems were consistently overrepresented relative to network size, whereas visual and limbic systems were underrepresented. Together, these findings suggest that the archetypal motifs most informative for distinguishing cognitive states are sparse, distributed subnetworks enriched for higher-order association systems. More broadly, the results demonstrate that MS-AA provides a useful framework for studying the compressibility, geometry, and multiscale organization of cognitive brain states.