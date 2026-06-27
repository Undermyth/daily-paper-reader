---
title: Stimulus and circuit contributions to the information geometry of neural manifolds
title_zh: 刺激与回路对神经流形信息几何的贡献
authors: "Goedeke, S., Kautz, J. K., Leibold, C."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.21.733384v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 神经流形的信息几何、连接性、费舍尔信息
tldr: 神经群体活动常呈现低维流形，但缺乏联系流形几何与网络机制的严格框架。本文提出微分几何方法，推导了速率递归网络中神经流形的拉回度量，并证明稳态Fisher信息矩阵也具拉回度量结构，直接关联流形几何与刺激可区分性。慢噪声下递归效应抵消，信息几何仅由前馈连接决定；快噪声下递归改善编码。以网格细胞为例，仅前馈连接即可生成环形流形，无需递归或吸引子动力学。贡献在于建立了网络机制到表征几何的解析桥梁。
source: biorxiv
selection_source: fresh_fetch
motivation: 缺乏将神经流形几何与网络突触机制及信息编码相联系的严格理论框架。
method: 采用微分几何，推导递归网络中流形的拉回度量及Fisher信息矩阵。
result: 前馈连接在慢噪声下决定信息几何；快噪声下递归改善编码；前馈可生成网格细胞环形流形。
conclusion: 前馈连接足以构建结构化空间表征，递归连接实现选择性降噪。
---

## 摘要
理解网络连接如何塑造神经表征是系统神经科学的核心问题。虽然降维方法揭示了群体记录中的低维流形结构，但缺乏将流形几何与网络机制及信息编码联系起来的严格框架。我们发展了一种微分几何方法，用于分析在接收调谐前馈输入的速率基递归网络中的神经流形。我们推导了神经流形的拉回度量表达式，展示了输入调谐曲线、前馈和递归突触连接如何塑造流形几何。关键的是，我们建立了稳态下的Fisher信息矩阵也具有拉回度量的结构，直接将内在流形几何与刺激可分辨性和信息编码联系起来。对于通过网络传播的具有慢时间相关性的噪声，我们表明递归效应在信息几何上相互抵消：Fisher信息仅依赖于前馈连接。因此，前馈连接关键地决定了表征几何。作为例子，我们证明了一个六边形网格细胞模块对于随机分布的网格相位大致是等距的。此外，一个线性前馈变换可以将空间随机输入调谐曲线映射到一群六边形网格细胞，形成环面流形。因此，仅前馈连接就能生成结构化的空间表征，而无需精心调整的递归连接或连续吸引子动力学。然而，递归连接被证明能在快噪声下改善刺激编码，从而实现选择性降噪。

## Abstract
Understanding how network connectivity shapes neural representations is central to systems neuroscience. While dimensionality reduction methods uncover low-dimensional manifold structure in population recordings, a rigorous framework connecting manifold geometry to network mechanisms and information encoding remains lacking. We develop a differential geometric approach for analyzing neural manifolds in rate-based recurrent networks receiving tuned feedforward inputs. We derive expressions for the pullback metric of neural manifolds, showing how input tuning curves, feedforward and recurrent synaptic connectivity shape manifold geometry. Critically, we establish that the Fisher information matrix at steady states also has the structure of a pullback metric, directly linking intrinsic manifold geometry to stimulus discriminability and information encoding. For noise with slow temporal correlations propagated through the network, we show that recurrent effects on information geometry cancel: Fisher information depends only on the feedforward connectivity. Thus, feedforward connectivity critically determines representational geometry. As an example, we demonstrate that the representation of space by a module of hexagonal grid cells is approximately isometric for random distribution of grid phases. Moreover, a linear feedforward transformation can map spatially random input tuning curves into a population of hexagonal grid cells, forming a toroidal manifold. Thus, feedforward connectivity alone can generate structured spatial representations without requiring carefully tuned recurrent connectivity or continuous attractor dynamics. Recurrent connectivity, however, is shown to improve stimulus encoding under fast noise, thereby implementing a selective noise reduction.