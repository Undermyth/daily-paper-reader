---
title: Unsupervised Representation Learning Reveals Individualized Neurophysiological Profiles
title_zh: 无监督表征学习揭示个体化神经生理特征
authors: "Lapatrie, M., da Silva Castanheira, J., Aydin, I., Baillet, S."
date: 2026-06-26
pdf: "https://www.biorxiv.org/content/10.64898/2026.02.10.705127v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 无监督自编码器神经生理学特征提取
tldr: "现有脑电剖面建模依赖标签或监督目标，难以区分稳定生物学特征与可剥削的个体特异信号。本文提出参与者无关的自编码器框架，仅以重建为训练目标，从短时静息态MEG中学习潜在空间，无标签下自发形成具有区分力的剖面。120秒数据内剖面识别准确率93.3%，短至14秒仍有效；跨会话准确率49.5%高于随机，年龄预测R²=0.318，解码器支持谱和连接空间的敏感性分析。"
source: biorxiv
selection_source: fresh_fetch
motivation: 现有模型依赖标签或监督目标，难以区分稳定生物学特征与可剥削的个体差异，需要无标签的剖面学习方法。
method: 提出参与者无关的自编码器，以重建损失为唯一目标，从短时静息态MEG学习潜在空间，无需参与者标签。
result: "120秒内剖面识别准确率93.3%，短至14秒有效；跨会话准确率49.5%高于随机，年龄预测R²=0.318。"
conclusion: 参与者无关表示学习可生成可解释、可泛化的神经生理剖面，为大规模个体化脑功能建模提供新范式。
---

## 摘要
人类大脑活动包含稳定、个体特定的特征，这些特征可持续数月乃至数年，形成神经生理特征。大多数基于模型的剖绘方法使用参与者标签或监督目标，使得难以确定成功的区分是反映了稳定的生物学特征还是可被利用的特异性。我们引入了一种参与者无关的自编码器框架，通过将重建作为唯一训练目标，从短暂的静息态脑磁图（MEG）片段中提取特征。从学习到的潜在空间中，无需参与者标签即可产生具有区分性的特征。在同一次记录中，自编码器特征在120秒时达到93.3%的准确率，当源重建中未使用参与者特定的解剖结构时，即便记录短至14秒，其表现也优于功能连接、频谱和对比基线。在不同记录会话之间，区分能力高于随机水平（预训练自编码器的会话间准确率为49.5%）。这些特征在年龄预测上也比基线更准确（r^2=0.318），并且解码器支持在频谱和连接空间中进行基于扰动的敏感性分析。这确立了参与者无关的表征学习作为一种可扩展且可解释的剖绘方法。

## Abstract
Human brain activity contains stable, individual-specific features that persist over months to years, forming neurophysiological profiles. Most model-based profiling approaches use participant labels or supervised objectives, making it difficult to determine whether successful differentiation reflects stable biology or exploitable idiosyncrasies. We introduce a participant-agnostic autoencoder framework that derives profiles from brief resting-state magnetoencephalography (MEG) segments using reconstruction as sole training objective. Discriminative profiles emerged from the learned latent space without participant labels. Within-session, autoencoder profiles reached 93.3% accuracy at 120 s, exceeding functional-connectivity, spectral, and contrastive baselines with recordings as short as 14 s when participant-specific anatomy was withheld from source reconstruction. Differentiation generalized above chance across recording sessions (between-session accuracy 49.5% for the pretrained autoencoder). Profiles also predicted age more accurately than baselines (r^2=0.318), and the decoder enabled perturbation-based sensitivity analyses in spectral and connectivity spaces. This establishes participant-agnostic representation learning as a scalable and interpretable profiling.