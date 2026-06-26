---
title: Unsupervised Representation Learning Reveals Individualized Neurophysiological Profiles
title_zh: 无监督表示学习揭示个体化神经生理特征
authors: "Lapatrie, M., da Silva Castanheira, J., Aydin, I., Baillet, S."
date: 2026-06-26
pdf: "https://www.biorxiv.org/content/10.64898/2026.02.10.705127v2.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 使用无监督自编码器从脑磁图学习神经生理特征，属于计算神经科学表征学习。
tldr: "现有神经生理概况方法依赖参与者标签或有监督目标，难以区分稳定生物学与可利用特质。本文提出参与者无关的自动编码器框架，仅以重构为训练目标，从短至14秒的静息态MEG片段中学习判别性潜在空间。会话内120秒准确率93.3%，短片段仍超越基线；跨会话泛化高于偶然（49.5%），年龄预测精度更高（r²=0.318）。该方法可扩展且可解释，为无监督个体概况建模提供了新途径。"
source: biorxiv
selection_source: fresh_fetch
motivation: 现有基于标签的概况方法难以区分稳定生物学与特质，需标签无关的模型以揭示内在神经特征。
method: 采用参与者无关的自动编码器，仅以信号重构为目标，从静息态MEG片段学习潜在空间，无监督提取判别性概况。
result: "会话内120秒准确率93.3%，14秒仍优于基线；跨会话准确率49.5%高于偶然；年龄预测r²=0.318。"
conclusion: 参与者无关的无监督表征学习可提供可扩展、可解释的个体神经生理概况，无需标签或个体解剖信息。
---

## 摘要
人类大脑活动包含稳定、个体特定的特征，这些特征可持续数月甚至数年，形成神经生理特征。大多数基于模型的特征提取方法使用参与者标签或有监督目标，导致难以判断成功的区分是否反映了稳定的生物学特征还是可利用的特异性。我们引入了一个参与者无关的自编码器框架，该框架以重构作为唯一训练目标，从短暂静息态脑磁图（MEG）片段中提取特征。在无参与者标签的情况下，从学习到的潜在空间中出现了具有区分性的特征。在会话内，自编码器特征在120秒时达到93.3%的准确率，当在源重建中隐藏了参与者特定的解剖结构时，仅需14秒的记录即可超越功能连接、频谱和对比基线。在跨记录会话中，区分能力高于随机水平（预训练自编码器的会话间准确率为49.5%）。这些特征在预测年龄方面也比基线更准确（r^2=0.318），并且解码器能够在频谱和连接空间中进行基于扰动的敏感性分析。这确立了参与者无关的表示学习作为一种可扩展且可解释的特征提取方法。

## Abstract
Human brain activity contains stable, individual-specific features that persist over months to years, forming neurophysiological profiles. Most model-based profiling approaches use participant labels or supervised objectives, making it difficult to determine whether successful differentiation reflects stable biology or exploitable idiosyncrasies. We introduce a participant-agnostic autoencoder framework that derives profiles from brief resting-state magnetoencephalography (MEG) segments using reconstruction as sole training objective. Discriminative profiles emerged from the learned latent space without participant labels. Within-session, autoencoder profiles reached 93.3% accuracy at 120 s, exceeding functional-connectivity, spectral, and contrastive baselines with recordings as short as 14 s when participant-specific anatomy was withheld from source reconstruction. Differentiation generalized above chance across recording sessions (between-session accuracy 49.5% for the pretrained autoencoder). Profiles also predicted age more accurately than baselines (r^2=0.318), and the decoder enabled perturbation-based sensitivity analyses in spectral and connectivity spaces. This establishes participant-agnostic representation learning as a scalable and interpretable profiling.