---
title: "Stars2Cells: Astrometric Tracking of Neurons Across Imaging Sessions"
title_zh: Stars2Cells：跨成像会话的神经元天体测量追踪
authors: "Peden-Asarch, A. M., Honan, L. E., Bai, J. Z., Asarch, E. M., Quinn, J. A., Coffey, K. R., Neumaier, J. F."
date: 2026-07-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.03.736144v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 使用天文方法跨成像会话跟踪神经元
tldr: "慢性钙成像跨天追踪相同神经元是研究学习与可塑性的关键，但现有方法因依赖易退化的空间或时序特征而成功率低。本文提出Stars2Cells(S2C)，借鉴天体测量板解，利用旋转平移缩放不变的局部几何描述符仅基于质心坐标匹配神经元。在合成基准上F1达98.4%，远高于标准ROI匹配的36.0%。应用至背内侧纹状体成像，揭示群体水平稳定响应掩盖了单神经元完全更替的表现漂移，该信号在传统群体记录中不可见。S2C以GUI应用形式发布，无需编程环境。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1691, \"height\": 950, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1490, \"height\": 1364, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1682, \"height\": 1432, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1693, \"height\": 1206, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1656, \"height\": 1073, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1311, \"height\": 1284, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1628, \"height\": 781, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-03-736144-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1364, \"height\": 1589, \"label\": \"Table\"}]"
motivation: 现有跨天神经元追踪方法依赖易退化的空间或时间特征，导致成功率低，阻碍学习与可塑性研究。
method: 借鉴天体测量板解，用旋转平移缩放不变的quad描述符表示局部几何，结合质心匹配、RANSAC验证与匈牙利分配。
result: "合成基准F1=98.4%远超标准ROI匹配(36.0%)；在DMS成像中揭示群体响应掩盖单神经元完全更替。"
conclusion: S2C实现跨天精准单神经元追踪，以易用GUI应用推动纵向钙成像研究。
---

## 摘要
慢性钙成像为了解单个神经元和群体活动在数天间的变化提供了一扇窗口，而确定同一神经元在不同会话中的对应关系是回答关于学习、漂移和可塑性随时间变化问题的前提。然而，目前仅有约2-3%的成像实验室发表纵向跨会话工作，因为现有的配准工具依赖于空间足迹或时间相关性，而这些在重复记录会话中会退化。在此，我们介绍Stars2Cells（S2C），一种受天体测量板解算启发的追踪流程，它将每个神经元的局部几何形状表示为对旋转、平移和均匀缩放不变的4维象限描述符。S2C纯粹基于质心坐标运行，结合了描述符空间匹配、随机样本一致性（RANSAC）验证和匈牙利分配。在跨越100-1000个神经元、8种扰动条件以及1个身份混淆基线的1262对配对运行的合成基准测试中，S2C的合并F1分数达到98.4%，而基于标准ROI匹配的为36.0%。为展示其能力，我们将该流程应用于口服芬太尼行为经济学自我给药期间的背内侧纹状体（DMS）成像。在此，我们显示DMS中一个保守的群体奖励杠杆按压反应掩盖了几乎完全的单个神经元更替。我们展示的这种表征漂移特征在整体光度测量中不可见，而解析它需要S2C提供的同细胞追踪。S2C作为基于图形用户界面的独立应用程序分发，适用于macOS和Windows，无需Python、命令行或虚拟环境设置。

## Abstract
Chronic calcium imaging offers a window into how single neurons and ensemble activity change across days where identifying the same neurons from one session to the next is the prerequisite for answering questions regarding learning, drift, and plasticity over time. Yet only [~]2-3% of imaging laboratories publish longitudinal cross-session work, because existing registration tools depend on spatial-footprint or temporal correlations that degrade under repeated recording sessions. Here, we introduce Stars2Cells (S2C), a tracking pipeline inspired by astrometric plate-solving that represents each neurons local geometry as a four-dimensional quad descriptor invariant to rotation, translation, and uniform scaling. S2C operates purely on centroid coordinates and combines descriptor-space matching, Random Sample Consensus (RANSAC) verification, and Hungarian assignment. Across a synthetic benchmark of 1,262 paired runs spanning 100-1,000 neurons and 8 perturbation conditions plus 1 identity sanity-floor, S2C reached pooled F1 = 98.4% compared to the standard ROI-based matching of 36.0%. To show what this enables, we applied the pipeline to dorsomedial striatum (DMS) imaging during oral fentanyl behavioral-economics self-administration. Here, we show that a conserved population-rewarded lever press response in DMS masks near-complete single-neuron turnover. This representational-drift signature we demonstrated is invisible to the bulk photometry, and resolving it requires the same-cell tracking S2C provides. S2C is distributed as a GUI-driven standalone application for both macOS and Windows, requiring no Python, command line, or virtual environment setup.