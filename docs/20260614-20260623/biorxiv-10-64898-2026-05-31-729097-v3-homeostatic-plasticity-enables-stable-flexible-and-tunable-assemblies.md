---
title: "Homeostatic Plasticity Enables Stable, Flexible, and Tunable Assemblies"
title_zh: 稳态可塑性实现稳定、灵活且可调的神经集合
authors: "Miller, M. C., Miehl, C., Doiron, B."
date: 2026-06-22
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.31.729097v3.full.pdf"
tags: ["query:comp-neuro"]
score: 9.0
evidence: 突触可塑性与稳态可塑性在神经集群形成中的作用
tldr: 传统Hebbian可塑性模型通常导致二元组装结果，即网络要么无组装要么最强连接。本文引入抑制性稳态可塑性，使兴奋-兴奋突触的可塑性在稳态目标发放率下平衡，从而在突触权重空间中形成线吸引子连续谱。该连续谱下神经元发放率保持恒定，但网络动态响应特性（如增益和时间尺度）可连续调节。该工作提供了基于稳态的可调灵活组装学习框架，克服了二元性限制。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统Hebbian可塑性导致二元组装结果，缺乏灵活性和可调性。
method: 结合稳态抑制可塑性与Hebbian可塑性，平衡兴奋性神经元在目标发放率下的增强与抑制。
result: 突触强度形成线吸引子连续谱，发放率不变但网络增益和时间尺度可调。
conclusion: 提供基于稳态的可调灵活组装学习框架，克服二元性，实现连续可调网络动态。
---

## 摘要
通过突触可塑性机制动态形成的强互连神经元群体，称为神经集合，被认为是大脑中记忆的基础。许多集合形成模型使用赫布型兴奋-兴奋可塑性，其中协调活动加强了递归结构。然而，这些模型通常产生二值化的集合结果：具有弱连接（无集合）或最强连接（有集合）的网络。我们考虑结合赫布型兴奋-兴奋可塑性和抑制-兴奋突触可塑性的网络，后者通过稳态方式将兴奋性神经元的放电稳定在目标值。当我们设置兴奋-兴奋可塑性为稳态顺从型，即在稳态目标放电率下增强和抑制达到平衡时，我们发现突触强度存在稳定的连续统，集合结构不再是二值的。我们使用尖峰神经元模型的递归网络和相关的平均场理论来识别这个连续统为突触权重空间中的线吸引子。沿吸引子，稳态确保神经元放电率不变，但网络的动态响应特性相当可塑，强耦合网络具有高增益和更长时间的响应。通过我们的平均场理论，我们展示了兴奋性神经元之间的相关随机尖峰活动如何破坏线吸引子，但当相关输入在兴奋性和抑制性神经元之间共享时，这种破坏可以得到缓解。总之，我们提供了一种基于稳态的替代学习框架，其中可实现可调且灵活的集合结构。

## Abstract
Strongly interconnected neuronal populations, called assemblies, dynamically form through synaptic plasticity mechanisms and are thought to be a substrate for memories in the brain. Many assembly formation models use Hebbian excitatory-to-excitatory plasticity, where coordinated activity strengthens recurrent structure. However, these models typically yield binary assembly outcomes: networks with either weak (no assembly) or maximally strong (assembly) connectivity. We consider networks with a combination of Hebbian excitatory-to-excitatory plasticity and inhibitory-to-excitatory synapses with plasticity that homeostatically stabilizes excitatory neuron firing at a target value. When we set excitatory-to-excitatory plasticity to be homeostatically compliant, in that potentiation and depression are balanced at the homeostatic target firing rate, we find a stable continuum of synaptic strengths, and assembly structure is no longer binary. We use a recurrent network of spiking neuron models and an associated mean-field theory to identify this continuum as a line attractor in synaptic weight space. While along the attractor, homeostasis ensures that neuronal firing rates are invariant, the dynamical response properties of the network are quite malleable, with strongly coupled networks having high gain and longer timescale responses. Using our mean-field theory we show how correlated stochastic spiking activity among the excitatory neurons can destroy the line attractor, yet this can be mitigated when correlated inputs are shared across the excitatory and inhibitory neurons. Altogether, we provide an alternative learning framework based on homeostasis, where a tunable and flexible assembly structure is possible.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：传统Hebbian可塑性（E→E）在递归网络中会导致不稳定的二元结构——要么弱连接（无集合），要么最强连接（集合）。这种二元性限制了神经集合对经验强度进行灵活编码的能力。
- **研究动机**：大脑中的神经集合需要通过突触可塑性形成稳定但可调的回路，以支持记忆、学习和行为。现有模型通常依赖硬阈值或权重归一化来稳定，导致集合强度只有“有/无”两种状态，缺乏连续可调性。
- **整体含义**：本文提出将抑制性稳态可塑性（I→E）与“稳态顺从型”兴奋可塑性（E→E）结合，可以在突触权重空间中产生一条“线吸引子”（line attractor）。沿该吸引子，神经元发放率保持恒定，但网络动态响应特性（增益、时间尺度、变异性等）连续可调。这为神经集合编码提供了一个更灵活、更自然的框架。

## 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

### 2.1 核心思想
- 使用抑制性稳态可塑性（I→E）将兴奋性神经元发放率稳定在目标值 \(b\) 附近（如20Hz）。
- 兴奋可塑性（E→E）设置为“稳态顺从型”：即当 \(r_E = b\) 时，增强和抑制恰好平衡，无净权重变化。
- 当两者结合时，\((\bar{w}_{EE}, \bar{w}_{EI})\) 形成一条连续平衡的线吸引子。

### 2.2 关键技术细节
- **网络模型**：递归兴奋-抑制（EI）网络，各含500个神经元（\(N_E = N_I = N_X = 500\)），使用Hawkes过程生成尖峰。突触核函数为指数衰减，时间常数 \(\tau_E=8\)ms, \(\tau_I=16\)ms。
- **可塑性规则**：基于STDP，可塑性方程：
  \[
  \tau_{w\alpha} \frac{dw^{E\alpha}_{ij}}{dt} = \frac{1}{2}(x_i^E S_j^\alpha + x_j^\alpha S_i^E) - b_{E\alpha} \tau_p S_j^\alpha
  \]
  其中 \(x\) 为资格迹，\(\tau_p\) 为STDP时间尺度（120ms），\(b_{E\alpha}\) 为LTD系数。
- **稳态顺从条件**：\(b_{EE} = b_{EI} = b\)，即两种可塑性的LTD阈值相等。
- **平均场理论**：利用快-慢时间尺度分离，推导出平均场速率动力学和权重动力学方程：
  - 速率：\(\vec{\tau}_r \frac{d\vec{r}}{dt} = -\vec{r} + \mathbf{W}\vec{r} + \mathbf{W}_X \vec{r}_X\)
  - 权重：\(\tau_{wE} \frac{dw_{EE}}{dt} = \tau_p r_E (r_E - b)\)，\(\tau_{wI} \frac{dw_{EI}}{dt} = \tau_p r_I (r_E - b)\)
  - 固定点：当 \(r_E = b\) 时，\(w_{EI}^* = \frac{w_{II}(b w_{EE}^* + a_E w_{EX})}{b w_{IE} + a_I w_{IX}}\)，即一条直线。
- **线吸引子稳定性条件**：
  1. \(w_{II} < \sqrt{\frac{\tau_{wE}}{\tau_{wI}}} w_{IE}\)（总是稳定），或
  2. \(b < b_{\max} = \frac{w_{IX} a_I}{\sqrt{\tau_{wE}/\tau_{wI}} w_{II} - \sqrt{\tau_{wE}/\tau_{wI}} w_{IE}}\)（有条件稳定）。
- **相关性与漂移**：引入Ornstein-Uhlenbeck噪声模拟共享波动，权重漂移通过积分STDP核与尖峰交叉谱的卷积描述；E-I共享相关（\(c_X\)）可抵消漂移。

### 2.3 流程概要
1. 初始化网络权重，运行尖峰模拟（Hawkes过程）。
2. 计算平均场参数，求解速率固定点。
3. 在权重空间中找到线吸引子，分析其稳定性和吸引域。
4. 施加外部扰动或相关噪声，测量响应能量、衰减时间、平衡指数、信噪比等。
5. 调整E-I共享相关性，验证其对漂移的抑制效果。

## 3. 实验设计：数据集、场景与对比方法

### 3.1 数据集与场景
- **无真实数据集**：全部基于理论模型和数值模拟（Hawkes过程网络）。
- **主要场景**：
  - 不同初始权重（\(\bar{w}_{EE}\)）的权重演化实验。
  - 给网络施加2ms单脉冲扰动，测量动态响应。
  - 重复刺激学习协议（0.2Hz频率给予30ms脉冲）观察权重生长。
  - 部分刺激（20%E神经元）测试模式完成。
  - 引入共享OU噪声，测量相关性对权重漂移的影响。
  - 对比不同\(c_X\)（E-I共享比例）的抑制漂移效果。

### 3.2 基准与对比方法
- **基线**：无稳态可塑性的纯Hebbian E→E塑性（导致二元结果）。
- **对比规则**：
  - 非对称STDP（因果）规则。
  - 三叉STDP规则（triplet STDP）。
  - 动态阈值可塑性规则（\(\tau_b db/dt = r_E - b\)）。
- **方法对比**：直接模拟尖峰网络 vs 平均场理论预测。

### 3.3 是否对比了其他方法
- 是，比较了不同STDP变体（对称、非对称、三叉）以及不同参数（\(w_{IE}\)、\(b\)等）下的行为，验证了线吸引子的存在条件。

## 4. 资源与算力

- **文中未明确提及使用的GPU型号、数量或训练时长**。
- 仅给出了模拟参数：dt=0.1ms，模拟时间通常20-80秒（图2-8），每个实验重复15-20次，总计算量中等。
- 使用Python（推测）进行模拟，未说明硬件。考虑到500神经元网络和平均场计算，对算力要求不高。

## 5. 实验数量与充分性

### 5.1 实验数量
- **图2**：不同初始权重（约5条曲线）、线吸引子拟合（\(r^2=0.99\)）。
- **图3**：沿吸引子不同位置（约10个点）测量能量、衰减时间、平衡指数、方差、模式完成等。
- **图5**：对稳定性条件进行参数扫描（\(w_{IE}, w_{II}, b\)），包括吸引域可视化。
- **图6**：沿吸引子的动态响应指标（理论 vs 模拟）对比，包括SNR。
- **图7-8**：不同噪声强度（\(\sigma_\eta\)）和共享比例（\(c_X\)）下的漂移实验（多个参数值）。
- 总量约几十组模拟实验，覆盖主体结论。

### 5.2 充分性与客观性
- **充分性**：实验设计系统，从发现线吸引子到分析其响应特性，再到相关性扰动与对策，逻辑链条完整。
- **客观性**：理论预测与模拟结果高度一致（如能量、衰减时间等对比良好），统计显著性通过误差带/标准差展示。
- **公平性**：对比不同规则时采用了相同网络结构与参数，公平合理。

## 6. 论文的主要结论与发现

1. **稳态顺从型可塑性产生连续吸引子**：当 \(b_{EE}=b_{EI}\) 时，\((\bar{w}_{EE}, \bar{w}_{EI})\) 在权重空间中形成一条稳定的线吸引子，集合强度可调。
2. **发放率不变但动态可调**：沿吸引子，平均发放率保持恒定（\(r_E^*=b\)），但增益、响应能量、衰减时间、变异性、信噪比等动态特性连续变化。
3. **学习可作为沿着吸引子的“棘轮”**：重复刺激可使权重沿吸引子向上移动，形成强集合。
4. **相关尖峰活动破坏线吸引子**：共享外部波动导致E→E相关性，引起正向权重漂移，最终导致不稳定。
5. **E-I共享相关可缓解漂移**：将相关性在E和I外部输入中共享（\(c_X\)接近1），可抵消漂移，恢复近似异步状态。

## 7. 优点

1. **理论创新**：提出了“稳态顺从型可塑性”这一新概念，并利用线吸引子统一理解稳态与Hebbian可塑性的交互。
2. **数学完备性**：建立了从微观STDP到平均场权重动力学的完整推导，给出了线吸引子的存在条件和稳定性分析（包括特征边界）。
3. **动态视角**：揭示了即使发放率恒定，网络动态响应仍可连续变化，为“相同活动、不同处理”提供了机制解释。
4. **实用性洞察**：识别出相关噪声引起的漂移问题，并提出了E-I共享相关作为生物合理的解决方案（如皮层中常见的共同抑制性输入）。
5. **实验验证**：平均场预测与尖峰网络模拟高度匹配，验证了理论的正确性。

## 8. 不足与局限

1. **实验覆盖有限**：所有模拟基于相同大小的网络（500神经元），未测试不同网络规模或更现实的稀疏连接结构。
2. **未考虑多个集合的交互**：论文仅研究单一集合（全E种群作为集合），实际大脑中多个集合同时存在并相互作用（如模式分离）。
3. **忽略了突触可塑性的生物学细节**：未包含短期可塑性、异突触可塑性、多时间尺度稳态等更复杂因素，可能影响结论的普适性。
4. **线吸引子稳定性对参数敏感**：条件（如 \(w_{II} < \sqrt{\frac{\tau_{wE}}{\tau_{wI}}} w_{IE}\)）需要精细调节，实际生物网络中是否自然满足存疑。
5. **未涉及学习后遗忘或退化**：论文展示的学习是单向增强，未探讨长期记忆维持或衰退的动力学。
6. **相关漂移的缓解仅理论验证**：E-I共享相关方案在真实皮层中的具体实现和有效性需进一步实验支持。
7. **无真实神经数据验证**：所有结论来自模型模拟，缺乏与电生理或成像数据的定量比较。

（完）
