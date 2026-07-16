---
title: "Stars2Cells: Astrometric Tracking of Neurons Across Imaging Sessions"
title_zh: Stars2Cells：跨成像会话的神经元天文测量跟踪
authors: "Peden-Asarch, A. M., Honan, L. E., Bai, J. Z., Asarch, E. M., Quinn, J. A., Coffey, K. R., Neumaier, J. F."
date: 2026-07-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.03.736144v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 用于纵向钙成像的神经元追踪流程
tldr: "慢性钙成像研究神经元长期活动时，跨会话配准因依赖易退化的空间或时间特征而困难。受天体测量启发，Stars2Cells将神经元局部几何编码为旋转平移缩放不变的quad描述符，仅需质心坐标进行匹配。在合成数据上F1达98.4%，远高于传统ROI匹配的36.0%。应用于纹状体成像揭示了群体响应掩盖下的单神经元完全更替，为研究表征漂移提供关键工具。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1691, \"height\": 950}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1490, \"height\": 1364}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1682, \"height\": 1432}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1693, \"height\": 1206}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1656, \"height\": 1073}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1311, \"height\": 1284}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1628, \"height\": 781}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1364, \"height\": 1589}]"
motivation: 现有跨会话神经元匹配方法依赖易退化的空间或时间特征，导致大部分实验室无法进行纵向研究。
method: 基于质心坐标，将局部几何编码为四维不变量，结合描述符空间匹配、RANSAC验证和匈牙利分配。
result: "在合成基准测试中F1达98.4%，并在芬太尼自我给药实验中揭示纹状体群体反应掩盖单神经元完全更替。"
conclusion: 提供无需编程的跨会话神经元跟踪工具，使表征漂移研究成为可能。
---

## 摘要
长期钙成像为了解单个神经元和群体活动如何随天数变化提供了一个窗口，其中从一次成像到下一次成像中识别同一神经元是回答关于随时间推移的学习、漂移和可塑性问题的先决条件。然而，由于现有的配准工具依赖于空间足迹或时间相关性，这些相关性在重复记录过程中会退化，因此只有约2-3%的成像实验室发表纵向跨会话工作。在这里，我们引入Stars2Cells（S2C），一种受天文测量板解法启发的跟踪流程，它将每个神经元的局部几何表示为对旋转、平移和均匀缩放不变的四维四元描述符。S2C仅基于质心坐标运行，结合了描述符空间匹配、随机抽样一致性（RANSAC）验证和匈牙利指派。在包含100-1000个神经元和8种扰动条件以及一个身份基准底线的1,262个配对运行的合成基准测试中，S2C达到了综合F1=98.4%，而基于ROI的标准匹配为36.0%。为了展示其能力，我们将该流程应用于口服芬太尼行为经济学自我给药期间的背内侧纹状体（DMS）成像。在这里，我们展示了DMS中保守的群体奖励杠杆按压反应掩盖了接近完全的单神经元更替。这种我们展示的表征漂移特征在整体光度测量中是看不见的，而解决它需要S2C提供的同细胞跟踪。S2C作为GUI驱动的独立应用程序分发，适用于macOS和Windows，无需Python、命令行或虚拟环境设置。

## Abstract
Chronic calcium imaging offers a window into how single neurons and ensemble activity change across days where identifying the same neurons from one session to the next is the prerequisite for answering questions regarding learning, drift, and plasticity over time. Yet only [~]2-3% of imaging laboratories publish longitudinal cross-session work, because existing registration tools depend on spatial-footprint or temporal correlations that degrade under repeated recording sessions. Here, we introduce Stars2Cells (S2C), a tracking pipeline inspired by astrometric plate-solving that represents each neurons local geometry as a four-dimensional quad descriptor invariant to rotation, translation, and uniform scaling. S2C operates purely on centroid coordinates and combines descriptor-space matching, Random Sample Consensus (RANSAC) verification, and Hungarian assignment. Across a synthetic benchmark of 1,262 paired runs spanning 100-1,000 neurons and 8 perturbation conditions plus 1 identity sanity-floor, S2C reached pooled F1 = 98.4% compared to the standard ROI-based matching of 36.0%. To show what this enables, we applied the pipeline to dorsomedial striatum (DMS) imaging during oral fentanyl behavioral-economics self-administration. Here, we show that a conserved population-rewarded lever press response in DMS masks near-complete single-neuron turnover. This representational-drift signature we demonstrated is invisible to the bulk photometry, and resolving it requires the same-cell tracking S2C provides. S2C is distributed as a GUI-driven standalone application for both macOS and Windows, requiring no Python, command line, or virtual environment setup.