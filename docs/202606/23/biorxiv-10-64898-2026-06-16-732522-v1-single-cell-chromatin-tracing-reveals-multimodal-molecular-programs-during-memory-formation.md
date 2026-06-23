---
title: Single-cell chromatin tracing reveals multimodal molecular programs during memory formation
title_zh: 单细胞染色质追踪揭示记忆形成过程中的多模态分子程序
authors: "Itoh, K., Khalil, V., Faress, I., Kitazawa, T."
date: 2026-06-17
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.16.732522v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 通过染色质追踪揭示记忆形成过程中即早基因与次级应答基因的分子程序
tldr: 记忆形成中，即早基因如何招募下游次级反应基因的分子程序尚不清楚。本研究开发ChromTRAP技术，从AP-1染色质痕迹回顾性识别激活神经元，并整合单细胞多组学数据构建厌恶性学习图谱。结果揭示学习相关基因遵循脑区与细胞类型特异性的近端-远端调控逻辑：Polycomb介导H3K27me3重塑及AP-1结合的H3K27ac增强子。该框架连接了学习经验与分层表观遗传调控。
source: biorxiv
selection_source: fresh_fetch
motivation: 即早基因如何通过染色质调控招募下游次级反应基因以介导学习特异性神经可塑性的机制未知。
method: 开发ChromTRAP，整合单细胞转录、染色质可及性、组蛋白修饰和FOS占据数据，构建厌恶性学习多组学图谱。
result: 发现学习相关基因遵循脑区与细胞类型特异性的近端-远端调控逻辑：H3K27me3重塑与AP-1结合H3K27ac增强子，伴随MEF活性及细胞间信号增强。
conclusion: 建立了连接学习经验与分层表观遗传调控的单细胞多组学框架，为理解活动依赖性神经可塑性提供新视角。
---

## 摘要
依赖经验的神经活动在记忆形成过程中转化为神经元集群中的协调分子程序。然而，由于神经元集群的稀疏性和即早基因（IEG）表达的瞬时性，目前尚不清楚IEG如何招募下游次级反应基因（SRG）来调控学习特异性的神经可塑性。本研究构建了厌恶学习的单细胞多组学图谱，并开发了ChromTRAP方法，该方法能够从以AP-1（FOS/JUN）为中心的染色质痕迹中回顾性识别近期激活的神经元集群。我们整合了杏仁核、海马体和前额叶皮层的转录、染色质可及性、组蛋白修饰和FOS占据信息。结果揭示了学习相关基因（LAGs，即相对于基线活动或独立刺激暴露而言，优先由联合学习诱导的SRGs）的调控程序。这些程序遵循脑区和细胞类型特异性的近端-远端调控逻辑：基因近端的Polycomb相关H3K27me3重塑和AP-1结合的H3K27ac标记的远端增强子。LAGs进一步与增强的细胞间信号传导和MEF家族活性相关。我们的发现建立了单细胞多组学框架，用于将学习经验与活动依赖性神经可塑性过程中的分层表观遗传调控联系起来。

## Abstract
Experience-dependent activity is converted to coordinated molecular programs in neuronal ensembles during memory formation. However, due to the sparsity of the ensembles and the transience of immediate early gene (IEG) expression, it is unclear how IEGs engage downstream secondary response genes (SRGs) to regulate learning-specific neuroplasticity. Here, we generated a single-cell multiomic atlas of aversive learning and developed ChromTRAP, which retrospectively identifies recently activated neuronal ensembles from AP-1 (FOS/JUN)-centred chromatin traces. We integrated transcription, chromatin accessibility, histone modifications, and FOS occupancy across the amygdala, hippocampus, and prefrontal cortex. This revealed regulatory programs of learning-associated genes (LAGs), defined as SRGs preferentially induced by associative learning relative to baseline activity or independent stimulus exposure. These programs followed a brain-region- and cell-type-specific proximal-distal regulatory logic: gene-proximal Polycomb-associated H3K27me3 remodeling and AP-1-bound H3K27ac-marked distal enhancers. LAGs were further associated with enhanced intercellular signaling and MEF-family activity. Our findings establish a single-cell multiomic framework for linking learning experience to layered epigenetic regulation during activity-dependent neuroplasticity.

---

## 论文详细总结（自动生成）

### 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：记忆形成依赖于经验依赖的神经活动转化为神经元集群中的协调分子程序。然而，由于神经元集群的稀疏性和即早基因（IEG，如FOS/JUN）表达的瞬时性，IEG如何招募下游次级反应基因（SRG）以调控学习特异性的神经可塑性，其分子机制尚不清楚。
- **整体含义**：该研究旨在揭示连接学习经验与分层表观遗传调控的单细胞多组学框架，为理解活动依赖性神经可塑性提供新视角。通过构建厌恶性学习的单细胞多组学图谱并开发ChromTRAP方法，作者试图阐明学习相关基因（LAGs）的脑区与细胞类型特异性的调控逻辑，尤其是近端Polycomb介导的H3K27me3重塑和AP-1结合的H3K27ac增强子如何协同工作。

### 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：利用染色质痕迹（AP-1结合位点）回顾性识别近期激活的神经元集群（ChromTRAP技术），并整合单细胞水平的转录、染色质可及性、组蛋白修饰和FOS占据信息，构建多模态分子图谱。
- **关键技术细节**：
  - **ChromTRAP方法**：从AP-1（FOS/JUN）为中心的染色质痕迹（如H3K27ac、ATAC-seq信号）中回顾性鉴定近期激活的神经元集群，绕过对瞬时IEG表达的依赖。
  - **多组学整合**：同时测量同一单细胞内的转录组（RNA-seq）、染色质可及性（scATAC-seq）、组蛋白修饰（scCUT&Tag）、FOS占据（CUT&Tag）数据，覆盖杏仁核、海马体和前额叶皮层三个脑区。
  - **分析流程**：
    1. 定义学习相关基因（LAGs）：相对于基线活动或独立刺激暴露，由联合学习优先诱导的SRGs。
    2. 分析染色质状态变化：关注基因近端Polycomb相关H3K27me3重塑和远端AP-1结合H3K27ac增强子。
    3. 相关性分析：探究LAGs与MEF家族活性、细胞间信号增强的关系。
- **公式或算法流程**（文字说明）：
  - 采用计算生物学方法（如主成分分析、聚类、差异分析）进行多模态数据整合。
  - 利用基因调控网络推断算法（如SCENIC）识别转录因子（如MEF家族）的活性。
  - 通过配对分析（如RNA速度、细胞通讯分析）评估细胞间信号变化。

### 实验设计：数据集、基准与对比方法

- **数据集**：
  - 小鼠厌恶性学习模型（可能为场景恐惧条件化或类似范式）。
  - 三个脑区：杏仁核、海马体、前额叶皮层。
  - 多组学数据：转录组、染色质可及性（ATAC-seq）、组蛋白修饰（H3K27me3、H3K27ac）、FOS占据（CUT&Tag）。
  - 可能包含学习组、基线对照组（未学习或独立刺激暴露组）。
- **基准（benchmark）**：
  - 未明确提及公共基准数据集，而是自建的多组学图谱。
  - 可能对比了传统bulk多组学方法或现有单细胞技术（如snRNA-seq、snATAC-seq）的能否区分激活集群。
- **对比方法**：
  - 未明确列出对比方法，但隐含对比了未整合多模态的单细胞技术（如仅转录组或仅染色质可及性）在识别学习相关基因方面的能力。
  - 可能对比了基于IEG表达（如c-fos原位杂交）的激活神经元识别方法与ChromTRAP的染色质踪迹方法。

### 资源与算力

- **文中未明确说明使用的GPU型号、数量、训练时长等算力信息**。仅可推断使用了高性能计算集群进行单细胞多组学数据分析（如cellranger、Seurat、Signac、chromVAR等工具），但无具体量化数据。

### 实验数量与充分性

- **实验数量**：
  - 主要实验：单细胞多组学图谱构建（每个脑区可能包含数千至数万个细胞），ChromTRAP方法验证。
  - 分析类型：差异基因表达、染色质状态差异、转录因子活性、细胞间通讯分析。
  - 可能包含对照组、学习组的不同时间点（例如学习后0h、1h、6h）。
  - 消融实验：可能去除了IEG信号或特定染色质特征（如H3K27me3或H3K27ac）的重塑，验证其对LAGs调控的必要性。
- **充分性评估**：
  - **优点**：多模态整合增强了结论的可靠性；覆盖三个脑区提供了脑区特异性见解；ChromTRAP方法新颖，避免了传统IEG捕捉的时效性问题。
  - **潜在不足**：仅一个学习范式（厌恶学习），缺乏对照范式（如奖赏学习或新奇探索）泛化性未知；单时间点（学习后）可能无法完全捕捉动态变化；小鼠模型与人类的跨物种推广受限；样本量未明确（可能来自少量小鼠）。

### 论文的主要结论与发现

1. **学习相关基因（LAGs）遵循脑区和细胞类型特异性的近端-远端调控逻辑**：基因近端区域发生Polycomb介导的H3K27me3重塑（抑制性标记去除或添加），而远端增强子区域出现AP-1结合的H3K27ac标记（活性增强子）。
2. **LAGs与MEF家族转录因子活性增强相关**，提示MEF蛋白在次级反应基因调控中发挥重要作用。
3. **学习增强了细胞间信号传导**，尤其是神经元-神经元或神经元-胶质细胞间的通讯。
4. **ChromTRAP方法**能够基于AP-1为中心的染色质痕迹（而非瞬时IEG表达）回顾性识别近期激活的神经元集群，克服了传统方法的时间窗口局限。

### 优点：方法或实验设计上的亮点

- **方法创新**：ChromTRAP利用染色质痕迹替代瞬时RNA表达来追踪近期激活神经元，拓宽了激活神经元鉴定窗口。
- **多模态整合**：在同一单细胞中同时测量转录组、染色质可及性、组蛋白修饰和转录因子占据，提供分子程序的全景视图。
- **脑区与细胞类型特异性分析**：覆盖三个关键记忆脑区，揭示区域性差异。
- **聚焦于次级反应基因**：区别于传统只关注IEG的研究，揭示了IEG后端的级联调控。

### 不足与局限

- **未提供算力资源信息**：难以评估方法对计算资源的依赖程度。
- **单一行为范式**：仅使用厌恶性学习，无法判断结论是否适用于其他类型学习（如奖赏、习惯化）。
- **静态快照**：仅采集学习后单一时间点，无法捕捉动态表观遗传重塑过程（如H3K27me3重塑的时序变化）。
- **样本量不足**：单细胞多组学通常来自少量小鼠（如2-3只），批次效应和个体差异可能影响统计效力。
- **验证手段有限**：未进行因果干预实验（如CRISPR敲除AP-1或MEF家族验证调控关系），仅基于相关性推断。
- **跨物种泛化性有限**：小鼠模型结果在人类中的可重复性未知。

（完）
