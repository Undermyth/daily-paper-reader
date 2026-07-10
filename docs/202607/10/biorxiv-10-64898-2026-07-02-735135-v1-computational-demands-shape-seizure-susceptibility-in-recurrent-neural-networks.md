---
title: Computational demands shape seizure susceptibility in recurrent neural networks
title_zh: 计算需求塑造递归神经网络的癫痫易感性
authors: "Li, M., Eydam, S., Ramzan, I., Polygalov, D., Huang, A. J. Y., Taguas, I., Nemeth, H., Yanagihara, D., McHugh, T. J., Kang, L."
date: 2026-07-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.02.735135v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 计算需求影响递归神经网络中的癫痫易感性
tldr: 大脑区域对癫痫发作的易感性存在差异，但其机制不明。本研究通过手造和训练递归神经网络发现，支持连续表示的网络比离散状态网络对癫痫扰动更敏感，表现出更高活动和更早性能下降。体内记录证实，具有连续吸引子动力学的内嗅皮层比离散记忆存储的CA3更容易引发癫痫放电。选择性突触沉默表明该差异依赖于内嗅连接。计算需求是影响神经网络病理转换脆弱性的基本因素。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1780, \"height\": 765}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1783, \"height\": 1851}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1685, \"height\": 1851}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1809, \"height\": 1784}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1790, \"height\": 1709}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1200, \"height\": 926}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1194, \"height\": 971}]"
motivation: 大脑区域癫痫易感性差异的机制不明，以往研究聚焦解剖生理因素，本文探索计算需求的影响。
method: 手造和训练递归神经网络支持连续或离散表示，结合体内电生理记录和突触沉默实验。
result: 连续表示网络在癫痫扰动下活动更高、性能下降更早；内嗅皮层比CA3更易诱发癫痫放电。
conclusion: 神经网络的计算需求影响其癫痫易感性。
---

## 摘要
不同脑区对局灶性癫痫发作的内在易感性存在差异，但支配这种风险的原理仍不清楚。尽管以往研究聚焦于解剖和生理因素，但我们在本研究中观察到，潜在神经网络所执行的计算起到了基础性作用。与稳定离散、分离状态的对等网络相比，支持连续表征的手工构建和训练的递归神经网络对癫痫干扰的反应表现出更高的活动性和更早的性能下降。与这一预测一致，体内记录显示，内侧内嗅皮层（其网格细胞表现出连续吸引子动力学）相比海马CA3亚区（与离散记忆存储相关）驱动急性癫痫样放电时具有更强的参与度和更平滑的状态轨迹。此外，选择性突触沉默表明，这种癫痫反应差异取决于完整的内嗅连接。因此，神经网络用于处理信息的计算也影响了它们对病理状态转变的脆弱性。

## Abstract
Brain areas differ in their inherent susceptibility to focal seizures, but the principles governing this risk remain unclear. While prior work has focused on anatomical and physiological factors, here we observed a fundamental contribution from the computations performed by the underlying neural network. Handcrafted and trained recurrent neural networks supporting continuous representations respond to seizure perturbations with higher activity and earlier performance decline relative to matched networks stabilizing discrete, well-separated states. Consistent with this prediction, in vivo recordings revealed that medial entorhinal cortex, whose grid cells exhibit continuous attractor dynamics, drives acute epileptiform discharges with stronger involvement and smoother state trajectories compared to CA3, a hippocampal subfield associated with discrete memory storage. Moreover, selective synaptic silencing demonstrated that this difference in seizure responses depends on intact entorhinal connectivity. Thus, the computations that enable neural networks to process information also influence their vulnerability to pathological transitions.