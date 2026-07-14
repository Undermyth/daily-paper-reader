---
title: Generative and discriminative recurrence employ opposing strategies for robust vision
title_zh: 生成性与判别性循环在鲁棒视觉中采用对立策略
authors: "Schmitt, L.-M., Koot, M., Heilbron, M., de Lange, F."
date: 2026-07-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.02.736066v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 视觉中循环连接的计算机制
tldr: 循环连接如何增强视觉鲁棒性仍不清楚。本文在卷积神经网络中比较了不同循环架构（侧向/反馈）和训练目标（生成/判别）的影响。结果发现，生成反馈采用降维去噪策略，在中等噪声下不需噪声训练即可实现鲁棒性；而判别循环（侧向和反馈）采用升维锐化策略，但需噪声训练。该研究揭示了两种不同的计算机制，为生物视觉中循环连接的形式提供可检验预测。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736066-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1352, \"height\": 816, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736066-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1295, \"height\": 729, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736066-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1336, \"height\": 1446, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736066-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1303, \"height\": 732, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736066-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1304, \"height\": 779, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736066-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1324, \"height\": 788, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-02-736066-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1272, \"height\": 353, \"label\": \"Table\"}]"
motivation: 探究不同类型的循环连接和训练目标是否采用不同的计算策略来增强视觉鲁棒性。
method: 为 CNN 赋予不同循环架构（侧向/反馈）和训练目标（生成/判别），评估内部表征及不同噪声下的行为。
result: 生成反馈通过降维去噪实现鲁棒性；判别循环通过升维锐化实现鲁棒性，但需噪声训练。
conclusion: 视觉鲁棒性存在两种根本不同的计算机制，为大脑中循环连接的形式提供可检验预测。
---

## 摘要
循环被认为能增强生物视觉的鲁棒性，但其实现机制尚不明确。感知鲁棒性可通过两种方式实现：一是通过侧向连接支持处理阶段内的局部整合，二是通过反馈连接利用来自更高层次的更广泛背景；同时可通过两种目标优化：一是优化任务相关分类的判别性目标，二是学习重建视觉输入原因的生成性目标。但不同类型的循环是否采用不同的计算策略？由于这一问题难以在体内验证，我们为卷积神经网络配备了不同的循环架构和训练目标，并评估了其内部表征和在不同噪声水平下行为的影响。结果揭示了两种截然不同的计算策略：生成性反馈遵循还原论策略，通过去噪使表征降维，在中等噪声水平下无需噪声训练即可实现鲁棒性；判别性侧向和反馈循环则遵循扩张论策略，通过提高维度以增强可辨别性而不去噪，但需要噪声训练才能实现鲁棒性。这些可分离的特征反映了鲁棒视觉的根本不同计算机制，并为大脑采用哪种循环形式提供了可测试的预测。

## Abstract
Recurrence is thought to enhance the robustness of biological vision, but how it achieves this feat is largely unknown. Perceptual robustness can be implemented through either lateral connections supporting local integration within a processing stage or feedback connections drawing on broader context from higher stages, and through either a discriminative objective optimising task-relevant classification or a generative objective learning to reconstruct the causes of visual input. But do these different types of recurrence engage distinct computational strategies? As this question is difficult to test in vivo, we endowed convolutional neural networks with varying recurrent architectures and training objectives, and evaluated the consequences for internal representations and behaviour across noise levels. Two distinct computational strategies emerged. Generative feedback followed a reductionist strategy, with representations becoming lower-dimensional through denoising, achieving robustness at moderate noise levels without noise training. Both discriminative lateral and feedback recurrence followed an expansionist strategy, increasing dimensionality to sharpen discriminability without denoising, but requiring noise training to achieve robustness. These dissociable signatures reflect fundamentally different computational mechanisms of robust vision and provide testable predictions for which form of recurrence the brain employs.