---
title: "Representational geometry as a fidelity metric for connectome-constrained networks: evidence from the Drosophila visual system"
title_zh: 表示几何作为连接组约束网络的保真度度量：来自果蝇视觉系统的证据
authors: "Zhou, M. G., Hasler, J. O."
date: 2026-06-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.10.731214v4.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 表征几何作为连接组约束网络生物保真度的度量
tldr: 生物布线对神经计算的具体贡献难以仅通过行为测试评估，因为行为保真度不保证生物保真度。本文提出用表征几何（群体响应距离结构）作为保真度指标，对Flyvis果蝇视觉系统连接组约束网络（50个）和随机基线进行RSA和CKA分析。发现连接组网络产生平滑的圆形方向几何，随机网络无法复现，且几何与生物T4/T5方向调谐高度匹配（r=0.930 vs 0.603）。未训练的网络也展现几何先验（r≈0.24），表明布线编码几何先验，训练放大。因此表征几何能区分生物与任意布线，为连接组仿真提供保真度度量。
source: biorxiv
selection_source: fresh_fetch
motivation: 行为保真度不足以区分生物布线是否真实，需要群体水平指标。
method: 用RSA和CKA分析Flyvis连接组约束网络与随机基线的表征几何。
result: 连接组网络的方向几何显著更平滑且匹配生物数据（r=0.930），未训练网络已有几何先验。
conclusion: 表征几何可作为区分生物与任意布线的保真度指标。
---

## 摘要
生物布线对神经计算究竟有何贡献？行为实验可以检验模型是否产生正确的输出，但无法确定其内部表示是否具有生物学保真度。Brunton等人（2026）具体化这一问题：用深度强化学习训练的秀丽隐杆线虫连接组生成了逼真的果蝇行走行为——然而该模型在生物学上毫无意义，因为行为保真度可以在缺乏生物学保真度的情况下实现。我们需要一个群体层面的度量，能够区分真实的生物布线与任意布线，而不需要行为解码器。

我们提出将表示几何作为该度量。表示几何——群体对不同刺激的反应之间成对距离的结构——捕捉了神经回路如何组织其表示空间，独立于其驱动的行为。我们将表示相似性分析（RSA）和中心核对齐（CKA）应用于Flyvis预训练的果蝇视觉系统集合（Lappalainen等人，2024）：50个网络，其架构固定为Flyvis连接组（从部分电子显微镜数据重建），与稳定性约束的随机基线（保持符号的权重洗牌，拒绝采样以确保动态稳定性，n=50）进行比较。

连接组约束网络产生平滑的圆形方向几何，随机网络无法复制：对于ON边缘刺激，RSA Spearman r=0.686（p<0.0001），对于ON+OFF边缘刺激，r=0.846（p<0.0001），CKA验证了结果（两个实验中p<0.05）。该几何还跟踪了活体果蝇中记录的生物T4/T5方向调谐（Maisak等人，2013）：连接组约束几何比随机几何更接近生物学（r=0.930对比r=0.603，差值Δr=0.327，p<0.0001）。在每个刺激极性内，ON通路比OFF通路编码方向时具有更强的几何分离（Δr=0.138，95% CI [0.091, 0.236]）；我们将其报告为模型集成表示的一个属性，而非已确立的生物学差异：Maisak等人（2013）发现T4和T5除了对比度极性外功能等效。为了解决训练混淆，我们将未训练的网络与洗牌基线进行比较：连接组先验在任何任务训练之前就在集成层面塑造了方向几何（r=0.260，p=0.041和r=0.215，p=0.048；均呈边缘显著，未校正），表明布线编码了一种被训练放大的几何先验。

这些结果确立了表示几何作为候选保真度度量，仅使用对结构化刺激集的群体反应即可区分生物布线与非生物布线，并为接近哺乳动物皮层的连接组规模仿真提供了一条通往保真度度量的实际路径。

## Abstract
What does biological wiring actually contribute to neural computation? Behavioral experiments can test whether a model produces the right outputs, but they cannot determine whether its internal representations are biologically faithful. Brunton et al. (2026) made this concrete: a C. elegans worm connectome trained with deep reinforcement learning produces realistic Drosophila fly walking -- yet the model is biologically meaningless, because behavioral fidelity is achievable without biological fidelity. We need a population-level metric that discriminates real biological wiring from arbitrary wiring, without requiring a behavioral decoder.

We propose representational geometry as that metric. Representational geometry -- the structure of pairwise distances between population responses to different stimuli -- captures how a neural circuit organizes its representational space, independently of what behavior it drives. We apply representational similarity analysis (RSA) and centered kernel alignment (CKA) to the Flyvis pretrained Drosophila melanogaster visual system ensemble (Lappalainen et al. (2024)): 50 networks whose architecture is fixed to the Flyvis connectome (reconstructed from partial electron-microscopy sources), compared against stability-constrained random baselines (sign-preserving weight shuffles, rejection-sampled for dynamic stability, n = 50).

Connectome-constrained networks produce a smooth circular direction geometry that random networks cannot replicate: RSA Spearman r = 0.686 (p < 0.0001) for ON edge stimuli and r = 0.846 (p < 0.0001) for ON+OFF edge stimuli, corroborated by CKA (p < 0.05 in both experiments). The geometry also tracks biological T4/T5 direction tuning recorded in living flies (Maisak et al. 2013): connectome-constrained geometry matches biology substantially better than random geometry (r = 0.930 vs. r = 0.603, gap {Delta}r = 0.327, p < 0.0001). Within each stimulus polarity, the ON pathway encodes direction with stronger geometric separation than the OFF pathway ({Delta}r = 0.138, 95% CI [0.091, 0.236]); we report this as a property of the model ensembles representations rather than an established biological difference: Maisak et al. (2013) find T4 and T5 functionally equivalent except in contrast polarity. To address the training confound, we compared untrained networks against shuffled baselines: the connectome prior shapes directional geometry at the ensemble level before any task training (r = 0.260, p = 0.041 and r = 0.215, p = 0.048; both marginal, uncorrected), suggesting wiring encodes a geometric prior that training amplifies.

These results establish representational geometry as a candidate fidelity metric that discriminates biological from arbitrary wiring using only population responses to a structured stimulus set, and suggest a practical path toward fidelity metrics for connectome-scale emulations approaching mammalian cortex.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）
- **核心问题**：生物布线（connectome）对神经计算的具体贡献难以通过行为测试评估，因为行为保真度可以在缺乏生物学保真度的情况下实现（如Brunton et al. 2026所示：用秀丽隐杆线虫连接组训练出的模型可产生逼真的果蝇行走行为，但生物学上无意义）。需要一种不依赖行为解码器的群体层面度量，能够区分真实的生物布线与非生物（任意）布线。
- **整体含义**：提出将**表示几何**（representational geometry）——群体对不同刺激响应之间成对距离的结构——作为候选保真度度量，用于判断连接组约束的网络是否具有生物学真实内部表示。

## 2. 提出的方法论：核心思想、关键技术细节
- **核心思想**：表示几何捕捉神经回路如何组织其表示空间，独立于其驱动的行为。通过比较连接组约束网络与随机基线网络的表示几何，并与活体生物数据对比，评估保真度。
- **关键技术细节**：
  - 使用**表示相似性分析（RSA）**：计算不同刺激条件下群体响应成对距离矩阵，通过Spearman秩相关比较不同网络几何的相似性。
  - 使用**中心核对齐（CKA）**：另一种度量表示相似性的方法，作为RSA的验证。
  - 网络来源：Flyvis预训练果蝇视觉系统集合（50个连接组约束网络，架构固定为Flyvis连接组）。
  - 随机基线：保持符号的权重洗牌（sign-preserving weight shuffles），并通过拒绝采样确保动态稳定性，共50个网络。
  - 刺激：ON边缘、ON+OFF边缘。
  - 生物基准：活体果蝇T4/T5方向调谐记录（Maisak et al. 2013）。

## 3. 实验设计
- **数据集/场景**：
  - Flyvis预训练果蝇视觉系统集合（50个连接组约束网络）。
  - 50个稳定性约束随机基线网络。
  - 刺激类型：ON边缘刺激、ON+OFF边缘刺激。
  - 生物数据：Maisak et al. 2013记录的T4/T5方向调谐曲线。
- **Benchmark**：以活体生物数据的方向调谐几何作为真实基准，衡量连接组网络与随机网络的接近度。
- **对比方法**：
  - 连接组约束网络 vs. 随机基线网络（RSA与CKA比较）。
  - 连接组网络 vs. 随机网络 vs. 生物数据（方向调谐几何匹配度，r值）。
  - 未训练连接组网络 vs. 洗牌基线（检验布线先验的作用）。

## 4. 资源与算力
- 论文未明确说明使用的GPU型号、数量、训练时长等计算资源信息。仅提及使用了预训练模型，但训练细节未披露。

## 5. 实验数量与充分性
- **实验组数**：
  - 主要比较：连接组约束网络（n=50）与随机基线（n=50）在ON和ON+OFF刺激下的RSA和CKA。
  - 生物匹配度比较：连接组几何 vs. 随机几何 vs. 生物数据（T4/T5调谐），计算相关系数r及差异显著性。
  - 未训练网络消融：未训练连接组网络（n=50）与洗牌基线（n=50）比较。
- **充分性评价**：实验结果提供了统计检验（p值、95% CI），方法稳健，但仅针对果蝇视觉系统单一系统。两个独立刺激条件以及CKA验证增加了可靠性。未训练网络消融有助于排除训练混淆。但未与其他保真度度量（如行为解码、神经预测）做直接比较，且未涉及跨物种或不同脑区的验证。整体而言，实验设计较充分，但泛化性有待更多数据检验。

## 6. 主要结论与发现
- **连接组约束网络产生平滑圆形方向几何**：RSA Spearman r=0.686（ON边缘，p<0.0001）、r=0.846（ON+OFF边缘，p<0.0001），CKA验证一致（p<0.05），而随机网络无法复制该几何。
- **连接组几何更接近生物数据**：连接组网络与T4/T5方向调谐几何匹配度r=0.930，随机网络仅r=0.603，差异Δr=0.327（p<0.0001）。
- **ON通路方向几何分离更强**：在模型集成中ON通路比OFF通路有更强的方向几何分离（Δr=0.138，95% CI [0.091, 0.236]），但作者谨慎表示此差异为模型属性，而非已确立的生物学差异。
- **未训练网络已具有几何先验**：连接组先验在任务训练前即塑造了方向几何（r=0.260，p=0.041；r=0.215，p=0.048），但边缘显著，未校正。说明布线编码几何先验，训练放大这种几何。
- **结论**：表示几何可作为区分钟生物布线与任意布线的保真度度量，仅需结构化刺激集下的群体反应，为连接组仿真的保真度评估提供了可行路径。

## 7. 优点
- **方法新颖**：不依赖行为解码或完整神经活动预测，仅利用群体响应内部结构，易于计算和比较。
- **生物验证**：直接与活体神经记录（T4/T5方向调谐）对比，提供生物学真实性验证。
- **消融充分**：分析了未训练网络，区分了布线先验与训练放大的贡献。
- **统计严谨**：使用多种度量（RSA、CKA）、置信区间和假设检验，结果可靠。
- **实用性强**：为未来大规模连接组仿真（如哺乳动物皮层）提供了一种实际的保真度指标候选。

## 8. 不足与局限
- **实验覆盖**：仅针对果蝇视觉系统的方向调谐，未测试其他刺激维度的几何（如颜色、对比度、运动速度等），也未验证其他脑区或物种的泛化性。
- **未训练网络结果边缘显著**：p值接近0.05且未校正多重比较，统计稳定性偏弱，需更多样本或更严格的验证。
- **ON/OFF差异的生物学解释存疑**：作者指出现有文献显示T4和T5除对比度极性外功能等效，因此模型中的差异可能源于模型构建的偏差而非真实生物学。
- **与其他指标缺乏比较**：未比较表征几何与行为保真度、神经预测误差等传统度量的一致性，其优劣尚不明确。
- **计算资源缺失**：未报告训练或分析所需的算力，影响可重复性和可扩展性评估。
- **应用限制**：该方法要求有结构化刺激集和群体记录数据，对于缺乏详细记录的系统可能难以直接应用。

（完）
