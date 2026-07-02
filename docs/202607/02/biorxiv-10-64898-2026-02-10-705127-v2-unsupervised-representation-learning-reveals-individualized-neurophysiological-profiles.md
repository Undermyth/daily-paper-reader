---
title: Unsupervised Representation Learning Reveals Individualized Neurophysiological Profiles
title_zh: 无监督表征学习揭示个体化神经生理特征
authors: "Lapatrie, M., da Silva Castanheira, J., Aydin, I., Baillet, S."
date: 2026-06-26
pdf: "https://www.biorxiv.org/content/10.64898/2026.02.10.705127v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 基于无监督表征学习的个体化神经生理特征提取
tldr: "人脑活动存在稳定的个体特征，但现有模型依赖标签或监督目标，难以区分生物学信号与个体特殊性。本文提出参与者无关的自编码器，仅以重构为训练目标，从静息态MEG片段中学习潜在表示。在会话内区分准确率达93.3%（120秒），短至14秒仍有效，跨会话准确率49.5%，年龄预测r²=0.318。该方法可扩展且可解释，适用于个性化神经生理图谱。"
source: biorxiv
selection_source: fresh_fetch
motivation: 基于标签的神经生理图谱方法难以区分稳定生物学与个体特殊性，需参与者无关的表示学习。
method: 提出自编码器框架，以重构为唯一目标，从简短静息态MEG片段中学习个体特异性的潜在表征。
result: "会话内准确率93.3%（120秒），14秒仍有效；跨会话准确率49.5%；年龄预测r²=0.318。"
conclusion: 参与者无关表示学习可生成可解释、个性化的神经生理图谱，具有可扩展性和鲁棒性。
---

## 摘要
人类大脑活动包含稳定且个体特定的特征，这些特征可持续数月甚至数年，形成神经生理特征。大多数基于模型的特征提取方法使用参与者标签或有监督的目标，因此难以确定成功的区分是反映了稳定的生物学特征还是可被利用的独特性。我们引入了一种参与者无关的自编码器框架，该框架以重建作为唯一训练目标，从短暂的静息态脑磁图（MEG）片段中提取特征。在无参与者标签的情况下，从学习到的潜在空间中涌现出具有判别性的特征。在会话内，自编码器特征在120秒时达到93.3%的准确率，当在源重建中隐藏参与者特定解剖结构时，即使记录时间短至14秒，其性能也超过了功能连接、频谱和对比基线。跨会话的区分能力高于随机水平（预训练自编码器的会话间准确率为49.5%）。这些特征在预测年龄方面也比基线更准确（r²=0.318），并且解码器能够在频谱和连接空间中实现基于扰动的敏感性分析。这确立了参与者无关的表征学习作为一种可扩展且可解释的特征提取方法。

## Abstract
Human brain activity contains stable, individual-specific features that persist over months to years, forming neurophysiological profiles. Most model-based profiling approaches use participant labels or supervised objectives, making it difficult to determine whether successful differentiation reflects stable biology or exploitable idiosyncrasies. We introduce a participant-agnostic autoencoder framework that derives profiles from brief resting-state magnetoencephalography (MEG) segments using reconstruction as sole training objective. Discriminative profiles emerged from the learned latent space without participant labels. Within-session, autoencoder profiles reached 93.3% accuracy at 120 s, exceeding functional-connectivity, spectral, and contrastive baselines with recordings as short as 14 s when participant-specific anatomy was withheld from source reconstruction. Differentiation generalized above chance across recording sessions (between-session accuracy 49.5% for the pretrained autoencoder). Profiles also predicted age more accurately than baselines (r2=0.318), and the decoder enabled perturbation-based sensitivity analyses in spectral and connectivity spaces. This establishes participant-agnostic representation learning as a scalable and interpretable profiling.