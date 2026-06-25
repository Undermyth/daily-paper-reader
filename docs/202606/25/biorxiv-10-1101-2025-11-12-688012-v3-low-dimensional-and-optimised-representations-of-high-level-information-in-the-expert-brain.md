---
title: Low-Dimensional and Optimised Representations of High-Level Information in the Expert Brain
title_zh: 专家大脑中高层信息的低维优化表征
authors: "Costantino, A. I., Platonov, A., Fontana Vieira, F., Van Hove, E., Bilalic, M., Op de Beeck, H."
date: 2026-06-22
pdf: "https://www.biorxiv.org/content/10.1101/2025.11.12.688012v3.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 专家大脑中的低维优化表征
tldr: 专家与新手的大脑表征有何不同？本研究以国际象棋为模型，结合功能磁共振成像与多变量模式分析，发现专家大脑的表征内容从表面视觉特征转变为高阶关系信息；表征结构从高维变为低维优化，更紧凑有序但保留细节；表征区域从感觉皮层转移到额顶网络。这些结果表明专家大脑用更少的神经空间编码更丰富的知识，支持快速灵活决策。
source: biorxiv
selection_source: fresh_fetch
motivation: 探索专家大脑如何通过特定神经表征实现高水平技能，以理解从新手到专家的转变机制。
method: 采用国际象棋任务，使用功能磁共振成像和多变量模式分析解析专家与新手大脑的表征差异。
result: 专家大脑的表征呈现三大变化：内容高阶化、结构低维优化、区域向额顶网络转移。
conclusion: 专家大脑将更多知识压缩到更少、更有组织的表征中，从而实现高效决策。
---

## 摘要
什么使新手转变为专家？数十年的研究表明，专业知识依赖于特定领域的知识，但这种转变的神经机制仍然零碎：我们不清楚专家表征编码了哪些信息，它们如何被组织以高效利用，以及它们在大脑中的位置。以国际象棋为模型系统，我们将神经影像与多变量模式分析相结合，揭示了专家大脑的三个原则。专业知识推动了表征内容从表面视觉特征向高层关系信息的转变。同时伴随着结构性的变化，即低维、优化的表征：编码变得更加紧凑和有序，但仍保留了精确评估所需的细节。最后，表征负荷从感觉特异性皮层转移到领域通用性的额顶网络。专家大脑将更多信息压缩到更少、组织更好的表征中，以支持快速、灵活的决策。

## Abstract
What transforms a novice into an expert? Decades of research show that expertise relies on domain-specific knowledge, but a neural account of this transformation has remained fragmentary: we lack an understanding of what information expert representations encode, how they are structured for efficient use, and where in the brain they reside. Using chess as a model system, we combine neuroimaging with multivariate pattern analysis to reveal three principles of the expert brain. Expertise drives a shift in representational content, from surface visual features to high-level, relational information. It is accompanied by a structural change to low-dimensional, optimised representation: codes become more compact and better organised, yet retain the detail needed for precise evaluation. Finally, the representational load shifts from sensory-specific cortices to domain-general frontoparietal networks. The expert brain packs more into less, concentrating richer knowledge into fewer, better-organised representations that support the rapid, flexible decisions of mastery.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：新手如何转变为专家？专家大脑中的知识表征在内容、结构、脑区分布上与新手有何本质区别？
- **研究背景**：已有行为研究表明专家依赖领域特定知识，但神经层面的转变机制尚不清晰。缺乏对专家表征“编码什么信息”、“如何组织”、“位于何处”的系统理解。
- **整体含义**：揭示专家大脑通过低维、优化的表征将更多知识压缩到更少的神经空间中，从而支持快速灵活的决策，为技能习得和教育提供神经基础。

### 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：以国际象棋为模型系统，利用功能磁共振成像（fMRI）结合多变量模式分析（MVPA）来解析专家与新手大脑表征的差异。
- **关键技术细节**：
  - 采用MVPA中的表征相似性分析（RSA）等方法，比较不同刺激条件下的神经激活模式，以推断表征的内容和结构。
  - 通过分析不同脑区的表征维度（低维 vs 高维）、组织程度（优化 vs 杂乱）以及信息类型（表面视觉特征 vs 关系信息）来量化表征差异。
  - 利用额顶网络（domain-general frontoparietal networks）与感觉特异性皮层的负荷转移作为区域变化指标。
- **公式或算法流程**：文中未提供具体公式或算法步骤，但MVPA的一般流程包括：提取体素激活模式、计算两两刺激之间的相似度矩阵、与行为或模型预测的相似度矩阵进行相关比较。

### 3. 实验设计：数据集、场景、基准、对比方法

- **数据集/场景**：使用国际象棋棋局作为刺激材料，包括不同复杂度和关系的棋局。受试者包括国际象棋专家（如大师级）和新手（或业余爱好者）。具体数量未在摘要中说明。
- **基准**：以新手表征作为基线，对比专家表征的变化。可能还包含随机棋局或控制条件。
- **对比方法**：无明确提到的其他方法对比，论文主要是通过自身分析揭示专家与新手的内在差异，可能未与其他机器学习或神经解码方法进行系统对比。

### 4. 资源与算力

- 文中未提及使用任何GPU、训练时长或计算资源。由于是fMRI研究，主要涉及磁共振扫描和后续的统计分析，一般不需要大规模深度学习算力。因此无法给出具体算力信息。

### 5. 实验数量与充分性

- **实验数量**：根据摘要，研究似乎围绕“三个原则”展开（内容高阶化、结构低维优化、区域转移），每个原则有对应的统计分析。但未明确说明进行了多少组独立实验或子分析。
- **充分性**：从摘要看，实验设计较为完整，但缺乏具体样本量、刺激数量和重复次数。由于期刊为预印本（biorxiv），且分数8.0较高，推测实验设计较严谨。但客观性方面：可能存在专家与新手的个体差异、棋局选择的代表性、以及fMRI分析中多重比较校正等问题，需阅读全文才能判断。整体而言，实验数量可能有限但对于揭示核心原则是充分的。

### 6. 论文的主要结论与发现

- **内容转变**：专业知识推动表征从表面视觉特征转向高层关系信息（如棋局结构、战术含义）。
- **结构优化**：专家表征呈现低维、紧凑、有序的结构，同时保留精确评估所需的细节（即“optimised”，优化而非简化）。
- **区域转移**：表征负荷从感觉特异性皮层（如视觉皮层）转移到领域通用性的额顶网络，支持更灵活的认知操作。
- **总体**：专家大脑将更多知识压缩到更少、组织更好的表征中，实现快速灵活决策。

### 7. 优点

- **多维度分析**：同时考察表征的内容、结构、脑区分布三个层面，提供了系统性的神经机制解释。
- **结合fMRI与MVPA**：既有高空间分辨率又能解码表征模式，适合研究抽象知识。
- **模型选择恰当**：国际象棋是研究专业知识的经典范式，便于控制刺激和量化专业知识。
- **发现具有普遍性**：低维优化表征原则可能适用于其他认知领域（如音乐、医学诊断），具有推广潜力。

### 8. 不足与局限

- **实验覆盖有限**：仅使用单一领域（国际象棋）和单一模态（fMRI），未在其他领域或使用其他神经成像技术（如EEG、MEG）验证。
- **偏差风险**：专家样本可能具有特殊性（如男性为主、高智商），新手组匹配可能不完美，存在混淆因素（如年龄、智力、动机）。
- **具体方法细节缺失**：摘要未给出刺激数量、被试人数、统计分析细节（如交叉验证、多重比较校正），无法完全评估实验的稳健性。
- **应用限制**：研究为横断面比较，无法直接推断因果关系（即训练如何导致表征变化）。纵向追踪或干预研究才能验证。
- **缺乏计算模型**：未构建计算模型来定量描述低维表征的形成过程。

（完）
