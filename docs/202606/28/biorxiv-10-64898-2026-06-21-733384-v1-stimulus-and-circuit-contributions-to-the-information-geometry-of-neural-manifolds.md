---
title: Stimulus and circuit contributions to the information geometry of neural manifolds
title_zh: 刺激与回路对神经流形信息几何的贡献
authors: "Goedeke, S., Kautz, J. K., Leibold, C."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.21.733384v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 神经流形的信息几何、循环网络、Fisher信息
tldr: 神经群体记录揭示低维流形结构，但缺乏连接机制与信息编码的严格框架。我们开发微分几何方法，推导拉回度量，揭示前馈与递归连接如何塑造流形几何。关键发现：慢噪声下递归效应抵消，Fisher信息仅由前馈决定；快噪声下递归实现选择性降噪改善编码。前馈连接足以生成网格细胞空间表征，无需吸引子动力学。
source: biorxiv
selection_source: fresh_fetch
motivation: 建立网络连接机制与神经流形几何及信息编码之间的严格理论框架。
method: 推导率基递归网络中神经流形的拉回度量，并分析Fisher信息矩阵的结构。
result: 慢噪声下递归对信息几何影响抵消，信息仅由前馈连接决定；快噪声下递归改善编码。
conclusion: 前馈连接足以生成结构化空间表征，递归连接实现选择性噪声抑制。
---

## 摘要
理解网络连接如何塑造神经表征是系统神经科学的核心问题。虽然降维方法揭示了群体记录中的低维流形结构，但将流形几何与网络机制及信息编码联系起来的严格框架仍然缺乏。我们开发了一种微分几何方法，用于分析接收调谐前馈输入的基于发放率的递归网络中的神经流形。我们推导了神经流形拉回度量的表达式，展示了输入调谐曲线、前馈和递归突触连接如何塑造流形几何。关键的是，我们建立了稳态下的费舍尔信息矩阵也具有拉回度量的结构，直接将内在流形几何与刺激可分辨性和信息编码联系起来。对于通过网络传播的具有慢时间相关性的噪声，我们表明递归效应对信息几何的影响相互抵消：费舍尔信息仅依赖于前馈连接。因此，前馈连接关键性地决定了表征几何。作为一个例子，我们证明了六边形网格细胞模块对空间的表征对于随机分布的网格相位近似等距。此外，线性前馈变换可以将空间随机的输入调谐曲线映射到一群六边形网格细胞上，形成环面流形。因此，仅通过前馈连接就能生成结构化的空间表征，无需精心调谐的递归连接或连续吸引子动力学。然而，递归连接在快噪声下被证明可以改善刺激编码，从而实现了选择性的降噪。

## Abstract
Understanding how network connectivity shapes neural representations is central to systems neuroscience. While dimensionality reduction methods uncover low-dimensional manifold structure in population recordings, a rigorous framework connecting manifold geometry to network mechanisms and information encoding remains lacking. We develop a differential geometric approach for analyzing neural manifolds in rate-based recurrent networks receiving tuned feedforward inputs. We derive expressions for the pullback metric of neural manifolds, showing how input tuning curves, feedforward and recurrent synaptic connectivity shape manifold geometry. Critically, we establish that the Fisher information matrix at steady states also has the structure of a pullback metric, directly linking intrinsic manifold geometry to stimulus discriminability and information encoding. For noise with slow temporal correlations propagated through the network, we show that recurrent effects on information geometry cancel: Fisher information depends only on the feedforward connectivity. Thus, feedforward connectivity critically determines representational geometry. As an example, we demonstrate that the representation of space by a module of hexagonal grid cells is approximately isometric for random distribution of grid phases. Moreover, a linear feedforward transformation can map spatially random input tuning curves into a population of hexagonal grid cells, forming a toroidal manifold. Thus, feedforward connectivity alone can generate structured spatial representations without requiring carefully tuned recurrent connectivity or continuous attractor dynamics. Recurrent connectivity, however, is shown to improve stimulus encoding under fast noise, thereby implementing a selective noise reduction.