---
title: HEALTHY AGING AS INFORMATION DIVERGENCE IN THE MULTIPLEX BRAIN
title_zh: 健康衰老作为多层级大脑中的信息散度
authors: "Ghosh, D., Ray, D., Das, M., Uddin, L. Q."
date: 2026-07-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.29.728670v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 多路复用网络模型研究大脑老化
tldr: 人脑结构连接与功能连接随年龄变化的共进化关系尚不清晰。本研究将大脑建模为多通路网络，利用Jensen Shannon散度量化结构-功能耦合在589名健康成年人中的变化。结果发现功能动态逐渐脱离结构约束，皮层下核团为解耦热点，而边缘系统保持稳定。该发现为正常认知衰退提供机制性解释，并可作为神经退行性疾病的早期区分基线。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-728670-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1649, \"height\": 947, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-728670-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1551, \"height\": 1240, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-728670-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1711, \"height\": 1289, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-728670-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1695, \"height\": 955, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-05-29-728670-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1704, \"height\": 631, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-05-29-728670-v2/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1508, \"height\": 265, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-05-29-728670-v2/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1594, \"height\": 812, \"label\": \"Table\"}]"
motivation: 现有研究多独立关注结构或功能老化，缺乏统一框架分析二者联合轨迹。
method: 将大脑建模为多通路网络，用Jensen Shannon散度和相对熵度量结构-功能耦合随年龄变化。
result: 功能-结构解耦呈线性增加，皮层下核团为解耦中心，边缘系统保持稳定。
conclusion: 健康老龄化特征是皮层下功能独立性增加与边缘记忆回路弹性并存，可作为认知衰退的生物标记。
---

## 摘要
理解人类大脑结构支架与功能流量在整个成年期的共同演化仍然是神经科学中的一个基本挑战。虽然灰质和功能激活的年龄相关退化已有充分记录，但由于缺乏整合框架，结构和功能连接组的联合轨迹常常被忽视。在这里，我们将大脑建模为一个多层级网络，以量化来自剑桥衰老与神经科学中心（CamCAN）数据集的589名健康个体（年龄18至88岁）横断面队列中这两层之间的信息论相互依赖性。使用詹森-香农散度和相对熵指标，我们识别出一个健康衰老的基本组织原则，其特征是渐进的信息散度，其中功能动力学逐渐脱离其潜在的结构约束。我们的结果表明，这种解耦遵循稳健的线性轨迹，但在空间上高度异质。使用多层级映射方程的介观尺度社区分析识别出皮层下枢纽——特别是壳核、苍白球、尾状核和丘脑——作为年龄相关结构与功能连接组散度的主要中心。这种皮层下枢纽朝向功能独立性的拓扑转变，为伴随衰老的流体智力和运动适应能力下降提供了机制性的连接组特征。与之形成鲜明对比的是，边缘核心（海马体和内嗅皮层）在整个生命周期中表现出显著的稳定性，这表明在全局通信重新布线中，存在保护高保真记忆回路的生物学必要性。通过将健康衰老框架化为系统的皮层下脱离与边缘弹性，我们的工作提供了一个强大的新多层级基线，以区分正常认知衰退与神经退行性疾病的早期拓扑信号。

## Abstract
Understanding the coevolution of the human brain's structural scaffold and functional traffic across the adult lifespan remains a fundamental challenge in neuroscience. While age related degradation in grey matter and functional activation is well documented, the joint trajectory of the structural (SC) and functional (FC) connectomes is often overlooked due to the lack of an integrative framework. Here, we model the brain as a multiplex network to quantify the information theoretic interdependencies between these two layers in a cross-sectional cohort of 589 healthy individuals (ages 18 to 88) from the Cambridge Centre for Ageing and Neuroscience (CamCAN) dataset. Using Jensen Shannon Divergence and relative entropy metrics, we identify a fundamental organizing principle of healthy aging characterized by a progressive information divergence where functional dynamics increasingly untether from their underlying structural constraints. Our results reveal that this decoupling follows a robust linear trajectory, yet is highly spatially heterogeneous. Meso-scale community analysis using the Multiplex Map Equation identifies subcortical hubs specifically the putamen, pallidum, caudate, and thalamus as the primary epicenters of age-related SC FC divergence. This topological shift toward functional independence in subcortical switchboards provides a mechanistic connectomic signature for the well documented decline in fluid intelligence and motor adaptation that accompanies aging. In striking contrast, the limbic core (hippocampus and entorhinal cortex) exhibits remarkable stability across the lifespan, suggesting a biological imperative to preserve high fidelity memory circuits amidst global communicative rewiring. By framing healthy aging as a systematic subcortical untethering alongside limbic resilience, our work provides a powerful new multiplex baseline to distinguish normative cognitive decline from the early topological signals of neurodegenerative disease.