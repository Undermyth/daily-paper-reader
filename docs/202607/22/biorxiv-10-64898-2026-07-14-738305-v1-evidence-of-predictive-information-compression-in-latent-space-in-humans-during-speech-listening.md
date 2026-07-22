---
title: Evidence of predictive information compression in latent space in humans during speech listening
title_zh: 人类言语聆听时潜在空间中预测信息压缩的证据
authors: "Corsini, A., Schneider, S., Tomassini, A., Pedani, L., Fadiga, L., D'Ausilio, A."
date: 2026-07-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.14.738305v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 语音感知中的预测压缩模型
tldr: 语音感知的计算原理尚不明确，经典高效编码理论认为神经活动最优压缩感官输入，而另一些观点认为神经优先编码预测信息。本研究对比了三种模型：深度自编码器（最优压缩）、预测自编码器（预测重建）和对比学习（潜在空间预测信息）。结果表明，仅潜在空间预测信息表征能够最好地解释听语音时的脑电图活动，且其选择性压缩预测信息而非最大化压缩或输入预测，预测了行为表现。这说明人类语音神经表征以压缩预测信息的方式组织。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1761, \"height\": 1488, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1755, \"height\": 1174, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1737, \"height\": 1225, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1741, \"height\": 1639, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1726, \"height\": 1316, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1745, \"height\": 1713, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1752, \"height\": 1089, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1753, \"height\": 805, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738305-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1749, \"height\": 1569, \"label\": \"Figure\"}]"
motivation: 探究语音感知中神经表征的计算原则：是追求最优压缩，还是优先编码预测信息。
method: 构建三种模型（深度自编码器、预测自编码器、对比学习潜在空间预测），比较其潜在表征与听语音EEG的一致性。
result: 对比学习潜在空间预测信息表征最好地解释EEG潜在活动，且仅该表征选择性压缩预测信息并预测行为。
conclusion: 人类语音神经表征并非最大化压缩或输入预测，而是有选择地压缩潜在空间中的预测信息。
---

## 摘要
言语感知需要将听觉输入转化为支持语言理解的神经表征，但其潜在的计算原理仍不清楚。经典的高效编码理论主张对感官输入进行最优压缩，而另一些理论则认为神经系统优先编码支持预测的信息。一个关键未解问题是，这种预测编码是基于固定输入还是灵活的内部表征。我们实例化了三种言语处理假设模型：(i) 基于深度自编码器的最优压缩，(ii) 基于预测自编码器的预测重建，以及(iii) 通过对比学习进行潜在空间预测的预测信息表征。我们将得到的言语潜在表征与言语聆听期间的脑电图(EEG)活动进行比较。在预测信息目标下学习的表征最能解释神经潜在活动。关键的是，只有选择性压缩预测信息的表征才能预测行为表现，这表明神经言语表征的结构是为了在潜在空间中编码预测信息，而不是为了最大化压缩或输入预测。

## Abstract
Speech perception requires transforming acoustic input into neural representations that support linguistic understanding, yet its underlying computational principles remain unclear. Classical efficient coding theories posit optimal compression of sensory input, whereas alternative accounts propose that neural systems preferentially encode information that supports prediction. A key open question is whether such predictive encoding operates on fixed inputs or on flexible internal representations. We instantiated three hypothesis models of speech processing: (i) optimal compression with deep autoencoders, (ii) predictive reconstruction with predictive autoencoders, and (iii) predictive information representation via latent-space prediction using contrastive learning. We compared resulting speech latent representations to electroencephalographic (EEG) activity during speech listening. Representations learned under the predictive information objective best explained neural latents. Crucially, only representations that selectively compressed predictive information predicted behavioral performance, suggesting that neural speech representations are structured to encode predictive information in latent space rather than to maximize compression or input prediction.