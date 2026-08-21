---
title: Symbolic regression enables coarse-grained model discovery of intracellular signalling dynamics
title_zh: 符号回归实现细胞内信号动力学粗粒化模型发现
authors: "de Pomereu, T., Fröhlich, F."
date: 2026-08-21
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.20.745973v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 数据驱动的细胞内信号动力学粗粒化建模方法，可迁移至突触可塑性信号通路的计算建模
tldr: 蛋白信号网络的动力学建模常受数据和算力限制，粗粒化方法多依赖强假设。本文提出用符号回归从部分观测数据中自动发现可解释的紧凑模型，并在合成酶系统中恢复米氏动力学，在真实ERK数据中识别出癌症相关基因过表达下的简化速率定律。相比神经ODE，符号回归在能学习时更简洁，失败时提示动力学更复杂。这为判断何时适用粗粒化模型提供了数据驱动依据。
source: biorxiv
selection_source: fresh_fetch
motivation: 经典粗粒化建模依赖强假设，难以判断部分实验观测能否支持降维动力学描述。
method: 利用符号回归从时间序列数据中自动发现变量间的紧凑数学表达式，作为粗粒化模型。
result: 在合成酶系统恢复米氏动力学，在ERK数据中识别出可解释的磷酸化速率定律，且优于神经ODE。
conclusion: 符号回归能测试紧凑粗粒化描述的适用性，并指导新测量或机制假设的提出。
---

## 摘要
细胞通过蛋白质网络响应其环境，这些网络在癌症中常常失调，因此动力学建模至关重要。实验数据和计算资源的限制促使采用粗粒化方法构建低维描述。然而，经典的粗粒化建模方法依赖强假设，使得在部分实验观测支持系统动力学的简化描述时，其适用性尚不明确。在此，我们表明符号回归（SR）提供了一种数据驱动的方式，用于检验信号系统动力学是否以及如何在所测变量上实现粗粒化，以及当它们确实实现时，能够推断出具有机理解释性的模型。在合成酶系统中，SR恢复了两步机制和三步扩展下的米氏动力学。随着数据质量下降，SR简化为有效的动力学定律，同时保持正确的理论极限。将SR应用于已发表的时间分辨ERK磷酸化数据，SR在选定的与癌症相关的基因过表达背景下识别出紧凑的磷酸化ERK速率定律，产生可解释的动力学效应。一个稀疏神经ODE基线在SR成功的少数输入情况下需要少量输入，但在SR失败的情况下平均需要更多输入，这表明在完全可学习简化模型的情况下，SR失败与更复杂的动力学相关，而简单的数学模型无法描述这些动力学。综合来看，这些发现确立了符号回归作为一种检验何时需要紧凑粗粒化描述的方法，在存在紧凑描述时生成假设，在不存在时推动潜在的新测量。

## Abstract
Cells respond to their environment through protein networks often dysregulated in cancer, making dynamical modelling crucial. Limitations in experimental data and computational resources motivate coarse-graining methods to build low-dimensional descriptions. Yet classical approaches to coarse-grained modelling rely on strong assumptions, leaving it unclear when partial experimental observations support reduced descriptions of system dynamics. Here we show that symbolic regression (SR) provides a data-driven way to test whether, and how compactly, the dynamics of a signalling system coarse-grain over the measured variables, and, when they do, infers mechanistically interpretable models. In synthetic enzyme systems, SR recovers Michaelis-Menten kinetics for the two-step mechanism and under three-step extensions. As data quality is degraded, SR simplifies toward effective kinetic laws while preserving correct theoretical limits. Applied to published time-resolved ERK phosphorylation data, SR identifies compact phospho-ERK rate laws in selected cancer-relevant gene overexpression contexts, yielding interpretable kinetic effects. A sparse neural ODE baseline requires few inputs where SR succeeds, but on average more where it fails, indicating that, where a reduced model is learnable at all, SR failure is associated with more complex dynamics that a simple mathematical model cannot describe. Together, these findings establish symbolic regression as a way to test when a compact coarse-grained description is warranted, generating hypotheses where one holds and motivating potential new measurements where it does not.