---
title: The Physics Network is Distinct from the Multiple Demand System in the Human Brain
title_zh: 物理学网络与人类大脑中的多重需求系统是不同的
authors: "Pramod, R., Hutchinson, S., Kanwisher, N. G."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.19.739417v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 神经科学中的推理计算机制
tldr: 直觉物理推理依赖大脑中的物理网络（PN），但其是否独立于临近的通用多需求网络（MD）尚不清楚。本研究通过fMRI扫描20名参与者，测量了两网络的空间重叠、任务响应差异及静息态相关性。结果发现PN与MD在个体内重叠极小，且各自在不同任务中呈现独特功能轮廓，网络内部子区域间的时间相关性高于跨网络。这表明PN在空间和功能上与MD可分离，支持其作为直觉物理推理专用系统的独立性。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739417-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1310, \"height\": 846, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739417-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1380, \"height\": 1190, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739417-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1394, \"height\": 1653, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-19-739417-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 993, \"height\": 712, \"label\": \"Figure\"}]"
motivation: 验证物理网络（PN）是否在空间和功能上独立于多需求网络（MD），以明确直觉物理推理的神经基础是否领域特异。
method: 对20名参与者进行fMRI扫描，通过空间重叠、任务响应差异和静息态功能连接定量比较PN与MD的相似性。
result: PN与MD重叠极小，任务下功能轮廓不同，网络内子区域时间相关性显著高于网络间。
conclusion: 物理网络与多需求系统在空间和功能上均可分离，支持其作为直觉物理推理的独立领域特异性系统。
---

## 摘要
近期研究表明，人类双侧额顶皮层的区域在直观物理推理中发挥作用——即我们在物理世界中感知、预测和规划的能力。然而，目前尚不清楚这个“物理网络”（PN）是否构成一个独特的、领域特定的系统，还是与邻近的领域一般性多重需求（MD）网络重叠。为了回答这个问题，我们在一项预注册研究中通过fMRI扫描参与者（N=20），测量了PN和MD网络之间的空间重叠、反应特征差异以及静息态相关性。我们发现：（1）在单个参与者内，PN和MD网络仅存在最小程度的重叠；（2）每个网络在一系列广泛任务中表现出不同的功能特征；（3）同一网络内子区域之间的功能反应时间进程的相关性高于不同网络子区域之间的相关性。这些发现表明，物理网络在空间和功能上均与多重需求系统可分离，支持其在直观物理推理中的独特作用。

## Abstract
Recent studies implicate regions of the human bilateral fronto-parietal cortices in intuitive physical reasoning -- our ability to perceive, predict, and plan in the physical world. However, it remains unclear whether this "Physics Network" (PN) constitutes a distinct and domain-specific system, or whether instead it overlaps with the nearby domain-general multiple demand (MD) network. To answer this question, we scanned participants (N = 20) with fMRI in a pre-registered study and measured spatial overlap, response profile differences, and resting-state correlation between the PN and MD networks. We find that: (1) The PN and MD networks overlap only minimally within individual participants, (2) Each network exhibits distinct functional profiles across a broad array of tasks, and (3) Time courses of functional response are more correlated between subregions within the same network than subregions between networks. These findings indicate that the Physics Network is dissociable from the Multiple Demand system both spatially and functionally, supporting its distinct role in intuitive physical reasoning.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）

- **研究动机**：人类具备直观物理推理能力（感知、预测、规划物体行为），近期神经影像学发现“物理网络”（Physics Network, PN）——双侧额顶皮层的一组区域——专门参与这类推理。但PN是否是一个**领域特异性**系统，还是仅仅是附近**领域通用性**的“多重需求网络”（Multiple Demand, MD）的组成部分，尚不清楚。
- **核心问题**：PN与MD在空间位置和功能上是否可分离？若存在大量重叠，则挑战现有对二者独立性的理解；若分离微弱或不存在，则表明物理推理只是MD的一般性认知需求的一个特例。
- **整体含义**：明确PN的独立性有助于揭示大脑中领域特异性系统的组织原则，并阐明直觉物理推理的神经基础是否具有独特的计算架构。

### 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

- **核心思想**：结合**空间重叠量化**、**功能选择剖面分析**和**静息态功能连接**三个层次，在个体水平上检验PN与MD的分离性。
- **关键技术细节**：
  - **个体水平定位（fROI）**：采用“组约束-个体特异性”（Group-constrained Subject-Specific, GSS）方法。首先使用预定义的群组概率图谱定义额叶和顶叶的ROI包裹（parcel），再在每个参与者的原生空间内，依据特定定位对比（p<0.001或至少50个体素）选取显著激活体素。
  - **PN定位**：使用“Towers”任务（物理推理 vs. 颜色判断）的对比：`物理 > 颜色`。
  - **MD定位**：使用空间工作记忆任务（困难 vs. 简单）的对比：`困难 > 容易`。另用数学任务（Math > Non-math）作为替代定义进行鲁棒性检验。
  - **空间重叠量化**：计算Dice-Sorensen系数，公式为 \( \text{Dice} = \frac{2 |S_{\text{PN}} \cap S_{\text{MD}}|}{|S_{\text{PN}}| + |S_{\text{MD}}|} \)，其中 \( S_{\text{PN}} \) 和 \( S_{\text{MD}} \) 分别为两个网络显著体素集合。在独立数据分割（奇偶分割）上计算，并采用10,000次bootstrap检验显著性。
  - **功能选择性分析**：在分离的PN选择性体素和MD选择性体素（分别取自半数据）中，测量另一半数据（held-out）中四个定位（物理、颜色、困难、简单）的反应，进行三因素ANOVA（区域×定位器×条件）。进一步在13个额外任务条件下比较两个网络的反应剖面。
  - **静息态功能连接**：将PN和MD的体素按半球（左/右）和脑叶（额/顶）分为8个子区域，计算各子区域时间序列间的Pearson相关，比较网络内与网络间的平均相关。

### 3. 实验设计：数据集/场景、benchmark、对比方法

- **参与者**：20名（10女），年龄18-50岁，来自MIT及波士顿地区。每个参与者进行2小时fMRI扫描。
- **任务/场景**：
  - **Towers局部定位任务**（2个run）：每个run包含23个18秒的block（3个注视，10个物理任务，10个颜色任务）。物理任务判断塔倒下后更多方块落在红色还是绿色半侧；颜色任务判断塔中蓝色还是黄色方块更多。
  - **空间工作记忆局部定位任务**（2个run）：每个run包含48个8秒trial（易/难交替），困难条件需要记忆8个位置，容易条件记忆4个位置。
  - **高效多功能局部定位器（EMFL）**（5个run）：10种视觉类别×5种听觉类别的组合，可提取13个额外条件（动态面部、场景、身体、物体、文字；静态面部、物体、场景、打乱物体；语言局部定位中的书面句子和非词；疼痛矩阵中描述身体疼痛和情感疼痛的书面故事）。
  - **静息态fMRI**：24分钟。
  - **各对比基准**：无传统benchmark，而是通过在个体内计算**网络内Dice系数**（奇偶分割）作为“自身一致性”的基准，并与网络间Dice系数比较。另通过bootstrap随机分配体素生成零分布作为偶然水平基准。
- **对比方法**：主要比较PN与MD在空间、功能和连接性上的差异。同时使用替代MD定义（数学任务）验证鲁棒性。未与其他方法（如其它网络划分）进行系统对比。

### 4. 资源与算力

- **未明确说明**：论文未提及使用的GPU型号、数量或训练时长。数据分析主要依赖FreeSurfer和MATLAB（2015B）在标准工作站上完成。fMRI数据采集使用西门子3T Trio扫描仪。

### 5. 实验数量与充分性

- **实验组数**：
  - 主要空间重叠分析：基于20名参与者，每个参与者在网络内（PN-PN、MD-MD）和网络间（PN-MD）分别计算Dice系数，并进行了bootstrap检验。
  - 功能选择性分析：包括4个定位器条件的ANOVA及13个额外条件的ANOVA，每个条件均有20名参与者的数据。
  - 静息态功能连接分析：计算20名参与者的8×8相关矩阵。
  - 鲁棒性检验：使用替代MD定义（数学任务）重复空间和功能分析（见补充图S4、S5）。
- **充分性评判**：
  - **优点**：实验设计预注册，使用独立数据（held-out）避免双倍使用同一数据，三种不同层次的证据（空间、功能、连接）交叉验证，结果稳健（不同阈值、不同MD定义）。
  - **不足**：样本量20属于中等，对于个体差异大的fMRI研究可能不够大；未进行独立样本复现；未探索所有可能的任务域（如仅使用一种物理推理任务定位PN）。但整体实验设计较为充分和客观。

### 6. 论文的主要结论与发现

1. **空间分离**：个体水平上PN与MD重叠极小（平均Dice系数=0.077），显著低于网络内一致性（PN内0.37，MD内0.33），且远超偶然水平。该结果在不同统计阈值、不同脑叶（额叶/顶叶）以及不同MD定义下均成立。
2. **功能分离**：PN选择性体素在物理任务中反应强于MD任务，而MD选择性体素相反（三因素交互显著，p=0.0001）。在13个额外条件下，两个网络的功能剖面显著不同：PN对动态视觉刺激反应更强，对身体疼痛故事反应显著高于情感疼痛（MD中该差异较弱）。
3. **连接网络分离**：静息态下，PN子区域间及MD子区域间的功能连接强度（r≈0.52）显著高于PN-MD间连接（r≈0.37），证明二者形成不同的功能网络。
4. **综合结论**：PN和MD在空间、功能和连接性上均为可分离系统，PN是一个领域特异性的直觉物理推理网络，而非MD的一般性扩展。

### 7. 优点：方法或实验设计上的亮点

- **预注册**：方法和分析计划提前在OSF注册（https://osf.io/6vg2a/），增强可信度。
- **个体水平分析**：避免组水平平均导致的虚假重叠，使用GSS方法在原生空间定义fROI。
- **独立数据验证**：所有功能选择性分析均在held-out数据上进行，避免双重蘸料。
- **多维度证据**：空间、功能、连接三个层面相互独立且互补，提供强有力证据。
- **鲁棒性检验**：使用不同统计阈值、不同脑叶、替代MD定义（数学任务）验证结果一致性。
- **量化网络连接**：首次为PN作为独立网络提供静息态功能连接证据，排除单纯空间邻近导致的伪相关。

### 8. 不足与局限

- **fMRI空间分辨率局限**：无法区分单个神经元层面的混合选择性，少量重叠体素可能反映混杂细胞群或真正双重响应神经元。
- **仅关注核心额顶区域**：PN的其他可能区域（如小脑、前额叶前部）未纳入分析，可能低估网络范围。
- **单一物理推理任务**：仅使用“Towers”任务定位PN，未验证其他物理推理任务（如碰撞预测、稳定性判断）是否得到相似分离结果。
- **未与所有近邻网络比较**：未系统比较PN与动作观察网络、工具处理网络、数字认知网络，无法排除与其他网络的潜在重叠。
- **样本量中等**：20名参与者对于个体变异较大的fMRI研究可能不足，且未进行外部样本复制。
- **静息态网络定义方法**：采用功能先验ROI方式，可能遗漏静息态数据中自发形成的其他相关网络结构。作者承认未来需使用无先验聚类方法补充分析。
- **应用限制**：作为预印本，未经同行评审，结论需进一步验证。

（完）
