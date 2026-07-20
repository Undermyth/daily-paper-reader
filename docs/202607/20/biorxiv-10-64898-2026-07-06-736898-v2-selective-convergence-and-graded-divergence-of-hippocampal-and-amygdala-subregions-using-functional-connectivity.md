---
title: Selective convergence and graded divergence of hippocampal and amygdala subregions using functional connectivity
title_zh: 基于功能连接的海马和杏仁核亚区的选择性汇聚与分级发散
authors: "Erigüc, D. Y., Marsiglia, M., John, A., Bayrak, S., Wan, B., Jakovcic, A., DeKraker, J., Royer, J., Bernhardt, B., Valk, S. L."
date: 2026-07-18
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.06.736898v2.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 海马子区与皮层功能连接图谱，直接相关海马计算表示
tldr: 海马与杏仁核亚区在皮层中的功能连接模式尚不明确。本研究基于722名HCP被试的静息态fMRI，采用皮尔逊相关和GLASSO偏相关量化连接，并引入优势度和共享度指标。结果发现，直接关联下两结构共享旁边缘区域，但海马亚区偏好默认模式和视觉网络，杏仁核偏好腹侧注意和边缘网络；宽泛共波动则扩展到更多网络。该工作揭示了海马与杏仁核亚区在皮层中形成结构化、空间组织的共存，而非离散系统。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736898-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1633, \"height\": 1567, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736898-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 694, \"height\": 447, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736898-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1624, \"height\": 1850, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736898-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 809, \"height\": 374, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736898-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 724, \"height\": 1245, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736898-v2/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 804, \"height\": 372, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736898-v2/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 757, \"height\": 1195, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736898-v2/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1656, \"height\": 365, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736898-v2/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1668, \"height\": 561, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-06-736898-v2/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1562, \"height\": 475, \"label\": \"Figure\"}]"
motivation: 尽管海马和杏仁核与记忆和情感密切相关，但其亚区如何共同嵌入分布式皮层系统仍不清楚。
method: 利用722名HCP被试的静息态fMRI数据，计算Pearson相关和GLASSO偏相关以评估亚区-皮层连接，并引入优势度和共享度指标。
result: 直接关联下两结构共享旁边缘区域；偏相关显示海马亚区耦合默认模式与视觉网络，杏仁核偏向腹侧注意与边缘网络，且宽泛共波动模式不同。
conclusion: 海马与杏仁核亚区并非离散皮层系统，而是通过结构化、空间组织的共表征嵌入皮层，沿长轴和特定核团存在梯度差异。
---

## 摘要
海马和杏仁核是邻近的内侧颞叶结构，与记忆和情感相关，但它们的亚区如何共同嵌入到分布式的等皮层系统中仍不清楚。利用来自722名人类连接组计划年轻成年参与者的静息态fMRI数据，我们在统一的皮层广泛框架内绘制了海马和杏仁核亚区图，通过Pearson相关（宽泛共同波动）和GLASSO偏相关（相对更直接的功能关联）量化亚区-皮层连接。我们引入了两个基于计数的指标：优势度（相对海马与杏仁核表征）和共享度（平衡共同表征）。直接关联显示两个结构均与边缘旁区域以及（较温和地）默认模式区域共享耦合，而更宽泛的共同波动则延伸到体运动和边缘旁网络。发散模式取决于估算器：在直接关联下，海马亚区优先与默认模式和视觉网络耦合，而杏仁核核团偏向腹侧注意和边缘网络；更宽泛的共同波动还涉及杏仁核的体运动皮层和海马的视觉皮层。这些原则在亚区/核团水平上成立，沿海马长轴变化，并确定旁板层核为最像海马的杏仁核亚区。数据驱动的连接梯度证实了两个系统的分离和精细尺度的交错。因此，海马和杏仁核亚区并非作为离散系统嵌入皮层，而是通过结构化的、空间组织的共同表征方式嵌入。

## Abstract
The hippocampus and amygdala are neighboring medial temporal lobe structures linked to memory and affect, yet how their subregions are jointly embedded within distributed isocortical systems remains unclear. Using resting-state fMRI from 722 Human Connectome Project Young Adult participants, we mapped hippocampal and amygdalar subregions within a unified cortex-wide framework, quantifying subregion-to-cortex connectivity via Pearson correlation (broad co-fluctuation) and GLASSO partial correlation (relatively more direct functional association). We introduced two count-based metrics: dominance (relative hippocampal vs. amygdalar representation) and sharedness (balanced co-representation). Direct associations showed both structures sharing coupling with paralimbic areas and, more modestly, default mode regions, while broader co-fluctuations extended into somatomotor and paralimbic networks. Divergence patterns depended on the estimator: hippocampal subregions preferentially coupled with default-mode and visual networks under direct association, while amygdalar nuclei favored ventral attention and limbic networks; broader co-fluctuations additionally implicated somatomotor cortex for amygdala and visual cortex for hippocampus. These principles held at the subfield/nucleus level, varying along the hippocampal long axis and identifying the paralaminar nucleus as the most hippocampus-like amygdalar subregion. Data-driven connectivity gradients confirmed both systems' separation and fine-scale interdigitation. Hippocampal and amygdalar subregions are thus embedded in cortex not as discrete systems, but through structured, spatially organized co-representation.

---

## 论文详细总结（自动生成）

# 论文详细总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：海马和杏仁核是紧密相邻的内侧颞叶结构，分别与记忆和情感处理密切相关，但它们的亚区（海马子区、杏仁核核团）如何共同嵌入到分布式的皮层系统中仍不清楚。传统研究多将两个结构分开考察，或仅关注整体水平，忽视了内部异质性以及两者在皮层上的汇聚与分化模式。
- **整体含义**：理解海马-杏仁核系统的联合皮层组织，有助于揭示记忆-情感交互的神经基础，并为精神疾病（如 PTSD、焦虑、抑郁）中两个结构的功能失调提供新的视角。

## 2. 论文提出的方法论

### 核心思想
- 在一个统一的皮层参考框架内，联合分析海马和杏仁核亚区的功能连接，量化它们在全脑皮层上的“优势度”（dominance，相对贡献）和“共享度”（sharedness，平衡共表征），并通过数据驱动梯度揭示低维组织轴。

### 关键技术细节
- **被试**：Human Connectome Project Young Adult (HCP-YA) 2025 reprocessed release，最终纳入722名严格质控的参与者（年龄28.48±3.75岁，380名女性）。
- **皮层与亚区分割**：
  - 皮层采用 Glasser 多模态图谱（358个区域，排除2个海马分区）。
  - 海马：使用 HippUnfold 1.5.1 分割出 CA1、CA2、CA3、CA4、Subiculum 5个子区，再沿长轴分成前、中、后三段，共15个亚区/半球。
  - 杏仁核：使用 FreeSurfer `segment_subregions` 分割出9个核团/半球（基于Saygin等2017概率图谱）。
- **功能连接（FC）估计**：
  - **Pearson 相关**：捕捉宽泛的共波动（包含直接和间接关联）。
  - **GLASSO（Graphical Lasso）偏相关**：通过L1正则化获得稀疏的条件依赖图，旨在减少间接效应，反映相对更直接的连接。正则化参数通过4折交叉验证（每折一个rfMRI run）优化。
- **关键指标**：
  - **优势度（Dominance）**：对于每个皮层节点，计算归一化的杏仁核连接计数与海马连接计数之差（归一化到[-1,1]）。正值表示杏仁核占优，负值表示海马占优。
  - **共享度（Sharedness）**：同时考虑两个结构的连接总量和平衡性，范围[0,2]，值越大表示两个结构对该皮层节点的贡献越强且越平衡。
- **指标生成**：仅在方法特异性掩膜内计算（各子区前10%最强/最一致的连接），并验证不同阈值（5%,15%）的稳定性。
- **数据驱动的联合梯度**：使用 BrainSpace 工具箱，基于48个亚区（18杏仁核+30海马）到358皮层节点的FC矩阵，构建相似性图（normalized-angle kernel，保留前10%），应用扩散映射（diffusion embedding）提取低维梯度，并投影回皮层表面。

### 算法流程（文字描述）
1. 对每个被试，提取所有406个节点的BOLD时间序列，计算Pearson相关和GLASSO稀疏偏相关矩阵。
2. 组水平平均（对GLASSO，只对非零边进行平均），得到两种组水平FC矩阵。
3. 对于每个子区，在PG/GLASSO矩阵中分别选取前10%最强（或最一致）的皮层连接，形成方法特异性掩膜。
4. 在掩膜内，计算每个皮层节点的优势度和共享度，并映射到皮层表面。
5. 为评估子区特异性，采用留一子区法（LOSO）计算每个子区的优势度偏好和共享度偏好得分。
6. 计算海马-杏仁核之间的直接耦合矩阵。
7. 对48×358的全矩阵（GLASSO需额外用10%共识掩膜过滤）进行扩散嵌入，得到联合梯度，并投影皮层。

## 3. 实验设计

### 数据集
- **主要数据集**：Human Connectome Project Young Adult (HCP-YA) S1200 2025 reprocessed release，722名参与者的4次15分钟静息态fMRI（共1小时），2mm各向同性体素，TR=0.72s，同时提供高分辨率结构T1（0.7mm）。
- **Benchmark**：无显式基准数据集。实验以自身对比为主（两种FC估计器之间的比较）。
- **对比方法**：主要对比 Pearson 相关（全相关）和 GLASSO 偏相关（条件稀疏相关）两种FC估算方式，以及不同阈值（5%,10%,15%）的稳定性，和 split-half 复现性。

### 实验种类
1. **子区-皮层FC图谱**：每个海马和杏仁核子区的前10%皮层连接可视化。
2. **优势度与共享度地图**：在两种FC估计下生成全脑皮层地图，并按 Yeo-7 网络汇总。
3. **种子特异性偏好**：LOSO方法计算每个子区的优势度和共享度偏好得分。
4. **海马-杏仁核直接耦合**：内部交叉连接矩阵及列归一化，并与皮层共享度偏好做相关。
5. **联合梯度分析**：前两个扩散梯度，投影皮层，与经典皮层梯度（G1-G3）和优势度/共享度地图做空间相关。
6. **稳健性验证**：
   - 不同阈值（5%,15%）与10%的对应性。
   - 基于强度的优势度验证（与计数优势度做相关）。
   - 200次随机 split-half 复现性（Dice系数、斯皮尔曼相关）。

## 4. 资源与算力

- **文中未明确提及**任何GPU型号、数量、训练时长或具体计算资源。仅提到使用HCP预处理流程（标准工作站可运行的开源工具），以及自定义分析脚本。数据量中等（722人×4次扫描×406个区域），计算量主要体现在个体级GLASSO（4折交叉验证）和组水平分析。推测在标准服务器或集群上完成，但无具体细节。

## 5. 实验数量与充分性

- **实验数量**：所述实验覆盖了从描述性（FC图谱）到推断性（梯度、相关）的多层次分析，共包含约6大类主要实验，外加3种稳健性验证（阈值、强度验证、split-half）。整体上实验设计较为完整。
- **充分性与公平性**：
  - 使用了公开且高质量的数据集（HCP-YA），预处理标准化。
  - 两种FC估计器的对比使得可以区分“宽泛共波动”和“相对直接连接”，解释更细致。
  - 阈值验证和split-half复现确保了结果不依赖于参数选择和样本。
  - 统计上采用空间自相关保持的Moran谱随机化进行多重比较校正（FDR），控制假阳性。
  - **客观性**：作者在局限性中坦承了方法假设（如GLASSO不反映因果、指标计数性质），结论谨慎，未过度推广。

## 6. 论文的主要结论与发现

1. **皮层上不是离散系统，而是结构化、空间组织的共表征**：海马和杏仁核亚区对皮层的投射并非简单的“海马域”和“杏仁核域”分离，而是一个从一侧占优到双侧平衡的连续梯度。
2. **双FC估计揭示不同组织层次**：
   - GLASSO（条件稀疏）显示共享核心主要位于旁边缘/边缘皮层（如眶额、颞极、前岛叶），并呈现杏仁核对腹侧注意网络、海马对视觉和默认网络的偏好。
   - Pearson（宽泛共波动）将共享范围扩展到体运动网络，且杏仁核在体运动区占优更明显。
3. **海马长轴梯度**：后部海马更“海马样”（偏好默认模式/视觉网络），前部海马更“杏仁核样”（共享度更高、与杏仁核耦合更强），表明前部海马是连接杏仁核汇聚区的主要接口。
4. **旁板层核（paralaminar nucleus）是杏仁核中最像海马的核团**：它在所有梯度上都更接近海马轮廓。
5. **内在耦合与外在共享度的不对称**：海马亚区的强杏仁核耦合预测更高的皮层共享度，但杏仁核核团则没有这种关系。
6. **联合梯度**：第一梯度主要分离海马与杏仁核（尤其Pearson），第二梯度关注海马长轴内部变异和亚区间交错（尤其GLASSO），并映射到皮层经典功能梯度（G1-G3）和优势度/共享度地图。

## 7. 优点

- **方法论创新**：提出“优势度”和“共享度”两个直观的计数指标，将复杂的多子区-皮层关系转化为可解释的全脑地图。
- **双重FC估计**：同时使用Pearson和GLASSO，区分“宽泛共波动”与“相对直接关联”，深化了对功能连接本质的理解。
- **精细亚区分割**：海马采用HippUnfold沿长轴切分为3段×5子区，杏仁核采用9个核团，分辨率高于多数前期研究（通常只分前后或整体）。
- **稳健性验证充分**：阈值敏感性、强度验证、split-half复现、空间统计校正等多层次验证，增强了可信度。
- **与演化理论联系**：讨论中将结果与皮层双起源假说（archicortical vs paleocortical）结合，为观察到的分离-汇聚模式提供进化解释框架。
- **开放科学**：代码公开在GitHub，数据使用公开HCP数据集，可复现性高。

## 8. 不足与局限

- **静息态FC限制**：不直接测量任务状态下的功能交互或因果关系，无法捕捉情感记忆编码/检索时的动态变化。
- **指标性质**：优势度和共享度基于“前10%连接计数”而非连接强度，可能受稀疏性影响。虽然强度验证支持有效性，但绝对值解释需谨慎。
- **GLASSO局限性**：尽管比Pearson更接近直接连接，但仍为统计模型，不反映有效连接或纤维示踪证据；稀疏性依赖于正则化参数，且个体间λ变化可能引入偏差。
- **信号质量问题**：海马和杏仁核的BOLD信号在标准fMRI中信噪比偏低，且HCP数据未针对亚皮层做特殊优化，可能限制对细小核团差异的敏感性。
- **方法特异性掩膜定义不一**：GLASSO使用“支持率”（正边出现比例）选择前10%，而Pearson使用“连接强度”，导致直接对比不完全等同。
- **缺少任务验证**：所有结果基于静息态，未在记忆/情感任务中验证这些组织轴是否重配置。
- **临床推广性**：样本为健康年轻成年（HCP-YA），结果向不同年龄、疾病人群推广需谨慎。

（完）
