---
title: Generating whole-brain neural activity and behavior through unified latent dynamics
title_zh: 通过统一潜在动力学生成全脑神经活动和行为
authors: "Nuzzi, D., Mattia, M., Pezzulo, G."
date: 2026-07-14
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.05.730482v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 通过统一潜在动力学生成神经和行为
tldr: 高维神经活动与行为如何从共享底层动力学涌现是神经科学难题。本文提出NEBULA生成框架，联合建模线虫全脑神经活动与行为，学习统一潜在动力学。该模型能长期生成神经与行为轨迹、模拟真实行为，并通过虚拟干预揭示行为转换点、操控神经状态。工作为数字孪生大脑奠定基础，实现可扩展的虚拟实验。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1599, \"height\": 1654, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1598, \"height\": 1461, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1568, \"height\": 1573, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1693, \"height\": 1163, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1648, \"height\": 1465, \"label\": \"Figure\"}]"
motivation: 现有模型难以同时捕捉全脑神经活动与行为的长期依赖关系，缺乏统一动力学视角。
method: 基于变分自编码器与循环神经网络，学习神经与行为共享的低维潜在动力学，支持长时程生成。
result: 模型精准生成神经活动与行为轨迹，扰动分析发现行为转换关键状态，定向干预无需重训练即可操控神经行为。
conclusion: NEBULA为理解脑-行为关联提供可解释生成框架，推动神经科学虚拟实验发展。
---

## 摘要
理解高维神经活动和行为如何从共享的底层动力学中涌现仍然是神经科学的一个基本挑战。解决这一问题对于实现能够忠实再现和预测生命系统多尺度脑-行为动力学的数字孪生至关重要。在此，我们提出NEBULA（通过统一潜在动力学进行神经和行为建模），一个联合建模全脑神经活动和行为的生成框架。利用秀丽隐杆线虫的全脑记录，该模型学习了一个统一的潜在动力学结构，支持神经和行为轨迹的长时程生成、行为逼真模拟以及定向虚拟干预。对所学动力学的扰动揭示了行为相关的转换点，而引导性干预则在无需重新训练的情况下实现了对神经和行为状态的控制性操作。这些结果为将脑动力学与生物体行为建立联系提供了一个框架，并为神经科学中可扩展的虚拟实验奠定了基础。

## Abstract
Understanding how high-dimensional neural activity and behavior emerge from shared underlying dynamics remains a fundamental challenge in neuroscience. Addressing this problem is key to enabling digital twins that can faithfully reproduce and predict the multiscale brain-behavior dynamics of living systems. Here we present NEBULA (NEural and Behavioral modeling through Unified LAtent dynamics), a generative framework that jointly models whole-brain neural activity and behavior. Using brain-wide recordings from C. elegans, the model learns a unified latent dynamical structure that supports long-horizon generation of neural and behavioral trajectories, realistic simulations of behavior, and targeted virtual interventions. Perturbations of the learned dynamics reveal behaviorally relevant transition points, whereas steering interventions enable controlled manipulation of neural and behavioral states without retraining. These results establish a framework for linking brain dynamics to behavior in a living organism and provide a foundation for scalable virtual experimentation in neuroscience.