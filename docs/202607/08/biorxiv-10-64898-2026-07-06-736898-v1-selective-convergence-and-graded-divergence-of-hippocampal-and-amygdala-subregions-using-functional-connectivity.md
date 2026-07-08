---
title: Selective convergence and graded divergence of hippocampal and amygdala subregions using functional connectivity
title_zh: 使用功能连接的海马和杏仁核亚区的选择性趋同与分级分异
authors: "Erigüc, D. Y., Marsiglia, M., John, A., Bayrak, S., Wan, B., Jakovcic, A., DeKraker, J., Royer, J., Bernhardt, B., Valk, S. L."
date: 2026-07-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.06.736898v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 海马亚区功能连接图谱
tldr: 海马体和杏仁核是记忆与情感相关的重要脑区，其亚区如何共同嵌入皮层网络尚不完全清楚。本研究利用静息态fMRI数据，通过Pearson相关和GLASSO偏相关分析，量化了各亚区与皮层连接的特性。结果发现，两者在边缘旁区域选择性汇聚，而在默认模式、腹侧注意等网络呈现梯度发散。直接关联下海马体偏好默认模式网络，杏仁核偏好腹侧注意网络；广泛共波动则涉及更多感觉运动区域。这些发现揭示了海马体和杏仁核亚区以结构化、空间组织的共同表征形式嵌入皮层，而非离散系统。
source: biorxiv
selection_source: fresh_fetch
motivation: 阐明海马体和杏仁核亚区在皮层功能组织中的汇聚与发散模式，以理解它们如何共同支持记忆与情感处理。
method: 使用722名被试静息态fMRI数据，通过Pearson相关和GLASSO偏相关量化亚区-皮层连接，并引入优势度与共享度指标进行对比分析。
result: 直接关联显示两者在边缘旁和默认模式区域共享连接；海马体偏好默认模式与视觉网络，杏仁核偏好腹侧注意与边缘网络；广泛共波动中杏仁核额外涉及感觉运动皮层。
conclusion: 海马体和杏仁核亚区通过选择性汇聚和梯度发散嵌入皮层，呈现结构化共表征，而非完全分离的独立系统。
---

## 摘要
海马和杏仁核是相邻的内侧颞叶结构，与记忆和情感相关，然而它们的亚区如何共同嵌入到分布的新皮层系统中仍不清楚。利用来自722名人类连接组计划年轻成人参与者的静息态功能磁共振成像数据，我们在统一的皮层范围内绘制了海马和杏仁核亚区图，通过皮尔逊相关（宽泛的共同波动）和图形套索偏相关（相对更直接的功能关联）量化了亚区到皮层的连接。我们引入了两种基于计数的指标：优势度（海马相对于杏仁核的代表性）和共享度（平衡的共同代表性）。直接关联显示，这两个结构共享与旁边缘区域的耦合，并且更适度地与默认模式区域耦合，而更宽泛的共同波动则扩展到了体运动和旁边缘网络。分异模式取决于估计量：在直接关联下，海马亚区优先与默认模式和视觉网络耦合，而杏仁核核团则偏向腹侧注意和边缘网络；更宽泛的共同波动还涉及杏仁核的体运动皮层和海马的视觉皮层。这些原理在亚场/核团水平上成立，沿着海马长轴变化，并将旁层核识别为最类似海马的杏仁核亚区。数据驱动的连接梯度证实了这两个系统的分离和精细尺度的交错。因此，海马和杏仁核亚区并非作为离散系统嵌入皮层，而是通过结构化的、空间组织的共同表征嵌入。

## Abstract
The hippocampus and amygdala are neighboring medial temporal lobe structures linked to memory and affect, yet how their subregions are jointly embedded within distributed isocortical systems remains unclear. Using resting-state fMRI from 722 Human Connectome Project Young Adult participants, we mapped hippocampal and amygdalar subregions within a unified cortex-wide framework, quantifying subregion-to-cortex connectivity via Pearson correlation (broad co-fluctuation) and GLASSO partial correlation (relatively more direct functional association). We introduced two count-based metrics: dominance (relative hippocampal vs. amygdalar representation) and sharedness (balanced co-representation). Direct associations showed both structures sharing coupling with paralimbic areas and, more modestly, default mode regions, while broader co-fluctuations extended into somatomotor and paralimbic networks. Divergence patterns depended on the estimator: hippocampal subregions preferentially coupled with default-mode and visual networks under direct association, while amygdalar nuclei favored ventral attention and limbic networks; broader co-fluctuations additionally implicated somatomotor cortex for amygdala and visual cortex for hippocampus. These principles held at the subfield/nucleus level, varying along the hippocampal long axis and identifying the paralaminar nucleus as the most hippocampus-like amygdalar subregion. Data-driven connectivity gradients confirmed both systems' separation and fine-scale interdigitation. Hippocampal and amygdalar subregions are thus embedded in cortex not as discrete systems, but through structured, spatially organized co-representation.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

海马体和杏仁核是内侧颞叶中相邻的结构，分别与记忆（海马体）和情绪（杏仁核）密切相关。尽管解剖学和动物示踪研究表明二者存在广泛的相互连接以及对皮层（尤其是前额叶和内侧颞叶皮层）的互补投射，但**在人类大脑中，它们的亚区（海马子区与杏仁核核团）如何共同嵌入到大规模皮层网络系统中仍然不清楚**。以往大多数研究要么将海马或杏仁核视为整体，要么分别研究其与皮层的连接，缺乏在一个统一的皮层参照框架下同时考察二者所有亚区的共同表征模式。因此，本文的核心动机是：**量化海马和杏仁核亚区与皮层连接的汇聚（convergence）与分异（divergence）模式，揭示它们是否以离散系统还是结构化共表征的方式嵌入皮层**。

整体意义：该研究推进了对内侧颞叶-皮层整合的理解，表明海马和杏仁核并非两个独立的记忆/情感系统，而是沿着一个从相对偏好到平衡共表征的连续统（continuum）分布在皮层上，且内部亚区（如海马长轴、杏仁核旁层核）具有重要的特异性。

## 2. 论文提出的方法论：核心思想、关键技术细节

### 核心思想
- **统一皮层框架**：将海马（15个亚区：5个亚场 × 3个前后段）和杏仁核（9个核团，双侧共18个）的种子区与360个皮层区（Glasser分区）的静息态功能连接（FC）整合到一个共同的分析空间。
- **两种连接估计量**：使用**Pearson相关**（捕捉宽泛的共波动，包含直接和间接关系）和**GLASSO（图形套索）偏相关**（正则化稀疏估计，旨在提取相对更直接的条件关联），以区分不同层面的皮层-亚区关系。
- **两种基于计数的皮层映射指标**：
  - **优势度（Dominance）**：每个皮层区中，海马与杏仁核种子区贡献的相对偏好（归一化后计数差异，范围-1到+1）。
  - **共享度（Sharedness）**：每个皮层区中，海马与杏仁核贡献的总强度与平衡度（范围0到2，越高表示共同表征越强且越均衡）。
- **联合梯度分析**：对杏仁核-海马-皮层连接矩阵进行扩散嵌入（BrainSpace工具箱），提取低维主成分（梯度），揭示亚区间的分离与交错。

### 关键技术细节
- **数据预处理**：HCP最小预处理流程 + ICA-FIX去噪 + 额外亚区分割：杏仁核使用FreeSurfer概率图谱（软掩膜保留部分体积）；海马使用HippUnfold生成5亚场+前后3等分，构建15个表面包裹。
- **FC矩阵构建**：每个被试406×406矩阵（358皮层区+18杏仁核+30海马），取Fisher-z变换后组平均；GLASSO的λ参数通过4折跨被试交叉验证选择。
- **掩膜定义**：每个种子区取前10%的强连接（Pearson）或最高支持率连接（GLASSO），取各种子区掩膜的并集作为分析基础。
- **留一子区（LOSO）分析**：计算每个子区的皮层偏好得分，避免循环分析。
- **空间统计**：使用Moran谱随机化（neuromaps）校正空间自相关，FDR多重比较校正。

## 3. 实验设计：数据集、基准、对比方法

- **数据集**：人类连接组计划年轻成人（HCP-YA）S1200 2025再加工版本。纳入722名被试（平均年龄28.48±3.75岁；380名女性），排除标准包括运动超标、数据不全、缺乏皮层重建等。
- **基准与对比**：
  - **连接估计量的对比**：主要对比Pearson相关（宽泛共波动）与GLASSO偏相关（稀疏条件关联），解释为直接与间接连接的差异。
  - **指标与已知组织轴对比**：将优势度/共享度与Yeo-7网络划分、Margulies等人报道的经典皮层功能梯度（G1-G3）进行空间对应分析。
  - **子区水平对比**：海马前后轴变化、杏仁核各核团的差异（重点观察旁层核）。
  - **阈值稳定性检验**：将前10%掩膜与前5%、前15%比较，验证指标鲁棒性。
  - **强度验证**：计算基于连接强度的杏仁核-海马差异图，与基于计数的优势度相关分析。
  - **分半可靠性**：200次随机分半重复生成所有掩膜和指标，评估稳定性。

**未与其他独立方法（如动态因果模型、结构连接）直接对比**，但文中详细讨论了与灵长类动物解剖示踪研究（Saunders & Rosene, 1988; Aggleton等, 2015）的一致性。

## 4. 资源与算力

论文中**未明确说明**使用的计算资源（如GPU型号、数量、训练时长）。仅提及使用了HCP预处理后的数据及若干软件工具箱（FreeSurfer、HippUnfold、BrainSpace、Actflow Toolbox等），未涉及深度学习训练过程（HippUnfold的U-Net是预训练好的，论文直接应用）。因此无法总结具体算力消耗，但可指出研究基于722名被试的静息态数据，矩阵规模和梯度计算可通过标准CPU集群完成。

## 5. 实验数量与充分性

- **主要实验组**：两个连接估计量（Pearson / GLASSO）分别生成优势度和共享度皮层图；联合梯度分析（每个估计量2个梯度）。
- **验证实验**：
  - 阈值敏感性（5%、10%、15%）的对比（补充图1）。
  - 强度验证（基于连接强度的优势度与计数优势度相关）。
  - 分半可靠性（200次随机分半，计算Dice系数和相关性，结果高度稳定）。
  - 左右半球分别分析（补充图3），使用Procrustes对齐。
  - 子区种子-皮层偏好LOSO分析。
  - 内部交叉结构耦合（海马-杏仁核FC）与外部共享度偏好的相关性（零阶与偏相关）。
- **充分性评价**：
  - **充分且客观**：样本量较大（722人），预处理严格，多种控制分析（运动、阈值、分半）支持结果稳定性。
  - **不足之处**：仅使用静息态，未在任务态或病变条件下验证；未与结构连接或有效连接对照；GLASSO与Pearson的掩膜定义方式略有差异（强度vs支持率），但作者承认是为处理稀疏性而设计，并建议视为互补而非直接比较。

## 6. 论文的主要结论与发现

1. **皮层非离散系统**：海马和杏仁核亚区的皮层连接并非划分为两个分离的专属区域，而是沿着优势度连续统从海马偏好（视觉、默认模式网络）到杏仁核偏好（腹侧注意、体运动网络），并有有限的选择性共享区域（旁边缘、眶额皮层）。
2. **共享区域取决于连接估计量**：直接关联（GLASSO）聚焦于旁边缘/边缘核心区域；宽泛共波动（Pearson）延伸到更广泛区域，尤其是体运动皮层。
3. **海马前后轴梯度**：后部海马与海马偏好皮层耦合更强，前部海马更接近杏仁核共享区域并具有更强的内在海马-杏仁核耦合。
4. **杏仁核内部异质性**：旁层核（paralaminar nucleus）在所有梯度中始终与海马最相似，最接近海马-杏仁核交界区。
5. **内在-外在关联不对称**：海马亚区中，更强的海马-杏仁核内在耦合预测更高的皮层共享度（正向关系），但杏仁核核团无此关联。
6. **联合梯度**：低维嵌入同时展现了结构水平的分离（G1）与精细尺度的交错（G2），且GLASSO梯度更多强调海马内部前后分化，Pearson更多强调海马-杏仁核宏观分离。

## 7. 优点：方法或实验设计上的亮点

- **统一框架**：首次在海马和杏仁核所有亚区水平建立联合皮层参照框架，超越了以往单独研究或整体研究的局限。
- **双重估计量**：通过Pearson与GLASSO对比有效分离了宽泛共波动与条件直接关联，揭示不同组织尺度，并得到动物解剖学初步支持。
- **可解释的映射指标**：优势度与共享度简洁直观，且经过强度验证、阈值稳定性和分半可靠性多重验证，具有鲁棒性。
- **严格的统计控制**：使用Moran谱随机化校正空间自相关，避免假阳性；LOSO分析减少循环性；分半检验保证可重复性。
- **公开数据与代码**：使用HCP公开数据，承诺发布代码，促进可复制性。
- **与经典组织轴衔接**：将结果映射到Yeo-7网络和Margulies梯度，使低维模式具有宏观神经生物学意义。

## 8. 不足与局限

- **仅基于静息态**：无法直接推断任务状态（如情绪记忆编码）下的功能组织变化，结论仅限于内在功能连接。
- **计数指标本质**：优势度和共享度反映的是相对代表性（前10%的种子覆盖数），而非绝对连接强度，可能受阈值影响（虽然经过稳定性检验）。
- **GLASSO局限**：虽然比Pearson更接近直接关联，但仍是统计模型，并非有效或结构连接；稀疏性导致部分边缘缺失，影响组平均。
- **信噪比限制**：亚皮层（尤其是较小杏仁核核团）的BOLD信号信噪比在标准3T fMRI中较低，HCP虽然经过优化但未专门针对亚区分辨率设计，可能限制检测细微差异。
- **未使用多模态证据**：缺乏结构连接（如弥散张量成像）、有效连接（如动态因果模型）或任务态激活的交叉验证，解释力主要依赖前人动物文献。
- **被试范围有限**：仅包含健康年轻成人（HCP-YA），结论向儿童、老年或临床症状的泛化性未知。
- **亚区分割的误差**：杏仁核核团和HippUnfold分割依赖于概率图谱和自动算法，个体间变异未完全消除，可能存在配准误差。

---

（完）
