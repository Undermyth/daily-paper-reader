---
title: Stimulus and circuit contributions to the information geometry of neural manifolds
title_zh: 刺激和回路对神经流形信息几何的贡献
authors: "Goedeke, S., Kautz, J. K., Leibold, C."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.21.733384v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 神经流形信息几何
tldr: 神经群体活动的低维流形几何与网络机制的关系缺乏严格理论。本文提出微分几何框架，推导率网络神经流形的拉回度量，并证明稳态Fisher信息矩阵也具有相同结构，从而直接链接流形几何与刺激编码。应用于网格细胞，发现仅前馈连接即可将随机输入映射为环面流形，无需递归或吸引子动态；递归连接则通过选择性降噪改善快噪声下的编码。工作揭示了前馈连接决定表征几何的核心作用。
source: biorxiv
selection_source: fresh_fetch
motivation: 缺乏将神经流形几何与网络连接及信息编码联系起来的严格理论框架。
method: 提出微分几何方法，推导率网络中神经流形的拉回度量，并证明Fisher信息矩阵也具有相同结构。
result: 前馈连接单独即可生成网格细胞环面流形；递归连接仅改善快噪声下的编码。
conclusion: 前馈连接决定表征几何，递归连接实现选择性降噪，无需连续吸引子机制。
---

## 摘要
理解网络连接如何塑造神经表征是系统神经科学的核心。虽然降维方法揭示了群体记录中的低维流形结构，但将流形几何与网络机制和信息编码联系起来的严格框架仍然缺乏。我们开发了一种微分几何方法，用于分析速率递归网络中接收调谐前馈输入的神经流形。我们推导了神经流形的拉回度量表达式，展示了输入调谐曲线以及前馈和递归突触连接如何塑造流形几何。关键地，我们证明了稳态下的Fisher信息矩阵也具有拉回度量的结构，直接将内在流形几何与刺激可辨别性和信息编码联系起来。对于通过网络传播的具有慢时间相关性的噪声，我们表明递归效应对信息几何的影响抵消：Fisher信息仅依赖于前馈连接。因此，前馈连接关键地决定了表征几何。我们将我们的方法应用于六边形网格细胞模块对空间的表征。我们首先证明了对于随机分布的网格相位，表征近似等距。此外，线性前馈变换可以将空间随机输入调谐曲线映射到六边形网格细胞群体，生成环面神经流形。因此，单独的前馈连接就可以生成结构化的空间表征，而不需要精心调谐的递归连接或连续吸引子动力学。然而，递归连接被证明可以在快速噪声下改善刺激编码，从而实现选择性降噪。

## Abstract
Understanding how network connectivity shapes neural representations is central to systems neuroscience. While dimensionality reduction methods uncover low-dimensional manifold structure in population recordings, a rigorous framework connecting manifold geometry to network mechanisms and information encoding remains lacking. We develop a differential geometric approach for analyzing neural manifolds in rate-based recurrent networks receiving tuned feedforward inputs. We derive expressions for the pullback metric of neural manifolds, showing how input tuning curves together with feedforward and recurrent synaptic connectivity shape manifold geometry. Critically, we establish that the Fisher information matrix at steady states also has the structure of a pullback metric, directly linking intrinsic manifold geometry to stimulus discriminability and information encoding. For noise with slow temporal correlations propagated through the network, we show that recurrent effects on information geometry cancel: Fisher information depends only on the feedforward connectivity. Thus, feedforward connectivity critically determines representational geometry. We apply our approach to the representation of space by a module of hexagonal grid cells. We first demonstrate that the representation is approximately isometric for a random distribution of grid phases. Moreover, a linear feedforward transformation can map spatially random input tuning curves into a population of hexagonal grid cells, generating a toroidal neural manifold. Thus, feedforward connectivity alone can generate structured spatial representations without requiring carefully tuned recurrent connectivity or continuous attractor dynamics. Recurrent connectivity, however, is shown to improve stimulus encoding under fast noise, thereby implementing a selective noise reduction.