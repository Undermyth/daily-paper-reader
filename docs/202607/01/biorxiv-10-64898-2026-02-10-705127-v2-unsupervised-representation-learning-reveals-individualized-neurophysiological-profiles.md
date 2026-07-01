---
title: Unsupervised Representation Learning Reveals Individualized Neurophysiological Profiles
title_zh: 无监督表征学习揭示个性化神经生理特征
authors: "Lapatrie, M., da Silva Castanheira, J., Aydin, I., Baillet, S."
date: 2026-06-26
pdf: "https://www.biorxiv.org/content/10.64898/2026.02.10.705127v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 无监督表示学习用于神经生理学特征板
tldr: "脑活动存在稳定个体特征，但现有监督方法难以区分生物学稳定与数据伪影。本文提出参与者不可知的自动编码器，仅用重建目标从短时静息态MEG数据学习潜在表征。120秒内识别准确率达93.3%，14秒即超越基线，且跨会话泛化、年龄预测优于基线。该方法为可扩展、可解释的神经生理轮廓提供了新范式。"
source: biorxiv
selection_source: fresh_fetch
motivation: 现有依赖标签的个体差异建模难以区分稳定生物学与数据伪影，需无监督方法挖掘真实神经特征。
method: 提出参与者不可知的自动编码器，仅以重建为目标从静息态MEG片段学习潜在空间，不使用任何标签。
result: "120秒内准确率93.3%，14秒超基线；跨会话准确率49.5%（高于随机），年龄预测r²=0.318。"
conclusion: 无监督表示学习可生成可解释、跨会话泛化的个体化神经生理轮廓，适用于短时记录分析。
---

## 摘要
人类大脑活动包含稳定且个体特异的特征，这些特征可持续数月乃至数年，形成神经生理特征。大多数基于模型的特征分析方法使用参与者标签或有监督目标，因此难以确定成功的区分是否反映了稳定的生物学特性还是可利用的特异性。我们提出了一种参与者无关的自编码器框架，该框架仅以重建为训练目标，从短时静息态脑磁图（MEG）片段中提取特征。在无参与者标签的情况下，从学习到的潜在空间中涌现出了具有区分能力的特征。在同一会话内，自编码器特征在120秒时达到93.3%的准确率，当源重建中隐去参与者特有的解剖结构时，即便使用短至14秒的记录，其性能也超过了功能连接、频谱和对比基线方法。特征在不同会话间的区分能力高于随机水平（预训练自编码器的会话间准确率为49.5%）。此外，特征对年龄的预测准确率也高于基线方法（r²=0.318），而解码器能够在频谱和连接空间中进行基于扰动的敏感性分析。这确立了参与者无关的表征学习作为一种可扩展且可解释的特征分析方法。

## Abstract
Human brain activity contains stable, individual-specific features that persist over months to years, forming neurophysiological profiles. Most model-based profiling approaches use participant labels or supervised objectives, making it difficult to determine whether successful differentiation reflects stable biology or exploitable idiosyncrasies. We introduce a participant-agnostic autoencoder framework that derives profiles from brief resting-state magnetoencephalography (MEG) segments using reconstruction as sole training objective. Discriminative profiles emerged from the learned latent space without participant labels. Within-session, autoencoder profiles reached 93.3% accuracy at 120 s, exceeding functional-connectivity, spectral, and contrastive baselines with recordings as short as 14 s when participant-specific anatomy was withheld from source reconstruction. Differentiation generalized above chance across recording sessions (between-session accuracy 49.5% for the pretrained autoencoder). Profiles also predicted age more accurately than baselines (r2=0.318), and the decoder enabled perturbation-based sensitivity analyses in spectral and connectivity spaces. This establishes participant-agnostic representation learning as a scalable and interpretable profiling.