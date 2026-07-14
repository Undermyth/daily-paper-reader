---
title: Computational demands shape seizure susceptibility in recurrent neural networks
title_zh: 计算需求塑造递归神经网络的癫痫易感性
authors: "Li, M., Eydam, S., Ramzan, I., Polygalov, D., Huang, A. J. Y., Taguas, I., Nemeth, H., Yanagihara, D., McHugh, T. J., Kang, L."
date: 2026-07-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.02.735135v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 通过网格细胞吸引子动力学的海马计算
tldr: 大脑区域对局灶性癫痫的易感性不同，但原因尚不明确。本研究通过构建并训练两类循环神经网络（RNN）发现，支持连续表示的网络对癫痫扰动响应更强烈且性能下降更快。体内记录表明，具有连续吸引子动力学的内嗅皮层比离散记忆存储的CA3更易驱动癫痫样放电，且该差异依赖于完整的内嗅连接。因此，神经网络的计算需求会显著影响其病理转变风险。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1780, \"height\": 765}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1783, \"height\": 1851}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1685, \"height\": 1851}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1809, \"height\": 1784}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1790, \"height\": 1709}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1200, \"height\": 926}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-02-735135-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1194, \"height\": 971}]"
motivation: 现有研究关注解剖和生理因素，但忽视了神经网络计算本身对癫痫易感性的贡献。
method: 构建并训练支持连续表示与离散稳定状态的RNN，结合小鼠体内电生理记录与突触沉默实验。
result: 连续计算网络对癫痫反应更强且性能更早下降；内嗅皮层驱动更强癫痫样放电和更平滑轨迹，且依赖连接完整性。
conclusion: 神经计算方式（连续vs离散）是决定癫痫易感性的关键因素。
---

## 摘要
不同脑区对局灶性癫痫的固有易感性存在差异，但支配这种风险的原理尚不清楚。尽管先前的研究聚焦于解剖和生理因素，但此处我们观察到基础神经网络执行的计算功能具有根本性贡献。与稳定化离散、良好分离状态的匹配网络相比，支持连续表示的人工制作和训练的递归神经网络在面对癫痫扰动时，表现出更高的活动水平和更早的性能下降。与这一预测一致，在体记录显示，内侧内嗅皮层（其网格细胞呈现连续吸引子动力学）驱动急性癫痫样放电时，参与程度更强且状态轨迹更平滑，而CA3（与离散记忆存储相关的海马亚区）则相反。此外，选择性突触沉默表明，这种癫痫反应的差异依赖于完整的内嗅连接。因此，使神经网络能够处理信息的计算功能也影响其对病理转变的脆弱性。

## Abstract
Brain areas differ in their inherent susceptibility to focal seizures, but the principles governing this risk remain unclear. While prior work has focused on anatomical and physiological factors, here we observed a fundamental contribution from the computations performed by the underlying neural network. Handcrafted and trained recurrent neural networks supporting continuous representations respond to seizure perturbations with higher activity and earlier performance decline relative to matched networks stabilizing discrete, well-separated states. Consistent with this prediction, in vivo recordings revealed that medial entorhinal cortex, whose grid cells exhibit continuous attractor dynamics, drives acute epileptiform discharges with stronger involvement and smoother state trajectories compared to CA3, a hippocampal subfield associated with discrete memory storage. Moreover, selective synaptic silencing demonstrated that this difference in seizure responses depends on intact entorhinal connectivity. Thus, the computations that enable neural networks to process information also influence their vulnerability to pathological transitions.