---
title: Stimulus and circuit contributions to the information geometry of neural manifolds
title_zh: 刺激与回路对神经流形信息几何的贡献
authors: "Goedeke, S., Kautz, J. K., Leibold, C."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.21.733384v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 发展神经流形的微分几何框架，连接连接性与信息几何
tldr: 神经网络群体活动常呈现低维流形结构，但其与网络机制的联系缺乏严格框架。本文提出微分几何方法，推导出神经流形的拉回度量，并证明Fisher信息矩阵同样具有拉回度量结构，从而直接联系流形几何与信息编码。关键发现是慢相关噪声下递归连接的影响抵消，前馈连接单独决定表征几何。将理论应用于网格细胞空间表征，证明前馈变换可将随机调谐曲线映射为环形流形，无需递归连接或持续吸引子动力学。
source: biorxiv
selection_source: fresh_fetch
motivation: 缺乏严格框架连接神经网络流形几何与网络机制及信息编码。
method: 推导率编码递归网络中神经流形的拉回度量与Fisher信息的统一表达式。
result: 前馈连接决定流形几何，递归连接仅改善快速噪声下的编码。
conclusion: 前馈连接即可生成结构化网格细胞空间表征，无需特定递归连接或持续吸引子。
---

## 摘要
理解网络连接如何塑造神经表征是系统神经科学的核心问题。虽然降维方法揭示了群体记录中的低维流形结构，但将流形几何与网络机制及信息编码联系起来的严格框架仍然缺乏。我们发展了一种微分几何方法，用于分析接收调谐前馈输入的基于发放率的递归网络中的神经流形。我们推导了神经流形的拉回度量的表达式，展示了输入调谐曲线以及前馈和递归突触连接如何塑造流形几何。关键地，我们证明了稳态下的费希尔信息矩阵也具有拉回度量的结构，直接将内在流形几何与刺激可辨别性和信息编码联系起来。对于通过网络传播的具有慢时间相关性的噪声，我们展示了递归对信息几何的效应相互抵消：费希尔信息仅依赖于前馈连接。因此，前馈连接关键地决定了表征几何。我们将该方法应用于一个六边形网格细胞模块对空间的表征。我们首先证明，对于随机的网格相位分布，该表征近似等距。此外，线性前馈变换可以将空间随机的输入调谐曲线映射成一群六边形网格细胞，生成环形神经流形。因此，仅前馈连接就能生成结构化的空间表征，而无需精细调谐的递归连接或连续吸引子动力学。然而，递归连接被证明可以在快噪声下改进刺激编码，从而实现选择性降噪。

## Abstract
Understanding how network connectivity shapes neural representations is central to systems neuroscience. While dimensionality reduction methods uncover low-dimensional manifold structure in population recordings, a rigorous framework connecting manifold geometry to network mechanisms and information encoding remains lacking. We develop a differential geometric approach for analyzing neural manifolds in rate-based recurrent networks receiving tuned feedforward inputs. We derive expressions for the pullback metric of neural manifolds, showing how input tuning curves together with feedforward and recurrent synaptic connectivity shape manifold geometry. Critically, we establish that the Fisher information matrix at steady states also has the structure of a pullback metric, directly linking intrinsic manifold geometry to stimulus discriminability and information encoding. For noise with slow temporal correlations propagated through the network, we show that recurrent effects on information geometry cancel: Fisher information depends only on the feedforward connectivity. Thus, feedforward connectivity critically determines representational geometry. We apply our approach to the representation of space by a module of hexagonal grid cells. We first demonstrate that the representation is approximately isometric for a random distribution of grid phases. Moreover, a linear feedforward transformation can map spatially random input tuning curves into a population of hexagonal grid cells, generating a toroidal neural manifold. Thus, feedforward connectivity alone can generate structured spatial representations without requiring carefully tuned recurrent connectivity or continuous attractor dynamics. Recurrent connectivity, however, is shown to improve stimulus encoding under fast noise, thereby implementing a selective noise reduction.