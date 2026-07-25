---
title: Emergent topological structure in spontaneous brain-organoid activity
title_zh: 自发脑类器官活动中的涌现拓扑结构
authors: "Bodnia, E., Basart, M., Hai, S., Ford, L., Miolane, N., Kosik, K. S., Bouwmeester, D., Carr, L. D."
date: 2026-07-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.17.739228v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 脑类器官活动的拓扑分析
tldr: 神经活动一般认为在低维结构上组织，但小规模脑类器官的拓扑结构尚未明确。本研究应用持久同调分析人类和小鼠皮质类器官的微电极阵列记录（26-234个单元），通过Vietoris-Rips过滤构建相关网络，发现14/18数据集的第一个同调显著高于随机基线。该环结构对随机单元移除鲁棒但被目标移除破坏，且拓扑丰富度随网络规模增长。结果表明持久同调能在实验实际规模的记录中解析出非平凡的拓扑结构。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-17-739228-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1605, \"height\": 528, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-17-739228-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1607, \"height\": 1265, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-17-739228-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 853, \"height\": 624, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-17-739228-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1573, \"height\": 351, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-17-739228-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1620, \"height\": 261, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-17-739228-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1583, \"height\": 694, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-17-739228-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1605, \"height\": 662, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-17-739228-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 889, \"height\": 729, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-17-739228-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 903, \"height\": 749, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-17-739228-v1/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1612, \"height\": 456, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-17-739228-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1022, \"height\": 622, \"label\": \"Table\"}]"
motivation: 探索小规模神经网络（如脑类器官）中是否涌现拓扑结构，以及持久同调能否解析有限节点数的记录。
method: 对26-234个单元的MEA记录，构建相关性加权网络，应用Vietoris-Rips持久同调计算H1和H2，并与速率和群体不变的零模型比较。
result: 14/18数据集的H1显著高于零模型，H2仅在较大网络中显著；环结构对随机单元鲁棒但被关键单元破坏。
conclusion: 持久同调在实验实际规模下可揭示神经活动中的微观拓扑结构，为类器官研究提供新视角。
---

## 摘要
神经活动普遍被认为组织在嵌入高维状态空间的低维结构上。持续同调直接从成对相关模式中读取这种结构，而无需预先假设哪些变量是相关的。我们将持续同调应用于来自人类（Lancaster）和小鼠（Paşca）皮层类器官自发活动的微电极阵列（MEA）记录，涵盖26至234个同步分选的单元，并探究拓扑数据分析是否能在神经记录实际提供的节点数上解析出结构。在相关空间中构建加权网络并通过Vietoris–Rips滤流对其进行表征，我们发现，在18个数据集中有14个的第一同调（H1，环）显著高于保留速率和种群的空模型。这种环结构占据了一个非冗余核心：它对随机移除单元具有鲁棒性，但通过针对性移除承载它的单元而被破坏。拓扑丰富度随网络规模增长，第二同调（H2）仅在较大网络中显著高于空模型。这些结果表明，持续同调在实际实验所达到的尺度上解析了神经记录中的结构化拓扑。

## Abstract
Neural activity is widely held to organize on low-dimensional structure embedded in a high-dimensional state space. Persistent homology reads such structure directly from the pattern of pairwise correlations, without assuming in advance which variables are relevant. We apply persistent homology to microelectrode-array (MEA) recordings of spontaneous activity from human (Lancaster) and mouse (Pa\c{s}ca) cortical organoids, spanning $26$--$234$ simultaneously sorted units, and ask whether topological data analysis resolves structure at the node counts that neural recordings actually deliver. Building weighted networks in correlation space and characterizing them by Vietoris--Rips filtration, we find that the first homology ($H_1$, loops) rises significantly above a rate- and population-preserving null in $14$ of $18$ datasets. This loop structure occupies a non-redundant core: it is robust to random removal of units yet disrupted by targeted removal of the units that carry it. Topological richness grows with network size, and second homology ($H_2$) emerges significantly above the null only in the larger networks. These results show that persistent homology resolves structured topology in neural recordings at the scale experiments actually deliver.