---
title: Topological decoding of grid cell activity via path lifting to covering spaces
title_zh: 通过路径提升到覆盖空间对网格细胞活动进行拓扑解码
authors: "Yao, Y. J., Yoon, I. H. R."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.17.683158v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 内嗅皮层网格细胞的拓扑解码，涉及海马体表示计算
tldr: 网格细胞活动组织在环面流形上，但其周期性编码使得直接解码空间位置存在困难。本文提出拓扑解码框架，利用拓扑数据分析提取环面坐标，并通过路径提升方法将环面轨迹映射回物理空间，实现了无需外部位置信息或训练数据的路径重建。在连续吸引子网络模拟与实验记录中，单个网格细胞模块的局部轨迹被可靠重建，仅相差仿射变换。该结果表明网格细胞模块足以支持路径整合，为空间导航的神经计算机制提供了新见解。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-683158-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1640, \"height\": 469, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-683158-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 682, \"height\": 541, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-683158-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 685, \"height\": 351, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-683158-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1457, \"height\": 727, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-683158-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1248, \"height\": 818, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-683158-v2/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1627, \"height\": 892, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-683158-v2/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 927, \"height\": 642, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-683158-v2/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1655, \"height\": 787, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-683158-v2/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1651, \"height\": 915, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-683158-v2/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1650, \"height\": 361, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-17-683158-v2/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1638, \"height\": 543, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-1101-2025-10-17-683158-v2/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1628, \"height\": 435, \"label\": \"Table\"}]"
motivation: 网格细胞的周期性编码使大脑难以直接从环面流形理解空间状态。
method: 通过拓扑数据分析和路径提升，从网格细胞活动提取环面坐标并重建物理空间轨迹。
result: 在仿真和实验数据上，单个网格细胞模块无需外部信息即可重建局部轨迹，仅差仿射变换。
conclusion: 共模块网格细胞包含足够信息用于路径整合，揭示空间导航的潜在计算机制。
---

## 摘要
高维神经活动通常存在于低维子空间中，称为神经流形。内侧内嗅皮层中的网格细胞提供了一个与空间环境无关、组织在环面流形附近的周期性空间编码。由于其编码的周期性，大脑如何利用环面流形理解其在空间环境中的状态尚不清楚。我们提出了一种新框架，利用拓扑从网格细胞活动中解码空间信息。该方法使用拓扑数据分析从网格细胞群体活动中提取环面坐标，并通过路径提升重建物理空间中的轨迹。重建的路径与原始路径相差一个仿射变换。我们在连续吸引子网络模拟和网格细胞实验记录上验证了该方法，表明无需外部位置信息或训练数据，即可从单个网格细胞模块可靠重建局部轨迹。这些结果表明，共模块网格细胞包含足够的路径积分信息，并提示了空间导航的潜在计算机制。

## Abstract
High-dimensional neural activity often reside in a low-dimensional subspace, referred to as neural manifolds. Grid cells in the medial entorhinal cortex provide a periodic spatial code that are organized near a toroidal manifold, independent of the spatial environment. Due to the periodic nature of its code, it is unclear how the brain utilizes the toroidal manifold to understand its state in a spatial environment. We introduce a novel framework that decodes spatial information from grid cell activity using topology. Our approach uses topological data analysis to extract toroidal coordinates from grid cell population activity and employs path-lifting to reconstruct trajectories in physical space. The reconstructed paths differ from the original by an affine transformation. We validated the method on both continuous attractor network simulations and experimental recordings of grid cells, demonstrating that local trajectories can be reliably reconstructed from a single grid cell module without external position information or training data. These results suggest that co-modular grid cells contain sufficient information for path integration and suggest a potential computational mechanism for spatial navigation.