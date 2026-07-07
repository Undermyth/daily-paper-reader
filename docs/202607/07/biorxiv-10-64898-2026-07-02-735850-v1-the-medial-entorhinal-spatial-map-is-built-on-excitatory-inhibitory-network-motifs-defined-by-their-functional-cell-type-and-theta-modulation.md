---
title: The medial entorhinal spatial map is built on excitatory-inhibitory network motifs defined by their functional cell type and theta modulation
title_zh: 内侧内嗅皮层空间地图建立在由功能细胞类型和θ节律调制的兴奋-抑制网络基序上
authors: "Kerekes, P., Bauza, M., Krupic, J."
date: 2026-07-03
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.02.735850v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 内侧内嗅皮层空间地图及细胞类型特异性连接
tldr: 内侧内嗅皮层（mEC）包含多种功能特异神经元，但其如何交互构建空间地图未知。本研究通过同时记录小鼠在虚拟导航中数百个mEC神经元的活动，发现连接模式呈细胞类型特异性和θ节律依赖性，θ调制连接占主导，功能同类神经元优先互连，且存在共享抑制性中间神经元池。网格细胞与中间神经元连接最强，且最少形成对线索的响应场。揭示了由细胞类型和θ节律组织的抑制性网络架构，其中网格细胞作为核心枢纽。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究mEC中功能特异神经元和θ节律如何组织连接以形成异中心空间地图。
method: 同时记录小鼠在虚拟轨迹导航中数百个mEC神经元的活动，分析不同视觉线索条件下的连接模式。
result: 发现细胞类型特异性和θ节律依赖的连接，网格细胞与抑制性中间神经元连接最强且最少形成线索响应场。
conclusion: 抑制性网络以网格细胞为枢纽，通过细胞类型和θ节律组织mEC异中心空间地图。
---

## 摘要
内侧内嗅皮层含有对空间记忆和导航至关重要的功能特定神经元，包括网格细胞、边界细胞、空间细胞、头部方向细胞和线索细胞。然而，这些神经元如何相互作用以构建空间地图仍不清楚。在此，我们通过同时记录小鼠在具有不同数量视觉标志的虚拟轨道上导航时数百个功能定义的内侧内嗅皮层神经元，揭示了定义内侧内嗅皮层功能网络架构并将其与异源性地图形成原理联系起来的连接基序。我们发现细胞间的连接是细胞类型特异性的，并根据其功能和θ节律调制分组为子网络，其中θ节律调制的连接占主导地位。功能不同的神经元优先连接到自身类型，它们的相互作用由一个共享的中间神经元抑制池协调，且兴奋性到抑制性的连接比例高于兴奋性细胞间的连接。这伴随着所有内侧内嗅皮层细胞类型形成的野数目随可用线索数目的亚线性增加。无论其θ节律调制如何，网格细胞显示出与中间神经元最强的相对连接，从而连接了原本大部分孤立的θ节律流和非θ节律流。网格细胞也最不可能因线索而形成野。总之，这些发现揭示了由细胞类型和θ节律依赖性组织的内侧内嗅皮层网络架构，其中以网格细胞为最强枢纽的抑制性相互作用在构建内侧内嗅皮层异源性地图中起核心作用。

## Abstract
The medial entorhinal cortex (mEC) contains functionally specific neurons crucial for spatial memory and navigation, including grid, border, spatial, head direction, and cue cells. However, how these neurons interact to build spatial maps remains unclear. Here, using simultaneous recordings from hundreds of functionally defined mEC neurons in mice navigating virtual tracks with varying numbers of visual landmarks, we uncovered connectivity motifs that define the mEC functional network architecture and link it to the principles governing allocentric map formation. We found that connectivity between cells was cell-type-specific and grouped into subnetworks based on their function and theta modulation, with theta-modulated connections dominating over non-theta. Functionally distinct neurons preferentially connected to their own type, and their interactions were coordinated by a shared inhibitory pool of interneurons, with a higher proportion of excitatory-to-inhibitory connections than between excitatory cells. This was accompanied by the number of fields formed across all mEC cell types increasing sublinearly with the number of available cues. Grid cells showed the strongest relative connectivity to interneurons regardless of their theta modulation, linking otherwise largely isolated theta and non-theta streams. Grid cells were also least likely to form a field in response to cues. Together, these findings reveal an mEC network architecture organised by cell type and theta dependency, in which inhibitory interactions, with grid cells as the strongest hub, play a central role in building the mEC allocentric map.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）
- **研究背景**：内侧内嗅皮层（mEC）是空间记忆和导航的关键脑区，包含多种功能特异性神经元（网格细胞、边界细胞、头部方向细胞、空间细胞、线索细胞）。虽然这些神经元各自的功能已被广泛研究，但它们如何通过相互作用构建一个统一的**异中心空间地图**仍不清楚。
- **核心问题**：mEC中不同功能类型的兴奋性细胞之间，以及它们与抑制性中间神经元之间的连接模式是什么？这种连接架构如何解释视觉线索驱动下空间野的形成？θ节律调制在其中扮演什么角色？
- **整体含义**：揭示mEC网络的组织原则，特别是**抑制性网络**（以网格细胞为枢纽）在协调不同功能流、实现亚线性线索-野关系中的核心作用，为理解空间认知的神经机制提供新视角。

## 2. 方法论：核心思想、关键技术细节、算法流程
- **核心思想**：通过同时记录数百个功能定义的mEC神经元，利用**突触连接推断**（基于尖峰-时间互相关图）分析细胞类型特异性和θ节律调制的连接基序，并关联到不同视觉线索条件下的空间野形成。
- **关键技术细节**：
  - **记录技术**：Neuropixels 2.0高密度硅探针（同时记录数百个神经元）+ 四极管记录，小鼠在**虚拟现实（VR）** 环境中进行头部固定线性导航。
  - **功能分类**：基于真实2D方形围栏中的活动，定义网格细胞（网格得分>0.27）、边界细胞（边界得分>2）、头部方向细胞（瑞利向量长度>0.19）、空间细胞（空间信息>1.3）、线索细胞（在VR中形成稳定野）。
  - **抑制性中间神经元识别**：基于波形波峰-波谷潜伏期（≤0.3 ms）。
  - **θ节律调制**：通过自相关图功率谱计算θ得分（6–10 Hz峰附近1 Hz内平均功率 / 2–125 Hz平均功率，>5为θ调制）。
  - **连接推断**：计算所有同步记录细胞对的**交叉相关图**（bin=1ms，窗口±10ms），通过两次置换检验确定显著的单突触连接（峰值在1-5ms内，且通过半交叉相关稳定性检验）。
- **算法流程**：空间野检测 → 功能分类 → θ节律分类 → 对每对细胞计算交叉相关图 → 统计显著性检验 → 构建连接矩阵（按细胞类型和θ类别分组）→ 比较不同条件下的野数量、稳定性、连接比例等。

## 3. 实验设计
- **数据集/场景**：
  - **虚拟现实（VR）线形轨道**：9米长，三种视觉条件——无线索（nC，仅自运动线索）、单一线索（1C，一个1米宽的近端线索在2.5米处）、多线索（Cr，九个1米宽线索+四对远端线索）。此外有黑暗间隔（dark inter-lap）作为对照。
  - **真实环境（RE）**：正方形围栏（1m×1m或0.6m×0.6m），用于功能分类。
  - **实验流程**：A-B-A-C设计（nC1 → 1C → nC2 → Cr），之后记录RE。
- **Benchmark**：无明确的对比方法，本研究是首次系统描述mEC功能细胞类型之间的连接基序。内部对照包括：暗轨道 vs 无线索轨道；1C vs Cr vs nC。
- **对比方法**：未与其他模型或方法直接对比，主要是自身不同条件下的比较以及不同细胞类型间的比较。

## 4. 资源与算力
- **文中未明确说明使用的GPU型号、数量、训练时长等算力信息**。仅提及使用Neuropixels 2.0探针和四极管进行记录，数据分析使用了Matlab R2019a和Python 3.12，以及PyTorch库进行GPU加速交叉相关计算。未提及具体的计算集群或训练开销。

## 5. 实验数量与充分性
- **实验数量**：
  - 共15只C57BL/6J雄性小鼠，其中6只植入Neuropixels 2.0，9只植入四极管。
  - 记录到的功能神经元数量：网格细胞944个（分三个网格模块）、边界细胞186个、头部方向细胞155个、空间细胞760个、线索细胞1115个。
  - 交叉相关分析中：共分析E-I对48040对，E-E对288331对。
  - 每个VR条件下记录20-25 laps；每个细胞有多个重复（如nC两次、1C、Cr、dark）。
- **充分性**：
  - **初步充分**：样本量较大，涵盖五种主要mEC细胞类型；连接分析基于大量神经元对，统计检验使用置换检验、Wilcoxon秩和检验等，校正了多重比较（Bonferroni）。
  - **局限**：
    - 仅使用了雄性小鼠，未报告性别差异。
    - VR环境简化（1D线性轨道），真实空间编码可能更复杂。
    - 突触连接基于尖峰时序相关性推断，存在假阳性/假阴性风险（尽管经过双重置换检验）。
    - 未进行因果关系验证（如光遗传学操纵）。

## 6. 主要结论与发现
1. **线索依赖性野形成**：无线索时，几乎所有mEC细胞仅在轨道边界形成稳定野；单一线索显著增加野数目，但网格细胞形成野的能力最弱（且倾向于编码线索末端）；多线索导致野数目**亚线性增加**，网格细胞再次表现出最弱的线索响应。
2. **网格细胞距离编码**：网格细胞在无线索和单线索轨道中仍表现出周期性活动（周期约为2D网格尺度的1.87倍），但不足以支持小鼠精确导航至奖励位置（小鼠速度未在奖励前减速）。
3. **连接基序**：
   - **基序1（主导）**：兴奋性-抑制性连接比例显著高于兴奋性-兴奋性连接。
   - **基序2**：同类型功能细胞优先互连。
   - **基序3**：θ调制细胞间的连接占主导，但**网格细胞例外**，它们对θ和非θ细胞连接强度相当。
   - **基序4**：非θ调制的主细胞接收更多的抑制性投射。
4. **网格细胞作为核心枢纽**：网格细胞与抑制性中间神经元形成**最强的双向连接**，且整合θ和非θ流；θ调制的线索细胞是向其他细胞类型发送最强投射的“感觉信息中心”；θ调制的头部方向细胞是接收跨类型输入最强的“整合输出枢纽”。
5. **共享抑制池**：大部分中间神经元接收来自多个不同功能类型主细胞的输入，并向多个细胞类型发送抑制输出，表明mEC空间地图通过**共享抑制网络**实现协调。

## 7. 优点
- **技术先进性**：使用Neuropixels 2.0实现大规模同时记录，能够同时捕获数百个功能定义神经元，且通过两次置换检验提高了连接推断的可靠性。
- **系统性分类**：将细胞功能类型、θ节律调制、兴奋/抑制类型三维结合，构建了细粒度的连接矩阵，揭示了以往未发现的网络基序。
- **行为与神经关联**：将连接特性与行为表现（速度减速、导航准确性）相关联，增强了结论的行为相关性。
- **统计严谨**：针对不等样本量进行了校正（下采样置换检验），多重比较校正，结果稳健。
- **开放性**：数据和代码将在发表后公开（Zenodo和GitHub），促进可重复性。

## 8. 不足与局限
- **因果关系缺失**：仅基于相关性分析推断连接，未使用光遗传学或化学遗传学直接操纵特定连接来验证功能作用。
- **VR环境局限性**：1D线性轨道和头部固定条件无法完全反映自然空间导航（缺乏主动运动、嗅觉、触觉等），且可能影响网格细胞等编码。
- **性别偏差**：仅雄性小鼠，可能遗漏性别差异。
- **中间神经元分类粗糙**：仅基于波形宽度（≤0.3ms）区分中间神经元，未细分PV、SOM、VIP等亚型，而这些亚型在mEC中功能不同（如Miao et al., 2017）。
- **θ分类阈值**：θ得分>5的定义可能过于粗糙，且θ节律在清醒运动时可能不稳定。
- **样本偏差**：部分细胞类型（如头部方向细胞）数量较少（155个），可能影响连接分析的统计效力。
- **缺乏跨区域比较**：未与海马或其他皮层区域对比，无法判断这些基序是mEC特有还是通用的。

（完）
