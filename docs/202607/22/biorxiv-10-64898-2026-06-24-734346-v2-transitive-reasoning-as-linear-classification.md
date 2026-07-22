---
title: Transitive reasoning as linear classification
title_zh: 传递性推理作为线性分类
authors: "Ferrera, V. P., Lippl, S., Kay, K., Munoz, F., Jin, Y., Jensen, G., Terrace, H."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.24.734346v2.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 传递推理作为线性分类
tldr: 传递推理（TI）被认为依赖于对项目的排序线性表示。本研究将TI问题转化为线性分类任务，使用最小二乘估计（LSE）学习一个线性分类器，该分类器将任务条件映射到行为结果。实验表明，该方法无需显式传递性或排序假设，即可重现TI的关键现象：训练集外的泛化能力和符号距离效应。分类器对单个项目的应用自然产生内部排序表示，并通过差分操作实现成对决策，挑战了传统认知机制观点。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734346-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1156, \"height\": 765, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734346-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1437, \"height\": 515, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734346-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1702, \"height\": 704, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734346-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1696, \"height\": 631, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734346-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1059, \"height\": 915, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734346-v2/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1023, \"height\": 698, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734346-v2/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 989, \"height\": 633, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-24-734346-v2/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 828, \"height\": 877, \"label\": \"Figure\"}]"
motivation: 探究传递推理是否可以通过简单的线性分类机制实现，而不需要复杂的认知假设。
method: 应用最小二乘估计（LSE）对序列学习任务进行线性分类器学习。
result: 成功重现了传递推理的泛化能力和符号距离效应，并自然生成内部排序表示。
conclusion: 传递推理可视为线性分类问题，挑战了传统认知机制的假设。
---

## 摘要
传递性推理（TI）是对有序项目集合中的传递关系进行推理的能力（例如，如果A>B且B>C，则A>C）。人们普遍认为，TI依赖于对这些项目的序列（等级）顺序的线性表征。在学习过程中，这种顺序是通过何种计算机制构建的，又是如何用于做出符合传递性的选择的？在这里，我们采用了一种极简主义方法，将最小二乘估计（LSE）应用于常用于测试人类和动物TI的序列学习任务。在这种表述中，LSE计算一个线性分类器，将任务条件映射到行为结果。该算法没有对传递性或序列顺序做出明确的假设，但它再现了TI的关键经验特征；即，超越训练集进行泛化的能力，以及表现准确度中的符号距离效应（SDE）。将分类器应用于单个项目会产生一个内部的等级有序表征，泛化和SDE都自然地从该表征中产生。该方法还产生了一个决策机制，以差分操作的形式，用于从任何一对中选择正确的项目。这些发现将TI重新定义为线性分类问题，挑战了关于传递性推理所需认知机制的传统假设。

## Abstract
Transitive inference (TI) is the ability to reason about transitive relationships in an ordered set of items (e.g., if A>B and B>C, then A>C). TI is widely held to depend on a linear representation of the serial (rank) order of those items. By what computational mechanism is such an ordering constructed during learning, and how is it used to make choices that obey transitivity? Here we take a minimalist approach, applying least-squares estimation (LSE) to a serial learning task commonly used to test TI in humans and animals. In this formulation, LSE computes a linear classifier that maps task conditions onto behavioral outcomes. This algorithm makes no explicit assumptions about transitivity or serial order, yet it reproduces key empirical features of TI; namely, the ability to generalize beyond the training set, and a symbolic distance effect (SDE) in performance accuracy. Applying the classifier to individual items produces an internally ordered representation of rank from which both generalization and the SDE naturally emerge. The approach also yields a decision mechanism, in the form of a differencing operation, for selecting the correct item from any pair. These findings reframe TI as a linear classification problem, challenging conventional assumptions about the cognitive mechanisms required for transitive reasoning.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）

- **研究动机**：传递性推理（Transitive Inference, TI）被认为是需要复杂认知机制（如构建心理线性表征）的高级推理能力。作者质疑这一传统假设，试图探究TI是否可以被更简单的计算框架——线性分类——所解释。
- **背景**：TI在人类和动物中广泛研究，已有多种计算模型（如强化学习、神经网络），但这些模型通常包含大量自由参数和复杂假设。作者希望从任务结构的数学本质出发，找出实现TI的最小必要条件。
- **整体含义**：论文表明，一个简单的、无自由参数的线性最小二乘估计（LSE）算法，无需显式假设传递性或顺序，就能再现TI的两个关键行为特征：泛化到未训练的非相邻对，以及符号距离效应（SDE）。这挑战了TI必须依赖“心理线”或逻辑规则的认知假设，将TI重新定义为线性分类问题。

### 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

- **核心思想**：将TI任务形式化为一个线性系统 \( \mathbf{W} \mathbf{x} = \mathbf{y} \)。其中：
  - \( \mathbf{W} \) 是任务设计矩阵，每一行对应一个训练试次（相邻刺激对及其空间配置），由两个刺激的特征向量拼接而成。
  - \( \mathbf{y} \) 是行为结果向量（如 +1 表示选择左侧刺激，-1 表示选择右侧刺激）。
  - \( \mathbf{x} \) 是要学习的线性分类器（权重向量）。
- **关键技术细节**：
  - 每个刺激用一个随机特征向量（“条形码”）表示，特征维度 \( p \geq n-1 \)（\( n \) 为刺激数量）。
  - 训练集仅包含相邻对（如 A/B, B/C, …），且每个对呈现两次以平衡左右位置。
  - 使用 Moore-Penrose 伪逆求解最小二乘解：\( \mathbf{x} = \text{pinv}(\mathbf{W}^\top \mathbf{W}) \mathbf{W}^\top \mathbf{y} \)。
  - 所得分类器具有反对称性（anti-symmetry），即上半部分与下半部分互为相反数，这自然实现了差分决策机制。
- **算法流程（文字说明）**：
  1. 生成 \( n \) 个刺激的随机特征向量（\( p \) 维）。
  2. 给每个刺激分配一个真实等级（A > B > ...）。
  3. 构造训练设计矩阵 \( \mathbf{W} \)：对每个相邻对（例如 A/B, B/A 两个方向），将左、右刺激的特征向量拼接成一行，共 \( 2(n-1) \) 行。
  4. 构造结果向量 \( \mathbf{y} \)：+1 表示正确选择左侧，-1 表示正确选择右侧。
  5. 计算线性分类器 \( \mathbf{x} \) 的伪逆解。
  6. **泛化**：对任意测试对（非相邻对），将左右刺激的特征向量拼接后与 \( \mathbf{x} \) 做内积，符号为正则选左，为负则选右。
  7. **符号距离效应**：内积的绝对值随两刺激的等级距离增大而增大。
- **决策机制**：由于分类器的反对称性，内积自动等于左刺激得分减右刺激得分，相当于差分操作。

### 3. 实验设计：使用了哪些数据集 / 场景，它的 benchmark 是什么，对比了哪些方法

- **数据集 / 场景**：全部为计算机模拟数据，没有使用真实生物实验数据。主要场景是标准的7项传递推理任务（6个相邻对训练，21个所有对测试）。此外还有：9项最小任务（无空间平衡）、添加噪声的任务、横向模式（闭环）对比、感知机增量学习。
- **Benchmark**：没有外部基准。作者自设标准：相邻对训练后能否正确分类所有非相邻对（泛化成功率）以及是否出现符号距离效应（内积大小与等级距离相关）。
- **对比方法**：
  - 未系统对比其他方法（如强化学习模型、神经网络），但提到感知机（Perceptron）也能收敛到类似LSE的解。
  - 对比了有/无空间平衡（indeterminacy实验）、有无噪声（噪声导致对称性破坏）、有无横向模式（闭环 vs 开环）。
  - 自身作为对比：同一任务下LSE batch解与感知机增量解的一致性。

### 4. 资源与算力：如果文中有提到，请总结使用了多少算力（GPU 型号、数量、训练时长等）。若未明确说明，也请指出这一点

- **未明确说明**：论文仅在方法中提到“Simulations were run in Matlab 2023b”，没有提及GPU型号、数量、分布式训练、训练时间等算力信息。所有模拟计算简单（矩阵伪逆计算），推测不需要大型计算资源。

### 5. 实验数量与充分性：大概做了多少组实验（如不同数据集、消融实验等），这些实验是否充分、是否客观、公平

- **实验数量**：共展示了6组主要模拟实验（对应图2-8），每组实验通常只呈现一次典型结果（未重复或统计）。具体包括：
  - 4项极简示例（图2，说明线性映射存在性）
  - 标准7项任务（图3-4）
  - 9项最小任务（无空间平衡，图5）
  - 噪声影响（图6，展示一次成功一次失败）
  - 横向模式对比（图7）
  - 感知机仿真（图8，展示学习曲线和权重收敛）
- **充分性评价**：
  - **优点**：实验覆盖了任务核心变体（有无空间平衡、有无噪声、开环/闭环），证明了线性分类的适用范围和边界。
  - **不足**：
    - 所有实验均为单次模拟，缺乏重复性和统计显著性检验。
    - 未与真实生物行为数据（如人类/猴子表现）进行对比或拟合，无法说明模型是否能定量解释实验数据。
    - 消融实验仅涉及任务层面（如空间平衡、闭环），未对刺激特征维度、噪声水平等进行系统扫描。
    - 无交叉验证或超参数搜索（因为模型无自由参数，除了描述长度 \( p \)，但 \( p \) 的选择未做敏感性分析）。
  - **公平性**：对比条件（如横向模式）明确区分了可解与不可解情形，客观展示了线性分类的局限性。

### 6. 论文的主要结论与发现

1. **线性分类解决TI**：最小二乘估计（LSE）学得的线性分类器，仅用相邻对训练，就能正确泛化到所有非相邻对，并产生符号距离效应。
2. **隐含的排序表示**：分类器对单个刺激的内积自然形成等级排序，相当于“心理线”。
3. **差分决策机制**：分类器的反对称性结构隐含了“左刺激得分减右刺激得分”的决策规则。
4. **空间平衡的必要性**：没有空间平衡时（每个对只呈现一次），任务设计矩阵不可逆，LSE解无法正确排序和泛化。
5. **噪声敏感性**：噪声可能破坏分类器的反对称性，导致泛化失败；对称性是成功的关键。
6. **横向模式（闭环）不可线性求解**：加入 G>A 对后，线性分类不再存在，表明线性可分性依赖于开环拓扑。
7. **感知机收敛到LSE解**：增量学习的感知机能渐进逼近LSE解，并表现出“灾难性改进”（从相邻对到非相邻对时性能突然提升）。

### 7. 优点：方法或实验设计上有哪些亮点

- **极简主义框架**：方法无自由参数（仅需刺激特征维度足够），透明可解析，从数学上揭示了TI任务本身的结构——线性可分性。
- **挑战传统认知假设**：直接表明“心理线”和差分机制是线性分类的必然结果，而非需要特别学习出的认知结构。
- **揭示任务结构的作用**：强调许多行为现象（泛化、SDE）可能源于任务本身的数学结构，而非模型的复杂性。
- **清晰的边界分析**：通过横向模式、无空间平衡等反例，明确了线性分类的适用条件，有助于理解真正需要非线性/更复杂机制的情形。
- **统一解释**：LSE与感知机结果一致，链接了批量学习与增量学习，增加了鲁棒性。

### 8. 不足与局限：包括实验覆盖、偏差风险、应用限制等

- **实验覆盖不充分**：
  - 仅用模拟数据，缺少与真实生物实验的定量比较（如准确率、反应时间分布）。
  - 未考虑学习过程中的错误反馈、遗忘、短期记忆等实际因素。
  - 噪声模型过于简单（独立同分布高斯噪声），而生物噪声可能具有结构。
- **偏差风险**：
  - 作者可能有意选择容易线性可分的数值示例（随机特征向量），未讨论特征维度与真实刺激（如图片像素）之间的非线性关系。虽然声称用图片也不改变结论，但未演示。
  - 仅测试了标准7项和9项任务，未测试更长列表（如15项）或其他变体（如非对称奖励）。
- **应用限制**：
  - 该框架仅适用于任务结构完全已知且静态的场景，无法直接解释学习过程中对未见过刺激的原始编码（如无特征向量时）。
  - 对生物神经系统是否真的能实现伪逆计算，未提供足够证据（虽引用Tapson & van Schaik 2013，但该工作仅为理论提议）。
  - 线性分类不能处理横向模式等“需要灵活重排序”的认知任务，因此不能作为通用推理模型。
- **缺乏统计稳健性**：无重复实验、无置信区间，结论基于单次演示。

（完）
