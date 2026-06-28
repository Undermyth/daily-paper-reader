---
title: Hippocampal-cortical coupling dynamics drive system consolidation of remote memory
title_zh: 海马-皮层耦合动力学驱动远程记忆的系统巩固
authors: "Sheng, T., Wang, S., Zhang, J., Xing, D., Wu, Y., Wang, Q., Lu, W."
date: 2026-06-26
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.22.733680v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 海马-皮层耦合、系统巩固、记忆表征
tldr: 系统巩固将海马依赖记忆转化为皮层长期存储，但神经机制不明。本研究通过记录大鼠恐惧记忆形成中脑区电活动，发现学习时海马快伽玛相位相对前额叶皮层theta振荡渐进前移，此相移模式在睡眠巩固期通过尖波涟漪-皮层纺锤波事件重现。跨过程，区域间相互作用从海马驱动的伽玛相干性转变为前额叶皮层控制的低频相干性。闭环光遗传扰动证实这一耦合相移是近期到远程记忆转化的关键因果机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 探索系统巩固过程中海马-皮层耦合动态如何介导近期记忆向远程记忆转化。
method: 记录大鼠恐惧记忆形成中脑区局部场电位和单神经元活动，结合闭环光遗传扰动验证因果关系。
result: 发现海马快伽玛相位相对前额叶皮层theta渐进前移，并在睡眠巩固期重现；区域间相互作用从海马驱动转化为前额叶皮层驱动。
conclusion: 海马-前额叶皮层耦合相移是系统巩固近期到远程记忆转化的关键神经底物。
---

## 摘要
系统巩固将记忆的临时海马表征转化为皮层的长期存储。然而，其潜在的神经基质仍然是个谜。在这里，我们追踪了恐惧记忆形成过程中行为动物海马-皮层局部场电位和单神经元尖峰的时空演变。在学习期间，海马快速伽马相对于前额叶皮层θ振荡表现出渐进的相位偏移，伽马功率对齐到前额叶皮层θ周期的逐渐延迟阶段。引人注目的是，在随后的巩固过程中，与海马尖波涟漪和NREM睡眠期间的短暂前额叶皮层纺锤波事件相关联，一种相关的相位偏移耦合模式重新出现。在这个过程中，区域间相互作用从近期阶段的海马驱动的皮层伽马相干性演变为远程阶段的前额叶皮层介导的皮层低频相干性。利用闭环光遗传扰动，我们展示了远程记忆形成背后耦合事件的逐步因果链。我们的研究揭示了海马-前额叶皮层耦合相位偏移作为介导记忆从近期到远程转化的可行基质。

## Abstract
System consolidation transforms temporary hippocampal representation of memory into long-term storage in cortex. The underlying neural substrate, however, remains enigmatic. Here, we tracked the spatiotemporal evolution of hippocampus (HPC)-cortex local field potentials and single-neuron spikes in behaving animals during fear memory formation. During learning, HPC fast gamma exhibited a progressive phase shift relative to PFC theta oscillations, with gamma power aligning to progressively later phases of the PFC theta cycle. Strikingly, a related phase-shifted coupling pattern re-emerged during subsequent consolidation in association with hippocampal sharp-wave ripples and transient PFC spindle events during NREM sleep. Across this process, interregional interactions evolved from HPC-driven cortical gamma coherence at recent stages to PFC-mediated cortical low-frequency coherence at remote stages. Using closed-loop optogenetic perturbations, we demonstrated a stepwise causal chain of coupling events underlying remote memory formation. Our study revealed HPC-PFC coupling phase shift as a feasible substrate mediating recent-to-remote transformation of memory.

---

## 论文详细总结（自动生成）

### 论文深度分析报告
**论文标题**：海马-皮层耦合动力学驱动远程记忆的系统巩固  
**研究对象**：大鼠在痕迹恐惧条件化任务中的海马（HPC）-前额叶皮层（PFC）及其他皮层（ACC、PPC）的神经振荡耦合动态。

---

#### 1. 核心问题与整体含义
- **背景**：系统巩固是记忆从海马依赖向皮层长期存储转移的过程，但其神经基质尚不明确。以往研究多关注早期突触与环路机制，对后期（尤其远程记忆形成）的神经活动时空特征了解甚少。
- **核心问题**：海马与皮层之间如何通过振荡耦合动态实现从近记忆到远程记忆的转化？是否存在一个可观测、可因果验证的神经标志物？
- **整体含义**：揭示了一种新的跨频段相位-幅度耦合偏移（Phase-Amplitude Shift, PAS）现象，并证明其在系统巩固中起因果桥梁作用，为理解记忆的长期存储与大脑信息传递提供了关键机制。

---

#### 2. 方法论
- **核心思想**：结合多脑区同步电生理记录（LFP与单神经元尖峰）与闭环光遗传扰动，动态追踪恐惧记忆形成与巩固过程中海马-皮层耦合的变化，并验证其因果关系。
- **关键技术细节**：
  - **多通道电极阵列**：自行设计可同时记录HPC、PFC、ACC、PPC的LFP和spike的3D打印电极，实现高频次、长时间跨天记录。
  - **振荡分析**：使用小波分解提取θ（4-12 Hz）、慢γ（30-45 Hz）和快γ（60-90 Hz）频段；采用调制指数（MI）量化相位-幅度耦合（PAC）。
  - **相位偏移量化**：通过圆-线性回归计算每只动物在连续条件化训练中快γ功率相对于PFC θ相位的斜率（phase slope），定义为PAS。
  - **脑状态分类**：结合EEG、EMG、呼吸、心率以及视频监控，区分清醒、NREM、REM睡眠及冻结/不动状态。
  - **闭环光遗传干预**：
    - 随机低频相位干扰：在巩固期（day 4-21）随机脉冲抑制PFC低频节律，破坏PAS。
    - 实时相干性检测：基于实时计算HPC-皮层γ相干性，触发光遗传抑制HPC或PFC，分别干扰近期γ相干性和远程低频相干性。
    - SWR-triggered闭环：抑制尖波涟漪（SWRs）以检验其对PAS重现的必要性。
- **算法流程**：
  - 实时LFP → 带通滤波 → 滑动窗口FFT计算相干性 → 超过阈值（>3 SD）触发光脉冲（400 ms）。
  - 相位-幅度耦合：相位分50 bin，计算每个bin上γ平均幅值，用MI度量耦合强度。
  - 斜率拟合：对每只动物，以训练试次（或天数）为自变量，以γ功率的θ相位为因变量做圆-线性回归，得到斜率。

---

#### 3. 实验设计
- **任务与行为**：大鼠痕迹恐惧条件化（trace fear conditioning），CS（音调）与US（足底电击）之间有18秒间隔，学习后分别在day 7（近期记忆）和day 28（远程记忆）进行情境回忆测试（冻结行为）。
- **数据集与场景**：
  - 条件化阶段：记录ITI期间（40秒）的LFP与spike。
  - 巩固阶段（day 0-28）：每日在home cage中记录3-5小时，覆盖各种行为状态（清醒、NREM、REM）。
- **对比方法**：
  - 条件化组（CS-US） vs. CS only组 vs. 电击only组。
  - 对比不同脑区对（HPC-PFC、HPC-ACC、HPC-PPC）和不同频段组合。
  - 对照条件：shuffled数据（时间平移γ幅值）验证PAC显著性；延迟光遗传干预作为对照。
- **Benchmark**：无外部标准benchmark，但以冻结行为百分比和学习表现作为行为基准。

---

#### 4. 资源与算力
- **文中未明确说明**：未提及GPU型号、数量或训练时长。数据处理主要在MATLAB（Chronux工具箱、定制脚本）中完成，使用CPU计算（如小波变换、FFT、相干性分析）。闭环系统涉及实时计算（MATLAB + GPU并行加速），但未提供具体配置。因此，无法量化算力消耗。

---

#### 5. 实验数量与充分性
- **实验组数量**：
  - 行为学：CS-US组（n=6-8只大鼠）、CS only组（n=6-8只）。
  - 电生理：每只大鼠多通道（PFC 20/32 ch，HPC 16/32 ch，ACC 12 ch，PPC 16 ch），纵向连续28天。
  - 单细胞分析：共记录数百个（如46个 phase-locked 单元，104个 non-phase-locked；巩固期51个单元）。
  - 光遗传干预：每组n=4-5只。
- **消融实验**：
  - 因果关系验证：抑制HPC-皮层γ相干性 → 检查PAS和远程低频相干性及行为；抑制PFC低频相位 → 检查后续耦合转换。
  - 控制条件：SWR抑制、延迟干预、不同类型神经元分类（锥体细胞与中间神经元）。
- **充分性与客观性**：
  - 研究覆盖了从学习到巩固全过程（0-28天），对睡眠状态、冻结状态、运动状态进行了分类控制，排除了呼吸节律、volume conduction等混淆因素。
  - 统计方法严谨（圆-线性回归、置换检验、Bonferroni校正、t检验、ANOVA等），结果在多个动物中一致重复。
  - 不足：单细胞追踪仅限于短期（用平均相位代替单细胞长期追踪），缺乏对编码期与巩固期间一神经元活动的直接比较。

---

#### 6. 主要结论与发现
- **发现1**：条件化学习中，HPC快γ功率相对于PFC θ相位发生渐进性向前相移（PAS），且该偏移与学习表现正相关。
- **发现2**：在巩固期（day 4-21）的NREM睡眠期间，伴随SWRs，PAS重新出现，且同样存在相位偏移，偏移幅度与编码期相似。
- **发现3**：时序上先发生HPC-皮层快γ相干性（近期，day 0-7），然后PAS重现（day 4-21），最后出现PFC-皮层低频相干性（远程，day 14-28）。
- **发现4**：对话组织者和信息流方向发生转移——近期以HPC为中心、HPC→PFC；远程以PFC为中心、PFC→ACC/PPC。
- **发现5**：因果验证——破坏PAS会阻止后续低频相干性转换、中心性转移以及远程记忆巩固；破坏早期γ相干性同样消除PAS和后续事件；破坏远程低频相干性则损害记忆稳定。
- **总结结论**：PAS是系统巩固中从近记忆到远程记忆转化的关键神经机制，通过“手递手”式逐步耦合事件完成记忆的皮层化存储。

---

#### 7. 优点
- **创新性**：首次报道了学习-巩固全过程中的渐进式相位偏移（PAS），并将其明确为系统巩固的生理标志。
- **技术整合**：结合多脑区长期记录、行为学分类、实时闭路光遗传干预，实现了对跨区域振荡耦合的因果因果检验。
- **严格对照**：排除了多种混淆（呼吸、容积传导、运动状态、睡眠阶段等），并通过shuffle、延迟干预等严格对照验证。
- **系统性**：完整描绘了从学习、近期巩固到远程巩固的“手递手”式动态序列，为系统巩固理论提供了具体的神经活动框架。

---

#### 8. 不足与局限
- **细胞/环路机制未解析**：PAS的细胞机制（如突触可塑性、兴奋性调节）未直接研究。
- **编码内容未知**：未检验PAS期间是否存在特定的神经元序列重放，无法确定其携带的记忆表征内容。
- **长期追踪困难**：无法在数周内稳定追踪同一单细胞，限制了编码与巩固阶段直接比较。
- **算力信息缺失**：未报告硬件资源，可能影响可重复性。
- **模型单一性**：仅使用痕迹恐惧条件化，未验证其他记忆类型（如空间、程序性记忆）中PAS的普适性。
- **样本量较小**：光遗传每组n=4-5只，虽统计显著但潜在偏倚较大。

---

（完）
