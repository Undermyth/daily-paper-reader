---
title: Condition-Dependent Noise Correlations without Condition-Dependent Spike Counts
title_zh: 依赖条件的噪声相关性不需要依赖条件的尖峰计数
authors: "Kim, D., Panichello, M., Moore, T."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.08.723078v4.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 检查前额叶神经元群体中噪声相关性作为条件依赖信息的潜在来源，与突触可塑性机制相关
tldr: 噪声相关性（NCs）通常被认为与神经元发放数（SCs）的条件选择性相关。本研究通过猕猴前额叶皮层记录，发现即使在没有SC条件选择性的神经元对中，NCs也表现出条件依赖性，且幅度与有选择性者相当。这表明NCs可独立于SCs编码条件信息，为神经编码提供新维度。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-08-723078-v4/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1724, \"height\": 776, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-08-723078-v4/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1293, \"height\": 775, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-08-723078-v4/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1704, \"height\": 923, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-08-723078-v4/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1704, \"height\": 923, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-08-723078-v4/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1730, \"height\": 677, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-08-723078-v4/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1722, \"height\": 868, \"label\": \"Figure\"}]"
motivation: 探究噪声相关性（NCs）是否能在缺乏发放数（SCs）条件依赖性的情况下，单独携带条件信息。
method: 记录猕猴前额叶皮层在执行空间延迟反应任务（含视觉、记忆、运动阶段）时的大种群活动，分析神经元对的SCs和NCs条件依赖性。
result: 发现无SC选择性的神经元对仍表现出条件依赖的NCs，且其幅度与有SC选择性的神经元对大体相当。
conclusion: 噪声相关性可以独立于发放数的条件依赖性，作为神经编码中条件信息的额外来源。
---

## 摘要
大脑编码信息和控制行为的能力依赖于大型分布神经群体的协调活动。相同条件下跨试次的神经元尖峰活动相关性，即噪声相关性（NCs），被认为是共享突触连接的反映，也是影响神经群体信息容量的因素。NCs对编码的影响通常是在尖峰计数（SCs）表现出强烈条件依赖信息的神经元群体中考虑的。然而，理论研究表明，NCs可能提供独立于SCs的条件依赖信息源。我们检查了猕猴在执行包含视觉、记忆和运动期的空间延迟反应任务时前额叶皮层大型神经群体的活动。我们发现，在SCs中表现出视觉、记忆和运动选择性的神经元对，常常在其NCs中也表现出选择性，且独立于尖峰计数。然而，我们也发现，在不同任务期没有SC选择性的神经元对仍然表现出依赖条件的NCs。此外，我们发现无论是否有SC选择性，神经对之间的条件依赖NCs幅度大致相当。这些结果表明，即使在没有条件依赖性SCs的情况下，尖峰活动中的相关变异性也可以是条件依赖的。

## Abstract
The ability of the brain to encode information and control behavior depends on the coordinated activity of large and distributed neuronal populations. Correlations in neuronal spiking activity across trials of the same condition, or noise correlations (NCs), have been interpreted as a reflection of shared synaptic connectivity and as a contributing factor to the information capacity of neuronal populations. The impact of NCs on coding is most often considered in populations of neurons exhibiting robust condition-dependent information in their spike counts (SCs). However, theoretical work suggests that NCs could provide a source of condition-dependent information separate from SCs. We examined the activity of large neuronal populations in prefrontal cortex of macaques while they performed a spatial delayed response task composed of visual, memory, and motor epochs. We found that pairs of neurons that displayed visual, memory, and motor selectivity in their SCs often exhibited selectivity in their NCs, independent of spike count. However, we also found that pairs of neurons without SC selectivity during the different task epochs nonetheless exhibited condition-dependent NCs. Moreover, we found that the magnitude of condition-dependent NCs were largely comparable across neuronal pairs with or without SC selectivity. These results demonstrate that correlated variability in spiking activity can be condition-dependent even in the absence of condition-dependent SCs.

---

## 论文详细总结（自动生成）

### 论文详细中文总结

#### 1. 核心问题与整体含义（研究动机和背景）
- **核心问题**：噪声相关性（Noise Correlations, NCs）通常被认为与神经元尖峰计数（Spike Counts, SCs）的条件选择性相关，但理论预示NCs可能作为独立于SCs的条件信息源。本研究旨在验证：在没有SC条件选择性的神经元对中，NCs是否仍然能表现出条件依赖性，从而提供额外编码维度。
- **研究背景**：传统观点认为神经编码主要通过平均发放率进行，但忽略试次间波动的相关结构。NCs反映共享突触输入并影响群体信息容量。以往研究多关注SC选择性神经元中的NCs，而对非SC选择性神经元中NCs的条件依赖性质缺乏实证。本研究利用猕猴前额叶皮层（LPFC）大规模记录，填补这一空白。

#### 2. 方法论：核心思想、关键技术细节、公式或算法流程
- **核心思想**：通过线性回归模型检测NCs是否随条件（cue位置）变化，并与SC选择性独立。即使两个神经元均无SC选择性，其协方差仍可能依赖条件。
- **关键技术细节**：
  - **SC选择性分类**：使用多类线性SVM解码器（fitcecoc）分类8个cue位置，结合递归特征消融（recursive feature ablation）确定选择性神经元——当移除某个神经元后解码性能首次降至机会水平（12.5%）以下时，之前移除的神经元为“选择性”，之后为“非选择性”。
  - **NCs计算**：对每个任务期（Visual: 0-300ms; Delay: 400-1200ms; Motor: -125-0ms），将每个神经元的尖峰计数在每个cue条件内z-score标准化，然后计算配对皮尔逊相关系数 \( r_{sc} \)，即噪声相关性。
  - **条件依赖性检验**：对每个神经元对，建立线性回归模型：
\[
N_2 \sim \beta_0 + \beta_1 N_1 + \beta_2 (N_1 \times C)
\]
其中\( N_1, N_2 \)为z-score后的SC，\( C \)为cue位置的类别编码。若交互项\( \beta_2 \)显著（p<0.05，ANOVA F检验），则表明NCs受cue位置调制。
  - **空间距离分析**：计算神经元模板质心的欧氏距离，分析NCs随距离衰减。

#### 3. 实验设计：使用的数据集/场景、benchmark、对比方法
- **数据集**：
  - 3只雄性恒河猴（Monkey A, H, J），执行空间延迟反应任务（两种变体：Match-to-Sample和Memory-Guided Saccade），有8个可能cue位置。任务分为Visual、Delay、Motor三个时期。
  - 使用Neuropixels探针记录LPFC（area 8/9/46），共25 session，8225个神经元（平均329 ± 46个同时记录）。
- **Benchmark**：无外部基准方法，主要进行自身对照分析。对比组：
  - 选择性神经元对（S: 两神经元均为选择性）
  - 非选择性神经元对（NS: 两神经元均为非选择性）
  - 混合对（S×NS: 一个选择性，一个非选择性）
- **对比分析**：比较三类神经元对中条件依赖性NCs的比例，并检验与随机水平（5%）的差异，以及组间比例差异（卡方检验）。

#### 4. 资源与算力
- **未明确说明**：论文由Stanford University完成，未提及使用的GPU型号、数量或训练时长。分析主要依赖MATLAB和常规计算资源（用于SVM、回归、统计检验），未强调大规模算力需求。

#### 5. 实验数量与充分性
- **实验数量**：
  - 单神经元层面：分析了8225个神经元在各epoch的选择性比例（Visual 47.4%, Delay 44.3%, Motor 57.0%）。
  - 神经元对层面：对所有同时记录的神经元对计算NCs，并基于距离<1000μm的子集（约数千对）统计条件依赖性比例。
  - 每个epoch（Visual, Delay, Motor）独立分析，并对比三类配对（S, NS, Mixed）。
  - 还分析了空间距离对条件依赖性NCs的影响（图5），并进行了线性回归检验。
- **充分性评价**：
  - 实验设计合理，在多个epoch、多种配对类型中重复验证，统计检验（卡方、Spearman相关、线性回归）充足。
  - 控制了解码机会水平（12.5%），使用10折交叉验证，选择性和非选择性分类有明确阈值。
  - 但未报告试次数量，可能影响回归分析功效；仅做了静态cue位置条件，未涉及连续任务变量。
  - 总体客观且充分，但缺乏与其他动物或脑区的比较。

#### 6. 主要结论与发现
- **核心发现**：条件依赖性NCs不仅在SC选择性神经元对中存在，而且在SC非选择性神经元对中也广泛存在，且比例大致相当（图6）。例如，Visual和Motor epoch中非选择性对的比例甚至略高于选择性对。
- **空间依赖性**：条件依赖性NCs随神经元间距增大而显著衰减（图5），说明局部共享连接是关键。
- **跨epoch差异**：Motor epoch中条件依赖性NCs比例最高（尽管整体|r_sc|最小），推测与运动准备相关。
- **独立信息源**：NCs可独立于SCs编码任务条件，为群体编码提供额外维度，不能仅由共享输入的非条件驱动解释。

#### 7. 优点
- **技术亮点**：
  - 使用高密度Neuropixels探头同时记录数百个神经元，支持空间距离和共享连接分析。
  - 采用回归模型直接检验NCs的条件调制，避免传统平均后相关性方法。
  - 通过递归特征消融分离SC选择性，方法严格且可重复。
- **实验设计亮点**：
  - 覆盖多个任务期（视觉、记忆、运动），全面展示NCs条件依赖性的普适性。
  - 对比三种配对类型，清晰揭示选择性无关的NCs效应。
  - 引入空间距离衰减分析，强化机制解释（局部共享输入）。

#### 8. 不足与局限
- **实验覆盖**：
  - 仅涉及前额叶皮层一个脑区，缺乏对感觉皮层或运动皮层的比较。
  - 仅使用空间延迟反应任务，条件变量单一（8个cue位置），未测试其他类型条件（如特征、模态）。
- **偏差风险**：
  - 非选择性神经元的定义依赖于解码器性能，可能受分类器选择、交叉验证稳定性影响。
  - 未排除或控制试次内共变（如注视误差、瞳孔、行为反应）的混淆效应。
- **应用限制**：
  - 无法确定NCs条件依赖性的具体突触来源（局部/亚皮层/跨皮层）；仅提出推测（抑制性输入、GABA调制）。
  - 未量化NCs携带的信息量（需协方差估计，受试次限制），因而难以评估其对下游读取的实际贡献。
  - 样本量偏小（3只动物，25 session），可推广性有待更多个体验证。

（完）
