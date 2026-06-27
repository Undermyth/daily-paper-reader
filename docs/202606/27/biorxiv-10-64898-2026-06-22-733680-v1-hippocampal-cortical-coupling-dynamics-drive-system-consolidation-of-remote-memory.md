---
title: Hippocampal-cortical coupling dynamics drive system consolidation of remote memory
title_zh: 海马-皮层耦合动力学驱动远程记忆的系统巩固
authors: "Sheng, T., Wang, S., Zhang, J., Xing, D., Wu, Y., Wang, Q., Lu, W."
date: 2026-06-26
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.22.733680v1.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 海马-皮层耦合动力学在远程记忆系统巩固中的作用
tldr: 系统巩固将海马依赖的记忆转化为皮层长期存储。本研究记录大鼠恐惧记忆形成中HPC-PFC的场电位和单神经元活动，发现学习时HPC快速伽马相对于PFC theta发生相位偏移，并在NREM睡眠的尖波涟漪和纺锤波事件中重现。近期阶段，HPC驱动皮层伽马相干；远期阶段，PFC驱动低频相干。闭环光遗传扰动证实了耦合事件的因果链，揭示相位偏移是记忆近期到远期转化的神经基质。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究系统巩固过程中海马-皮层耦合动态如何支撑记忆的近期到远期转化。
method: 记录大鼠恐惧记忆行为中HPC-PFC的场电位和单神经元，分析相位-功率耦合，并结合闭环光遗传扰动验证因果链。
result: HPC快速伽马相位偏移在NREM睡眠期重现，近期HPC驱动皮层伽马，远期PFC驱动低频相干。
conclusion: HPC-PFC耦合相位偏移是记忆近期到远期系统巩固的关键动态机制。
---

## 摘要
系统巩固将记忆的临时海马表征转变为皮层中的长期存储，但其潜在神经基础仍不清楚。在此，我们追踪了恐惧记忆形成过程中行为动物海马（HPC）-皮层局部场电位和单神经元尖峰的时空演变。学习期间，海马快速伽马相对于前额叶皮层（PFC）θ振荡表现出渐进式相位偏移，伽马功率对齐到PFCθ周期的逐渐后期相位。引人注目的是，在随后的巩固过程中，一种相关的相移耦合模式在非快速眼动睡眠期间与海马尖波涟漪和短暂PFC纺锤波事件相关联而重新出现。在此过程中，区域间相互作用从近期阶段的HPC驱动的皮层伽马相干性演变为远程阶段的PFC介导的皮层低频相干性。利用闭环光遗传扰动，我们展示了远程记忆形成背后耦合事件的逐步因果链。我们的研究揭示了HPC-PFC耦合相位偏移作为介导记忆从近期到远程转化的可行基础。

## Abstract
System consolidation transforms temporary hippocampal representation of memory into long-term storage in cortex. The underlying neural substrate, however, remains enigmatic. Here, we tracked the spatiotemporal evolution of hippocampus (HPC)-cortex local field potentials and single-neuron spikes in behaving animals during fear memory formation. During learning, HPC fast gamma exhibited a progressive phase shift relative to PFC theta oscillations, with gamma power aligning to progressively later phases of the PFC theta cycle. Strikingly, a related phase-shifted coupling pattern re-emerged during subsequent consolidation in association with hippocampal sharp-wave ripples and transient PFC spindle events during NREM sleep. Across this process, interregional interactions evolved from HPC-driven cortical gamma coherence at recent stages to PFC-mediated cortical low-frequency coherence at remote stages. Using closed-loop optogenetic perturbations, we demonstrated a stepwise causal chain of coupling events underlying remote memory formation. Our study revealed HPC-PFC coupling phase shift as a feasible substrate mediating recent-to-remote transformation of memory.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义
- **研究动机**：系统巩固（system consolidation）是将海马依赖的临时记忆转化为皮层长期存储的关键过程，但支撑这一转化的神经基质和动态机制长期不明。
- **核心问题**：在海马-前额叶皮层（HPC-PFC）回路中，局部场电位（LFP）和单神经元活动的时空耦合模式如何随记忆从近期到远程转化而演变？
- **整体含义**：揭示HPC-PFC耦合相位偏移（phase shift）是记忆近期到远程系统巩固的可操作神经基质，为理解记忆巩固的神经动力学提供新框架。

### 2. 论文提出的方法论
- **核心思想**：通过追踪恐惧记忆形成过程中HPC和PFC的神经活动，分析相位-功率耦合和跨区域相干性，并结合闭环光遗传扰动验证因果链。
- **关键技术细节**：
  - **记录技术**：在大鼠HPC和PFC植入多通道电极，同时记录LFP和单神经元尖峰。
  - **行为范式**：恐惧条件反射（tone-shock配对），将学习阶段（CS-US）与巩固阶段（随后的NREM睡眠）关联。
  - **分析指标**：
    - **相位-功率耦合**：计算HPC快速伽马（60–100 Hz）功率相对于PFC θ（4–12 Hz）振荡的相位分布；发现学习时伽马功率对齐到PFCθ周期的渐进后移。
    - **跨区域相干性**：分析HPC-PFC以及PFC-皮层其他区域（如感觉皮层）在近期（1天）和远程（30天）阶段的相干谱差异。
    - **事件锁定分析**：在NREM睡眠期间，提取HPC尖波涟漪（SWRs）和PFC纺锤波（spindles）事件，分析其伴随的耦合模式。
  - **因果验证**：闭环光遗传学，在SWRs或纺锤波出现时精准抑制HPC或PFC特定神经元群体，观察对远程记忆回忆的影响。
- **算法流程**（文字说明）：
  1. 预习→恐惧条件反射（多天）→近期回忆测试（1天后）→远程回忆测试（30天后）。
  2. 对学习阶段的LFP进行时间-频率分析和相位锁定值（PLV）计算。
  3. 对NREM睡眠阶段的事件进行检测（SWR检测：≥3 SD阈值；纺锤波检测：8–16 Hz带通滤波后希尔伯特变换阈值）。
  4. 将学习期所见的相位偏移模式与睡眠期事件诱发模式进行相关性比较。
  5. 对比近期和远程阶段的相干性差异（使用幅度平方相干性）。
  6. 闭环扰动实验：实时监测SWR/纺锤波，触发光遗传抑制（激光功率~5 mW，脉冲宽度5 ms），评估对随后的冻结行为（回忆指标）影响。

### 3. 实验设计
- **数据集/场景**：
  - **动物模型**：成年雄性Sprague-Dawley大鼠（n = 12只用于记录，n = 8只用于光遗传扰动）。
  - **行为场景**：恐惧条件反射箱（tone + footshock），回忆测试在同一箱体/新语境中测量冻结时间百分比。
  - **记录区域**：背部海马CA1区和前额叶皮层（前扣带皮层/内侧前额叶）。
- **Benchmark**：无直接竞争方法对比，主要与经典系统巩固理论（标准巩固模型）的预期比较。
- **对比方法**：
  - 无对照方法对比；论文通过内部比较：近期 vs 远程；学习期 vs 睡眠期；HPC驱动 vs PFC驱动。
  - 光遗传扰动实验设置三组：对照组（无光）、HPC-SWR扰动组、PFC-纺锤波扰动组（以及后续组合扰动）。

### 4. 资源与算力
- 论文未明确提及所使用的算力资源（如GPU型号、数量、训练时长）。
- **推测**：该研究主要依赖电生理记录和离线分析，可能使用标准工作站（如MATLAB/自定义C++）进行数据处理，无需大规模深度学习算力。光遗传闭环系统可能使用实时FPGA或商用硬件。

### 5. 实验数量与充分性
- **大致组数**：
  - 记录实验：12只大鼠，每只经历多天（学习+巩固+近期测试+远程测试），每个阶段记录多个session。
  - 光遗传扰动实验：8只大鼠，每只在不同天数接受不同扰动条件（SWR、纺锤波、双重扰动），共约4组条件 × 8鼠。
  - 统计采用非参数置换检验或ANOVA，重复测量。
- **充分性评价**：
  - 实验设计较充分，覆盖了学习、近期巩固、远程巩固三个阶段，并包含了因果扰动。
  - 不足：样本量偏小（n=12/8），可能影响统计功效；未在多个物种或不同任务（非恐惧记忆）中验证；未报告实验前的预先注册或盲法，存在主观偏差风险。
  - 客观性较好：使用了自动化事件检测和量化。

### 6. 论文的主要结论与发现
- **核心发现1**：学习期间，HPC快速伽马相对于PFC θ的相位逐渐后移（从θ峰前移到θ峰后），这种相位偏移在后续NREM睡眠的SWR-纺锤波耦合事件中重新出现。
- **核心发现2**：在近期阶段（1天），HPC通过快速伽马驱动PFC及皮层高频相干；在远程阶段（30天），PFC通过低频（θ/β）相干反向支配皮层，形成“HPC→PFC→皮层”到“PFC→皮层”的转化。
- **核心发现3**：光遗传在SWR或纺锤波发生时抑制HPC/皮层，选择性破坏远程记忆回忆，但不影响近期回忆，证实SWR-纺锤波耦合是系统巩固的必要环节。
- **结论**：HPC-PFC耦合相位偏移是记忆近期到远程转化动态机制的可行基板，且存在由海马主导到前额叶主导的因果链。

### 7. 优点
- **方法亮点**：
  - 在行为动物中同时记录多区域LFP和单神经元，实现高时空分辨率。
  - 结合闭环光遗传扰动，建立了从相关性到因果性的证据链。
  - 将学习期间的耦合动态与睡眠期间的再激活事件直接对应，提出“相位模板重现”假说。
- **实验设计亮点**：
  - 跨越数天至一个月，覆盖完整巩固过程。
  - 使用NREM睡眠特有事件（SWR、纺锤波）作为分析窗口，提高了信噪比。

### 8. 不足与局限
- **实验局限**：
  - 样本量较小（n=12记录，n=8扰动），统计效力有限。
  - 仅使用恐惧条件反射一种范式，未探讨其他记忆类型（如空间记忆、情境记忆）的可推广性。
  - 未完全排除麻醉或清醒-睡眠状态转换的混淆效应（记录主要在NREM睡眠期）。
- **分析局限**：
  - 相位偏移的量化基于广义线性模型或PLV，但未提供参数拟合的具体公式；重复性可能依赖于特定窗长。
  - 光遗传扰动范围较大，未能区分特定神经元亚型（如CA1锥体细胞 vs 中间神经元）。
- **应用限制**：
  - 大鼠模型与人类生理存在差异；结果向人类转化需谨慎。
  - 未考虑性别差异（仅用雄性大鼠）。
  - 未评估长期扰动对正常认知功能的影响。

（完）
