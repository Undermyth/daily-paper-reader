---
title: "Representational geometry as a fidelity metric for connectome-constrained networks: evidence from the Drosophila visual system"
title_zh: 表征几何作为连接组约束网络的保真度度量：来自果蝇视觉系统的证据
authors: "Zhou, M. G., Hasler, J. O."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.10.731214v10.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 表征几何作为连接组约束网络的度量，与计算神经科学相关
tldr: 行为保真度无法保证生物保真度，需要一种仅依赖种群响应的度量来区分真实生物线路与任意线路。本文提出表示几何作为保真度度量，对果蝇视觉系统连接组约束网络（Flyvis）进行代表相似性分析（RSA）和中心核对齐（CKA）。发现连接组约束网络产生平滑的圆形方向几何，随机网络无法复制，且与真实T4/T5神经元方向调谐高度匹配（r=0.930 vs 0.603）。训练前网络已显示几何先验，表明表示几何能有效区分生物与任意线路，为连接组尺度仿真的保真度评估提供了实用路径。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-10-731214-v10/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1446, \"height\": 388}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-10-731214-v10/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1439, \"height\": 382}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-10-731214-v10/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1084, \"height\": 1128}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-10-731214-v10/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1231, \"height\": 402}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-10-731214-v10/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1445, \"height\": 396}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-10-731214-v10/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1444, \"height\": 1134}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-10-731214-v10/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1441, \"height\": 394}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-06-10-731214-v10/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1284, \"height\": 522}]"
motivation: 行为保真度不等于生物保真度，需要种群级度量区分真实与任意线路。
method: 使用RSA和CKA分析Flyvis连接组约束网络，比较其与随机基线网络的方向表示几何。
result: 连接组约束网络产生平滑方向几何（RSA r=0.686~0.846），优于随机网络且匹配生物学（r=0.930）。
conclusion: 表示几何可作为区分生物与任意线路的保真度度量，无需行为解码器。
---

## 摘要
生物布线实际上对神经计算有何贡献？行为实验可以测试模型是否产生正确的输出，但无法确定其内部表征是否具有生物学保真度。Brunton等人（2026）将这一点具体化：一个使用深度强化学习训练的秀丽隐杆线虫连接组能够产生逼真的果蝇行走行为——然而该模型在生物学上是无意义的，因为行为保真度可以在没有生物学保真度的情况下实现。我们需要一个群体水平的度量标准，能够区分真实的生物布线与任意布线，且无需行为解码器。我们提出表征几何作为该度量标准。表征几何——群体对不同刺激响应的成对距离结构——捕捉了神经电路如何组织其表征空间，独立于其驱动的行为。我们将表征相似性分析（RSA）和中心核对齐（CKA）应用于Flyvis预训练的果蝇视觉系统集成（Lappalainen等人2024）：50个网络，其架构固定为Flyvis连接组（从部分电子显微镜源重建），并与稳定性约束的随机基线（保号权重打乱，通过动态稳定性拒绝抽样，n = 50）进行比较。

连接组约束网络产生平滑的圆形方向几何，随机网络无法复制：对于ON边缘刺激，RSA Spearman r = 0.686（p < 0.0001），对于ON+OFF边缘刺激，r = 0.846（p < 0.0001），CKA也证实了这一点（两项实验均p < 0.05）。该几何还追踪了活蝇中记录的生物T4/T5方向调谐（Maisak等人2013）：连接组约束几何与生物学的匹配程度显著优于随机几何（r = 0.930对比r = 0.603，差值Δr = 0.327，p < 0.0001）。在每个刺激极性内，ON通路编码的方向几何分离度强于OFF通路（Δr = 0.138，95% CI [0.091, 0.236]）；我们将此报告为模型集成表征的一个属性，而非已建立的生物学差异：Maisak等人（2013）发现T4和T5除了对比度极性外功能上等价。为了解决训练混淆问题，我们将未训练网络与打乱基线进行比较：连接组先验在任务训练之前就在集成水平上塑造了方向几何（r = 0.260，p = 0.041和r = 0.215，p = 0.048；两者均为边缘显著，未校正），表明布线编码了训练放大的几何先验。

这些结果确立了表征几何作为候选保真度度量标准，仅使用对结构化刺激集的群体响应即可区分生物布线与任意布线，并提出了走向接近哺乳动物皮质的连接组规模仿真保真度度量的实用路径。

## Abstract
What does biological wiring actually contribute to neural computation? Behavioral experiments can test whether a model produces the right outputs, but they cannot determine whether its internal representations are biologically faithful. Brunton et al. (2026) made this concrete: a C. elegans worm connectome trained with deep reinforcement learning produces realistic Drosophila fly walking -- yet the model is biologically meaningless, because behavioral fidelity is achievable without biological fidelity. We need a population-level metric that discriminates real biological wiring from arbitrary wiring, without requiring a behavioral decoder. We propose representational geometry as that metric. Representational geometry -- the structure of pairwise distances between population responses to different stimuli -- captures how a neural circuit organizes its representational space, independently of what behavior it drives. We apply representational similarity analysis (RSA) and centered kernel alignment (CKA) to the Flyvis pretrained Drosophila melanogaster visual system ensemble (Lappalainen et al. (2024)): 50 networks whose architecture is fixed to the Flyvis connectome (reconstructed from partial electron-microscopy sources), compared against stability-constrained random baselines (sign-preserving weight shuffles, rejection-sampled for dynamic stability, n = 50).

Connectome-constrained networks produce a smooth circular direction geometry that random networks cannot replicate: RSA Spearman r = 0.686 (p < 0.0001) for ON edge stimuli and r = 0.846 (p < 0.0001) for ON+OFF edge stimuli, corroborated by CKA (p < 0.05 in both experiments). The geometry also tracks biological T4/T5 direction tuning recorded in living flies (Maisak et al. 2013): connectome-constrained geometry matches biology substantially better than random geometry (r = 0.930 vs. r = 0.603, gap {triangleup}r = 0.327, p < 0.0001). Within each stimulus polarity, the ON pathway encodes direction with stronger geometric separation than the OFF pathway ({triangleup}r = 0.138, 95% CI [0.091, 0.236]); we report this as a property of the model ensembles representations rather than an established biological difference: Maisak et al. (2013) find T4 and T5 functionally equivalent except in contrast polarity. To address the training confound, we compared untrained networks against shuffled baselines: the connectome prior shapes directional geometry at the ensemble level before any task training (r = 0.260, p = 0.041 and r = 0.215, p = 0.048; both marginal, uncorrected), suggesting wiring encodes a geometric prior that training amplifies.

These results establish representational geometry as a candidate fidelity metric that discriminates biological from arbitrary wiring using only population responses to a structured stimulus set, and suggest a practical path toward fidelity metrics for connectome-scale emulations approaching mammalian cortex.