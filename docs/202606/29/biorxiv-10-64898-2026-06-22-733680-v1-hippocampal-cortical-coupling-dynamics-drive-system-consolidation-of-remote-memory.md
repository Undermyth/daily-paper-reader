---
title: Hippocampal-cortical coupling dynamics drive system consolidation of remote memory
title_zh: 海马-皮层耦合动态驱动远程记忆的系统巩固
authors: "Sheng, T., Wang, S., Zhang, J., Xing, D., Wu, Y., Wang, Q., Lu, W."
date: 2026-06-26
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.22.733680v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 系统巩固远程记忆过程中的海马-皮层耦合动力学
tldr: 记忆系统巩固需要海马-皮层耦合动态变化。研究发现，学习时海马快伽马相对于前额叶theta振荡出现渐进相移，并在睡眠尖波涟漪和纺锤波事件中重现。随巩固过程，耦合从海马驱动的伽马相干性转变为前额叶驱动的低频相干性，通过闭环光遗传验证了因果链条。这些结果揭示海马-前额叶耦合相移是近期记忆向远程记忆转化的神经基质。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究系统巩固过程中海马与皮层耦合的动态变化及其因果机制。
method: 记录大鼠恐惧记忆形成中HPC-PFC场电位和单神经元活动，分析耦合模式，并用闭环光遗传扰动验证因果。
result: 学习期海马快伽马相对PFC theta相移，NREM睡眠中类似模式重现；耦合从近期HPC驱动变为远程PFC驱动低频相干。
conclusion: HPC-PFC耦合相移是记忆巩固中近期到远程转化的关键基质。
---

## 摘要
系统巩固将记忆的临时海马表征转化为皮层中的长期存储。然而，其潜在的神经基质仍然是个谜。在这里，我们追踪了恐惧记忆形成过程中行为动物海马-皮层局部场电位和单神经元尖峰的时空演变。在学习期间，海马快速伽马相对于前额叶皮层θ振荡表现出渐进式相位偏移，伽马功率对齐到前额叶皮层θ周期中逐渐延迟的相位。引人注目的是，在随后的巩固过程中，一种相关的相位偏移耦合模式重新出现，与非快速眼动睡眠期间海马尖波涟漪和前额叶皮层短暂梭形事件相关联。在整个过程中，区域间相互作用从近期阶段的由海马驱动的皮层伽马连贯性演变为远程阶段的由前额叶皮层介导的皮层低频连贯性。利用闭环光遗传学扰动，我们展示了远程记忆形成背后耦合事件的逐步因果链。我们的研究揭示了海马-前额叶皮层耦合相位偏移作为介导记忆从近期到远程转化的可行基质。

## Abstract
System consolidation transforms temporary hippocampal representation of memory into long-term storage in cortex. The underlying neural substrate, however, remains enigmatic. Here, we tracked the spatiotemporal evolution of hippocampus (HPC)-cortex local field potentials and single-neuron spikes in behaving animals during fear memory formation. During learning, HPC fast gamma exhibited a progressive phase shift relative to PFC theta oscillations, with gamma power aligning to progressively later phases of the PFC theta cycle. Strikingly, a related phase-shifted coupling pattern re-emerged during subsequent consolidation in association with hippocampal sharp-wave ripples and transient PFC spindle events during NREM sleep. Across this process, interregional interactions evolved from HPC-driven cortical gamma coherence at recent stages to PFC-mediated cortical low-frequency coherence at remote stages. Using closed-loop optogenetic perturbations, we demonstrated a stepwise causal chain of coupling events underlying remote memory formation. Our study revealed HPC-PFC coupling phase shift as a feasible substrate mediating recent-to-remote transformation of memory.

---

## 论文详细总结（自动生成）

# 论文结构化中文总结

## 1. 核心问题与整体含义（研究动机和背景）

- **核心问题**：系统巩固（system consolidation）是记忆从海马临时存储转移到皮层长期存储的过程，但其神经基质和动态机制尚不清楚。具体来说，缺乏对远程情景记忆形成过程中跨区域振荡耦合的全面刻画和因果证据。
- **研究动机**：已有研究识别了与记忆过程相关的特征性神经振荡（如θ相位进动、尖波涟漪SWR），但关于系统巩固中振荡特征的刻画很少，尤其是跨区域振荡连贯性的因果证据缺失。本文旨在填补这一空白。
- **整体含义**：揭示海马-前额叶皮层耦合相移（phase-amplitude shift, PAS）作为近期记忆向远程记忆转化的关键神经基质，并证明跨区域振荡耦合的动态变化构成记忆巩固的因果链条。

## 2. 方法论：核心思想、关键技术细节、算法流程

- **核心思想**：通过长期多脑区同步记录局部场电位（LFP）和单神经元尖峰，识别恐惧记忆形成过程中海马-皮层耦合的动态模式（相位-幅度耦合PAC），并利用闭环光遗传扰动验证因果作用。
- **关键技术细节**：
  - **多通道电极阵列**：自行设计的铂铱丝电极，实现海马CA1、前额叶PFC、前扣带皮层ACC和后顶叶皮层PPC同时记录。
  - **行为范式**：大鼠痕迹恐惧条件化（trace fear conditioning），CS（音调）和US（足部电击）间隔18秒，记录从训练前到第28天的神经活动。
  - **睡眠状态分类**：结合EEG、EMG、心率、呼吸信号，区分清醒、NREM和REM睡眠。
  - **相位-幅度耦合（PAC）分析**：计算调制指数（MI），检测PFC θ相位对海马快γ（60-90 Hz）振幅的调制，并观察相位偏移斜率（circular-linear regression）。
  - **闭环光遗传干预**：
    - 随机4-12 Hz相位干扰：在PFC表达eNpHR，随机脉冲扰乱低频率振荡。
    - 基于相干性的闭环干预：实时计算HPC-皮层γ相干性，当超过阈值时触发光遗传沉默，持续400 ms。
  - **因果分析**：通过Granger因果指数、尖峰-尖峰互相关、中枢节点分析等判断信息流向。
- **算法流程**（文字说明）：
  1. LFP预处理：带通滤波（4-12 Hz theta，60-90 Hz gamma），希尔伯特变换提取瞬时相位和振幅。
  2. PAC计算：将θ周期分为50个相位仓，计算每个相位仓平均γ振幅，再计算MI。
  3. 相位偏移测量：对每个试次（或每天）的偏好相位与试次数（或天数）做圆-线性回归，得到斜率。
  4. SWR检测：对LFP进行110-250 Hz滤波，计算均方根包络，阈值法（均值+4σ上界、+1σ下界）检测SWR。
  5. 相干性计算：多窗口法（multi-taper）计算功率谱和交叉谱，得到相干系数Cxy(f)。
  6. Sigmoid拟合：对HPC-皮层γ相干性和PAS斜率随天数的变化拟合Sigmoid函数，确定转换点。
  7. 闭环控制：基于400 ms窗口的傅里叶变换实时计算相干性，当超过均值+3σ时触发激光。

## 3. 实验设计：数据集/场景、基准、对比方法

- **数据集/场景**：
  - 动物模型：成年雄性Sprague-Dawley大鼠（8-15周龄，300-400g）。
  - 行为任务：痕迹恐惧条件化（trace fear conditioning），在条件化箱中进行5个试次，每个试次包括20秒音调→18秒痕迹间隔→2秒足部电击。
  - 记录时间窗：训练前（pre-FC）、训练中各试次间间隔（ITI，40秒）、训练后第0-28天（home cage记录，含NREM/REM/清醒）。
  - 睡眠记录：EEG/EMG电极，AccuSleep自动打分。
- **基准**：比较组包括CS only组（仅有音调无电击）、shock only组（仅有电击无音调），以及不同脑区组合（HPC-ACC、HPC-PPC）。
- **对比方法**：
  - 不同耦合类型：快γ（60-90 Hz） vs 慢γ（30-45 Hz） vs 涟漪（110-250 Hz）；不同频率带（4-7 Hz vs 7-12 Hz）。
  - 不同行为状态：NREM SWR+ vs SWR-，清醒，REM。
  - 不同干预方式：随机LF相位干扰、基于γ相干性的闭环HPC沉默、基于LF相干性的闭环PFC沉默、延迟干预对照、SWR闭环抑制。

## 4. 资源与算力

- **文中未明确说明**：未提及GPU型号、数量、训练时长等计算资源信息。方法中提到了使用MATLAB（2014b）、Chronux工具箱、Plexon系统等，但所有分析均在离线或实时（闭环）方式下进行，未讨论具体算力需求。
- 闭环系统使用NI-DAQ、Master-9刺激器、4-通道光纤等硬件；实时相干性计算依赖GPU并行（MATLAB GPU computing），但未给出具体GPU型号。

## 5. 实验数量与充分性

- **实验数量**：
  - 行为实验：CS-US组和CS only组各6-8只大鼠。
  - 电生理记录：8只CS-US组，6只CS only组（部分测量用到不同子集）。
  - 单单元分析：训练阶段记录了约150个HPC单元（46个相位锁定），巩固阶段51个单元（34.2%相位锁定）。
  - 光遗传实验：PAS干预组n=5，γ相干性闭环干预组n=5，LF相干性闭环干预组n=4，另有延迟对照和SWR抑制实验。
  - 药理学实验（CNQX）：每组n=4-5。
  - 跨区域分析：HPC-PFC、HPC-ACC、HPC-PPC、PFC-ACC、PFC-PPC，以及ACC-PPC组合。
  - 消融性质：包括随机相位干扰、闭环相干性抑制、SWR抑制、药理学失活等，覆盖主要假设。
- **充分性评价**：
  - **充分**：多维度实验（行为、电生理、光遗传、药理学）相互印证；对照设置全面（CS only、shock only、延迟干预、SWR-）；统计方法合理（t检验、ANOVA、Bonferroni校正、圆-线性回归、Pearson相关）。
  - **客观性**：实验人员对睡眠评分盲法；数据清洗和去伪迹标准化；随机化干预时间（随机间隔83-250 ms）。
  - **局限性**：样本量相对较小（每组4-8只），且均为雄性大鼠，可能存在性别偏差；没有独立验证数据集。

## 6. 主要结论与发现

1. **学习阶段存在渐进式相位偏移（PAS）**：恐惧条件化训练中，海马快γ功率在前额叶θ周期中的偏好相位逐渐后移（从上升相到下降相），称为相位-幅度偏移（PAS）。此现象在CS only组或HPC-ACC/HPC-PPC回路中不出现。
2. **PAS与学习表现正相关**：PAS斜率与训练末冻结百分比正相关（r=0.73, p=0.04）。
3. **PAS在系统巩固阶段（第4-21天）重新出现**：仅出现在NREM睡眠中SWR后的1秒窗口内，伴随PFC梭形低频事件；幅度与训练期相似。
4. **HPC-皮层γ相干性先于PAS出现**：在第0-7天（近期记忆阶段），SWR后出现HPC-PFC/ACC/PPC的γ相干性增强，随后PAS重新出现。Sigmoid拟合显示γ相干性下降先于PAS上升。
5. **PAS之后出现皮层间低频相干性**：在第14-28天（远程记忆阶段），SWR后PFC-ACC和PFC-PPC的低频（4-12 Hz）相干性增强，PAS下降先于皮层间相干性上升。
6. **组织者和方向性从HPC转向PFC**：近期阶段HPC为中枢节点，Granger因果为HPC→PFC；远程阶段PFC为中枢节点，Granger因果为PFC→ACC/PPC。
7. **因果验证**：
   - 随机PFC低频相位干扰（第4-21天）消除PAS，阻止后续皮层间相干性，损害远程记忆（第28天冻结降低）。
   - 闭环HPC沉默（基于γ相干性，第3-7天）消除γ相干性和PAS，损害远程记忆。
   - 闭环PFC沉默（基于低频相干性，第14-21天）消除皮层间相干性，损害远程记忆。
   - SWR抑制后PAS不再重新出现。
8. **结论**：HPC-PFC耦合动态（γ相干性→PAS→皮层间低频相干性）构成系统巩固的逐步因果链，其中PAS是近期-远程记忆转换的关键基质。

## 7. 优点

- **技术先进性**：开发了多通道同时记录LFP和单单元的系统，并实现基于实时相干性的闭环光遗传干预，时间精度高（20-40 ms延迟）。
- **数据全面性**：纵向追踪28天，覆盖编码、近期记忆、远程记忆三个阶段；同时监测行为状态（睡眠分期、心率、呼吸），排除混淆因素（呼吸节律、运动）。
- **因果证据**：通过多种扰动（随机相位干扰、闭环相干性抑制、SWR抑制）构建了完整的因果链，远超相关研究。
- **发现新颖性**：首次描述PAS现象及其在系统巩固中的重现和与组织者转移的关联。
- **方法稳健性**：使用多种分析技术（圆-线性回归、Sigmoid拟合、Granger因果、中枢节点分析）交叉验证结论。

## 8. 不足与局限

- **细胞和环路机制未解**：PAS的细胞基础（突触可塑性、兴奋性变化等）未直接研究。
- **神经元表征未知**：PAS是否携带类似重放的尖峰序列、具体信息内容未知。
- **长期追踪单单元困难**：无法直接比较编码期和巩固期同一神经元的放电模式，只能依赖群体平均相位分析。
- **动物模型局限性**：仅使用雄性大鼠，性别和物种推广性有限；样本量较小（每组4-8只），统计效力可能不足。
- **闭环干预的潜在混淆**：光遗传抑制可能非特异性地影响局部电路，虽然控制了延迟干预和随机干预对照。
- **预印本状态**：未经同行评审（bioRxiv），图表和细节可能不完整。

（完）
