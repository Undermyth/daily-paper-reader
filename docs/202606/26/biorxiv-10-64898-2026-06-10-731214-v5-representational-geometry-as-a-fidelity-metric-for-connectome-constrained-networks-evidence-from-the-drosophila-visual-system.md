---
title: "Representational geometry as a fidelity metric for connectome-constrained networks: evidence from the Drosophila visual system"
title_zh: 表征几何作为连接组约束网络的保真度指标：来自果蝇视觉系统的证据
authors: "Zhou, M. G., Hasler, J. O."
date: 2026-06-24
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.10.731214v5.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 提出表征几何作为连接组约束网络的保真度度量
tldr: 生物神经环路如何贡献于计算？行为保真度不能保证生物保真度。本文提出表征几何作为保真度量，通过结构化的刺激集下的群体响应距离结构来区分生物连接与任意连接。在果蝇视觉系统Flyvis模型上，连接组约束网络产生平滑的圆形方向几何，随机基线无法复制，且与活体T4/T5方向调谐高度匹配。结果证明表征几何能有效判别生物连接，为连接组规模仿真的保真评估提供实用路径。
source: biorxiv
selection_source: fresh_fetch
motivation: 行为保真度无法确保模型内部表征的生物真实性，亟需无需行为解码的群体水平保真度量。
method: 应用RSA和CKA比较Flyvis连接组约束网络与稳定性约束随机基线的表征几何结构，并用活体T4/T5调谐数据验证。
result: 连接组约束网络的方向几何显著优于随机基线（RSA r=0.686/0.846，CKA p<0.05），且与生物数据的匹配度远高（r=0.930 vs 0.603）。
conclusion: 表征几何可作为区分生物与任意连接保真度指标，且连接组先验在训练前已塑造方向几何，训练进一步增强。
---

## 摘要
生物布线究竟对神经计算有何贡献？行为实验可以测试模型是否产生正确的输出，但无法确定其内部表征是否具有生物学保真度。Brunton等人（2026）将此具体化：一只秀丽隐杆线虫的连接组经过深度强化学习训练后，产生了逼真的果蝇行走行为——然而该模型在生物学上毫无意义，因为行为保真度可以在没有生物学保真度的情况下实现。我们需要一种群体层面的指标，能够区分真实的生物布线与任意布线，且无需行为解码器。我们提出表征几何作为该指标。表征几何——群体对不同刺激的反应之间成对距离的结构——捕捉了神经回路如何组织其表征空间，独立于其驱动的行为。我们将表征相似性分析（RSA）和中心核对齐（CKA）应用于Flyvis预训练的果蝇视觉系统集成（Lappalainen等人，2024）：50个网络，其架构固定为Flyvis连接组（从部分电子显微镜来源重建），并与稳定性约束的随机基线（符号保持的权重打乱，通过动态稳定性进行拒绝采样，n = 50）进行比较。连接组约束网络产生平滑的圆形方向几何，随机网络无法复制：对于ON边缘刺激，RSA Spearman r = 0.686（p < 0.0001），对于ON+OFF边缘刺激，r = 0.846（p < 0.0001），CKA证实了这一点（两个实验p < 0.05）。该几何还跟踪了活体果蝇中记录的生物T4/T5方向调谐（Maisak等人，2013）：连接组约束几何比随机几何更好地匹配生物学（r = 0.930 vs. r = 0.603，差值Δr = 0.327，p < 0.0001）。在每个刺激极性内，ON通路编码的方向几何分离度优于OFF通路（Δr = 0.138，95% CI [0.091, 0.236]）；我们将其报告为模型集成表征的一个属性，而非已建立的生物学差异：Maisak等人（2013）发现T4和T5除了对比极性外功能等效。为了解决训练混杂因素，我们将未训练的网络与打乱基线进行比较：连接组先验在任何任务训练之前就在集成层面塑造了方向几何（r = 0.260，p = 0.041和r = 0.215，p = 0.048；两者都边缘显著，未校正），表明布线编码了训练放大的几何先验。这些结果确立了表征几何作为一个候选保真度指标，仅使用对结构化刺激集的群体反应即可区分生物布线与任意布线，并为接近哺乳动物皮层的连接组规模仿真提供了一条通向保真度指标的实用路径。

## Abstract
What does biological wiring actually contribute to neural computation? Behavioral experiments can test whether a model produces the right outputs, but they cannot determine whether its internal representations are biologically faithful. Brunton et al. (2026) made this concrete: a C. elegans worm connectome trained with deep reinforcement learning produces realistic Drosophila fly walking -- yet the model is biologically meaningless, because behavioral fidelity is achievable without biological fidelity. We need a population-level metric that discriminates real biological wiring from arbitrary wiring, without requiring a behavioral decoder. We propose representational geometry as that metric. Representational geometry -- the structure of pairwise distances between population responses to different stimuli -- captures how a neural circuit organizes its representational space, independently of what behavior it drives. We apply representational similarity analysis (RSA) and centered kernel alignment (CKA) to the Flyvis pretrained Drosophila melanogaster visual system ensemble (Lappalainen et al. 2024): 50 networks whose architecture is fixed to the Flyvis connectome (reconstructed from partial electron-microscopy sources), compared against stability-constrained random baselines (sign-preserving weight shuffles, rejection-sampled for dynamic stability, n = 50). Connectome-constrained networks produce a smooth circular direction geometry that random networks cannot replicate: RSA Spearman r = 0.686 (p < 0.0001) for ON edge stimuli and r = 0.846 (p < 0.0001) for ON+OFF edge stimuli, corroborated by CKA (p < 0.05 in both experiments). The geometry also tracks biological T4/T5 direction tuning recorded in living flies (Maisak et al. 2013): connectome-constrained geometry matches biology substantially better than random geometry (r = 0.930 vs. r = 0.603, gap {Delta}r = 0.327, p < 0.0001). Within each stimulus polarity, the ON pathway encodes direction with stronger geometric separation than the OFF pathway ({Delta}r = 0.138, 95% CI [0.091, 0.236]); we report this as a property of the model ensemble's representations rather than an established biological difference: Maisak et al. (2013) find T4 and T5 functionally equivalent except in contrast polarity. To address the training confound, we compared untrained networks against shuffled baselines: the connectome prior shapes directional geometry at the ensemble level before any task training (r = 0.260, p = 0.041 and r = 0.215, p = 0.048; both marginal, uncorrected), suggesting wiring encodes a geometric prior that training amplifies. These results establish representational geometry as a candidate fidelity metric that discriminates biological from arbitrary wiring using only population responses to a structured stimulus set, and suggest a practical path toward fidelity metrics for connectome-scale emulations approaching mammalian cortex.

---

## 论文详细总结（自动生成）

# 论文总结：Representational geometry as a fidelity metric for connectome-constrained networks

## 1. 核心问题与整体含义（研究动机和背景）

- **核心问题**：行为保真度（behavioral fidelity）是否足以衡量神经模型的生物学真实度？Brunton等人（2026）展示了反例：用线虫连接组通过深度强化学习训练出的模型能产生逼真的果蝇行走行为，但该模型在生物学上是无意义的——行为保真度可以在没有生物保真度的条件下实现。因此需要一种**无需行为解码器、在群体水平上区分真实生物布线与任意布线的保真度量**。
- **整体含义**：表征几何（representational geometry）——群体对不同刺激响应的成对距离的结构——能够捕捉神经回路如何组织其表征空间，独立于其驱动的行为。本文证明该几何可作为候选保真度指标，为连接组规模仿真提供实用的评估路径。

## 2. 方法论：核心思想、关键技术细节

- **核心思想**：利用表征相似性分析（RSA）和中心核对齐（CKA）比较连接组约束网络与随机基线的表征几何结构。如果连接组约束网络展现出的几何模式（如平滑的方向圆形结构）是随机网络无法复制的，则几何可作为一种保真信号。
- **关键技术与步骤**：
  - **网络模型**：使用Flyvis预训练的果蝇视觉系统集成（50个连接组约束的LIF网络，架构固定于FlyWire成年连接组，734个自由参数）。
  - **刺激**：MovingEdge数据集，速度19 deg/s，时长2s。实验1：ON边缘（12个方向，30°步长）；实验2：ON+OFF边缘（12方向×2极性=24条件）。
  - **群体向量**：每个模型对每个刺激，取所有细胞类型的峰值中央细胞电压，得到65维向量。
  - **构建RDM**：使用余弦距离计算成对刺激之间的群体响应不相似矩阵（RDM）。
  - **RSA度量**：用Spearman秩相关和Kendall τA比较两个RDM的上三角元素，显著性通过刺激标签置换检验（10,000次置换）。
  - **CKA验证**：线性CKA直接在原始激活矩阵上计算，提供独立的几何相似性验证。
  - **随机基线**：符号保持权重打乱（Shiu-style shuffle，保持兴奋/抑制身份），并经过动态稳定性拒绝采样（最多尝试100次），确保每个随机基线RDM来自真实群体响应。
  - **生物学参考**：基于Maisak等人T4/T5方向调谐数据，用von Mises调谐曲线（κ=2.5，HWHM≈67°）构建12×12生物RDM。对于ON+OFF情况，T4仅响应ON，T5仅响应OFF。
  - **未训练网络分析**：在梯度优化之前，对相同连接组架构施加随机高斯扰动生成50个实例，比较连接组约束与两种随机打乱（syn shuffle和sign shuffle）的几何。

## 3. 实验设计：数据集、Benchmark、对比方法

- **数据集与场景**：
  - 使用Flyvis预训练集成（50个连接组约束模型）和50个稳定性约束随机基线模型（由相同50个模型经符号保持权重打乱生成）。
  - 刺激：MovingEdge（ON边缘和ON+OFF边缘）。
  - 生物学基准：来自Maisak等人（2013）的T4/T5方向调谐测量数据（使用方波光栅，本文采用MovingEdge刺激，但方向调谐结构定性可比）。
- **Benchmark**：对比连接组约束网络（CC）与随机基线（Random）的RDM相似度，以及与生物参考RDM的匹配程度（Δr = r(CC vs Biology) - r(Random vs Biology)）。
- **对比方法**：
  - 主要对比：CC vs Random（RSA和CKA）
  - 生物学验证：CC vs Biology，Random vs Biology
  - 极性内分析：ON-ON和OFF-OFF子矩阵与圆形距离参考的相关性
  - 未训练条件：CC（未训练） vs syn shuffle vs sign shuffle
  - 鲁棒性检查：噪声白化RDM（Mahalanobis距离）、MDS可视化、UMAP集成分析

## 4. 资源与算力

- 文中说明：“Experiments 1, 2, and 4 were run on Google Colab with a T4 GPU. CKA validation and post-hoc analyses (MDS, whitened RDMs, UMAP) were run on CPU.” 未详细报告训练时长、GPU数量、总计算量等具体数据。因此算力资源较为有限（单T4 GPU），但实验规模较小（50个模型×少量刺激），计算需求不高。

## 5. 实验数量与充分性

- **实验组数**：本文包含主要实验4个（Exp1: ON边缘；Exp2: ON+OFF边缘及其极性内分析；Exp3: 生物参考比较；Exp4: 未训练网络），以及CKA验证、MDS、噪声白化RDM、UMAP等多组后验分析。
- **消融/对照**：使用稳定性约束随机基线（符号保持打乱）、未训练网络（分别比较syn shuffle和sign shuffle）、不同距离度量（余弦、欧几里得、Mahalanobis）、不同相似性度量（RSA、CKA）。
- **充分性评价**：
  - **优点**：实验设计系统，覆盖多个刺激集、度量方法、对照条件；进行了统计显著性检验（置换检验、bootstrap）和鲁棒性检查。
  - **不足**：生物参考仅包含T4/T5细胞（8/65），且刺激不匹配（光栅vs运动边缘）；未训练网络的几何信号仅边缘显著（p=0.041、0.048，未校正Bonferroni）；随机基线可能仍存在动态稳定性偏差；未验证跨任务或跨物种的泛化（仅限果蝇视觉系统）。总体实验设计较充分，但仍有局限性。

## 6. 主要结论与发现

- **核心发现**：连接组约束网络产生的表征几何（平滑圆形方向结构）是随机基线无法复制的，且与活体T4/T5方向调谐数据高度匹配（RSA r=0.930 vs 0.603，Δr=0.327）。该几何信号在RSA和CKA下均显著，且跨越多个实验条件。
- **极性内结果**：ON通路的方向几何分离度显著强于OFF通路（Δr=0.138，bootstrap 95% CI [0.091, 0.236]），这与已知T4/T5在方向选择性强度上的不对称性一致。
- **未训练网络**：连接组先验在训练前已在集成水平塑造了方向几何（尽管微弱且边缘显著），表明布线编码了几何先验，训练将其放大并聚焦到T4/T5相关几何。
- **总体结论**：表征几何可作为一种实用的、无需行为解码器的保真度指标，能够区分生物布线与任意布线。

## 7. 优点

- **方法创新**：提出表征几何作为保真度量，直接捕捉群体反应的组织结构，无需行为输出或单细胞记录，对实验者友好（仅需结构化刺激集）。
- **双验证**：使用RSA和CKA两种独立的几何相似性度量，增强可信度。
- **严谨的随机基线**：采用符号保持权重打乱并经过动态稳定性拒绝采样，确保随机基线反映真实的（稳定）群体响应，避免了动态不稳定引入的伪差异。
- **生物学验证**：直接与活体T4/T5调谐数据比较，并将绝对RSA值转化为与随机基线的差距（Δr），量化了连接组约束的额外贡献。
- **消融实验**：通过未训练网络分析，初步分离了布线本身与训练的影响。
- **鲁棒性检查**：包括噪声白化、MDS、UMAP、不同距离度量等，验证主要结果对分析选择的稳健性。

## 8. 不足与局限

- **生物学参考的局限性**：T4/T5参考仅覆盖65种细胞类型中的8种，且使用不同刺激（方波光栅vs运动边缘），限制了直接比较的可解释性。对于未训练网络，简化参考反而显示出虚假的随机网络优势。
- **训练混杂未完全解决**：未训练网络的几何信号边缘显著且未通过多重比较校正，因此无法确定方向几何是否完全来自先验。训练对几何的放大程度也未被量化。
- **统计力与样本量**：仅使用50个模型，噪声协方差估计病态（条件数~10^7），导致白化RDM结果敏感于正则化选择。
- **泛化性**：只测试了果蝇视觉系统、单一任务（光流估计）和单一模型族（Flyvis）。哺乳动物皮层（如小鼠V1）的初步模拟结果仅简要提及，未成为正式结果。
- **随机基线动态稳定性**：虽然进行了拒绝采样，但仍有部分随机模型产生接近溢出的激活，可能影响CKA bootstrap分布的双峰性。
- **计算资源**：实验在Google Colab T4 GPU上进行，算力较低，限制了大规模随机基线采样或更高维分析。
- **未报告关键细节**：如未报告训练过程的具体时长、超参数、模型收敛情况；未公开未训练网络的具体参数扰动分布。

（完）
