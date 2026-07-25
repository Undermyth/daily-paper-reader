---
title: Condition-Dependent Noise Correlations without Condition-Dependent Spike Counts
title_zh: 条件依赖的噪声相关性无需条件依赖的尖峰计数
authors: "Kim, D., Panichello, M., Moore, T."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.08.723078v4.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 计算神经科学中的噪声相关性与群体编码
tldr: 传统观点认为噪声相关性（NCs）影响神经编码依赖于发放率（SCs）的条件依赖性。本研究通过记录猕猴前额叶皮层在空间延迟响应任务中的群体活动，发现无SCs选择性的神经元对仍表现出条件依赖的NCs，且幅度与有SCs选择性对相当。这表明NCs可独立于SCs提供条件信息，拓展了对神经编码机制的理解。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-08-723078-v4/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1724, \"height\": 776, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-08-723078-v4/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1293, \"height\": 775, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-08-723078-v4/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1704, \"height\": 923, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-08-723078-v4/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1704, \"height\": 923, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-08-723078-v4/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1730, \"height\": 677, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-08-723078-v4/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1722, \"height\": 868, \"label\": \"Figure\"}]"
motivation: 探究噪声相关性（NCs）是否能在缺乏条件依赖发放率（SCs）的情况下，仍提供条件依赖信息。
method: 记录猕猴前额叶皮层神经元在空间延迟响应任务中的活动，分析视觉、记忆和运动时期SCs与NCs的选择性。
result: 无SCs选择性的神经元对仍表现出条件依赖的NCs，且其幅度与有SCs选择性对相当。
conclusion: 相关性变异性可在无条件依赖发放率时产生条件依赖，表明NCs是独立的信息源。
---

## 摘要
大脑编码信息和控制行为的能力依赖于大型分布式神经元群体的协同活动。同一条件下跨试次的神经元尖峰活动相关性，即噪声相关性（NCs），已被解释为共享突触连接性的反映，以及影响神经元群体信息容量的一个因素。NCs对编码的影响通常是在其尖峰计数（SCs）中表现出强烈条件依赖信息的神经元群体中考虑的。然而，理论研究表明，NCs可能提供独立于SCs的条件依赖信息源。我们检查了猕猴在执行包含视觉、记忆和运动阶段的空间延迟反应任务时前额叶皮层中大型神经元群体的活动。我们发现，在SCs中表现出视觉、记忆和运动选择性的神经元对，通常在其NCs中也表现出选择性，且独立于尖峰计数。然而，我们也发现，在不同任务阶段没有SC选择性的神经元对，仍然表现出条件依赖的NCs。此外，我们发现，无论神经元对是否具有SC选择性，条件依赖的NCs的幅度在很大程度上是可比较的。这些结果表明，即使在没有条件依赖的SCs的情况下，尖峰活动中的相关变异性也可以是条件依赖的。

## Abstract
The ability of the brain to encode information and control behavior depends on the coordinated activity of large and distributed neuronal populations. Correlations in neuronal spiking activity across trials of the same condition, or noise correlations (NCs), have been interpreted as a reflection of shared synaptic connectivity and as a contributing factor to the information capacity of neuronal populations. The impact of NCs on coding is most often considered in populations of neurons exhibiting robust condition-dependent information in their spike counts (SCs). However, theoretical work suggests that NCs could provide a source of condition-dependent information separate from SCs. We examined the activity of large neuronal populations in prefrontal cortex of macaques while they performed a spatial delayed response task composed of visual, memory, and motor epochs. We found that pairs of neurons that displayed visual, memory, and motor selectivity in their SCs often exhibited selectivity in their NCs, independent of spike count. However, we also found that pairs of neurons without SC selectivity during the different task epochs nonetheless exhibited condition-dependent NCs. Moreover, we found that the magnitude of condition-dependent NCs were largely comparable across neuronal pairs with or without SC selectivity. These results demonstrate that correlated variability in spiking activity can be condition-dependent even in the absence of condition-dependent SCs.

---

## 论文详细总结（自动生成）

# 论文总结：Condition-Dependent Noise Correlations without Condition-Dependent Spike Counts

## 1. 核心问题与整体含义（研究动机和背景）
- **核心问题**：传统观点认为，噪声相关性（NCs）对神经编码的影响通常依赖于神经元尖峰计数（SCs）的条件选择性。但理论研究表明，NCs 可能独立于 SCs 提供条件依赖信息。本文旨在实证检验：在缺乏条件依赖 SCs 的神经元对中，是否仍能观察到条件依赖的 NCs。
- **研究动机**：大脑群体编码不仅依赖于平均发放率，还依赖于跨试次的共同变异性（NCs）。以往研究多关注 SC 选择性神经元中的 NCs 调制，但非选择性神经元（如抑制性中间神经元或弱调谐的皮层细胞）也可能通过 NCs 携带任务相关信息。本文希望揭示 NCs 作为独立信息通道的潜力。
- **整体含义**：如果 NCs 确能在无条件选择性 SCs 下编码条件信息，则说明神经群体的信息编码机制比单纯基于发放率调谐更为丰富，NCs 可能是一种独立的、未被充分探索的信息载体。

## 2. 方法论：核心思想与关键技术细节
- **核心思想**：通过大尺度同步记录（Neuropixels），分别量化神经元的 SC 选择性（基于解码分析）和神经元对的 NC 条件依赖性（基于回归模型），并比较选择性/非选择性对之间的差异。
- **关键技术细节**：
  - **SC 选择性分类**：使用多类线性 SVM 解码器（fitcecof，10折交叉验证）预测 8 个空间位置的线索位置。通过递归特征消融（recursive feature ablation，即按权重逐次移除神经元），当解码准确度首次降至机会水平（12.5% 的 95% 二项置信区间包含机会线）时，之前移除的神经元定义为“选择性神经元”，剩余为“非选择性神经元”。
  - **NC 计算**：在每个线索位置条件下，对每个神经元的 SC 进行 z-score 标准化（减去该条件均值、除以标准差），然后计算配对 Pearson 相关系数（r_sc），作为噪声相关性。
  - **NC 条件依赖性检测**：对每个神经元对建立线性回归模型：\( N_2 \sim \beta_0 + \beta_1 N_1 + \beta_2 (N_1 \times C) \)，其中 \(C\) 是线索位置的分类编码。若交互项 \(\beta_2\) 显著（ANOVA F 检验，p<0.05），则表明 NCs 随条件变化，即存在条件依赖。
  - **距离依赖性**：根据 spike 模板的质心计算神经元对之间欧氏距离，分析 NC 幅度及条件依赖比例与距离的关系。

## 3. 实验设计
- **数据集与场景**：
  - 3 只雄性猕猴（A、H、J），执行空间延迟反应任务（延迟匹配样本 MTS 或记忆引导扫视 MGS），线索为 8 个可能位置。
  - 记录区域：外侧前额叶皮层（LPFC，包括 8 区、9/46 区），使用 Neuropixels 探针（384 通道，3.84 mm 跨度）。
  - 共 25 个 session，8225 个单元（包含 putative 单/多单位）。分析三个任务时期：视觉（刺激后 0-300 ms）、延迟（400-1200 ms）、运动（扫视开始前 -125-0 ms）。
- **Benchmark 与对比**：
  - 主要对比三类神经元对：两者均为 SC 选择性（S）、两者均为非选择性（NS）、混合型（一个选择性一个非选择性）。
  - 统计检验包括：与 5% 随机水平的卡方拟合优度检验、不同类别比例之间的卡方检验、距离依赖性 Spearman 相关等。
- **未提及与其他方法的横向对比**（如与其他脑区或模型比较），论文为描述性发现。

## 4. 资源与算力
- **文中未明确提及 GPU 型号、数量或训练时长**。数据预处理使用 Kilosort3（CPU 或 GPU 可加速），后续统计分析在 MATLAB 中完成，未涉及大规模深度学习训练，算力要求较低。
- 可推断使用了标准工作站或多核服务器，但无具体说明。

## 5. 实验数量与充分性
- **实验数量**：3 只动物、25 个 session、8225 个神经元；分析所有配对，并按距离 <1000 μm 限定主要结果。每个 epoch 分别分析。
- **充分性评估**：
  - **优点**：样本量较大（数百个同时记录的神经元），覆盖视觉、记忆、运动三个行为时期，距离依赖分析增强了结论可靠性。选择性/非选择性分类采用客观的解码消融法，避免主观阈值。
  - **不足**：
    - 仅记录一个脑区（LPFC），结论泛化性待验证。
    - 未进行因果操纵（如光遗传或药理学）证明 NCs 条件依赖性的功能作用。
    - 每个 session 中单个神经元对的数量可能不均衡（特别是非选择性对较少时）。
    - 未排除可能因 trial 数目差异导致统计力不足的问题（但使用了交叉验证和回归）。
  - **客观性与公平性**：统计方法标准，双尾检验，报告置信区间；但未进行多重比较校正（可能略微膨胀 I 类错误）。

## 6. 主要结论与发现
- **发现 1**：在 SC 选择性神经元对中，NCs 普遍随线索位置变化（条件依赖）。
- **发现 2**：在 SC 非选择性神经元对中，同样显著观察到条件依赖的 NCs，且比例与选择性对相当（甚至在视觉和运动时期更高）。
- **发现 3**：条件依赖 NCs 的普遍性随神经元对距离增大而递减，无论选择性类别如何。
- **发现 4**：所有 epoch 中，非选择性对的条件依赖 NCs 比例均显著高于随机水平（5%）。
- **核心结论**：相关变异性可以在缺乏条件依赖发放率的情况下编码条件信息，表明 NCs 是独立于 SCs 的额外信息通道。

## 7. 优点
- **方法学亮点**：
  - 使用大规模高密度探针（Neuropixels）同时记录数百个神经元，能够研究配对 NCs 的精细空间结构。
  - 通过解码消融法客观定义选择性，避免主观调谐阈值。
  - 回归模型直接检验 NC 条件依赖性，同时控制了 SC 的均值效应（z-score 化）。
- **概念创新**：首次系统展示非 SC 选择性群体中的条件依赖 NCs，挑战了“NCs 只有伴随调谐神经元才有编码意义”的传统看法。
- **结果稳健**：结论在三个不同任务时期和距离分析中一致，且使用了统计检验和置信区间。

## 8. 不足与局限
- **实验覆盖**：仅限猕猴前额叶皮层，未验证其他脑区（如感觉、运动皮层）或物种（如啮齿类）。
- **功能意义未确认**：虽然发现了条件依赖 NCs，但未直接量化这些 NCs 对下游解码或行为的贡献（缺乏群体协方差解码或信息论分析）。
- **潜在偏差**：神经元分类依赖于解码的敏感性，可能遗漏部分弱调谐但仍有贡献的神经元；非选择性对可能包含真正的非选择性细胞，也可能包含噪声大的未调谐细胞。
- **统计局限**：未对多重比较严格校正（如 Bonferroni 或 FDR），部分显著性可能为假阳性。
- **计算资源不透明**：未说明使用的硬件和时间，无法复现算力需求。
- **生理机制未阐明**：共享输入来源（局部、皮层下或跨皮层）以及非选择性神经元为何仍表现 NCs 条件依赖（如抑制掩膜假说）仅为推测，缺乏直接证据。

（完）
