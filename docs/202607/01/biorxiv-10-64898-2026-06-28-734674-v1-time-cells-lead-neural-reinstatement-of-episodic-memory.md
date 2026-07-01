---
title: Time cells lead neural reinstatement of episodic memory
title_zh: 时间细胞引导情景记忆的神经重现
authors: "Seger, S., Dulaney, A., Araiza Carranza, O., Mahesh Kumar, R., Jacobs, J., Lega, B."
date: 2026-06-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.28.734674v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 时间细胞引导情景记忆的神经重演
tldr: 情景记忆依赖于对时间背景的编码与恢复。人脑内侧颞叶中的时间细胞在编码时形成序列活动，并在检索时优先于其他神经元放电，启动序列重放。这种活动模式预测了上下文介导的记忆行为。此外，相位编码和自然场景中发现的上下文敏感神经元揭示了时间背景表征的普遍机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究时间细胞是否在情景记忆检索中参与时间背景的恢复，以及其如何驱动回忆行为。
method: 利用神经外科患者的微电极记录，在自由回忆和序列重建任务中分析时间敏感神经元的集群放电与序列活动。
result: 时间细胞在检索时优先放电，启动神经序列重放，且其活动模式与上下文介导的回忆行为相关。
conclusion: 内侧颞叶的时间细胞通过序列重放实现时间背景的编码与恢复，是情景记忆的细胞基础。
---

## 摘要
情景记忆系统赋予人类独特的能力来形成和提取丰富而详细的记忆。这种能力需要在编码时表示时间背景，并在提取时恢复它以驱动成功回忆。人类内侧颞叶皮层中的时间细胞和斜坡细胞被认为是时间背景的神经基础，但它们是否参与提取过程中的背景恢复仍不清楚。利用来自神经外科患者的微电极记录，在两种经典情景记忆范式——自由回忆和序列重建中，我们识别出时间敏感神经元，并证明这些神经元群体分别参与伽马和西塔时间尺度上的神经集群和有序序列。与情景加工行为模型预测的时间背景恢复一致，时间细胞放电先于更广泛的集群群体，并启动序列激活提取。这些特性预测了背景介导的回忆行为。我们还通过互补群体识别出相位编码作为汇聚机制，其招募取决于任务需求。最后，我们在一个缺乏经典实验范式可预测时间支架的自然观看数据集中展示了上下文敏感神经元的出现。这些发现揭示了人类内侧颞叶皮层在情景编码期间表示时间背景并在提取期间恢复它的细胞机制。

## Abstract
The episodic memory system provides humans with a unique ability to form and retrieve rich and detailed memories. This capacity requires representing temporal context at encoding and recovering it at retrieval to drive successful recall. Time cells and ramping cells in human medial temporal cortex have been proposed as substrates of temporal context, but whether they participate in context recovery during retrieval remains unknown. Using microelectrode recordings from neurosurgical patients across two classical episodic paradigms, free recall and serial reconstruction, we identify time sensitive neurons and demonstrate that these neuron populations participate in neuronal assemblies and organized sequences on gamma and theta time scales respectively. Consistent with recovery of temporal context predicted by behavioral models of episodic processing, time cell firing precedes the broader assembly population and initiates sequential activation retrieval. These properties predict contextually-mediated recall behavior. We also identify phase coding by complementary populations as convergent mechanisms whose recruitment depends on task demands. Finally, we demonstrate the emergence of context--sensitive neurons in a naturalistic viewing dataset lacking the predictable temporal scaffold of canonical assays. These findings identify cellular mechanisms by which the human medial temporal cortex represents temporal context during episodic encoding and recovers it during retrieval.

---

## 论文详细总结（自动生成）

### 论文详细中文总结

#### 1. 核心问题与整体含义（研究动机和背景）
- **核心问题**：情景记忆依赖于在编码时表示时间背景，并在检索时恢复该背景以驱动成功回忆。时间细胞和斜坡细胞被认为是大规模时间背景的神经基础，但它们是否参与检索过程中的背景恢复尚不清楚。
- **整体含义**：该研究旨在揭示人类内侧颞叶皮层如何通过细胞层面的机制编码和恢复时间背景，以支持情景记忆。通过比较自由回忆（需要内部生成时间背景）和序列重建（外部提供项目信息）两种任务，以及引入自然观看范式，探索时间背景表征的普遍性和任务依赖性。

#### 2. 方法论：核心思想、关键技术细节
- **核心思想**：时间细胞在编码时形成有序的放电序列，在检索时优先于其他细胞放电，启动神经重放，从而恢复时间背景并引导项目回忆。
- **关键技术细节**：
  - **数据采集**：使用Behnke-Fried深度电极（含9根40μm铂铱微丝）记录62例癫痫患者内侧颞叶（海马体、内嗅皮层、杏仁核、海马旁回）的单单元活动，采样率30kHz或32.6 kHz。
  - **时间细胞识别**：非参数方法：高斯核（σ=0.5s）卷积得到连续放电率，再按1s时窗分箱，用Kruskal-Wallis检验时间调制，并用1000次循环时间平移置换检验确定显著性（p<0.05）。时间场定义为连续高于平均放电率的区间（≥1s且出现在至少一半列表中）。
  - **斜坡细胞识别**：Poisson广义线性模型（GLM），预测变量包括会话时间、时期时间（或场景时间），以及字词呈现、列表开始等干扰回归量，采用逐步回归（进入p<0.01，剔除p<0.005），并用1000次循环平移进行显著性验证。
  - **群体解码**：多分类逻辑回归解码器，将编码列表分为20个时窗，输入群体放电率向量（平方根变换后z标准化，高斯平滑σ=0.5窗）。通过构建伪群体（每人每神经元随机有放回取样）进行10折交叉验证，比较时间细胞、斜坡细胞、两者并集、既非等四类细胞的解码精度。
  - **细胞组装检测**：PCA-ICA框架，将编码期25ms时间窗内放电率进行PCA（保留超过Marchenko-Pastur分布特征值的成分），再经快速ICA得到独立组装。组装成员定义为权重绝对值超过均值+1标准差。组装表达强度E(b)=R(b)ᵀ(O)R(b)，其中O为组装权重向量的外积并置对角元素为0。
  - **组装重激活**：检索期间表达强度超过全会话均值+2标准差的时窗视为重激活事件。
  - **θ相位领先分析**：针对每个组装，先确定其成员最锁相的θ频率（2-10Hz，最大平均相位锁定强度）。对于重激活事件，提取非组装成员的时间细胞在±150ms内尖峰对应的θ相位，与组装成员平均θ相位比较，负值表示时间细胞相位领先。
  - **序列检测**：使用SPADE算法（Spike Pattern Detection and Evaluation）在5ms分辨率的编码-检索串联时间线上检测重复的三神经元以上模式，经1000次抖动替代检验（泊松抖动）和FDR校正。
  - **θ相位编码分析**：仅对非时间-斜坡细胞进行。提取每个尖峰在θ波带（5-9Hz，复合瞬时相位）的相位，计算每个序列位置（或HMM状态）的均向量长度（MRL），用Rayleigh检验和循环平移置换检验。还计算了圆-线性相关性（序列位置与相位的相关性）。
  - **隐马尔可夫模型（HMM）**：左到右状态变量，对伪群体（所有被试合并）的z标准化放电率（σ=250ms高斯平滑，每列表500时间点）进行建模，通过EM估计（初始自转移概率0.95），用交叉验证选择最优状态数K。

#### 3. 实验设计
- **数据集/场景**：
  - **自由回忆任务**：27名患者（来自托马斯杰斐逊大学医院和德克萨斯大学西南医学中心），学习12或15个单音节词列表，算术分心后自由回忆30-45秒。共768个单神经元。
  - **序列重建任务**：35名患者（仅UTSW），学习10词列表，分心后按顺序重建。共247个神经元。
  - **自然观看任务**：12名UTSW患者观看28分钟《抑制热情》剧集（17个场景）。共90个神经元。
- **基准（Behavioral benchmarks）**：
  - 自由回忆中计算时间聚类因子（TCF），度量连续回忆词的编码位置邻近性。
  - 序列重建中计算顺序正确率（按绝对位置正确且连续两个正确）。
- **对比方法**：
  - 时间细胞 vs. 斜坡细胞 vs. 既非细胞的解码能力比较。
  - 含有时间细胞的组装 vs. 不含时间细胞组装的重新激活强度比较（按高低回忆列表分层）。
  - 时间细胞引导的序列重放 vs. 整体序列重放与TCF的相关性。
  - 相位编码与序列位置 vs. HMM状态的分析。

#### 4. 资源与算力
- 文中**未明确说明**所使用的GPU型号、数量或训练时长。数据处理和统计分析使用Python（scikit-learn、circular statistics toolbox）和Matlab。因此无法报告具体的算力资源。

#### 5. 实验数量与充分性
- **实验数量**：涵盖大量比较，例如：
  - 时间细胞比例在两个范式中的差异（χ²检验）。
  - 时间场宽度对比（Mann-Whitney U，p<1e-18）。
  - 斜坡细胞亚型分布对比。
  - 解码准确性（4种细胞池，2种范式，早期vs.后期，子采样后比较）。
  - 组装相关分析（80个组装来自19名受试者自由回忆，42个来自12名受试者序列重建）。
  - 相位领先的鲁棒性检验（不同θ频率、窗口宽度、直接时间测量）。
  - 序列检测（共数百个序列）、重放频率与TCF的相关性（17名受试者自由回忆，9名受试者序列重建）。
  - HMM建模与相位锁相分析（自由回忆413个非时间细胞，序列重建141个非时间细胞）。
  - 自然观看中斜坡细胞比例（32/90）。
- **充分性**：实验设计较为全面，包括行为-神经关联、多种统计检验（置换检验、线性混合效应模型、聚类bootstrap）。对比了不同任务、不同细胞类别、不同时间尺度。不过，由于是相关研究而非因果操纵，结论强度有限。此外，样本大小虽在单细胞记录中算较大，但跨被试的统计仍受个体差异影响。

#### 6. 主要结论与发现
- 在两种范式中均识别出时间细胞（自由回忆24.2%、序列重建27.9%）和斜坡细胞，但时间场宽度在自由回忆中更窄，斜坡细胞亚型分布有差异。
- 时间细胞池对编码时窗的群体解码最准确，且早期位置解码优于晚期。
- **时间细胞在检索时θ相位领先**：自由回忆中领先约-63°（~-29ms），序列重建中领先约-23°（~-11ms），均统计显著。
- **含有时间细胞的组装重新激活更强**，且在自由回忆中与回忆成功具有交互作用（高回忆列表上优势更明显）。
- 含时间细胞的组装内部，在自由回忆高回忆列表上，时间细胞在γ相位上领先非时间细胞成员（约-21°）。
- **时间细胞引导的序列重放频率与时间聚类因子正相关**（r=+0.23），且比整体重放率对行为的预测更强。
- **θ相位编码**：序列重建中更多神经元锁相，且存在跨序列位置的共享锁相群体；自由回忆中相位编码更多地与HMM隐藏状态（而非序列位置）相关。
- 自然观看中仅识别出斜坡细胞（35.6%），包括会话尺度和场景内斜坡，未见经典时间细胞。

#### 7. 优点
- **任务比较设计**：通过自由回忆与序列重建对比，揭示了时间背景内部生成 vs. 外部提供对神经编码的影响，解释力强。
- **多层面细胞机制整合**：同时研究了率编码（时间细胞、斜坡细胞）、相位编码、序列重放，并在同一框架下分析其与行为的关联。
- **生态效度延伸**：引入自然观看范式，证明斜坡细胞在无结构间隔的情况下仍存在，支持连续时间表征的默认性质。
- **严谨的统计方法**：大量使用置换检验、圆形统计、非线性混合效应模型、聚类bootstrap等，控制多重比较。
- **新颖的细胞-行为直接联系**：时间细胞启动的序列重放频率与时间聚类因子正相关，提供了时间背景恢复的细胞证据。

#### 8. 不足与局限
- **因果性缺失**：全部为相关性证据，未通过刺激或扰动验证时间细胞对回忆的必要性。
- **组装检测时效有限**：25ms时窗和ICA方法不能排除更精细的共放电结构，且只检测了特定时间尺度的组装。
- **缺乏项目内容读出**：无法直接记录项目（单词）对应的单细胞，因此无法同时观测项目恢复的一面，只能通过行为推断。
- **样本量限制**：虽然单细胞数可观，但跨被试分析时每个任务只有27-35人，自然观看仅12人，可能存在个体间差异。
- **虚部分析潜在偏差**：HMM状态数通过交叉验证选择，但状态定义依赖于伪群体，可能忽略个体特异性动态。
- **应用限制**：结果来自癫痫患者病理脑（药物难治性癫痫），可能不完全代表健康人脑。

（完）
