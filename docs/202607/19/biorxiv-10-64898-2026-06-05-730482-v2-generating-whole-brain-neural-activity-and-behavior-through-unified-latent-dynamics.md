---
title: Generating whole-brain neural activity and behavior through unified latent dynamics
title_zh: 通过统一潜在动力学生成全脑神经活动和行为
authors: "Nuzzi, D., Mattia, M., Pezzulo, G."
date: 2026-07-14
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.05.730482v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 生成框架NEBULA联合建模全脑神经活动与行为
tldr: 高维神经活动和行为如何从共享的低维动态中涌现是神经科学的核心问题。本文提出NEBULA生成框架，通过联合建模秀丽隐杆线虫的全脑神经活动和行为，发现共享的低维动力流形，支持长时程生成和虚拟干预。扰动学习动态揭示行为相关转换点，定向操控可无需重训练而控制神经与行为状态。该工作为连接脑动态与行为建立了框架，并奠定了可扩展虚拟实验的基础。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1599, \"height\": 1654, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1598, \"height\": 1461, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1568, \"height\": 1573, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1693, \"height\": 1163, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1648, \"height\": 1465, \"label\": \"Figure\"}]"
motivation: 现有模型难以联合生成全脑神经活动和行为，缺乏可干预的虚拟数字孪生。
method: 提出NEBULA生成框架，从全脑记录中联合学习神经活动和行为的共享低维潜在动态。
result: 发现共享低维流形，支持长时程生成；扰动揭示行为转换点，定向操控无需重训练。
conclusion: 建立脑动态与行为联系的生成框架，推动可扩展的虚拟神经科学实验。
---

## 摘要
理解高维神经活动和行为如何从共享的底层动力学中涌现，仍然是神经科学中的一个基本挑战。解决这一问题对于实现能够忠实再现和预测生命系统多尺度脑-行为动力学的数字孪生至关重要。本文提出NEBULA（通过统一潜在动力学进行神经和行为建模），这是一个联合建模全脑神经活动和行为的生成框架。通过将NEBULA应用于秀丽隐杆线虫的全脑记录，我们识别出神经活动和行为共有的低维动力学流形，从而实现长时间跨度的生成和靶向计算机干预。对学习到的动力学进行扰动揭示了行为相关的转换点，而导向干预则可以在无需重新训练的情况下可控地操纵神经和行为状态。这些结果为将大脑动力学与生物体行为联系起来建立了框架，并为神经科学中的可扩展虚拟实验奠定了基础。

## Abstract
Understanding how high-dimensional neural activity and behavior emerge from shared underlying dynamics remains a fundamental challenge in neuroscience. Addressing this problem is key to enabling digital twins that can faithfully reproduce and predict the multiscale brain-behavior dynamics of living systems. Here we present NEBULA (NEural and Behavioral modeling through Unified LAtent dynamics), a generative framework that jointly models whole-brain neural activity and behavior. By applying NEBULA to brain-wide recordings from C. elegans, we identify a shared low-dimensional dynamical manifold that underlies both neural activity and behavior, enabling long-horizon generation and targeted in silico interventions. Perturbations of the learned dynamics reveal behaviorally relevant transition points, whereas steering interventions enable controlled manipulation of neural and behavioral states without retraining. These results establish a framework for linking brain dynamics to behavior in a living organism and provide a foundation for scalable virtual experimentation in neuroscience.