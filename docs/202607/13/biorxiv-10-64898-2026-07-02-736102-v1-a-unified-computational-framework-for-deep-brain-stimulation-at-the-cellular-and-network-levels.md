---
title: A Unified Computational Framework for Deep Brain Stimulation at the Cellular and Network Levels
title_zh: 细胞和网络水平深部脑刺激的统一计算框架
authors: "Crompton, D. B., Milosevic, L., Lankarany, M."
date: 2026-07-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.02.736102v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 深度脑刺激调制尖峰活动的计算模型，纳入突触约束
tldr: 深部脑刺激（DBS）治疗机制不清，现有模型对微/中尺度电路激活刻画有限。本文提出统一现象学计算模型，整合实验验证的突触和细胞约束，研究电刺激对同质神经元群体放电的调节。关键发现：调节效果由刺激核团的内在特性、架构组织（连接强度与密度）及下游电路基序共同决定。该框架可集成至主流神经科学工具，为理解DBS在网络中的表示与传播提供机制，助力临床参数优化。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736102-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1324, \"height\": 578, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736102-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 777, \"height\": 400, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736102-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1268, \"height\": 315, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736102-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1330, \"height\": 1407, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736102-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1253, \"height\": 501, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736102-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1263, \"height\": 738, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736102-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1264, \"height\": 816, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736102-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1254, \"height\": 497, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-02-736102-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1176, \"height\": 1172, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-02-736102-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 405, \"height\": 374, \"label\": \"Table\"}]"
motivation: 现有DBS计算模型依赖纤维追踪或非生理电流注入，无法适应缺乏精细图谱的靶区，亟需统一且可扩展的仿真方法。
method: 提出现象学计算模型，整合实验约束，模拟刺激参数对同质神经元群体放电的调节，并开发编码器描述活动传播至下游网络的过程。
result: DBS调节效果取决于刺激核团的突触与细胞特性、架构组织（连接强度、密度）及后突触电路基序，不同架构产生不同编码模式与同步传播。
conclusion: 该统一框架适用于多种仿真工具，可整合细节模拟结果，为理解DBS机制和优化刺激参数提供理论与工具基础。
---

## 摘要
深部脑刺激已被证明是神经系统疾病成功的治疗干预手段，但其对神经元回路产生影响的机制仍不完全清楚。在本研究中，我们提出了一个全面的现象学计算模型，该模型考虑了电刺激参数对神经元回路的影响，同时整合了经过实验验证的突触和细胞约束。我们研究了DBS脉冲如何调节代表刺激核团的同质神经元群体中的放电活动，系统性地考察了回路架构的影响，包括突触连接强度（弱与强）和组织方式（稀疏与丰富）。为了表征DBS调节的神经活动如何通过下游网络传播，我们开发了一个简单的编码器，该编码器揭示了不同刺激核团架构配置所产生的不同编码模式。

此外，通过将刺激核团与递归连接的神经元群体相连，我们考察了DBS调节的神经元同步性在各种回路基序中的传播。我们的结果表明，三个关键因素塑造了DBS调节的神经活动：（a）刺激核团的内在突触和细胞特性，（b）刺激核团在突触强度和连接密度方面的架构组织，以及（c）由刺激核团的突触后靶标形成的回路基序。该统一模型为理解神经网络中DBS的表征和传播提供了一个机制性框架，其见解可能为临床应用中刺激参数的优化提供指导。

作者总结深部脑刺激的计算模型已被证明在厘清多种疾病治疗中观察到的临床获益和不良反应方面极为有用。尽管如此，许多现有计算模型解释微/中尺度回路激活的能力仍然有限，因为它们主要依赖于对DBS电极周围通路的详细表征，或依赖于非生理约束的注入电流来模拟电刺激的影响。基于通路的方法仅适用于我们已详细表征的通路，而对于许多靶标结构（如基底节）而言，这些表征是缺失的。鉴于当前方法的限制，我们着手定义一种现象学方法，该方法尽可能适用于多种模拟方法，包括那些缺乏纤维束成像细节的方法，同时能够在可用时轻松整合详细模拟的结果。我们的方法具有可扩展性，并且在一些最流行的计算神经科学工具包中提供了实现示例，从而能够轻松整合到现有的网络模拟中。此外，我们展示了该方法如何支持对网络进行生理响应以及计算动力学（如信息复用和延迟局部诱发电位）的探究。

## Abstract
Deep brain stimulation (DBS) has been demonstrated to be a successful therapeutic intervention for neurological disorders, yet the mechanisms underlying its effects on neuronal circuits remain incompletely understood. In this study, we propose a comprehensive phenomenological computational model that accounts for the impact of electrical stimulation parameters on neuronal circuits while incorporating experimentally-validated synaptic and cellular constraints. We investigate how DBS pulses modulate spiking activity in populations of homogeneous neurons representing stimulated nuclei, systematically examining the influence of circuitry architecture, including synaptic connectivity strength (weak vs. strong) and organization (sparse vs. rich). To characterize how DBS-modulated neuronal activity propagates through downstream networks, we develop a simple encoder that reveals distinct encoding patterns arising from different architectural configurations of stimulated nuclei.

Furthermore, by connecting stimulated nuclei to recurrently connected neuronal populations, we examine the propagation of DBS-modulated neuronal synchrony across various circuit motifs. Our results demonstrate that three critical factors shape DBS-modulated neuronal activity: (a) the intrinsic synaptic and cellular properties of stimulated nuclei, (b) the architectural organization of stimulated nuclei in terms of synaptic strength and connectivity density, and (c) the circuit motifs formed by postsynaptic targets of stimulated nuclei. This unified model provides a mechanistic framework for understanding DBS representation and propagation in neuronal networks, offering insights that may inform optimization of stimulation parameters for clinical applications.

Author summaryComputational models of deep brain stimulation have proven to be supremely useful in disentangling the clinical benefits and adverse effects observed in the treatment of a variety of conditions. Despite this, the capacity for many of the existent computational models to account for micro/meso-circuit activation remains limited, as the major techniques rely on detailed characterization of tracts surrounding the DBS electrode, or depend on an non-physiologically constrained injected current intending to mimic the influence of electrical stimulation. The tract based methods only work for tracts that we have detailed characterization of, which are missing for many of the target structures, such as the basal ganglia. Given the restrictions of current methods we set out to define a phenomenological method that is applicable to as many simulation methods as possible, including those with missing details on tractography, while being able to readily integrate results of detailed simulations when available. Our approach is extensible and has examples implemented in some of the most popular computational neuroscience toolkits allowing for ready integration into existing network simulations. Further we demonstrate how this methodology supports interrogation of networks both for physiological responses but also computational dynamics, such as information multiplexing and delayed local evoked potentials.

---

## 论文详细总结（自动生成）

# 论文结构化总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

深部脑刺激（DBS）在多种神经和精神疾病中显示疗效，但其对神经元回路的作用机制尚未完全阐明。现有计算模型主要分为两类：
- **详细生物物理模型**：高精度刻画电极、组织相互作用，但依赖完整的3D纤维结构表征（如基底节内纤维常缺乏精确追踪），且计算成本高，难以扩展到大规模网络。
- **抽象模型**：采用电流注入或速率函数简化DBS效应，计算高效，但会丢失关键特征（如逆向激活、轴突-胞体解耦、突触可塑性的影响）。

因此，论文旨在提出一种**统一的现象学计算框架**，能够在**不依赖精细纤维追踪**的情况下，模拟DBS对神经元群体在**细胞和网络水平**的调节效应，同时允许整合已有详细模拟结果，并兼容多种主流计算神经科学工具（NEST、BRIAN、NEURON）。

## 2. 论文提出的方法论

### 核心思想
将DBS的作用建模为**对突触的直接激活**，包括：
- **传出突触激活**（orthodromic efferent）
- **传入突触激活**（orthodromic afferent）
- **逆向激活与侧支激活**（antidromic/collateral）

通过向突触传递事件时间（spike times）来模拟DBS脉冲的影响，而不是向胞体注入电流。

### 关键技术细节
- **Parrot神经元**：在NEST等不支持直接向突触发送事件的模拟器中，在每条突触前插入一个“鹦鹉神经元”，它转发接收到的所有尖峰（包括生理性尖峰和DBS诱导的尖峰），保证DBS与正常放电可以融合。
- **招募概率与延迟**：
  - 每个DBS脉冲以一定概率（`p_eff`, `p_aff`, `p_anti`, `p_anti_eff`）招募特定突触。
  - 激活延迟 = 轴突传导延迟λ + 突触延迟δ，不同方向延迟组合方式不同（见图2）。
- **选择函数 `Choose`**：决定哪些神经元/突触被激活，可依赖体积激活组织（VAT）估计、电场二阶导数、纤维方向等，支持不同抽象层次。
- **与突触可塑性的结合**：直接作用于突触自然继承其短时程可塑性（STP，如Tsodyks-Markram模型），从而捕捉频率依赖性效应（如高频刺激时突触易化或抑制）。

### 算法流程（伪代码描述）
1. 定义网络拓扑（神经元及突触，每突触有λ和δ）。
2. 利用`Choose(Net)`确定被DBS招募的神经元子集 `Activated`。
3. 确定传出突触子集 `S_eff` 和传入突触子集 `S_aff`。
4. 对于每个DBS脉冲时间t：
   - 对 `S_eff`：以概率`p_eff`尝试招募，在 `t + λ + δ` 时激活突触。
   - 对 `S_aff`：以概率`p_aff`尝试招募，在 `t + δ` 时激活突触。
   - 对逆向激活：以概率`p_anti`尝试招募传入轴突，然后进一步以概率`p_anti_eff`招募与该轴突相连的其他突触，执行相应延迟计算。

### 公式
- LIF神经元模型（带突触电流和alpha核函数）。
- Tsodyks-Markram短时程可塑性模型（方程(4)-(7)），描述易化和抑制。

## 3. 实验设计

- **数据集 / 场景**：全部为模拟生成，无真实神经数据。构建了多种人工神经网络：
  - **前馈网络**（两个兴奋性群体，刺激-输出）。
  - **前馈+侧抑制**（兴奋性群体+抑制性中间神经元）。
  - **前馈+递归抑制**（抑制性连接在输出群体内形成反馈）。
- **参数扫描**：
  - 连接概率：0.10 ~ 1.00（10个值）
  - 突触强度：0.500 ~ 3.750（10个值）
  - 刺激频率：10 Hz, 50 Hz, 100 Hz
  - 刺激强度（招募比例）：低（20%）、高（80%）
  - 突触可塑性设置：易化型（U=0.001, τ_fac=50ms）或抑制型（U=1, τ_rec=50ms）
- **评估指标**：
  - 脉冲间期（ISI）内放电同步性（spike时空标准差）
  - ISI内峰值频率（>250 Hz的峰数）
  - 归一化速率编码（峰值幅度/基线率）
  - 局部场电位（LFP）代理信号的振荡特征
- **基准与对比**：论文未与其他DBS模拟方法（如电流注入法）进行定量对比；主要展示本框架在不同条件下的表现，而非benchmark比较。

## 4. 资源与算力

- **未明确说明**：文中没有提及使用的GPU型号、数量或训练时长。
- **模拟平台**：使用NEST模拟器，神经元模型为LIF（150或500个/群体）。所有实验均在标准CPU上进行，计算负担主要来自parrot神经元导致的尖峰传播开销。
- **规模讨论**：作者指出方法对网络大小不敏感（补充图显示从150扩展到500仍保持行为一致），但未给出具体运行时间。

## 5. 实验数量与充分性

- **实验数量**：进行了多组参数组合扫描（连接概率×突触强度=100个点，每个点重复？未说明重复次数）；频率与强度组合（2×3=6种）；三种回路基序；LFP振荡分析等。整体实验量较大。
- **充分性评价**：
  - **优点**：广泛覆盖了不同网络架构、突触可塑性设置和刺激参数，展示了方法的灵活性和现象丰富性。
  - **不足**：
    - 缺乏**统计重复和显著性检验**，结果仅以热图或示例raster呈现，未提供置信区间。
    - **没有消融实验**，例如将本方法与简单电流注入法对比，以证明其优势。
    - **缺乏真实数据验证**：所有结论均基于模拟，未与临床或电生理实验结果对照。
    - **参数敏感性问题**：部分现象（如LFP振荡）仅出现在特定参数组合，但未讨论参数鲁棒性。

## 6. 论文的主要结论与发现

1. **三个关键因素**共同决定DBS的神经调节效果：
   - 刺激核团的内在突触与细胞特性（如STP类型）。
   - 核团的架构组织（连接强度、连接密度）。
   - 下游突触后靶标形成的回路基序（前馈、侧抑制、递归抑制）。
2. **信息编码模式**因架构而异：前馈网络中，时间精确性编码和归一化速率编码呈现非单调关系，而纯速率编码单调增加。
3. **抑制性回路的稳定作用**：侧抑制和递归抑制改变了同步性对连接参数的依赖，局部和全局最优值移动。
4. **LFP振荡**可由高频高强度DBS诱发，受短时程易化调节；延迟局部诱发电位（DLEP）随刺激参数变化。
5. 方法**可扩展**：可集成到NEST、BRIAN、NEURON等模拟器，并兼容VAT等外部纤维激活估计。

## 7. 优点

- **通用性强**：不依赖精细纤维追踪，适用于基底节内等缺乏详细通路表征的脑区。
- **生理学约束**：直接激活突触，自动继承突触可塑性、延迟、失败等特性，比电流注入更接近真实机制。
- **可扩展性**：用户可根据需求调整`Choose`函数，集成电场模型或详细纤维模拟结果。
- **计算可行**：与详细生物物理模型相比，计算成本低得多，可研究大规模网络动态。
- **明确算法接口**：给出伪代码和示意图，易于复现和集成。
- **开源工具示例**：在NEST中提供parrot神经元实现，降低使用门槛。

## 8. 不足与局限

- **亚阈值效应缺失**：未考虑DBS对胞体静息电位的亚阈值调制（可能影响兴奋性）。
- **招募计算依赖用户**：`Choose`函数需要用户自行基于VAT或电场模型定义，引入额外假设。
- **计算开销**：parrot神经元增加事件传递数量，在大型网络（数千神经元）中可能显著降低速度。
- **未与传统方法对比**：缺少与详细生物物理模型或电流注入法的定量比较，优势论证偏定性。
- **缺乏真实数据验证**：所有结果基于合成网络，能否预测实际DBS临床效果未验证。
- **参数空间探索有限**：仅测试了LIF神经元和alpha突触，对更真实神经元模型（如Hodgkin-Huxley）和复杂突触可塑性（如STDP）的兼容性未展示。
- **实验重复性**：未说明每次参数组合的重复次数，热图颜色是否代表单次还是平均结果未知。
- **可重现性**：虽然提到代码共享，但文中未提供具体仓库链接或完整配置。

（完）
