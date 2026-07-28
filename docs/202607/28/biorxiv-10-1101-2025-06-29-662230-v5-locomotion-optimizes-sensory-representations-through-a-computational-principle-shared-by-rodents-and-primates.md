---
title: Locomotion optimizes sensory representations through a computational principle shared by rodents and primates
title_zh: 运动通过啮齿动物和灵长类动物共享的计算原理优化感觉表征
authors: "Gant, J. M., Mlynarski, W. F."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.1101/2025.06.29.662230v5.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 运动通过跨物种共享的计算原则优化感觉表征
tldr: 运动行为对感觉神经元的调节在不同物种间表现多样。本文提出一个统一计算原则：感觉系统内部调节以匹配运动导致的刺激统计变化，从而维持编码效率。通过将模型神经元适应自然环境中运动记录的刺激，该原则成功预测并重现了啮齿类和灵长类视觉编码的多类实验现象。该工作揭示了运动通过匹配刺激统计优化感觉表征的跨物种普适机制。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1817, \"height\": 1582, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1825, \"height\": 1616, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1822, \"height\": 1511, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1822, \"height\": 1603, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1827, \"height\": 1228, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1804, \"height\": 436, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1848, \"height\": 425, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1347, \"height\": 1011, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1802, \"height\": 1342, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1687, \"height\": 1254, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-29-662230-v5/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1741, \"height\": 937, \"label\": \"Figure\"}]"
motivation: 运动对感觉编码的影响在不同物种中表现多样，缺乏统一计算原则解释其多样性。
method: 构建模型神经元适应自然环境中运动记录的刺激统计，模拟运动对视觉编码的调节。
result: 模型重现了啮齿类和灵长类中运动调节视觉编码的广泛实验现象。
conclusion: 运动通过匹配刺激统计变化维持编码效率，是跨物种共享的计算原则。
---

## 摘要
行为以多种方式调节感觉系统的活动：从单个神经元的增益变化到神经群体中相互作用的改变。这些效应并非普遍存在；虽然运动对啮齿动物的感觉编码有强烈影响，但对灵长类动物的影响不那么显著。运动对感觉神经元施加的效应多样性，以及物种之间的差异，引发了对行为中感觉可能存在的普遍原则的疑问。我们提出，感觉系统内部受到调节，以匹配运动引起的刺激统计的系统性变化，从而促进准确和高效的感觉编码。我们发现，根据自然环境中运动期间记录的刺激进行适应的模型神经元，能够预测并重现啮齿动物和灵长类动物中广泛的实验观察结果。这种在不同行为状态下维持编码效率的简单原则，调和了运动在不同动物物种中调节视觉编码的多样性方式。

## Abstract
Behavior modulates the activity of sensory systems in multiple ways: from gain changes in individual neurons to changing interactions in neural populations. These effects are not universal; while movement has a strong influence on sensory coding in rodents, its impact on primates is less prominent. The diversity of effects that locomotion exerts on sensory neurons, as well as disparities between species, raises questions about the existence of universal principles that may underlie sensation during behavior. We propose that sensory systems are internally modulated to match systematic changes in stimulus statistics caused by locomotion, to facilitate an accurate and efficient sensory code. We find that model neurons, adapted to stimuli recorded during movement in natural environments, predict and reproduce a broad spectrum of experimental observations in rodents and primates. This simple principle of maintaining coding efficiency across behavioral states reconciles the diversity of ways in which locomotion modulates visual coding in different animal species.