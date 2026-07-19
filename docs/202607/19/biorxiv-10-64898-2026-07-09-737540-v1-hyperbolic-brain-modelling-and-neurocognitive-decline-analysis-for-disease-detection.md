---
title: Hyperbolic Brain Modelling and Neurocognitive Decline Analysis for Disease Detection
title_zh: 用于疾病检测的双曲脑建模与神经认知衰退分析
authors: "Mukhopadhyay, A., Halder, K., Neogy, R."
date: 2026-07-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.09.737540v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 双曲几何用于脑网络分析，计算表示
tldr: 传统欧氏空间建模脑分层网络导致结构失真，影响疾病诊断。现有双曲模型计算复杂。本文提出基于Beltrami-Klein球模型的高效非欧框架，将双曲测地线投影为直线，简化计算。在精神分裂症、帕金森病和阿尔茨海默病数据集上，该方法诊断精度更高、速度更快，为神经认知衰退分析提供了新方案。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737540-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 926, \"height\": 377, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-09-737540-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 872, \"height\": 403, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-09-737540-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 929, \"height\": 299, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-09-737540-v1/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 902, \"height\": 298, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-09-737540-v1/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 900, \"height\": 277, \"label\": \"Table\"}]"
motivation: 欧氏空间建模脑网络产生结构失真，而现有双曲模型计算开销大，需高效非欧框架。
method: 采用Beltrami-Klein球模型，将双曲测地线投影为欧氏直线，距离计算简化为点积。
result: 在三种神经疾病数据集上，Klein框架比Poincare和Lorentz基线诊断精度更高，速度更快。
conclusion: 所提Klein模型为脑网络分析提供了高效诊断工具，可推广至其他神经疾病。
---

## 摘要
在传统欧几里得空间中映射分层脑网络会导致显著的结构扭曲，从而削弱神经影像诊断框架的有效性。尽管像庞加莱球这样的双曲模型能够保留这些嵌套拓扑结构，但由于复杂的莫比乌斯操作和曲率测地线，它们需要大量的计算开销。本文介绍了一种高效的非欧几里得框架，利用贝尔特拉米-克莱因球模型分析神经认知衰退。通过将双曲测地线投影为欧几里得直线，该方法将复杂的距离计算转化为简单的点积，大幅降低了处理需求。我们使用精神分裂症、帕金森病和阿尔茨海默病的数据集，与最先进的庞加莱和洛伦兹基线进行了验证。基于克莱因的框架在所有三种神经认知障碍中均表现出优越的性能，既提供了更高的诊断精度，也实现了更快的处理速度。

## Abstract
Mapping hierarchical brain networks within traditional Euclidean space causes significant structural distortion, undermining neuroimaging diagnostic frameworks. While hyperbolic models like the Poincare ball preserve these nested topologies, they demand heavy computational overhead due to intricate Mobius operations and curved geodesics. This paper introduces a highly efficient non-Euclidean framework for analyzing neurocognitive decline utilizing the Beltrami-Klein ball model. By projecting hyperbolic geodesics as Euclidean straight lines, this approach converts complex distance calculations into simple dot products, radically reducing processing demands. We validated our methodology against state-of-the-art Poincare and Lorentz baselines using datasets for Schizophrenia, Parkinsons Disease, and Alzheimers Disease. The Klein-based framework demonstrates superior performance, delivering both higher diagnostic precision and accelerated processing velocities across all three neurocognitive disorders.