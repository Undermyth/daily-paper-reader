---
title: Functional connectivity gradients depend on cortical sampling position and brain state
title_zh: 功能连接梯度取决于皮层采样位置和大脑状态
authors: "Li, M., Ding, Z., Gore, J. C."
date: 2026-07-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.14.738484v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 功能连接梯度依赖于皮层采样位置和脑状态
tldr: 功能连接分析常忽略皮层采样位置差异。本研究利用HCP静息态和电影观看fMRI数据，比较中厚层与灰质-白质边界表面的功能梯度。发现电影观看减弱表面间主梯度分离，但效应具有空间异质性：视觉、边缘和默认网络收敛，突显/腹侧注意皮层分化。状态变化反映两种表面的协同重构。表明采样位置是功能连接几何的可解释维度，影响宏观脑组织结论。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738484-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1449, \"height\": 1412, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738484-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 507, \"height\": 530, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738484-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 646, \"height\": 651, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738484-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1473, \"height\": 1271, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738484-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1451, \"height\": 1287, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738484-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1494, \"height\": 1450, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-14-738484-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1691, \"height\": 627, \"label\": \"Table\"}]"
motivation: 探究皮层采样位置（中厚层vs灰质-白质边界）是否为状态敏感的功能组织维度。
method: 分析176名HCP受试者4个静息态和4个电影观看7T fMRI运行，从个体表面采样BOLD，经400个皮层区嵌入共同梯度空间。
result: 电影观看减少了主梯度在表面间的分离，但视觉、边缘和默认网络收敛，而突显/腹侧注意皮层分化；状态变化由表面协同重构驱动。
conclusion: 皮层采样位置是功能连接几何的关键测量维度，其空间组织可重复，但幅度和状态依赖性可变，需注意采样位置对结论的影响。
---

## 摘要
功能连接分析通常将从皮层邻近位置采样的信号视为可互换的，尽管灰白质边界存在解剖学和血流动力学转变。我们测试了采样位置是否构成宏观功能组织的一个状态敏感维度。在176名人类连接组计划年轻成年人中，进行四次7T静息态和四次观看电影扫描，从个体特异性中厚度和灰白质边界表面提取BOLD时间序列，汇总到400个皮层区块，并嵌入共同的功能梯度空间。电影观看减少了表面之间的主梯度分离，但这种效应在空间上异质：视觉、边缘和默认网络趋同，而突显/腹侧注意皮层分化。Shapley分解和反事实分析表明，状态变化反映了两个表面表征的协调重配置，而非一个表面趋近于另一个。原始连接性配置文件的变化追踪了梯度变化，表明结果并非仅由嵌入引入。两个表面在电影期间也表现出刺激锁定的受试者间功能连接。然而，刺激共享的分离仅捕捉了电影状态组织的一部分，并未解释电影减去静息的变化。最后，在172名匹配参与者中，静息态分离图谱从7T推广到3T，而绝对幅度和跨场个体排名较不稳定。这些发现确立了皮层采样位置作为功能连接几何的一个可解释测量维度。其空间组织在不同采集过程中可重现，但其幅度和状态依赖性变化，强调BOLD信号相对于皮层边界采样的位置可能影响关于宏观脑组织的结论。

## Abstract
Functional-connectivity analyses often treat signals sampled from nearby cortical positions as interchangeable, despite anatomical and hemodynamic transitions at the gray-white boundary. We tested whether sampling position constitutes a state-sensitive dimension of macroscale functional organization. In 176 Human Connectome Project young adults with four 7 T resting-state and four movie-watching runs, BOLD time series were sampled from subject-specific midthickness and gray-white-boundary surfaces, summarized across 400 cortical parcels, and embedded in a common functional-gradient space. Movie viewing reduced principal-gradient separation between surfaces, but this effect was spatially heterogeneous: Visual, Limbic and Default networks converged, whereas Salience/ventral-attention cortex differentiated. Shapley decomposition and counterfactual analyses showed that the state change reflected coordinated reconfiguration of both surface representations rather than one surface approaching the other. Changes in the original connectivity profiles tracked gradient changes, indicating that the result was not solely introduced by embedding. Both surfaces also exhibited stimulus-locked intersubject functional connectivity during movies. However, stimulus-shared separation captured only part of movie-state organization and did not explain the movie-minus-rest change. Finally, in 172 matched participants, resting-state separation maps generalized from 7 T to 3 T, whereas absolute magnitude and cross-field individual ranking were less stable. These findings establish cortical sampling position as an interpretable measurement dimension of functional-connectivity geometry. Its spatial organization is reproducible across acquisitions, but its magnitude and state dependence vary, emphasizing that where BOLD signals are sampled relative to the cortical boundary can shape conclusions about macroscale brain organization.