---
title: "Representational geometry as a fidelity metric for connectome-constrained networks: evidence from the Drosophila visual system"
title_zh: 表征几何作为连接组约束网络的保真度指标：来自果蝇视觉系统的证据
authors: "Zhou, M. G., Hasler, J. O."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.10.731214v10.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 计算神经科学中评估神经表征生物保真度的方法。
tldr: 神经回路中生物布线对计算的具体贡献难以评估，行为保真度不足以判断模型是否具备生物学意义。本文提出以表征几何——群体响应的距离结构——作为保真度度量，对果蝇视觉系统的连接组约束网络（Flyvis）进行RSA和CKA分析。发现连接组约束网络产生平滑的圆形方向几何（RSA r=0.686），随机网络无法复制，且与生物T4/T5方向调谐高度匹配（r=0.930 vs 0.603）。即使未训练，连接组已提供几何先验（r=0.260）。该度量仅需结构化刺激下的群体响应即可区分生物与非生物布线，为大规模连接组仿真的保真度评估提供了实用路径。
source: biorxiv
selection_source: fresh_fetch
motivation: 需要一种无需行为解码器的种群级度量，区分真实生物布线与非生物布线，避免行为保真度的误导。
method: 对50个连接组约束网络和随机基线（符合同等动态稳定性），应用RSA和CKA量化表征几何结构。
result: 连接组约束网络产生平滑圆形方向几何（RSA r=0.686，p<0.0001），与生物T4/T5调谐匹配更好（r=0.930 vs 0.603）；未训练网络也显示几何先验。
conclusion: 表征几何可作为连接组仿真保真度的有效度量，仅凭群体响应即可区分生物与非生物布线。
---

## 摘要
生物布线究竟对神经计算有何贡献？行为实验可以测试模型是否产生正确的输出，但无法确定其内部表征是否具有生物学保真度。Brunton等人（2026）将这一点具体化：用深度强化学习训练的秀丽隐杆线虫连接组产生了逼真的黑腹果蝇行走行为——然而该模型在生物学上是无意义的，因为行为保真度可以在没有生物学保真度的情况下实现。我们需要一个群体水平的指标来区分真实的生物布线与任意布线，而无需行为解码器。我们提出表征几何作为该指标。表征几何——群体对不同刺激响应的成对距离结构——捕捉了神经回路如何组织其表征空间，独立于其驱动的行为。我们将表征相似性分析（RSA）和中心核对齐（CKA）应用于Flyvis预训练的黑腹果蝇视觉系统集成（Lappalainen等人，2024）：50个网络，其架构固定为Flyvis连接组（从部分电子显微镜来源重建），与稳定性约束的随机基线（保留符号的权重混洗，通过拒绝采样确保动态稳定性，n = 50）进行比较。

连接组约束的网络产生了平滑的圆形方向几何，随机网络无法复制：对于ON边缘刺激，RSA Spearman r = 0.686（p < 0.0001），对于ON+OFF边缘刺激，r = 0.846（p < 0.0001），CKA证实了这一点（两项实验p < 0.05）。该几何还追踪了活体果蝇中记录的生物T4/T5方向调谐（Maisak等人，2013）：连接组约束的几何与生物学的匹配显著优于随机几何（r = 0.930 对 r = 0.603，差值Δr = 0.327，p < 0.0001）。在每个刺激极性内，ON通路编码方向具有比OFF通路更强的几何分离（Δr = 0.138，95% CI [0.091, 0.236]）；我们报告这是模型集成表征的一个属性，而非已确立的生物学差异：Maisak等人（2013）发现T4和T5在对比极性之外功能等效。为了解决训练混淆问题，我们将未训练的网络与混洗基线进行比较：在任意任务训练之前，连接组先验在集成水平上塑造了方向几何（r = 0.260，p = 0.041和r = 0.215，p = 0.048；均边缘显著，未校正），表明布线编码了一种几何先验，训练放大了该先验。

这些结果确立了表征几何作为一种候选的保真度指标，仅使用对结构化刺激集的群体响应即可区分生物布线与非生物布线，并为接近哺乳动物皮层规模的连接组仿真提供了一条通往保真度指标的实用路径。

## Abstract
What does biological wiring actually contribute to neural computation? Behavioral experiments can test whether a model produces the right outputs, but they cannot determine whether its internal representations are biologically faithful. Brunton et al. (2026) made this concrete: a C. elegans worm connectome trained with deep reinforcement learning produces realistic Drosophila fly walking -- yet the model is biologically meaningless, because behavioral fidelity is achievable without biological fidelity. We need a population-level metric that discriminates real biological wiring from arbitrary wiring, without requiring a behavioral decoder. We propose representational geometry as that metric. Representational geometry -- the structure of pairwise distances between population responses to different stimuli -- captures how a neural circuit organizes its representational space, independently of what behavior it drives. We apply representational similarity analysis (RSA) and centered kernel alignment (CKA) to the Flyvis pretrained Drosophila melanogaster visual system ensemble (Lappalainen et al. (2024)): 50 networks whose architecture is fixed to the Flyvis connectome (reconstructed from partial electron-microscopy sources), compared against stability-constrained random baselines (sign-preserving weight shuffles, rejection-sampled for dynamic stability, n = 50).

Connectome-constrained networks produce a smooth circular direction geometry that random networks cannot replicate: RSA Spearman r = 0.686 (p < 0.0001) for ON edge stimuli and r = 0.846 (p < 0.0001) for ON+OFF edge stimuli, corroborated by CKA (p < 0.05 in both experiments). The geometry also tracks biological T4/T5 direction tuning recorded in living flies (Maisak et al. 2013): connectome-constrained geometry matches biology substantially better than random geometry (r = 0.930 vs. r = 0.603, gap {triangleup}r = 0.327, p < 0.0001). Within each stimulus polarity, the ON pathway encodes direction with stronger geometric separation than the OFF pathway ({triangleup}r = 0.138, 95% CI [0.091, 0.236]); we report this as a property of the model ensembles representations rather than an established biological difference: Maisak et al. (2013) find T4 and T5 functionally equivalent except in contrast polarity. To address the training confound, we compared untrained networks against shuffled baselines: the connectome prior shapes directional geometry at the ensemble level before any task training (r = 0.260, p = 0.041 and r = 0.215, p = 0.048; both marginal, uncorrected), suggesting wiring encodes a geometric prior that training amplifies.

These results establish representational geometry as a candidate fidelity metric that discriminates biological from arbitrary wiring using only population responses to a structured stimulus set, and suggest a practical path toward fidelity metrics for connectome-scale emulations approaching mammalian cortex.