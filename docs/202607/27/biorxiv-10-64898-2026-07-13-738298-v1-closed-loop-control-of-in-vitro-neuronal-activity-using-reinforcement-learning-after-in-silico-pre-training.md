---
title: Closed-loop control of in vitro neuronal activity using reinforcement learning after in silico pre-training
title_zh: 基于预训练强化学习的体外神经元活动闭环控制
authors: "Carvalho, E., Mateus, J. C., Pinto, R., Aroso, M., Aguiar, P."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.13.738298v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 基于强化学习的体外神经元活动闭环控制
tldr: 复杂生物神经网络的最优控制策略难以获取，强化学习需大量探索与组织生理耐受冲突。本文在生物物理校准的数字孪生模型上预训练强化学习策略，再直接迁移到体外培养的神经元网络，实现了对网络爆发的状态依赖控制。迁移策略优于启发式控制且刺激更少，钙成像揭示其利用局部拓扑与生理动力学。该工作验证了数字孪生到活体网络的策略可转移性，为闭环神经调控提供可操作平台。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738298-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1913, \"height\": 964, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738298-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1876, \"height\": 1619, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738298-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1915, \"height\": 1068, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-13-738298-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1892, \"height\": 1844, \"label\": \"Figure\"}]"
motivation: 生物神经网络非平稳特性使传统方法难获最优控制，而强化学习需大量探索与组织生理耐受冲突。
method: 在生物物理校准的数字孪生上预训练强化学习策略，再直接迁移到体外培养的神经元网络实现闭环控制。
result: 迁移策略在抑制网络爆发上优于启发式控制，刺激使用受限；钙成像显示智能体时空优化利用了网络拓扑与内在动力学。
conclusion: 证明数字孪生预训练强化学习策略可直接转移至活体网络，为闭环神经调控提供新范式。
---

## 摘要
通过电刺激控制特定的神经元动力学对于治疗性神经调控至关重要，但由于生物神经网络复杂且非平稳的特性，推导最优控制策略仍然具有挑战性。强化学习虽然提供了强大的闭环控制框架，但其对长时间刺激驱动探索的依赖难以与活体组织的生理极限相协调。本文展示了一种从硅基到体外（in silico-to-in vitro）的迁移策略，实现了对培养神经元网络爆发活动的有效状态依赖控制。迁移后的策略优于启发式控制，同时维持了受限的刺激使用。同步钙成像揭示了所学策略的机制基础：智能体在空间和时间上优化刺激，利用局部网络拓扑和内在生理时间动态。这些结果确立了体外脑芯片培养物作为基于强化学习的神经调控的可处理跳板，并证明有效的控制策略可以从生物物理校准的数字孪生中推导并直接迁移到活体网络。

## Abstract
Controlling specific neuronal dynamics with electrical stimulation is critical for therapeutic neuromodulation, yet deriving optimal control policies remains challenging due to the complex and non-stationary nature of biological neuronal networks. While reinforcement learning (RL) offers a powerful closed-loop control framework, its reliance on prolonged stimulus-driven exploration is difficult to reconcile with the physiological limits of living tissue. Here, we demonstrate an in silico-to-in vitro transfer strategy that achieves efficient state-dependent control of network bursting in cultured neurons. The transferred policy outperforms heuristic controls, while maintaining constrained stimulation usage. Concurrent calcium imaging reveals the mechanistic basis of the learned policy: the agent optimizes stimulation spatially and temporally, exploiting local network topology and intrinsic physiological temporal dynamics. These results establish in vitro brain-on-chip cultures as a tractable stepping stone for RL-based neuromodulation and demonstrate that effective control policies can be derived in biophysically calibrated digital twins and transferred directly to living networks.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义

- **研究动机**：精准控制神经活动是神经科学和神经调控（如深部脑刺激、脑机接口）的核心挑战。生物神经网络（BNNs）具有非线性、非平稳性和状态依赖性，传统开环或简单闭环控制方法难以适应其动态变化。强化学习（RL）能通过交互学习最优策略，但其依赖大量探索性刺激，与活体组织的生理耐受性（如细胞疲劳、非平稳漂移）存在根本冲突。
- **核心问题**：如何在满足生物网络生理约束的前提下，高效获取并应用闭环控制策略？
- **整体含义**：作者提出一种“先训练后迁移”的混合方案：在生物物理校准的数字孪生（silico model）上预训练RL策略，再直接部署到体外培养的神经元网络（in vitro BNNs）上，实现状态依赖的爆发控制。该方法将数据密集的策略学习阶段转移到稳定、可重复的仿真环境，避免了在活体网络中进行长时间探索性刺激导致的网络疲劳。该工作为闭环神经调控提供了可操作的验证平台，并展示了数字孪生到活体网络的策略可迁移性，具有潜在的临床转化意义。

## 2. 提出的方法论：核心思想、技术细节、算法流程

- **核心思想**：将闭环神经调控问题形式化为一个**上下文多臂老虎机（contextual bandit）**问题：目标是在每个时间步，根据当前网络状态（上下文）选择最优的电刺激电极（动作），最大化立即诱发网络爆发（NB）的概率，同时最小化刺激使用次数。由于该问题为“贪婪”的，且电极效率随网络恢复状态非线性变化，作者采用**近端策略优化（PPO）**算法（折扣因子 γ=0），并修改Critic为Q值函数以区分动作效果。采用**策略蒸馏（policy distillation）**将多个仿真中训练的专业化策略（Specialist）聚合为一个通用策略（Generalist），使其具有跨网络泛化能力。
- **关键技术细节**：
  - **仿真环境**：基于NEURON构建了包含200个Hodgkin-Huxley神经元的生物物理模型（95%锥体神经元，5%PV+中间神经元），包含AMPA、NMDA、GABAA受体及短时突触可塑性（抑制与易化）。网络连接采用稀疏概率连接，模拟了虚拟电极记录和刺激。通过调整连接参数再现体外培养海马网络的自发放电统计指标（网络爆发率、间期、时长、同步性等）。
  - **状态表示**：状态向量 `s_t = [τ, w1, w2, ..., wE]`，其中τ是自上次NB以来经过的时间（归一化到最近5次NB间期的中位数）；`w_e`是电极e的权重，基于最近5次NB中每个电极上的尖峰时间（按指数衰减加权），以反映电极在网络爆发中的早发性（越早放电极权重越高），从而作为网络兴奋性和电极端耦合的代理。
  - **动作空间**：每个时间步（200 ms）选择一根电极（或空动作）施加单相阴极脉冲（−400 mV，200 μs）。200 ms的步长兼顾了神经元膜恢复和网络响应延迟。
  - **奖励函数**：成功诱发NB且刺激后100 ms内爆发 → +1；刺激但未诱发 → -0.25；不刺激且无NB → +0.25；不刺激但出现自发NB → -1。奖励函数鼓励有效刺激和正确等待，惩罚无效刺激和自发事件。
  - **策略蒸馏**：先用PPO在多个不同种子网络（每个50个）上在线训练Specialist策略（约248个episode收敛），收集所有状态-动作概率对，然后用KL散度损失训练一个单层32单元的MLP作为Generalist策略。该Generalist可零样本泛化到未见过的仿真网络，并能在网络切换（如从网络A切换到网络B）后5个episode内快速适应。
- **算法流程**（文字描述）：
  1. 构建生物物理校准的数字孪生模型，确保仿真与体外培养的五个关键指标（NBR、NBD、NIBI、NIBI CV、SYNC）在统计上匹配。
  2. 在多个仿真网络上分别训练Specialist RL agent（PPO with modified critic），记录每个网络的状态-动作对。
  3. 聚合所有Specialist的状态-动作对，通过策略蒸馏训练Generalist agent（监督学习最小化KL散度）。
  4. 将Generalist策略迁移到体外BNN，进行闭环控制实验，并在部分实验中同步钙成像以解析策略机制。

## 3. 实验设计：数据集、基准、对比方法

- **数据集/场景**：
  - **仿真数据**：50个独立网络实例（不同随机种子）用于训练Specialist；另外200个实例用于验证Generalist的泛化性能。
  - **体外数据**：胚胎（E18）大鼠海马神经元培养在微电极阵列（MEA，3×3=9电极）上，培养天数DIV17-42。共使用132个独立MEA记录（来自15批次生物制备），仅选用呈现自发爆发的培养孔进行实验。其中23个孔用于Protocol 1（对比在线学习），55个孔用于Protocol 2（对比启发式控制，包含5个同步钙成像）。
- **基准**：
  - Protocol 1：对比**在线学习（Specialist）**与**预训练Generalist**在体外网络上的控制效果。采用平衡交叉设计（先S后G或先G后S）以控制顺序效应。
  - Protocol 2：对比**Generalist**与两种**启发式控制**：
    - **Without Best**：排除Generalist阶段识别的最优电极，仅在其他电极上随机刺激（保持总刺激次数）。
    - **Random**：以与Generalist相同的平均速率随机选择电极和时间步施加刺激（破坏空间选择性）。
    - 此外，还以**自发基线（Baseline）**作为对照。
- **对比方法**：
  - 主要指标：网络爆发间期（NIBI）和刺激使用率（stims步数比例）。
  - 统计方法：非参数检验（Mann-Whitney U、配对置换检验、Friedman检验、Kendall相关），多重比较经Holm-Bonferroni校正。

## 4. 资源与算力

论文中**未明确说明**使用的GPU型号、数量、训练时长等具体算力信息。仅在方法部分提到：
- 仿真实验在NEURON环境下运行，使用Python实现，在Intel i7-6700 CPU、32 GB RAM的工作站上进行。
- 强化学习模型为单层32单元MLP，训练批大小为256，10个epoch，小批量64，学习率3e-4，训练量相对较小。
- 体外闭环控制系统为自研C#应用，延时<20 ms。
- 作者未提供任何GPU使用信息，推测所有计算均在CPU上完成。

## 5. 实验数量与充分性

- **实验数量**：
  - 仿真：Specialist训练使用999个seed（在线学习收敛分析），200个独立仿真用于Generalist泛化验证，50个仿真用于网络切换压力测试。
  - 体外：
    - Protocol 1：23个实验（来自多个批次），每个实验包含Spontaneous Baseline（3分钟）→ 两种策略（Generalist 1分钟 vs Specialist 10分钟）→ Final Baseline（3分钟）。
    - Protocol 2：55个实验（包含5个同步钙成像），顺序为：Baseline → Generalist（1分钟）→ Without Best（1分钟）→ Random（1分钟）→ Final Baseline（控制策略顺序随机化）。
    - 补充验证：3分钟连续Generalist无显著性能衰减，未发现顺序效应。
- **充分性与公平性**：
  - 样本量较大（仿真≥200，体外≥55），涵盖多批次、多天龄培养，具有一定代表性。
  - 设计了顺序控制（Protocol 1交叉设计，Protocol 2随机化），控制了疲劳和顺序效应。
  - 对比了在线学习（Specialist）和两种启发式控制（Without Best和Random），分别检验空间选择性和刺激速率的重要性。
  - 统计方法合理，使用非参数检验和多重比较校正。
  - 但Protocol 1中因在线学习后出现严重网络疲劳，导致顺序分析受损，作者承认这种比较存在混淆（Generalist在Specialist后表现下降）。Protocol 2中由于刺激总时长较短（约3分钟），疲劳轻微，比较更为公平。
  - 总体上，实验设计较为严谨，但仍有改进空间（如增加完全随机化策略的其他变体）。

## 6. 主要结论与发现

1. **数字孪生模型成功复现了体外海马网络的爆发表型**：五个黄金指标（NBR、NBD、NIBI、NIBI CV、SYNC）均落在实验观测范围，PCA分析显示模型捕获了电生理表型，可作为功能数字孪生。
2. **通过策略蒸馏训练得到的Generalist agent在仿真和体外均表现出优于Specialist和启发式控制的性能**：
   - 在仿真中，Generalist与Specialist在NIBI降低上效果相当，但刺激使用率更低，泛化性更强。
   - 在体外，Generalist显著优于Random和Without Best控制（p<0.05），在NIBI降低上表现最好，且刺激使用率与启发式方法相当（甚至更低）。
3. **在线学习存在严重生理限制**：在体外直接训练Specialist需要约5分钟刺激才能收敛，但已显著诱导“网络疲劳”（自发放电率下降，22%的培养孔在基线后完全沉默），导致后续比较受干扰。预训练Generalist避免了这一耗损。
4. **钙成像揭示了Generalist策略的机制**：
   - 电极的刺激效能强烈依赖于其40 μm半径内的活跃体细胞密度（Pearson r=0.72, p<0.05）。
   - 网络对刺激的响应具有空间特异性和时间传播模式（延迟可达100 ms），解释了200 ms步长的设定。
   - Generalist学会了利用局部网络拓扑：优先选择与神经元耦合紧密、能够快速引发网络爆发的电极；但当该电极被排除后，可快速通过其他冗余有效电极维持控制（解释了Without Best策略仍能取得一定效果）。
5. **网络身份是控制效果的主导因素**：不同培养孔的自发NIBI与所有刺激条件下的NIBI呈中等相关（τ=0.38-0.47），且不同策略下的NIBI排序高度相关（τ=0.64-0.71），表明内在网络特性（如不应期）设定了可达到的最大爆发率上限。

## 7. 优点

- **创新性**：首次在生物物理校准的数字孪生上预训练RL策略并成功迁移到体外神经网络，为闭环神经调控提供了可行的“先仿真后部署”范式，解决了RL样本效率与生物组织耐受性之间的矛盾。
- **方法论合理**：将问题形式化为上下文多臂老虎机，采用PPO（γ=0）与Q值Critic，适合当下贪婪目标。状态表示设计精巧，融合了时间和空间特征（归一化时间+电极权重），有效捕捉网络兴奋性。策略蒸馏实现了跨网络泛化，且能快速适应网络切换。
- **实验设计严谨**：包括多种对比（在线学习、两种启发式控制）、顺序控制、大小样本统计检验，并引入同步钙成像提供机制证据，解释策略行为。
- **临床转化潜力**：所提出的框架可扩展到更复杂的任务（如病理性振荡抑制、多群体调控），且与自适应深部脑刺激等场景的数据稀缺性和安全性约束高度一致。
- **开放共享**：代码、数据、模型均计划公开，符合FAIR原则。

## 8. 不足与局限

- **实验覆盖有限**：
  - 仅测试了网络爆发诱发这一单一目标，未探索抑制爆发、频率调谐或多目标控制。
  - 体外培养仅有9个电极（3x3网格），空间分辨率较低。该设置可能限制了策略的普适性，大型高密度MEA或in vivo场景仍需验证。
  - 同步钙成像数据仅5组，样本量小，结论的统计稳健性有限。
- **模型简化**：
  - 仿真模型采用了单室Hodgkin-Huxley神经元，忽略了真实形态和轴突激活；刺激模型基于Stoney关系假设球形激活区，可能低估了通过轴突激活远距离细胞的能力。作者承认此点，但与所用电极尺寸相符。
  - 仿真模型忽略了长期突触可塑性、稳态调节等非平稳过程，因此其稳定性高于体外，可能带来策略泛化的偏差。
- **比较公平性**：
  - Protocol 1中因网络疲劳导致顺序效应，Generalist在Specialist之后性能下降，削弱了直接对比。作者虽使用了顺序平衡设计，但两阶段刺激时长差异大（1 min vs 10 min），疲劳程度不对称，比较仍存在混淆。
  - Without Best策略先确定了最佳电极后再排除，可能存在数据窥探偏差；Random策略虽然匹配了总刺激率，但未匹配电极序列的统计结构（如时间相关性）。
- **未报告算力消耗**：无GPU使用情况，计算资源细节缺失，影响可复现性评估。
- **潜在偏差**：仅选用自发爆发的培养孔，可能排除了发育不良或过度抑制的样本，结论外推需谨慎。多个培养孔被重复记录（最多3次），虽然作者将其视为独立观测，但可能引入重复测量相关性。
- **临床应用距离**：体外培养物缺乏大脑的整体回路和神经调质系统，迁移到in vivo可能需要更复杂的数字孪生（包括全脑尺度）和更稳健的策略。

（完）
