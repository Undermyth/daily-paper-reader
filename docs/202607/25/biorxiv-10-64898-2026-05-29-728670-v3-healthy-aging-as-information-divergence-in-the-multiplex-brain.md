---
title: HEALTHY AGING AS INFORMATION DIVERGENCE IN THE MULTIPLEX BRAIN
title_zh: 健康衰老作为多重脑网络中的信息发散
authors: "Ghosh, D., Uddin, L. Q., Ray, D., Das, M."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.29.728670v3.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 多路复用网络模型研究大脑老化
tldr: 大脑结构网络与功能网络的共同演化在衰老研究中缺乏整合框架。本研究将大脑建模为多网络，利用Jensen-Shannon散度和相对熵分析589名18-88岁健康人数据，发现功能性活动随年龄增长逐渐脱离结构约束，呈线性但空间异质的解耦过程。子皮层枢纽（壳核、苍白球、尾状核、丘脑）是分离中心，而边缘核心（海马、内嗅皮层）保持稳定。该工作为区分正常认知衰退与神经退行性疾病提供多网络基线。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-728670-v3/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1649, \"height\": 946, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-728670-v3/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1551, \"height\": 1240, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-728670-v3/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1711, \"height\": 1289, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-728670-v3/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1695, \"height\": 955, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-728670-v3/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1704, \"height\": 631, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-05-29-728670-v3/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1508, \"height\": 265, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-05-29-728670-v3/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1594, \"height\": 812, \"label\": \"Table\"}]"
motivation: 缺乏整合框架研究大脑结构-功能连接组在衰老中的共同演化。
method: 构建多网络脑模型，使用Jensen-Shannon散度和相对熵量化跨年龄结构-功能耦合。
result: 功能动态与结构解耦呈线性趋势，子皮层枢纽是分离中心，边缘核心稳定性显著。
conclusion: 健康衰老特征是子皮层解耦与边缘弹性，为鉴别正常与病理衰老提供多网络基准。
---

## 摘要
理解人类大脑结构支架与功能活动在成年寿命中的共同演化仍然是神经科学的一个基本挑战。虽然灰质和功能激活的年龄相关退化已有充分记录，但由于缺乏整合框架，结构连接组（SC）和功能连接组（FC）的共同轨迹常常被忽视。在此，我们将大脑建模为多重网络，以量化来自剑桥衰老与神经科学中心（CamCAN）数据集的589名健康个体（年龄18至88岁）的横截面队列中这两层之间的信息论相互依赖性。使用詹森-香农散度和相对熵指标，我们识别出健康衰老的一个基本组织原则，其特征在于渐进的信息发散，其中功能动力学越来越脱离其潜在的结构约束。我们的结果显示，这种解耦遵循稳健的线性轨迹，但在空间上高度异质。使用多重网络映射方程的中尺度社区分析确定皮层下枢纽——特别是壳核、苍白球、尾状核和丘脑——作为年龄相关SC-FC发散的主要中心点。这种皮层下交换板向功能独立性的拓扑转变，为伴随衰老的流体智力和运动适应性的众所周知衰退提供了机制性连接组特征。与此形成鲜明对比的是，边缘核心（海马体和内嗅皮层）在整个生命周期中表现出显著的稳定性，表明在全球通信重新布线中，存在保护高保真记忆回路的生物学必要性。通过将健康衰老视为系统性皮层下解脱与边缘弹性的结合，我们的工作提供了一种强大的新多重基线，以区分正常认知衰退与神经退行性疾病的早期拓扑信号。

## Abstract
Understanding the coevolution of the human brain's structural scaffold and functional traffic across the adult lifespan remains a fundamental challenge in neuroscience. While age related degradation in grey matter and functional activation is well documented, the joint trajectory of the structural (SC) and functional (FC) connectomes is often overlooked due to the lack of an integrative framework. Here, we model the brain as a multiplex network to quantify the information theoretic interdependencies between these two layers in a cross-sectional cohort of 589 healthy individuals (ages 18 to 88) from the Cambridge Centre for Ageing and Neuroscience (CamCAN) dataset. Using Jensen Shannon Divergence and relative entropy metrics, we identify a fundamental organizing principle of healthy aging characterized by a progressive information divergence where functional dynamics increasingly untether from their underlying structural constraints. Our results reveal that this decoupling follows a robust linear trajectory, yet is highly spatially heterogeneous. Meso-scale community analysis using the Multiplex Map Equation identifies subcortical hubs specifically the putamen, pallidum, caudate, and thalamus as the primary epicenters of age-related SC FC divergence. This topological shift toward functional independence in subcortical switchboards provides a mechanistic connectomic signature for the well documented decline in fluid intelligence and motor adaptation that accompanies aging. In striking contrast, the limbic core (hippocampus and entorhinal cortex) exhibits remarkable stability across the lifespan, suggesting a biological imperative to preserve high fidelity memory circuits amidst global communicative rewiring. By framing healthy aging as a systematic subcortical untethering alongside limbic resilience, our work provides a powerful new multiplex baseline to distinguish normative cognitive decline from the early topological signals of neurodegenerative disease.