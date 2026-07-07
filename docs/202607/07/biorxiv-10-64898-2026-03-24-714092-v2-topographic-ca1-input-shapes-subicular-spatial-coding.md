---
title: Topographic CA1 input shapes subicular spatial coding
title_zh: 地形学CA1输入塑造下托空间编码
authors: "Sun, Y., Pederick, D. T., Xu, X., Luo, L., Giocomo, L. M."
date: 2026-07-06
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.24.714092v2.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: CA1拓扑输入塑造下托空间编码
tldr: 海马下托的空间编码依赖于CA1输入的拓扑组织，但其功能意义未知。研究利用latrophilin-2条件敲除小鼠选择性破坏CA1-下托拓扑投射，发现精确拓扑塑造下托空间编码的解剖分布但不影响单细胞调谐。破坏拓扑选择性损害边界向量编码与长期网络稳定性。表明CA1输入为下托空间图谱提供关键支架。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究CA1拓扑输入对下托空间编码功能的意义。
method: 在latrophilin-2条件敲除小鼠中破坏CA1-下托拓扑投射。
result: 破坏拓扑选择性损害边界向量编码及长期网络稳定性，单细胞调谐不变。
conclusion: CA1拓扑输入是组织下托空间编码不可或缺的支架。
---

## 摘要
地形学组织是海马回路的特点，但其功能意义仍不清楚。通过在latrophilin-2条件性敲除小鼠中选择性破坏CA1到下托的地形投射，我们发现精确的地形学塑造了下托空间编码的解剖分布，同时保持单细胞调谐。被破坏的地形学也选择性地损害了边界向量编码和长期网络稳定性。因此，CA1输入为组织下托空间图和动态提供了不可或缺的支架。

## Abstract
Topographic organization characterizes hippocampal circuits, yet its functional significance remains unclear. By selectively disrupting CA1-to-subiculum topographic projections in latrophilin-2 conditional knockout mice, we show that precise topography shapes the anatomical distribution of subicular spatial coding while preserving single-cell tuning. Disrupted topography also selectively impairs boundary vector coding and long-term network stability. Thus, CA1 inputs provide an indispensable scaffold for organizing subicular spatial maps and dynamics.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）

- **研究动机**：海马回路（尤其是CA1到海马下托）具有精确的拓扑组织（topographic organization），但这一解剖结构的功能意义长期未知。
- **核心问题**：CA1到下托的拓扑输入是否独立于内嗅皮层（EC）的贡献，塑造下托神经元的空间编码特性？
- **整体含义**：通过选择性破坏CA1→下托的拓扑投射，发现该地形学是组织下托空间编码分布、边界向量编码以及长期网络动态的关键支架，而单细胞空间调谐基本保留。这表明地形学不仅是一种解剖结构，更是功能性组织原则。

### 2. 方法论：核心思想、关键技术细节、算法流程

- **核心思想**：利用latrophilin-2（Lphn2）条件敲除小鼠，选择性地破坏CA1→下托的拓扑投射（而保留EC→下托通路完整），从而分离出CA1地形学对下托空间编码的独立贡献。
- **关键技术细节**：
  - **小鼠模型**：`Nts-Cre; Lphn2 fl/fl`（Lphn2 cKO）与同窝对照 `Nts-Cre; Lphn2 +/+`（Ctrl）。
  - **钙成像**：AAV1-CamKII-GCaMP6f注射至背侧下托，植入GRIN透镜，使用单光子（1P）微型显微镜（miniscope）在自由行为小鼠中记录。
  - **数据预处理**：
    - 运动校正（NoRMCorre）。
    - 使用CNMF-E提取钙信号，OASIS反卷积获得二值化尖峰事件。
    - 跨会话图像注册（刚性x-y平移）。
  - **细胞分类**：
    - **位置细胞**：基于空间信息与shuffle检验（95%分位），排除低发放率细胞。
    - **边界向量细胞（BVC）**：基于border score（>0.6）及墙壁覆盖度（>70%）。
    - **角细胞**：基于corner score（距离环境中心与最近角的距离比），并需通过shuffle显著性检验。
    - **头方向细胞**：基于Rayleigh向量长度（99%分位shuffle阈值）。
  - **解剖分布分析**：将成像视野对齐至脑中线，计算每个像素bin内位置细胞的密度，并将二维密度矩阵沿近远轴或尾头轴投影为一维分布，跨小鼠标准化后比较峰值位置。

### 3. 实验设计：数据集、场景、基准与对比方法

- **数据集与场景**：
  - **开放场序列**：方形（30cm×30cm）– 圆形（直径35cm）– 方形，连续三天，每天20分钟。
  - **穿梭箱**：两个相连的方形盒子（25cm×25cm），具有不同视觉与触觉线索，记录20分钟/天，共两天。
- **对比方法**：主要对比Lphn2 cKO与Ctrl基因型；未与其他方法或模型对比，属于基因型对照实验。
- **benchmark**：未使用外部标准数据集，所有分析基于内部对照与shuffle分布。

### 4. 资源与算力

- 文中明确提及使用的计算资源：
  - **硬件**：Stanford University的Sherlock HPC集群，每个任务使用8–12个CPU核心、600–700 GB RAM。
  - **软件**：MATLAB、CNMF-E、OASIS、NoRMCorre、自定义脚本。
- **未提及GPU型号与训练时长**：论文未说明是否使用GPU或具体的训练时间（因主要依赖CPU密集型矩阵计算与shuffle）。

### 5. 实验数量与充分性

- **实验数量**：
  - 共21只小鼠（Ctrl 10只，Lphn2 cKO 11只，其中1只cKO缺少圆形环境数据）。
  - 每个小鼠记录多个会话（方形×2、圆形×1、穿梭箱×2）。
  - 分析涵盖：位置细胞性质（比例、发放率、场大小、稳定性、重映射）、BVC比例、角细胞比例、头方向细胞、协调细胞集合。
- **统计分析**：配对/非配对Wilcoxon检验、双因素ANOVA with Sidak多重比较；所有检验基于个体小鼠水平（per-mouse）。
- **充分性**：
  - 实验覆盖多种空间编码类型和时间尺度（分钟–天）。
  - 通过shuffle控制假阳性，通过重复采样控制采样变异。
  - 进行了替代定义（如加入coherence准则）验证结果一致性。
- **客观性与公平性**：组间比较公平，对照充分；但未进行行为学测试（如记忆任务），无法评估功能后果。

### 6. 论文的主要结论与发现

1. **位置细胞解剖分布近端移位**：Lphn2 cKO中位置细胞密度峰值向近侧下托偏移，但单细胞调谐性质（发放率、空间信息、场大小、稳定性、重映射）无显著变化。
2. **边界向量细胞选择性受损**：BVC数量减少、平均发放率降低、跨会话稳定性下降，且其相对位置细胞的优势（更稳定）消失；角细胞不受影响。
3. **头方向细胞不受影响**：头方向细胞占比、调谐性质、解剖分布均无变化。
4. **长期协调集合重激活减少**：Lphn2 cKO中，跨日程（方形–圆形、方形–方形）的协调细胞集合匹配率显著下降，但同日穿梭箱两侧之间无差异，表明长期（数小时至数天）网络稳定性受损。

### 7. 优点：方法或实验设计上的亮点

- **精准扰动**：利用Lphn2条件敲除仅破坏CA1→下托的拓扑，保留EC→下托以及下托内其他通路，隔离了地形学的因果作用。
- **多层面分析**：从单细胞调谐、解剖分布、种群动态三个层面全面评估，且涵盖多种空间编码（位置、边界、角、头方向）。
- **严格的统计控制**：shuffle检验、跨会话匹配的shuffle阈值、重复随机采样以控制采样变异。
- **跨环境一致验证**：在方形、圆形、穿梭箱三种情境下重复解剖分布偏移，增强结论可靠性。

### 8. 不足与局限

- **间接效应无法完全排除**：Lphn2 cKO也导致下托→内侧乳头体（MMN）通路误靶，可能间接影响前丘脑→下托头方向回路，但头方向细胞未变，提示影响有限。
- **成像深度限制**：单光子成像主要记录下托深层细胞，浅层细胞特性可能不同。
- **行为学后果未评估**：未测试地形学破坏对空间记忆、导航等行为的影响。
- **样本量有限**：每基因型10–11只小鼠，且为预印本，尚未同行评议。
- **仅一个扰动工具**：仅使用Lphn2 cKO，未使用其他拓扑破坏手段（如Ten3敲除）进行交叉验证。

（完）
