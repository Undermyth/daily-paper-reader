---
title: Symmetry and nonlinear-readout criteria for orientation-tuning dynamics in a cortical neural field
title_zh: 皮层神经场中方向调谐动力学的对称性与非线性读出准则
authors: "Fukushima, M."
date: 2026-07-16
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.29.696812v3.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 朝向调谐动力学的神经场模型
tldr: 在初级视觉皮层中，增益变化与调谐形状变化常相互混淆。本文采用平移不变神经场模型，分析旋转对称和各向异性递归核的影响。发现对称核保持归一化调谐曲线不变，而弱各向异性导致延迟锐化和最优方向漂移。非线性读出分类表明，不同池化方式会改变调谐形状。该框架提供了区分标量增益、特征特异性递归和非线性读出效应的实验可分离特征。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-29-696812-v3/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1171, \"height\": 530, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-29-696812-v3/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 578, \"height\": 429, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-29-696812-v3/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1509, \"height\": 634, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-29-696812-v3/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1661, \"height\": 1268, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-29-696812-v3/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1841, \"height\": 356, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2025-12-29-696812-v3/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1859, \"height\": 505, \"label\": \"Table\"}]"
motivation: 分离V1中增益与调谐形状变化，区分递归和反馈调制效应。
method: 构建平移不变神经场模型，分析旋转对称与弱各向异性递归核，并分类非线性读出。
result: 对称核无调谐形状变化；弱各向异性产生延迟锐化及方向漂移；非线性读出种类决定调谐展宽或锐化。
conclusion: 提供了区分V1中增益、特征特异性递归和非线性读出的紧凑零模型与实验可分离特征。
---

## 摘要
在初级视觉皮层（V1）的递归和反馈调制研究中，增益变化和调谐形状变化难以区分。我们在一个具有快速各向同性和较慢各向异性递归分量的平移不变神经场模型中分析了这一区别。在固定的空间和时间频率下，任何旋转对称的递归核都会通过一个与角度无关的复增益乘以线性响应，从而保留归一化方向分布的每一个度量。弱各向异性在一阶打破这种标量增益对称性，产生由相量和关系描述的延迟锐化和优选方向漂移。然后我们对非线性读出进行了分类。一个非调谐的分割归一化池仅保留增益不变性，而弱调谐池根据 eff (C) = [1 - {beta}{kappa}C/({sigma} + {kappa}C)] 改变有效调制：同方向池在增益增加时展宽调谐，交叉方向池则锐化调谐。点式超线性读出提供了形状变化的另一途径，其主要畸变由响应幅度、背景驱动和非线性指数控制。该框架为标量增益、特征特异性递归和非线性读出效应提供了实验上可分离的特征，并为解释V1中的对比度和反馈扰动提供了紧凑的零模型。

## Abstract
Gain changes and tuning-shape changes are difficult to separate in studies of recurrent and feedback modulation in primary visual cortex (V1). We analyze this distinction in a translation-invariant neural-field model with fast isotropic and slower anisotropic recurrent components. At fixed spatial and temporal frequency, any rotationally symmetric recurrent kernel multiplies the linear response by an angle-independent complex gain and therefore preserves every metric of the normalized orientation profile. Weak anisotropy breaks this scalar-gain symmetry at first order, producing delayed sharpening and preferred-orientation drift described by a phasor-sum relation. We then classify nonlinear readouts. An untuned divisive-normalization pool preserves gain-only invariance, whereas a weakly tuned pool changes the effective modulation according to eff (C) = [1 - {beta}{kappa}C/({sigma} + {kappa}C)]: same-orientation pools broaden tuning and cross-orientation pools sharpen it as gain increases. Pointwise supralinear readouts provide a distinct route to shape change, with a leading distortion controlled by response amplitude, background drive, and nonlinearity exponent. The framework yields experimentally separable signatures for scalar gain, feature-specific recurrence, and nonlinear readout effects, and provides a compact null model for interpreting contrast and feedback perturbations in V1.