---
title: "Representational geometry as a fidelity metric for connectome-constrained networks: evidence from the Drosophila visual system"
title_zh: 表征几何作为连接组约束网络的保真度指标：来自果蝇视觉系统的证据
authors: "Zhou, M. G., Hasler, J. O."
date: 2026-06-24
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.10.731214v5.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 表征几何作为连接组网络的保真度度量
tldr: 行为保真度无法保证生物保真度，需群体水平内部表征度量。本文提出用表征几何作为保真度指标，对果蝇视觉系统Flyvis连接组约束网络与随机基线进行RSA/CKA分析。结果表明连接组约束网络产生平滑圆形方向几何，与生物T4/T5调谐高度一致，而随机网络不能。该指标可区分生物与任意连接，为连接组仿真提供保真度评估路径。
source: biorxiv
selection_source: fresh_fetch
motivation: 行为保真度无法区分生物连接与任意连接，需要内部表征水平的保真度度量。
method: 对Flyvis连接组约束网络与随机基线进行表征相似性分析（RSA和CKA）。
result: 连接组约束网络的方向调谐几何与生物数据高度一致，随机网络则不能。
conclusion: 表征几何可作为评估生物连接保真度的有效指标，适用于连接组仿真。
---

## 摘要
生物布线对神经计算的实际贡献是什么？行为实验可以测试模型是否产生正确的输出，但无法确定其内部表征是否具有生物保真度。Brunton等人（2026）将这一点具体化：使用深度强化学习训练的秀丽隐杆线虫连接组能够产生逼真的果蝇行走行为——但该模型在生物学上是无意义的，因为行为保真度可以在没有生物保真度的情况下实现。我们需要一个群体水平的指标，能够区分真实的生物布线与任意布线，而不需要行为解码器。

我们提出将表征几何作为该指标。表征几何——群体对不同刺激的反应之间的成对距离结构——捕捉了神经电路如何组织其表征空间，而与它驱动何种行为无关。我们将表征相似性分析（RSA）和中心核对齐（CKA）应用于Flyvis预训练的黑腹果蝇视觉系统集成（Lappalainen等人，2024）：50个网络，其架构固定为Flyvis连接组（从部分电子显微镜来源重建），并与稳定性约束的随机基线（保持符号的权重洗牌，通过动态稳定性拒绝采样，n=50）进行比较。

连接组约束的网络产生了一种平滑的圆形方向几何，随机网络无法复制：对于ON边缘刺激，RSA Spearman r = 0.686（p < 0.0001），对于ON+OFF边缘刺激，r = 0.846（p < 0.0001），CKA也证实了这一点（两次实验中p < 0.05）。该几何还追踪了活体果蝇中记录的生物T4/T5方向调谐（Maisak等人，2013）：连接组约束的几何与生物学的匹配程度显著优于随机几何（r = 0.930 vs. r = 0.603，差值Δr = 0.327，p < 0.0001）。在每个刺激极性内，ON通路比OFF通路编码方向具有更强的几何分离（Δr = 0.138，95% CI [0.091, 0.236]）；我们将其报告为模型集成表征的一个属性，而非已确立的生物学差异：Maisak等人（2013）发现T4和T5在功能上除了对比度极性外是等效的。为了解决训练混杂因素，我们比较了未训练网络与洗牌基线：连接组先验在任何任务训练之前就在集成水平上塑造了方向几何（r = 0.260，p = 0.041和r = 0.215，p = 0.048；两者均为边缘性，未校正），表明布线编码了一种几何先验，而训练将该先验放大。

这些结果确立了表征几何作为候选保真度指标，仅使用对结构化刺激集的群体反应就能区分生物布线与任意布线，并为接近哺乳动物皮层的连接组规模模拟提供了通向保真度指标的实用路径。

## Abstract
What does biological wiring actually contribute to neural computation? Behavioral experiments can test whether a model produces the right outputs, but they cannot determine whether its internal representations are biologically faithful. Brunton et al. (2026) made this concrete: a C. elegans worm connectome trained with deep reinforcement learning produces realistic Drosophila fly walking -- yet the model is biologically meaningless, because behavioral fidelity is achievable without biological fidelity. We need a population-level metric that discriminates real biological wiring from arbitrary wiring, without requiring a behavioral decoder.

We propose representational geometry as that metric. Representational geometry -- the structure of pairwise distances between population responses to different stimuli -- captures how a neural circuit organizes its representational space, independently of what behavior it drives. We apply representational similarity analysis (RSA) and centered kernel alignment (CKA) to the Flyvis pretrained Drosophila melanogaster visual system ensemble (Lappalainen et al. (2024)): 50 networks whose architecture is fixed to the Flyvis connectome (reconstructed from partial electron-microscopy sources), compared against stability-constrained random baselines (sign-preserving weight shuffles, rejection-sampled for dynamic stability, n = 50).

Connectome-constrained networks produce a smooth circular direction geometry that random networks cannot replicate: RSA Spearman r = 0.686 (p < 0.0001) for ON edge stimuli and r = 0.846 (p < 0.0001) for ON+OFF edge stimuli, corroborated by CKA (p < 0.05 in both experiments). The geometry also tracks biological T4/T5 direction tuning recorded in living flies (Maisak et al. 2013): connectome-constrained geometry matches biology substantially better than random geometry (r = 0.930 vs. r = 0.603, gap {Delta}r = 0.327, p < 0.0001). Within each stimulus polarity, the ON pathway encodes direction with stronger geometric separation than the OFF pathway ({Delta}r = 0.138, 95% CI [0.091, 0.236]); we report this as a property of the model ensembles representations rather than an established biological difference: Maisak et al. (2013) find T4 and T5 functionally equivalent except in contrast polarity. To address the training confound, we compared untrained networks against shuffled baselines: the connectome prior shapes directional geometry at the ensemble level before any task training (r = 0.260, p = 0.041 and r = 0.215, p = 0.048; both marginal, uncorrected), suggesting wiring encodes a geometric prior that training amplifies.

These results establish representational geometry as a candidate fidelity metric that discriminates biological from arbitrary wiring using only population responses to a structured stimulus set, and suggest a practical path toward fidelity metrics for connectome-scale emulations approaching mammalian cortex.