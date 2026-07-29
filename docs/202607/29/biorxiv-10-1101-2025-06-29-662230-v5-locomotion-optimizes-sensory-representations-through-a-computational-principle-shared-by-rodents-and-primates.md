---
title: Locomotion optimizes sensory representations through a computational principle shared by rodents and primates
title_zh: 运动通过啮齿类和灵长类共享的计算原理优化感觉表征
authors: "Gant, J. M., Mlynarski, W. F."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.1101/2025.06.29.662230v5.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 提出了运动期间感觉表征优化的计算原则
tldr: 运动对感觉编码的影响在物种间存在差异，缺乏统一解释。本研究提出感觉系统通过内部调节匹配运动引起的刺激统计变化，以维持编码效率。模型神经元适应自然运动刺激后，成功预测并复现了啮齿类和灵长类的多种实验观测。该工作揭示了运动优化感觉表征的跨物种通用计算原则，弥合了不同动物间的表现差异。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1817, \"height\": 1582, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1825, \"height\": 1616, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1822, \"height\": 1511, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1822, \"height\": 1603, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1827, \"height\": 1228, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1804, \"height\": 436, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1848, \"height\": 425, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1347, \"height\": 1011, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1802, \"height\": 1342, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1687, \"height\": 1254, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1741, \"height\": 937, \"label\": \"Figure\"}]"
motivation: 揭示运动调节感觉编码的通用计算原则，统一啮齿类和灵长类中看似矛盾的现象。
method: 基于效率编码原理，构建模型神经元适应自然环境中运动时的刺激统计，模拟运动对视觉编码的调节。
result: 模型成功预测并复制了啮齿类和灵长类动物中运动调节视觉编码的多种实验结果。
conclusion: 维持跨行为状态的编码效率是运动优化感觉表征的普遍计算原则，弥合了物种差异。
---

## 摘要
行为以多种方式调节感觉系统的活动：从单个神经元的增益变化到神经群体中相互作用的改变。这些效应并非普遍存在；虽然运动对啮齿类的感觉编码有强烈影响，但对灵长类的影响则不那么显著。运动对感觉神经元施加的效应的多样性，以及物种间的差异，引发了关于是否存在可能构成行为中感觉基础的普遍原理的问题。我们提出，感觉系统受到内部调节，以匹配由运动引起的刺激统计量的系统性变化，从而促进准确且高效的感觉编码。我们发现，适应于自然环境中运动期间记录到的刺激的模型神经元，能够预测并复现啮齿类和灵长类中广泛范围的实验观察结果。这一在行为状态间维持编码效率的简单原则，调和了运动在不同动物物种中调节视觉编码的多样性方式。

## Abstract
Behavior modulates the activity of sensory systems in multiple ways: from gain changes in individual neurons to changing interactions in neural populations. These effects are not universal; while movement has a strong influence on sensory coding in rodents, its impact on primates is less prominent. The diversity of effects that locomotion exerts on sensory neurons, as well as disparities between species, raises questions about the existence of universal principles that may underlie sensation during behavior. We propose that sensory systems are internally modulated to match systematic changes in stimulus statistics caused by locomotion, to facilitate an accurate and efficient sensory code. We find that model neurons, adapted to stimuli recorded during movement in natural environments, predict and reproduce a broad spectrum of experimental observations in rodents and primates. This simple principle of maintaining coding efficiency across behavioral states reconciles the diversity of ways in which locomotion modulates visual coding in different animal species.