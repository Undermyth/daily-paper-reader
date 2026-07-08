---
title: "Representational geometry as a fidelity metric for connectome-constrained networks: evidence from the Drosophila visual system"
title_zh: 表征几何作为连接组约束网络的保真度度量：来自果蝇视觉系统的证据
authors: "Zhou, M. G., Hasler, J. O."
date: 2026-06-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.10.731214v8.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 表示几何作为生物保真度指标
tldr: 现有方法无法区分生物启发的神经回路与任意线路，因为行为匹配不能保证表征逼真。受此启发，文章提出用表征几何作为保真度指标，对果蝇视觉系统连接组约束网络进行表征相似性分析和中心核对齐。结果发现连接组约束网络生成光滑环形方向几何，随机网络无法复现，且更匹配生物数据；甚至未训练网络也体现方向几何先验。该指标仅需群体反应即可区分生物与随机线路，为皮层规模仿真保真度评估提供可行路径。
source: biorxiv
selection_source: fresh_fetch
motivation: 行为逼真度不足以保证神经表征的生物学保真度，需要能区分生物与随机线路的群体水平指标。
method: 对果蝇视觉系统连接组约束网络（Flyvis）进行表征相似性分析（RSA）和中心核对齐（CKA），与稳定随机基线比较。
result: 连接组约束网络产生光滑环形方向几何（RSA r=0.686-0.846），显著优于随机网络，且更匹配生物T4/T5细胞方向调谐（r=0.930 vs 0.603）。
conclusion: 表征几何可作为保真度指标，仅需群体反应即可区分生物与任意线路，为连接组仿真提供实用评估方法。
---

## 摘要
生物布线对神经计算的实际贡献是什么？行为实验可以测试模型是否产生正确的输出，但无法判断其内部表征是否具有生物学保真度。Brunton等人（2026）使这一点具体化：一个使用深度强化学习训练的秀丽隐杆线虫连接组产生了逼真的果蝇行走——然而该模型在生物学上是无意义的，因为行为保真度可以在没有生物学保真度的情况下实现。我们需要一个群体水平度量，能够区分真正的生物布线和任意布线，而不需要行为解码器。我们提出表征几何作为该度量。表征几何——群体对不同刺激的反应之间成对距离的结构——捕捉了神经电路如何组织其表征空间，而与其驱动的行为无关。我们将表征相似性分析（RSA）和中心核对齐（CKA）应用于Flyvis预训练的果蝇视觉系统集成（Lappalainen等人（2024））：50个架构固定为Flyvis连接组（基于部分电子显微镜源重建）的网络，与稳定性约束随机基线（保号权重混洗、通过拒绝采样确保动态稳定性，n=50）进行比较。

连接组约束网络产生平滑的圆形方向几何，随机网络无法复制：对于ON边缘刺激，RSA Spearman r = 0.686（p < 0.0001），对于ON+OFF边缘刺激，r = 0.846（p < 0.0001），CKA验证了结果（两项实验中p < 0.05）。该几何还跟踪了活体果蝇中记录的生物T4/T5方向调谐（Maisak等人2013）：连接组约束几何与生物学的匹配显著优于随机几何（r = 0.930 vs. r = 0.603，差值Δr = 0.327，p < 0.0001）。在每个刺激极性内，ON通路比OFF通路编码方向具有更强的几何分离（Δr = 0.138，95% CI [0.091, 0.236]）；我们将其报告为模型集成表征的属性，而非已建立的生物学差异：Maisak等人（2013）发现T4和T5在对比极性外功能等价。为解决训练混杂问题，我们将未训练网络与混洗基线进行比较：连接组先验在任务训练前已在集成水平塑造方向几何（r = 0.260，p = 0.041 和 r = 0.215，p = 0.048；两者均为边缘显著，未校正），表明布线编码了一种几何先验，训练后得到放大。

这些结果确立表征几何作为候选保真度度量，仅使用群体对结构化刺激集的响应即可区分生物布线与非生物布线，并为接近哺乳动物皮层的连接组尺度模拟提供了迈向保真度度量的实用路径。

## Abstract
What does biological wiring actually contribute to neural computation? Behavioral experiments can test whether a model produces the right outputs, but they cannot determine whether its internal representations are biologically faithful. Brunton et al. (2026) made this concrete: a C. elegans worm connectome trained with deep reinforcement learning produces realistic Drosophila fly walking -- yet the model is biologically meaningless, because behavioral fidelity is achievable without biological fidelity. We need a population-level metric that discriminates real biological wiring from arbitrary wiring, without requiring a behavioral decoder. We propose representational geometry as that metric. Representational geometry -- the structure of pairwise distances between population responses to different stimuli -- captures how a neural circuit organizes its representational space, independently of what behavior it drives. We apply representational similarity analysis (RSA) and centered kernel alignment (CKA) to the Flyvis pretrained Drosophila melanogaster visual system ensemble (Lappalainen et al. (2024)): 50 networks whose architecture is fixed to the Flyvis connectome (reconstructed from partial electron-microscopy sources), compared against stability-constrained random baselines (sign-preserving weight shuffles, rejection-sampled for dynamic stability, n = 50).

Connectome-constrained networks produce a smooth circular direction geometry that random networks cannot replicate: RSA Spearman r = 0.686 (p < 0.0001) for ON edge stimuli and r = 0.846 (p < 0.0001) for ON+OFF edge stimuli, corroborated by CKA (p < 0.05 in both experiments). The geometry also tracks biological T4/T5 direction tuning recorded in living flies (Maisak et al. 2013): connectome-constrained geometry matches biology substantially better than random geometry (r = 0.930 vs. r = 0.603, gap {triangleup}r = 0.327, p < 0.0001). Within each stimulus polarity, the ON pathway encodes direction with stronger geometric separation than the OFF pathway ({triangleup}r = 0.138, 95% CI [0.091, 0.236]); we report this as a property of the model ensembles representations rather than an established biological difference: Maisak et al. (2013) find T4 and T5 functionally equivalent except in contrast polarity. To address the training confound, we compared untrained networks against shuffled baselines: the connectome prior shapes directional geometry at the ensemble level before any task training (r = 0.260, p = 0.041 and r = 0.215, p = 0.048; both marginal, uncorrected), suggesting wiring encodes a geometric prior that training amplifies.

These results establish representational geometry as a candidate fidelity metric that discriminates biological from arbitrary wiring using only population responses to a structured stimulus set, and suggest a practical path toward fidelity metrics for connectome-scale emulations approaching mammalian cortex.