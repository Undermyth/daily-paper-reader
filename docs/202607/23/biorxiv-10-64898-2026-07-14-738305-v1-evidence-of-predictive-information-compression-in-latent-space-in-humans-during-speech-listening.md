---
title: Evidence of predictive information compression in latent space in humans during speech listening
title_zh: 言语聆听过程中人类潜在空间预测信息压缩的证据
authors: "Corsini, A., Schneider, S., Tomassini, A., Pedani, L., Fadiga, L., D'Ausilio, A."
date: 2026-07-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.14.738305v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 语音感知中的预测信息压缩，计算神经科学
tldr: 语音感知需将声学输入转化为支持语言理解的神经表征，但计算原则尚不明确。本研究比较三种假设模型：深度自编码器的最优压缩、预测自编码器的输入预测、以及基于对比学习的潜在空间预测信息压缩。通过对比语音表征与听语音时的脑电图，发现预测信息表征模型最佳解释神经活动，且仅选择性压缩预测信息的表征能预测行为表现。这表明人脑语音神经表征在潜在空间中编码预测信息，而非追求最大压缩或输入预测。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1761, \"height\": 1488, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1755, \"height\": 1174, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1737, \"height\": 1225, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1741, \"height\": 1639, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1726, \"height\": 1316, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1745, \"height\": 1713, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1752, \"height\": 1089, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1753, \"height\": 805, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1749, \"height\": 1569, \"label\": \"Figure\"}]"
motivation: 检验语音感知中神经表征是否优先编码预测信息，而非单纯压缩输入或预测输入。
method: 实例化三种计算模型（最优压缩、预测重建、潜在空间预测），比较其语音表征与EEG数据的匹配度。
result: 潜在空间预测表征最佳拟合脑电数据，且仅此表征能预测行为表现，表明预测信息压缩是关键。
conclusion: 人脑语音表征在潜在空间选择性压缩预测信息，而非最大化压缩或输入重建。
---

## 摘要
言语感知需要将听觉输入转化为支持语言理解的神经表征，但其基本的计算原理仍不清楚。经典高效编码理论认为感觉输入的最优压缩，而另一种观点提出神经系统优先编码支持预测的信息。一个关键未决问题是这种预测编码是否作用于固定输入还是灵活的内部表征。我们实例化了三种言语处理假设模型：(i) 使用深度自编码器的最优压缩，(ii) 使用预测自编码器的预测重建，以及(iii) 通过对比学习利用潜在空间预测的预测信息表征。我们将得到的言语潜在表征与言语聆听期间的脑电图（EEG）活动进行比较。在预测信息目标下学到的表征最能解释神经潜在变量。关键的是，只有选择性压缩预测信息的表征才能预测行为表现，这表明神经言语表征的结构是为了在潜在空间中编码预测信息，而不是最大化压缩或输入预测。

## Abstract
Speech perception requires transforming acoustic input into neural representations that support linguistic understanding, yet its underlying computational principles remain unclear. Classical efficient coding theories posit optimal compression of sensory input, whereas alternative accounts propose that neural systems preferentially encode information that supports prediction. A key open question is whether such predictive encoding operates on fixed inputs or on flexible internal representations. We instantiated three hypothesis models of speech processing: (i) optimal compression with deep autoencoders, (ii) predictive reconstruction with predictive autoencoders, and (iii) predictive information representation via latent-space prediction using contrastive learning. We compared resulting speech latent representations to electroencephalographic (EEG) activity during speech listening. Representations learned under the predictive information objective best explained neural latents. Crucially, only representations that selectively compressed predictive information predicted behavioral performance, suggesting that neural speech representations are structured to encode predictive information in latent space rather than to maximize compression or input prediction.