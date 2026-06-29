---
title: Stimulus and circuit contributions to the information geometry of neural manifolds
title_zh: 刺激与回路对神经流形信息几何的贡献
authors: "Goedeke, S., Kautz, J. K., Leibold, C."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.21.733384v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 神经流形几何与信息编码
tldr: 系统神经科学需要理解网络连接如何塑造神经表征，但现有框架缺乏严格联系流形几何与网络机制。我们开发了微分几何方法，推导出神经流形的拉回度量，并证明稳态下Fisher信息矩阵也具有相同结构，从而连接内在几何与刺激编码。对于慢相关噪声，递归效应抵消，仅前馈连接决定几何。应用于网格细胞，发现随机相位下表征近似等距，且线性前馈变换即可生成环形流形。贡献在于建立了量化流形几何与编码关系的理论，并揭示前馈连接的核心作用。
source: biorxiv
selection_source: fresh_fetch
motivation: 缺乏严格框架将神经流形几何与网络机制及信息编码联系起来。
method: 开发微分几何方法分析速率递归网络，推导拉回度量表征流形几何。
result: 前馈连接决定Fisher信息；网格细胞中随机相位产生等距表征，线性前馈生成环形流形。
conclusion: 前馈连接足以构建结构化空间表征，递归连接仅在快噪声下改善编码。
---

## 摘要
理解网络连接如何塑造神经表征是系统神经科学的核心。尽管降维方法在群体记录中揭示了低维流形结构，但将流形几何与网络机制及信息编码联系起来的严格框架仍然缺失。我们发展了一种微分几何方法，用于分析在接收调谐前馈输入的基于放电率的递归网络中的神经流形。我们推导了神经流形的拉回度量表达式，展示了输入调谐曲线以及前馈和递归突触连接如何塑造流形几何。关键的是，我们证明了稳态下的费希尔信息矩阵也具有拉回度量的结构，直接将内在流形几何与刺激可辨别性和信息编码联系起来。对于通过网络传播的具有慢时间相关性的噪声，我们展示了递归对信息几何的影响相互抵消：费希尔信息仅依赖于前馈连接。因此，前馈连接关键性地决定了表征几何。我们将我们的方法应用于一个六边形网格细胞模块的空间表征。我们首先证明，对于随机的网格相位分布，该表征近似等距。此外，线性前馈变换可以将空间随机的输入调谐曲线映射到一群六边形网格细胞，生成环面神经流形。因此，仅前馈连接就能生成结构化的空间表征，无需精心调谐的递归连接或连续吸引子动力学。然而，递归连接被证明可以在快速噪声下改善刺激编码，从而实现选择性降噪。

## Abstract
Understanding how network connectivity shapes neural representations is central to systems neuroscience. While dimensionality reduction methods uncover low-dimensional manifold structure in population recordings, a rigorous framework connecting manifold geometry to network mechanisms and information encoding remains lacking. We develop a differential geometric approach for analyzing neural manifolds in rate-based recurrent networks receiving tuned feedforward inputs. We derive expressions for the pullback metric of neural manifolds, showing how input tuning curves together with feedforward and recurrent synaptic connectivity shape manifold geometry. Critically, we establish that the Fisher information matrix at steady states also has the structure of a pullback metric, directly linking intrinsic manifold geometry to stimulus discriminability and information encoding. For noise with slow temporal correlations propagated through the network, we show that recurrent effects on information geometry cancel: Fisher information depends only on the feedforward connectivity. Thus, feedforward connectivity critically determines representational geometry. We apply our approach to the representation of space by a module of hexagonal grid cells. We first demonstrate that the representation is approximately isometric for a random distribution of grid phases. Moreover, a linear feedforward transformation can map spatially random input tuning curves into a population of hexagonal grid cells, generating a toroidal neural manifold. Thus, feedforward connectivity alone can generate structured spatial representations without requiring carefully tuned recurrent connectivity or continuous attractor dynamics. Recurrent connectivity, however, is shown to improve stimulus encoding under fast noise, thereby implementing a selective noise reduction.