---
title: Hippocampal replay reconfigures grid codes to support flexible navigation
title_zh: 海马重放重构网格编码以支持灵活导航
authors: "Zhang, B., Liu, J."
date: 2026-06-15
pdf: "https://www.biorxiv.org/content/10.1101/2023.02.19.529130v5.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 海马回放重构网格编码以支持导航
tldr: 认知地图的网格编码与海马回放的关系尚不明确。本研究通过脑磁图记录方向导航任务，发现逆向和正向回放先于网格编码出现，并分别锚定于网格轴的两个相反方向。回放重构了网格的六重结构，连续吸引子网络模拟证实回放提升网格性。行为数据进一步表明网格方向随目标导向旋转。这揭示了回放通过重新配置网格编码支持灵活导航的机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究海马回放如何组织内嗅皮层网格细胞的六重编码，以支持灵活导航。
method: 采集脑磁图数据进行方向导航任务，逐事件估计回放和网格样活动，并构建连续吸引子网络模拟。
result: 逆向回放锁定网格方向早期表达，正向回放锁定后期表达，两者编码网格轴的相反方向，共同覆盖六重结构。
conclusion: 回放通过锚定网格轴并重构其六重结构，动态调整网格编码以引导灵活导航。
---

## 摘要
大脑的认知地图依赖于内嗅皮层的网格细胞，其六边形放电模式为空间和抽象知识提供度量，同时也依赖于海马重放——即学习与规划过程中经验的压缩性再激活。海马重放是否有助于组织内嗅皮层的网格度量仍不明确。本研究在方向分辨的导航任务中记录了脑磁图，每位参与者产生1800个试次独有事件，能够在全360度范围内逐事件估计重放和内嗅皮层网格样活动。每个导航事件早期出现逆向和正向重放，随后是六重内嗅皮层网格编码。重放锚定在网格轴上，其中逆向重放与网格编码窗口早期表达的网格方向锁定，而正向重放与后期表达的方向锁定。值得注意的是，正向和逆向重放编码了每个网格轴的两个相反方向（相距180度），共同覆盖了整个六重结构。连续吸引子网络再现了这种组织，其中网格轴重放产生的网格性显著高于无重放的模拟。最后，导航行为证实了这些发现。在网格样活动出现前，运动速度表现出双向方向周期性，在相距180度的两个相反方向达到峰值，镜像了正向和逆向重放的反向调谐；而轨迹偏差在网格样活动出现后表现出双向周期性，并与网格方向对齐，表明网格方向旋转以引导朝向目标前进。

## Abstract
The brains cognitive map relies on entorhinal grid cells, whose hexagonal firing provides a metric for spatial and abstract knowledge, and on hippocampal replay, the compressed reactivation of experience that supports learning and planning. Whether hippocampal replay contributes to the organization of the entorhinal grid metric remains unresolved. Here we recorded magnetoencephalography during a direction-resolved navigation task that yielded 1,800 trial-unique events per participant, allowing replay and entorhinal grid-like activity to be estimated event-wise across the full 360{degrees}. Reverse and forward replay emerged early in each navigation event, followed by a six-fold entorhinal grid code. Replay was anchored to the grid axes, with reverse replay time-locked to the grid orientation expressed early in the grid-coding window and forward replay to that expressed later. Notably, forward and reverse replay encoded the two opposite directions (180{degrees} apart) of each grid axis, together spanning the full six-fold structure. A continuous-attractor network reproduced this organization, with grid-axis replay yielding significantly higher gridness than simulations without replay. Finally, navigation behaviour corroborated these findings. Movement speed showed two-fold directional periodicity before grid-like activity emerged, peaking at two opposite directions (180{degrees} apart) that mirrored the opposite tuning of forward and reverse replay, whereas trajectory deviation showed two-fold periodicity after grid-like activity emerged and aligned with the grid orientation, suggesting that the grid orientation rotates to guide heading toward the goal.

---

## 论文详细总结（自动生成）

### 论文核心问题与整体含义（研究动机和背景）
- **核心问题**：海马体的重放（replay）活动是否参与组织内嗅皮层的网格细胞编码（grid code），特别是其六边形度量结构？若参与，两者在几何上如何协调？
- **背景**：网格细胞提供空间度量，海马重放支持学习与规划。已有证据表明海马对网格模式有驱动作用（如海马失活破坏网格放电），但重放与网格轴几何之间在主动导航中的关系尚不明确。
- **整体意义**：揭示重放如何通过锚定网格轴并重构其六重方向结构，从而支持灵活导航，将重放从记忆工具提升为构建空间度量的几何驱动力。

### 论文提出的方法论：核心思想、关键技术细节
- **核心思想**：在方向分辨的导航任务中，利用MEG的高时间分辨率同时检测海马重放和内嗅皮层网格样活动，并通过方向对齐分析检验重放是否与网格轴几何一致。
- **关键技术细节**：
  - **任务设计**：参与者在球形视角上导航光标连接四个符号，每个试次包含三个依次连接（A→B→C→D），共120个均匀分布方向，5个session，每位参与者1800个独特事件。
  - **重放检测**：使用四种符号的logistic回归解码器（one-vs-rest）获得刺激特异性再激活时间序列；再通过时间延迟线性模型（TDLM）量化序贯性，识别逆向和正向重放。
  - **网格样活动检测**：基于六重正弦调制器 cos(6(θ-φ)) 拟合内嗅皮层源空间活动，通过五折交叉验证估计个体网格方向φ，并检验六重调制信号的显著性。
  - **重放-网格对齐分析**：将重放强度按120个方向估计，旋转对齐至个体网格方向φ，比较网格对齐方向（±15°内）与不对齐方向的差异，产生时间-时间对齐图。
  - **频谱分析**：对重放方向调谐进行FFT，检验一重、三重、六重功率，并利用正/逆向重放的反相关系在平均后保留六重成分。
  - **连续吸引子网络（CAN）模拟**：基于Fuhs & Touretzky模型，模拟无重放、运动轴重放、网格轴重放三种条件，比较网格性（gridness）的差异。

### 实验设计：数据集、基准、对比方法
- **数据集**：自行收集的25名大学生MEG数据（5 sessions × 120方向 × 3连接 = 1800试次/人）。刺激选自Omniglot数据集，每个session分配四个不同符号。
- **基准**：无明确外部基准，主要进行条件间对比（如网格对齐vs不对齐方向；重放类型间；不同折叠调制）。
- **对比方法**：
  - 对重放：逆向vs正向；对齐vs不对齐方向。
  - 对网格编码：六重vs四/五/七/八重对照。
  - CAN模拟：无重放 vs 运动轴重放 vs 网格轴重放。
  - 行为：速度与轨迹偏差的方向周期性及相位对齐。

### 资源与算力
- 文中未明确说明使用的GPU型号、数量及训练时长。仅提及CAN模拟在PyTorch中实现，但未提供硬件细节。因此算力资源未知。

### 实验数量与充分性
- **实验数量**：
  - 神经成像：25名参与者，每名5 session × 120方向 × 3连接 → 共1800次连接事件。
  - CAN模拟：11个网格尺度 × 12个运动方向 × 3个重放条件 = 396次独立模拟。
  - 行为分析：同神经成像数据，额外计算速度与轨迹偏差的方向周期性。
- **充分性与客观性**：
  - 样本量中等（25人），但MEG试次数庞大（每个参与者1800事件），统计力充足。
  - 采用交叉验证（五折）估计网格方向，避免循环分析。
  - 使用簇级置换检验控制多重比较，统计严谨。
  - 模拟实验覆盖多个尺度和方向，系统比较三种条件。
  - 行为分析与神经结果在时间顺序和方向结构上互相印证。
  - 不足：未进行独立数据集的重复验证；未控制运动速度等行为混淆；重放-网格因果关系主要通过模拟支持，实验证据为相关性。

### 论文的主要结论与发现
- 每个导航事件中，逆向重放（~150 ms）和正向重放（~500 ms）先后出现，随后是内嗅皮层六重网格编码（500-1000 ms）。
- 逆向重放锚定于网格编码窗口早期的网格方向，正向重放锚定于后期的网格方向。
- 逆向与正向重放分别编码每个网格轴的两个相反方向（180°对立），共同覆盖六个网格轴方向（六重结构）。
- 正/逆向重放各自表现出方向不对称性（一重、三重频谱），平均后产生六重频谱，与网格编码一致。
- CAN模拟显示，网格轴重放比运动轴重放或无重放产生更稳健的网格性，尤其在较大网格尺度下。
- 行为上，运动速度在早期（<500 ms）表现出与网格轴无关的双向周期性；轨迹偏差在后期（>500 ms）表现出与网格轴对齐的双向周期性，表明网格方向旋转以引导朝向目标。

### 优点
- **方法论创新**：利用MEG高时间分辨率同时捕捉重放与网格编码，并在全方向空间内逐事件分析，突破传统范式局限。
- **几何预测精确**：预先推导出正/逆向重放反相180°的几何关系，并通过多种分析（方向对齐、FFT相位差、相关矩阵）一致验证。
- **多模态证据链**：神经活动、计算模拟、行为三者相互印证，增强结论可靠性。
- **理论贡献**：提出重放打破网格轴的180°对称性，将轴向度量转化为指向性向量，为自我到目标的映射提供神经基础。
- **控制分析严格**：多折对照、置换检验、交叉验证、相位聚类检验等统计方法恰当。

### 不足与局限
- **因果性有限**：神经数据是相关性，因果关系主要依赖CAN模拟，缺乏直接干预（如重放抑制或光遗传操作）。
- **任务特殊性**：虚拟导航任务使用光标旋转，可能与真实身体运动不同；网格样活动可能受视觉注意影响。
- **样本量与人口学**：仅25名中国大学生，性别比例不均衡（18男7女），可能限制泛化性。
- **未报告算力资源**：无法评估模拟计算成本及可重复性。
- **行为混淆**：速度与轨迹偏差可能受任务难度、学习效应等影响，未完全控制。
- **空间分辨率局限**：MEG源定位精度有限，内嗅皮层区域较小，可能包含邻近结构。
- **未验证非空间推广**：论文讨论网格编码在抽象空间存在，但当前实验只涉及物理空间导航。

（完）
