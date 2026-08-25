---
title: Spatially resolved mapping of tau amplification rates via differentiable simulation of prion-like propagation
title_zh: 通过朊病毒样传播的可微模拟实现tau扩增率的空间分辨映射
authors: "Kondo, Y., Naoki, H., for the Alzheimer's Disease Neuroimaging Initiative,"
date: 2026-08-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.02.729568v2.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 通过可微分模拟推断tau蛋白扩增速率的神经退行性研究
tldr: 神经退行性疾病的病理扩散模式具有异质性，但如何从影像数据推断空间传播动力学仍是高维逆问题。我们提出可微分反应-扩散框架，将MRI信息融入正向模拟，通过误差反向传播从tau PET重建体素级tau扩增速率图。分析发现扩增速率与amyloid PET呈正相关，并识别出与扩增区域变异相关的基因表达程序。该框架为理解分子结构与大尺度传播动力学的联系提供了新工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有方法难以从影像数据推断全脑尺度空间异质的病理传播动力学，构成高维逆问题。
method: 提出可微分反应-扩散框架，结合MRI模拟与误差反向传播，从tau PET重建个体体素级扩增速率图。
result: 扩增速率与amyloid PET呈正相关，转录组整合识别出与区域扩增变异相关的基因表达程序。
conclusion: 框架连接分子结构与宏观传播动力学，为神经退行性疾病的机制研究提供数据驱动工具。
---

## 摘要
神经退行性疾病表现出特征性但异质性的病理扩散模式，其潜在决定因素仍不清楚。一个核心挑战在于，从神经影像数据推断空间异质的传播动力学构成了一个高维逆问题，在全脑尺度上一直难以处理。在此，我们提出一个可微的反应-扩散框架，能够从tau PET数据推断空间分辨的tau扩增率。通过将基于MRI的正向模拟与误差反向传播相结合，我们的方法重建了人脑中受试者特异的体素级tau扩增率图谱。对推断图谱的分析表明，扩增率与淀粉样蛋白PET呈正空间关联，提示它们捕捉了区域对淀粉样蛋白驱动的tau积累脆弱性的某些方面。此外，与转录组数据的整合确定了与扩增区域变异相关的基因表达程序。这些发现提供了一个数据驱动的框架，将分子结构与神经退行性变中的大规模传播动力学联系起来。

## Abstract
Neurodegenerative diseases exhibit characteristic yet heterogeneous patterns of pathological spread, whose underlying determinants remain unclear. A central challenge is that inferring spatially heterogeneous propagation kinetics from neuroimaging data constitutes a high-dimensional inverse problem that has remained intractable at the whole-brain scale. Here, we present a differentiable reaction-diffusion framework that enables inference of spatially resolved tau amplification rates from tau PET data. By integrating MRI-informed forward simulation with error backpropagation, our approach reconstructs subject-specific voxel-wise maps of tau amplification rates across the human brain. Analysis of the inferred maps showed that the amplification rates have a positive spatial association with amyloid PET, suggesting that they capture aspects of regional vulnerability to amyloid-driven tau accumulation. Furthermore, integration with transcriptomic data identified gene expression programs associated with regional variation in amplification. These findings provide a data-driven framework linking molecular architecture to large-scale propagation dynamics in neurodegeneration.