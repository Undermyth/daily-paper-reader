---
title: Decoding and Characterizing the Intracranial Representation of Semantic Information
title_zh: 解码与表征语义信息的颅内表征
authors: "Smith, C., Inchyna, S., Barrentine, B., Nelson, M. J."
date: 2026-07-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.13.738249v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 从颅内记录解码语义表征以支持推理
tldr: "脑机接口在解码运动/发音信号上表现优异，但高层语义解码尚不明确。本研究通过颅内立体脑电图(sEEG)记录患者进行语义任务时的神经活动，提取高伽马功率作为特征，利用机器学习分类15个语义类别。平均分类准确率达29.8%（随机水平6.7%），证明高伽马活动包含概念类别信息。该工作证实语义信息可从颅内群体活动解码，为发展基于概念而非纯发音信息的语言BCI提供新方向，并深化对语言网络分布式概念表征的理解。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738249-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1235, \"height\": 1127, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738249-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1027, \"height\": 1011, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738249-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1139, \"height\": 1114, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738249-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1534, \"height\": 1586, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-13-738249-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1336, \"height\": 1100, \"label\": \"Table\"}]"
motivation: 探索能否从人类颅内皮层活动中解码高层语义表征，以推动概念驱动型语言脑机接口的发展。
method: 记录癫痫患者进行语义任务时的sEEG信号，提取高伽马功率特征，用监督学习分类15个语义类别并通过交叉验证评估。
result: "语义分类平均准确率29.8%，显著高于随机水平6.7%，表明高伽马活动蕴含可单次提取的概念类别信息。"
conclusion: 颅内群体记录可解码语义信息，支持语义解码作为语言BCI的补充路径，并促进对分布式语言网络概念表征的理解。
---

## 摘要
脑机接口通过解码与语音产生相关的运动和发音信号已取得显著性能。然而，关于是否能够从人类皮层活动中解码更高层次的语义表征，我们知之甚少。展示语义解码将推动我们对语言组织的理解，以及依赖概念信息而非纯粹发音信息的脑机接口发展。我们记录了接受立体定向脑电图（sEEG）进行临床癫痫监测的患者在执行需要语义处理的语言任务时的颅内神经活动。从局部场电位中提取高伽马功率，并用于生成试验级特征以进行监督机器学习分类。使用交叉验证评估分类性能。语义类别信息的解码显著高于随机水平，15个语义类别的平均分类准确率达到29.8%（随机水平为6.7%）。这些发现表明，高伽马活动包含关于概念类别成员的信息，可以在单个试验中提取。这些结果提供了证据，表明语义信息可以从颅内群体记录中获取，并支持语义解码作为未来语言脑机接口的补充方向的可行性。除了神经假体应用外，这项工作还有助于理解概念知识如何在分布式人类语言网络中表征。

## Abstract
Brain-computer interfaces (BCIs) have achieved impressive performance by decoding motor and articulatory signals associated with speech production. However, considerably less is known about whether higher-level semantic representations can be decoded from human cortical activity. Demonstrating semantic decoding would advance both our understanding of language organization and the development of BCIs that rely on conceptual rather than purely articulatory information. We recorded intracranial neural activity from patients undergoing stereotactic electroencephalography (sEEG) for clinical epilepsy monitoring while they performed language tasks requiring semantic processing. High-gamma power was extracted from local field potentials and used to generate trial-level features for supervised machine-learning classification. Classification performance was evaluated using cross-validation. Semantic category information was decoded significantly above chance, with mean classification accuracy reaching 29.8% across 15 semantic categories (chance = 6.7%). These findings demonstrate that high-gamma activity contains information about conceptual category membership that can be extracted on individual trials. These results provide evidence that semantic information is accessible from intracranial population recordings and support the feasibility of semantic decoding as a complementary direction for future language BCIs. Beyond neuroprosthetic applications, this work contributes to understanding how conceptual knowledge is represented in the distributed human language network.