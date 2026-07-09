---
title: Computational demands shape seizure susceptibility in recurrent neural networks
title_zh: 计算需求塑造循环神经网络中的癫痫易感性
authors: "Li, M., Eydam, S., Ramzan, I., Polygalov, D., Huang, A. J. Y., Taguas, I., Nemeth, H., Yanagihara, D., McHugh, T. J., Kang, L."
date: 2026-07-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.02.735135v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 递归神经网络中的计算需求影响癫痫易感性
tldr: 大脑区域对局灶性癫痫的易感性差异难以解释。本研究通过循环神经网络发现，支持连续表示的网络对癫痫扰动更敏感，性能下降更早，而离散状态网络更稳定。体内记录表明内嗅皮层（连续吸引子）比CA3（离散存储）更易驱动癫痫放电。结论是神经计算需求影响病理易感性。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1780, \"height\": 765, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1783, \"height\": 1851, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1685, \"height\": 1851, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1809, \"height\": 1784, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1790, \"height\": 1709, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1200, \"height\": 926, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1194, \"height\": 971, \"label\": \"Table\"}]"
motivation: 探究大脑区域对局灶性癫痫易感性差异的计算机制，超越传统解剖生理因素。
method: 手工构建并训练循环神经网络，比较连续表示与离散状态网络对癫痫扰动的响应。
result: 连续表示网络响应更高、性能下降更早；内嗅皮层驱动更强癫痫放电，CA3则较弱。
conclusion: 神经网络的计算方式（连续vs离散）决定其对病理转变的脆弱性。
---

## 摘要
大脑区域对局灶性癫痫的固有易感性各不相同，但决定这种风险的原理仍不清楚。虽然以往研究关注了解剖和生理因素，但我们在此观察到，潜在神经网络执行的计算起到了根本性作用。与稳定离散、良好分离状态的匹配网络相比，支持连续表征的手工构建和训练循环神经网络在应对癫痫扰动时表现出更高的活动性和更早的性能下降。与这一预测一致，体内记录显示，其网格细胞呈现连续吸引子动力学的内嗅皮层内侧，相较于与离散记忆存储相关的海马亚区CA3，驱动急性癫痫样放电时表现出更强的参与度和更平滑的状态轨迹。此外，选择性突触沉默表明，这种癫痫反应差异依赖于完整的嗅皮层连接。因此，使神经网络能够处理信息的计算也影响其对病理性转变的脆弱性。

## Abstract
Brain areas differ in their inherent susceptibility to focal seizures, but the principles governing this risk remain unclear. While prior work has focused on anatomical and physiological factors, here we observed a fundamental contribution from the computations performed by the underlying neural network. Handcrafted and trained recurrent neural networks supporting continuous representations respond to seizure perturbations with higher activity and earlier performance decline relative to matched networks stabilizing discrete, well-separated states. Consistent with this prediction, in vivo recordings revealed that medial entorhinal cortex, whose grid cells exhibit continuous attractor dynamics, drives acute epileptiform discharges with stronger involvement and smoother state trajectories compared to CA3, a hippocampal subfield associated with discrete memory storage. Moreover, selective synaptic silencing demonstrated that this difference in seizure responses depends on intact entorhinal connectivity. Thus, the computations that enable neural networks to process information also influence their vulnerability to pathological transitions.