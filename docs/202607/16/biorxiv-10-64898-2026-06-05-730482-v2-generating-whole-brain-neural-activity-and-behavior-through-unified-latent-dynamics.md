---
title: Generating whole-brain neural activity and behavior through unified latent dynamics
title_zh: 通过统一潜在动力学生成全脑神经活动和行为
authors: "Nuzzi, D., Mattia, M., Pezzulo, G."
date: 2026-07-14
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.05.730482v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 全脑神经活动和行为的统一生成模型
tldr: 理解高维神经活动和行为如何从共享底层动力学涌现是神经科学的根本挑战。本文提出NEBULA生成式框架，通过统一潜在动力学联合建模全脑神经活动和行为，在线虫全脑记录上学习动力学结构。该模型支持长时间生成神经和行为轨迹、逼真的行为模拟以及定向虚拟干预，扰动分析揭示行为相关的转换点，干预可在无重训练下操控状态。这一框架建立了连接脑动力学与行为的桥梁，为可扩展的虚拟实验奠定了基础。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1599, \"height\": 1654, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1598, \"height\": 1461, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1568, \"height\": 1573, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1693, \"height\": 1163, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1648, \"height\": 1465, \"label\": \"Figure\"}]"
motivation: 为理解多尺度脑-行为动力学的涌现机制，需要能联合生成神经活动和行为的统一生成模型。
method: NEBULA学习一个统一的潜在动力学结构，同时重建全脑钙成像和行为视频，支持轨迹生成与虚拟干预。
result: 模型实现长时间神经和行为轨迹生成、逼真行为模拟；扰动揭示行为转换点，干预可操控状态无需重训练。
conclusion: 该框架在秀丽隐杆线虫上建立了脑动力学与行为的关联，为可扩展的虚拟神经科学实验提供了基础。
---

## 摘要
理解高维神经活动和行为如何从共享的底层动力学中涌现仍是神经科学的基本挑战。解决这一问题对于实现能够忠实地再现和预测生命系统多尺度脑-行为动力学的数字孪生至关重要。我们提出了NEBULA（通过统一潜在动力学的神经与行为建模），这是一个联合建模全脑神经活动和行为的生成框架。利用从秀丽隐杆线虫获得的全脑记录，模型学习了统一的潜在动力学结构，支持神经和行为轨迹的长期生成、行为的逼真模拟以及定向虚拟干预。对所学动力学的扰动揭示了行为相关的转折点，而导向干预则能够在不重新训练的情况下对神经和行为状态进行受控操作。这些结果建立了一个将生物体脑动力学与行为联系起来的框架，并为神经科学中可扩展的虚拟实验奠定了基础。

## Abstract
Understanding how high-dimensional neural activity and behavior emerge from shared underlying dynamics remains a fundamental challenge in neuroscience. Addressing this problem is key to enabling digital twins that can faithfully reproduce and predict the multiscale brain-behavior dynamics of living systems. Here we present NEBULA (NEural and Behavioral modeling through Unified LAtent dynamics), a generative framework that jointly models whole-brain neural activity and behavior. Using brain-wide recordings from C. elegans, the model learns a unified latent dynamical structure that supports long-horizon generation of neural and behavioral trajectories, realistic simulations of behavior, and targeted virtual interventions. Perturbations of the learned dynamics reveal behaviorally relevant transition points, whereas steering interventions enable controlled manipulation of neural and behavioral states without retraining. These results establish a framework for linking brain dynamics to behavior in a living organism and provide a foundation for scalable virtual experimentation in neuroscience.