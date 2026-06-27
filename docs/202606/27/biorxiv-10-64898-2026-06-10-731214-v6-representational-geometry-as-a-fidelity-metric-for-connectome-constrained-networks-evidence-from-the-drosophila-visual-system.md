---
title: "Representational geometry as a fidelity metric for connectome-constrained networks: evidence from the Drosophila visual system"
title_zh: 表征几何作为连接组约束网络的保真度度量：来自果蝇视觉系统的证据
authors: "Zhou, M. G., Hasler, J. O."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.10.731214v6.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 表征几何作为连接组约束网络的保真度指标
tldr: 仅靠行为保真度无法验证神经模型是否具有生物学意义。本文提出以表征几何作为群落级保真度指标，通过RSA和CKA分析果蝇视觉系统连接组约束网络（Flyvis）与随机基线。结果显示连接组约束网络产生平滑的方向几何，显著匹配真实生物T4/T5细胞调谐（r=0.930 vs 0.603），且未训练网络即存在几何先验。该指标无需行为解码即可区分生物与任意布线，为连接组规模仿真提供实用保真度评估路径。
source: biorxiv
selection_source: fresh_fetch
motivation: 行为保真度无法保证神经表示的真实性，需要不依赖行为解码的群落级保真度指标来区分生物与任意布线。
method: 运用表征几何指标，对Flyvis连接组约束网络与稳定性约束随机基线进行RSA和CKA相似性分析，并与真实T4/T5方向调谐数据比较。
result: 连接组约束网络产生随机网络无法复现的平滑圆形方向几何（RSA r=0.686-0.846），更贴近生物数据（r=0.930），且表征几何先验存在于未训练网络中。
conclusion: 表征几何可作为候选保真度指标，通过结构化刺激下种群响应区分生物与随机布线，并为连接组仿真提供评估工具。
---

## 摘要
生物布线实际上对神经计算有何贡献？行为实验可以测试模型是否产生正确的输出，但无法确定其内部表征是否具有生物学保真度。Brunton等人（2026）将这一点具体化：一个使用深度强化学习训练得到的秀丽隐杆线虫连接组模型能够产生逼真的果蝇行走行为——然而该模型在生物学上毫无意义，因为行为保真度可以在没有生物学保真度的情况下实现。我们需要一个群体层面的度量标准，能够区分真实的生物布线与任意布线，而不需要行为解码器。

我们提出将表征几何作为该度量标准。表征几何——群体对不同刺激的反应之间的成对距离结构——捕捉了神经电路如何组织其表征空间，独立于其所驱动的行为。我们将表征相似性分析（RSA）和中心核对齐（CKA）应用于Flyvis预训练的果蝇视觉系统集成（Lappalainen等人，2024）：50个网络，其架构固定为Flyvis连接组（从部分电子显微镜源重建），并与稳定性约束的随机基线（保持符号的权重洗牌，经动态稳定性拒绝采样，n=50）进行比较。

连接组约束的网络产生了一种平滑的圆形方向几何，随机网络无法复制：对于ON边缘刺激，RSA Spearman r = 0.686 (p < 0.0001)，对于ON+OFF边缘刺激，r = 0.846 (p < 0.0001)，并由CKA证实（两个实验均p < 0.05）。该几何结构还追踪了活果蝇中记录的生物学T4/T5方向调谐（Maisak等人，2013）：连接组约束几何比随机几何更好地匹配生物学（r = 0.930 对 r = 0.603，差值Δr = 0.327，p < 0.0001）。在每个刺激极性内，ON通路编码的方向几何分离度大于OFF通路（Δr = 0.138，95% CI [0.091, 0.236]）；我们将其报告为模型集成表征的一个属性，而非已确定的生物学差异：Maisak等人（2013）发现T4和T5除对比度极性外功能等效。为了解决训练混淆问题，我们将未训练网络与洗牌基线进行比较：连接组先验在任务训练之前就在集成层面塑造了方向几何（r = 0.260, p = 0.041 和 r = 0.215, p = 0.048；两者均边际显著，未校正），表明布线编码了一个几何先验，而训练放大了该先验。

这些结果确立了表征几何作为候选保真度度量，仅使用对结构化刺激集的群体反应即可区分生物布线与任意布线，并提出了朝着接近哺乳动物皮层的连接组尺度仿真保真度度量的实用路径。

## Abstract
What does biological wiring actually contribute to neural computation? Behavioral experiments can test whether a model produces the right outputs, but they cannot determine whether its internal representations are biologically faithful. Brunton et al. (2026) made this concrete: a C. elegans worm connectome trained with deep reinforcement learning produces realistic Drosophila fly walking -- yet the model is biologically meaningless, because behavioral fidelity is achievable without biological fidelity. We need a population-level metric that discriminates real biological wiring from arbitrary wiring, without requiring a behavioral decoder.

We propose representational geometry as that metric. Representational geometry -- the structure of pairwise distances between population responses to different stimuli -- captures how a neural circuit organizes its representational space, independently of what behavior it drives. We apply representational similarity analysis (RSA) and centered kernel alignment (CKA) to the Flyvis pretrained Drosophila melanogaster visual system ensemble (Lappalainen et al. (2024)): 50 networks whose architecture is fixed to the Flyvis connectome (reconstructed from partial electron-microscopy sources), compared against stability-constrained random baselines (sign-preserving weight shuffles, rejection-sampled for dynamic stability, n = 50).

Connectome-constrained networks produce a smooth circular direction geometry that random networks cannot replicate: RSA Spearman r = 0.686 (p < 0.0001) for ON edge stimuli and r = 0.846 (p < 0.0001) for ON+OFF edge stimuli, corroborated by CKA (p < 0.05 in both experiments). The geometry also tracks biological T4/T5 direction tuning recorded in living flies (Maisak et al. 2013): connectome-constrained geometry matches biology substantially better than random geometry (r = 0.930 vs. r = 0.603, gap {Delta}r = 0.327, p < 0.0001). Within each stimulus polarity, the ON pathway encodes direction with stronger geometric separation than the OFF pathway ({Delta}r = 0.138, 95% CI [0.091, 0.236]); we report this as a property of the model ensembles representations rather than an established biological difference: Maisak et al. (2013) find T4 and T5 functionally equivalent except in contrast polarity. To address the training confound, we compared untrained networks against shuffled baselines: the connectome prior shapes directional geometry at the ensemble level before any task training (r = 0.260, p = 0.041 and r = 0.215, p = 0.048; both marginal, uncorrected), suggesting wiring encodes a geometric prior that training amplifies.

These results establish representational geometry as a candidate fidelity metric that discriminates biological from arbitrary wiring using only population responses to a structured stimulus set, and suggest a practical path toward fidelity metrics for connectome-scale emulations approaching mammalian cortex.