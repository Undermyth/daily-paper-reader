---
title: Graph-based characterization of in vitro neuronal network maturation using machine learning and digital holographic microscopy
title_zh: 基于图论与机器学习及数字全息显微镜的体外神经网络成熟度表征
authors: "Yazdani, Z., Belanger, E., Moreaud, M., Llinares, J., Allard, A., Marquet, P., Desrosiers, P."
date: 2026-06-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.18.732973v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 使用机器学习和图论表征神经网络成熟的计算方法
tldr: "数字全息显微镜（DHM）无标记成像活细胞，但缺乏自动分析神经元网络成熟度的工具。本文结合U-Net深度学习分割和图论，从DHM定量相位图像中提取神经元形态连接，构建图指纹并计算18个图特征。结果表明细胞体和神经突分割AUC分别达0.98和0.91，网络密度和模块性随成熟度变化，随机森林分类器以87%准确率区分培养阶段。该方法为无标记神经网络的定量表征提供了新框架。"
source: biorxiv
selection_source: fresh_fetch
motivation: DHM提供无标记定量相位图像，但缺乏从图像中自动表征神经元网络组织与成熟度的计算方法。
method: 训练两个U-Net分别分割神经元胞体和神经突，根据分割图推断形态连接并构建图指纹，计算18个连接组学图特征。
result: "分割AUC达0.98（胞体）和0.91（神经突）；图特征反映成熟阶段变化，密度和模块性是关键指标，分类准确率87%。"
conclusion: 结合DHM、深度学习和图论可定量表征无标记神经元网络组织与成熟度，为药理实验和hiPSC衍生培养研究奠定基础。
---

## 摘要
意义：数字全息显微镜（DHM）能够提供活细胞的无标记定量相位图像（QPI），已成为研究细胞形态和动力学的强大工具。虽然大多数DHM研究集中在细胞层面分析，但利用DHM图像定量表征神经网络组织与成熟度仍鲜有探索，亟需专门的计算方法。

目的：我们旨在开发一个自动化框架，结合基于深度学习的图像分析与图论，定量表征原代大鼠皮层培养物中神经网络的组织、连接和成熟度。

方法：在手动标注的DHM相位图像上训练两个U-Net卷积神经网络，分别用于分割神经元胞体和神经突。由此产生的分割图用于推断神经元之间假定的形态连接，并生成神经网络的图表示，称为图指纹。随后计算18个基于连接组学的图特征，以表征培养成熟四个阶段中网络组织的局部和全局特性。

结果：胞体分割的接收者操作特征曲线下平均面积为0.98，神经突分割为0.91，表明近乎完美的识别。图论分析揭示了体外网络成熟过程中可重现的拓扑变化，包括密度增加、模块性降低和逐步的网络整合。相关性分析显示，18个图特征分为两个高度相关的族。随机森林分类器将密度和模块性确定为最具信息量的描述符，在分类神经元培养成熟阶段时达到87%的准确率。

结论：我们的结果表明，结合DHM、基于深度学习的分割和图论分析，能够从无标记相位图像中定量表征神经网络组织与成熟度。该框架为未来的药理学实验、神经网络表型分析以及人类诱导多能干细胞（hiPSC）来源的神经元培养研究奠定了基础，其中网络组织的定量评估仍是一大挑战。

## Abstract
SignificanceDigital Holographic Microscopy (DHM) provides label-free quantitative phase images (QPIs) of living cells and has become a powerful tool for studying cellular morphology and dynamics. While most DHM studies have focused on cell-level analysis, the quantitative characterization of neuronal network organization and maturation from DHM images remains largely unexplored, highlighting the need for dedicated computational approaches.

AimWe aimed to develop an automated framework combining deep-learning-based image analysis and graph theory to quantitatively characterize the organization, connectivity, and maturation of neuronal networks in primary rat cortical cultures imaged by DHM.

ApproachTwo U-Net convolutional neural networks were trained on manually annotated DHM phase images to segment neuronal cell bodies and neurites. The resulting segmentation maps were used to infer putative morphological connections between neurons and generate graph representations of neuronal networks, referred to as graph fingerprints. A panel of 18 connectomics-inspired graph features was then computed to characterize local and global properties of network organization across four stages of culture maturation.

ResultsThe mean area under the receiver operating characteristic curves was 0.98 for cell-body and 0.91 for neurite segmentation, indicating near-perfect identification. Graph-theoretical analysis revealed reproducible topological changes during network maturation in vitro, including increased density, reduced modularity, and progressive network integration. Correlation analysis showed that the 18 graph features grouped into two highly correlated families. A Random Forest classifier identified density and modularity as the most informative descriptors, achieving an accuracy of 87% in classifying maturation stages of neuronal cultures.

ConclusionsOur results demonstrate that combining DHM, deep-learning-based segmentation, and graphtheoretical analysis enables quantitative characterization of neuronal network organization and maturation from label-free phase images. This framework provides a foundation for future studies of pharmacological experiments, neuronal network phenotyping, and human induced pluripotent stem cell (hiPSC)-derived neuronal cultures, where quantitative assessment of network organization remains a major challenge.