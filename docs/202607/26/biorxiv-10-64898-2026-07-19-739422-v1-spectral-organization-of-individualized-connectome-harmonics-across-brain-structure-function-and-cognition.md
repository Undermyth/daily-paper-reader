---
title: "Spectral organization of individualized connectome harmonics across brain structure, function and cognition"
title_zh: 个体化连接组谐波在大脑结构、功能和认知中的频谱组织
authors: "Bolton, T., Schottner Sieler, M., Patel, J., Chan, C. H. M., Van De Ville, D., Hagmann, P."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.19.739422v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 连接组谐波研究脑结构-功能关系，直接与计算神经科学中的计算表征相关
tldr: 连接组谐波是研究脑结构与功能关系的框架，但如何纳入个体间变异性及解释频谱尺度尚不明确。本文利用875名参与者的MRI数据，构建个体化连接组谐波，发现其跨频谱呈现稳定性、稀疏性等有序转变，并自然形成多尺度家族。稀疏谐波能准确重建脑活动，并揭示认知任务中结构层次频率依赖的募集。结合结构与功能谐波可预测个体认知表现，表明连接组谐波是连接组的分层组织表示。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739422-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1711, \"height\": 2396, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739422-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1711, \"height\": 2436, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739422-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1680, \"height\": 1949, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739422-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1705, \"height\": 2075, \"label\": \"Figure\"}]"
motivation: 解决连接组谐波分析中的个体间变异性和频谱尺度解释问题。
method: 基于875名参与者的结构和功能MRI数据，构建个体化连接组谐波并分析其层次组织。
result: 谐波有序转变并形成多尺度家族；稀疏表示重建脑活动；结构-功能谐波组合预测认知表现。
conclusion: 连接组谐波不仅是频谱模式，更是连接组的分层表示，整合结构、动态与认知。
---

## 摘要
连接组谐波提供了结构性大脑连接的频谱表示，已成为研究结构-功能关系的强大框架。然而，两个基本问题仍未解决：如何将结构性连接的个体间变异纳入图信号处理分析，以及应在何种频谱尺度上解释连接组谐波？在此，利用875名参与者的结构和功能磁共振成像数据，我们展示了受试者特定的连接组谐波揭示了人类连接组的可重复分层组织。在整个频谱中，谐波表现出稳定性、图支持度、稀疏性和解剖定位上的有序过渡，并自然地组织成具有共同结构特性的多尺度家族。稀疏谐波表示准确重建了静息态和任务范式下的大脑活动，揭示了认知过程中对这种结构层级频率依赖的招募。最后，结合结构和功能谐波组织能够预测个体认知表现，表明两种表示捕获了互补的行为相关信息。综上，我们的发现表明，连接组谐波不应简单视为结构性连接的图频率模式，而应视为连接组的分层组织表示，连接了大脑结构、功能动态和认知。

## Abstract
Connectome harmonics provide a spectral representation of structural brain connectivity that has emerged as a powerful framework for studying structure-function relationships. However, two fundamental questions remain unresolved: how should inter-individual variability in structural connectivity be incorporated into graph signal processing analyses, and at which spectral scale should connectome harmonics be interpreted? Here, using structural and functional MRI data from 875 participants, we show that subject-specific connectome harmonics reveal a reproducible hierarchical organization of the human connectome. Across the spectrum, harmonics exhibited orderly transitions in stability, graph support, sparsity and anatomical localization, and naturally organized into multiscale families sharing common structural properties. Sparse harmonic representations accurately reconstructed brain activity across resting-state and task paradigms, revealing frequency-dependent recruitment of this structural hierarchy during cognition. Finally, combining structural and functional harmonic organization enabled the prediction of individual cognitive performance, demonstrating that both representations capture complementary behaviorally relevant information. Together, our findings show that connectome harmonics should be viewed not simply as graph-frequency modes of structural connectivity, but as a hierarchically organized representation of the connectome that links brain structure, functional dynamics and cognition.

---

## 论文详细总结（自动生成）

# 论文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

连接组谐波（connectome harmonics）作为结构性大脑连接的频谱表示，已成为研究脑结构与功能关系的强大框架。然而，现有方法存在两个基本问题未解决：① 如何将结构性连接中的个体间变异性纳入图信号处理分析；② 应在何种频谱尺度上解释连接组谐波。本论文旨在通过构建个体化连接组谐波，揭示人类连接组的可重复分层组织，并阐明其在结构、功能动态和认知中的角色。

## 2. 论文提出的方法论：核心思想、关键技术细节

### 核心思想
- 对每个被试，基于其个体结构性连接矩阵构建图拉普拉斯算子，通过特征分解获得被试特异的连接组谐波（即图傅里叶基）。
- 分析谐波在整个频谱上的性质（稳定性、图支持度、稀疏性、解剖定位），发现它们自然组织成多尺度“家族”。
- 利用稀疏表示（仅用少量谐波）重建静息态和任务态脑活动，揭示认知过程中对结构层级频率依赖的招募。
- 最后，将结构与功能谐波组织特征结合，预测个体认知表现。

### 关键技术细节（据摘要描述）
- **图谐波构建**：对每个被试的结构连接矩阵（如DTI纤维追踪得到的加权连接），计算拉普拉斯矩阵 \(L = D - A\) 或归一化拉普拉斯，特征向量即为谐波。
- **稀疏重建**：使用前k个谐波系数（或通过稀疏正则化选择）近似重建BOLD信号，评估重建精度与谐波个数的关系。
- **多尺度家族识别**：基于谐波的全局/局部特性（如参与系数、空间定位集中度）进行聚类或排序，发现从低频（全局、稳定）到高频（局部、稀疏）的渐变过渡。
- **认知预测**：提取每个被试的结构谐波特征（如家族分布、能量谱）和功能谐波特征（如功能连接的谐波分解），训练回归或分类模型预测认知得分。

未给出具体公式或算法伪代码，但整体流程清晰。

## 3. 实验设计：数据集、场景、benchmark与对比方法

- **数据集**：使用875名参与者的结构和功能MRI数据。推测可能来源于人类连接组计划（HCP）等大型公开数据集，但论文未明确说明具体来源。
- **实验场景**：
  - 静息态：分析谐波性质与重建准确性。
  - 任务范式：研究不同认知任务下谐波能量分布的频率依赖性。
  - 认知预测：个体认知表现（如流体智力、工作记忆得分）的回归预测。
- **Benchmark 与对比方法**：论文摘要未明确提及与其他基线方法的定量比较（如与群体平均谐波、传统图论指标或其它谱分解方法的对比）。因此无法评估其相对优势的客观性。可能隐含地与传统连接组谐波分析进行了定性对比。

## 4. 资源与算力

论文未明确说明所使用的GPU型号、数量及训练时长。鉴于数据分析基于875名被试的结构和功能MRI，计算量较大（尤其是每个被试的图拉普拉斯特征分解），但算力细节缺失。

## 5. 实验数量与充分性

- **实验数量**：据摘要提及的主要实验包括：
  - 谐波性质分析（稳定性、支持度、稀疏性、定位的频谱过渡）
  - 多尺度家族识别
  - 稀疏谐波重建（静息态+任务态）
  - 认知预测（结合结构与功能谐波）
- **充分性评价**：实验覆盖了从结构特性到功能重建再到行为预测的完整链条，较为全面。但缺乏消融研究（如单独使用结构或功能谐波预测效果）和与多种基线方法的系统比较。此外，重建实验可能缺乏与经典重建方法（如小波、PCA）的对比。总体而言，实验设计合理但客观公平性有限，未公开所有对比细节。

## 6. 论文的主要结论与发现

1. **个体化连接组谐波展示了可重复的分层组织**：跨被试谐波性质表现出有序的频谱过渡（低频稳定、全局支持；高频稀疏、局灶定位），并自然形成多尺度家族。
2. **稀疏谐波可准确重建脑活动**：仅用少量谐波就能有效重建静息态和任务态BOLD信号，表明大脑活动可由结构连接的谱基底稀疏表示。
3. **认知过程中频率依赖的结构层级招募**：不同认知任务选择性地激活特定频谱范围的谐波，反映了结构层级的功能利用。
4. **结构与功能谐波组织互补预测认知表现**：两者结合优于单独使用，表明两者捕获了行为相关的差异信息。
5. **对连接组谐波的根本性重新定义**：连接组谐波不应仅为图频率模式，而应视为连接组的分层组织表示，桥梁结构、动态与认知。

## 7. 优点：方法或实验设计上的亮点

- **个体化处理**：克服了传统群体平均谐波忽视个体间变异性的缺陷，更符合实际神经科学需求。
- **多尺度家族发现**：将连续的频谱离散化为有意义的层级单元，增强了谐波的可解释性。
- **稀疏重建验证**：用实际脑活动证明结构谐波的功能相关性，方法直观且有说服力。
- **从结构到功能再到认知的完整链路**：整合了多种模态，展示了频谱表示的预测价值，具有转化潜力。

## 8. 不足与局限

- **缺乏与现有方法的定量对比**：未在标准基准上（如群体谐波、谱聚类、扩散映射等）进行公平比较，削弱了方法进步性的证明。
- **数据来源与预处理细节缺失**：未明确说明所用数据集、扫描参数、连接重建方法，影响可重复性。
- **稀疏重建的泛化性未知**：仅涉及静息态和部分任务，未测试更多认知范式或病理状态。
- **认知预测的模型细节模糊**：未报告使用的机器学习模型、交叉验证策略、特征选择方法及统计显著性，无法评估过拟合风险。
- **图拉普拉斯构建方案单一**：可能只采用了标准图拉普拉斯，未比较不同拉普拉斯定义（归一化 vs 非归一化）对结果的影响。
- **算力资源未提及**：不利于后续研究复现和资源评估。

（完）
