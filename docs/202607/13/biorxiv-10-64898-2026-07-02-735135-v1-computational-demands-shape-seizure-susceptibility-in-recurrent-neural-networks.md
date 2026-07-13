---
title: Computational demands shape seizure susceptibility in recurrent neural networks
title_zh: 计算需求塑造递归神经网络中的癫痫易感性
authors: "Li, M., Eydam, S., Ramzan, I., Polygalov, D., Huang, A. J. Y., Taguas, I., Nemeth, H., Yanagihara, D., McHugh, T. J., Kang, L."
date: 2026-07-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.02.735135v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 递归神经网络基于计算需求建模癫痫易感性
tldr: 不同脑区对局灶性癫痫的易感性存在差异，但其机制尚不明确。以往研究多关注解剖和生理因素，本文发现神经网络的计算方式也有贡献。通过构建支持连续和离散状态表示的循环神经网络，发现连续表示网络对癫痫扰动更敏感，表现为更高活动水平和更早性能下降。在体记录证实，内侧内嗅皮层（连续吸引子）比CA3（离散存储）驱动更强癫痫样放电。这些结果表明，计算需求塑造了癫痫易感性，为理解脑区差异提供了新机制。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1780, \"height\": 765}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1783, \"height\": 1851}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1685, \"height\": 1851}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1809, \"height\": 1784}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1790, \"height\": 1709}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1200, \"height\": 926}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1194, \"height\": 971}]"
motivation: 探究神经网络的计算方式（连续vs离散）是否影响其对癫痫的易感性。
method: 构建并训练支持连续和离散表示的循环神经网络，对比癫痫扰动下的响应，并在动物模型进行在体记录和突触沉默验证。
result: 连续表示网络（类似内嗅皮层）比离散网络（类似CA3）对癫痫更敏感，活动更高且性能下降更早。
conclusion: 神经网络的计算需求决定了其病理转变易感性，为理解局灶性癫痫的脑区差异提供新机制。
---

## 摘要
大脑区域对局灶性癫痫的固有易感性各不相同，但支配这种风险的原理仍不清楚。虽然先前的研究集中在解剖和生理因素上，但这里我们观察到基础神经网络所执行的计算的根本贡献。与稳定离散、良好分离状态的匹配网络相比，支持连续表示的手工设计和训练的递归神经网络对癫痫扰动的反应具有更高的活动和更早的性能下降。与此预测一致，体内记录显示，内嗅皮层内侧（其网格细胞表现出连续吸引子动力学）驱动急性癫痫样放电，与海马亚区CA3（与离散记忆存储相关）相比，具有更强的参与和更平滑的状态轨迹。此外，选择性突触沉默表明，这种癫痫反应差异取决于完整的内嗅连接。因此，使神经网络能够处理信息的计算也影响其对病理转变的脆弱性。

## Abstract
Brain areas differ in their inherent susceptibility to focal seizures, but the principles governing this risk remain unclear. While prior work has focused on anatomical and physiological factors, here we observed a fundamental contribution from the computations performed by the underlying neural network. Handcrafted and trained recurrent neural networks supporting continuous representations respond to seizure perturbations with higher activity and earlier performance decline relative to matched networks stabilizing discrete, well-separated states. Consistent with this prediction, in vivo recordings revealed that medial entorhinal cortex, whose grid cells exhibit continuous attractor dynamics, drives acute epileptiform discharges with stronger involvement and smoother state trajectories compared to CA3, a hippocampal subfield associated with discrete memory storage. Moreover, selective synaptic silencing demonstrated that this difference in seizure responses depends on intact entorhinal connectivity. Thus, the computations that enable neural networks to process information also influence their vulnerability to pathological transitions.