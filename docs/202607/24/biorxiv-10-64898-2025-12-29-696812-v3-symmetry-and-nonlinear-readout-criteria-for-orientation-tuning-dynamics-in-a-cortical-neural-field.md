---
title: Symmetry and nonlinear-readout criteria for orientation-tuning dynamics in a cortical neural field
title_zh: 皮层神经场中方向调谐动力学的对称性与非线性读出判据
authors: "Fukushima, M."
date: 2026-07-16
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.29.696812v3.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 皮层神经场模型用于方向调谐动力学
tldr: 初级视觉皮层中增益变化与调谐形状变化难以区分。本文通过平移不变神经场模型，分析旋转对称与弱各向异性递归成分，发现对称核产生角度无关复增益，弱各向异性一阶导致延迟锐化和朝向漂移。非线性读出分类表明：未调谐归一化保持增益不变，弱调谐池改变调谐宽度，点式超线性读出产生形状失真。该框架为区分标量增益、特征递归和非线性读出提供了实验可分离的签名。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-29-696812-v3/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1171, \"height\": 530}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-29-696812-v3/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 578, \"height\": 429}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-29-696812-v3/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1509, \"height\": 634}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-29-696812-v3/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1661, \"height\": 1268}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-29-696812-v3/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1841, \"height\": 356}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2025-12-29-696812-v3/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1859, \"height\": 505}]"
motivation: 区分皮质递归和反馈调制中增益变化与调谐形状变化的不同机制。
method: 分析平移不变神经场模型中旋转对称和弱各向异性递归核的响应，并分类非线性读出（未调谐归一化、弱调谐池、逐点超线性读出）。
result: 对称核产生角度无关复增益；弱各向异性一阶产生延迟锐化与朝向漂移；非线性读出按类型改变有效调谐宽度。
conclusion: 框架提供实验可分离的标量增益、特征特异递归和非线性读出效应的签名。
---

## 摘要
在初级视觉皮层(V1)的反馈和反复调节研究中，增益变化和调谐形状变化难以区分。我们在一类平移不变的神经场模型中分析这一区别，该模型包含快速各向同性和较慢各向异性的循环成分。在固定的空间和时间频率下，任何旋转对称的循环核都将线性响应乘以一个与角度无关的复增益，从而保持归一化方向轮廓的所有度量。弱各向异性在一阶打破了这种标量增益对称性，产生延迟锐化和由相量和关系描述的优选方向漂移。然后我们对非线性读出进行分类。一个未调谐的分割归一化池保持仅增益不变性，而一个弱调谐池根据eff(C)=[1 - βκC/(σ+κC)]改变有效调制：同方向池展宽调谐，交叉方向池随着增益增加而锐化调谐。逐点超线性读出提供了形状变化的独特途径，其主导失真由响应幅度、背景驱动和非线性指数控制。该框架为标量增益、特征特异性循环和非线性读出效应提供了实验上可分离的特征，并为解释V1中的对比度和反馈扰动提供了紧凑的零模型。

## Abstract
Gain changes and tuning-shape changes are difficult to separate in studies of recurrent and feedback modulation in primary visual cortex (V1). We analyze this distinction in a translation-invariant neural-field model with fast isotropic and slower anisotropic recurrent components. At fixed spatial and temporal frequency, any rotationally symmetric recurrent kernel multiplies the linear response by an angle-independent complex gain and therefore preserves every metric of the normalized orientation profile. Weak anisotropy breaks this scalar-gain symmetry at first order, producing delayed sharpening and preferred-orientation drift described by a phasor-sum relation. We then classify nonlinear readouts. An untuned divisive-normalization pool preserves gain-only invariance, whereas a weakly tuned pool changes the effective modulation according to eff (C) = [1 - {beta}{kappa}C/({sigma} +{kappa} C)]: same-orientation pools broaden tuning and cross-orientation pools sharpen it as gain increases. Pointwise supralinear readouts provide a distinct route to shape change, with a leading distortion controlled by response amplitude, background drive, and nonlinearity exponent. The framework yields experimentally separable signatures for scalar gain, feature-specific recurrence, and nonlinear readout effects, and provides a compact null model for interpreting contrast and feedback perturbations in V1.