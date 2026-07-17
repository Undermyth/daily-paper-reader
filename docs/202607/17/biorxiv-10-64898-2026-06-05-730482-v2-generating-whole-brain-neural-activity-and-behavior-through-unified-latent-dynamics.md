---
title: Generating whole-brain neural activity and behavior through unified latent dynamics
title_zh: 通过统一潜在动力学生成全脑神经活动与行为
authors: "Nuzzi, D., Mattia, M., Pezzulo, G."
date: 2026-07-14
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.05.730482v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 连接神经活动与行为的全脑动力学生成模型
tldr: 神经科学面临高维神经活动与行为如何从共享底层动力学产生的问题。NEBULA通过统一潜变量动力学联合建模全脑神经活动和行为。应用于线虫全脑记录发现共享低维动力流形，实现长时间生成和模拟干预。该方法为建立脑动力学与行为联系提供了框架，支持可扩展虚拟实验。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1599, \"height\": 1654, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1598, \"height\": 1461, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1568, \"height\": 1573, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1693, \"height\": 1163, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-05-730482-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1648, \"height\": 1465, \"label\": \"Figure\"}]"
motivation: 理解高维神经活动与行为如何从共享底层动力学产生。
method: 提出NEBULA，用共享低维潜变量动力学联合生成全脑神经活动和行为。
result: 在线虫全脑记录中发现共享低维动力流形，实现长时间生成和定向状态操控。
conclusion: 建立了脑动力学与行为联系框架，为可扩展虚拟实验奠定基础。
---

## 摘要
理解高维神经活动与行为如何从共享的底层动力学中涌现，仍是神经科学的一项根本性挑战。解决这一问题对于实现能够忠实再现和预测生命系统多尺度脑-行为动力学的数字孪生至关重要。在此，我们提出NEBULA（通过统一潜在动力学进行神经与行为建模），这是一个联合建模全脑神经活动与行为的生成式框架。通过将NEBULA应用于秀丽隐杆线虫的全脑记录，我们识别出一个既支撑神经活动又支撑行为的共享低维动力流形，从而能够实现长时程生成和靶向计算机干预实验。对所学动力学的扰动揭示了行为相关的转换点，而引导干预则无需重新训练即可实现对神经和行为状态的可控操作。这些结果建立了一个将生物体脑动力学与行为联系起来的框架，并为神经科学中可扩展的虚拟实验奠定了基础。

## Abstract
Understanding how high-dimensional neural activity and behavior emerge from shared underlying dynamics remains a fundamental challenge in neuroscience. Addressing this problem is key to enabling digital twins that can faithfully reproduce and predict the multiscale brain-behavior dynamics of living systems. Here we present NEBULA (NEural and Behavioral modeling through Unified LAtent dynamics), a generative framework that jointly models whole-brain neural activity and behavior. By applying NEBULA to brain-wide recordings from C. elegans, we identify a shared low-dimensional dynamical manifold that underlies both neural activity and behavior, enabling long-horizon generation and targeted in silico interventions. Perturbations of the learned dynamics reveal behaviorally relevant transition points, whereas steering interventions enable controlled manipulation of neural and behavioral states without retraining. These results establish a framework for linking brain dynamics to behavior in a living organism and provide a foundation for scalable virtual experimentation in neuroscience.