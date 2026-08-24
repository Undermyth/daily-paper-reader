---
title: Parametric neural control differentiates top neural network models of primate visual cortex
title_zh: 参数化神经控制区分灵长类视觉皮层的顶级神经网络模型
authors: "Prince, J. S., Wang, B., Fel, T., Jagadeesh, A. V., Vaziri, P. A., Alvarez, G. A., Livingstone, M. S., Konkle, T."
date: 2026-08-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.16.745063v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 利用轴对齐特征增强进行闭环神经控制，区分灵长类视觉皮层的深度网络模型，推进计算神经科学。
tldr: "领先的深度神经网络编码模型在预测猕猴视觉皮层活动上准确度几乎相同，但可能没有收敛到相同的大脑对齐表征。为了验证，作者引入轴对齐特征强调，将每个模型拟合的编码轴转化为刺激扰动，并生成超过27,500个控制器刺激，在五只猕猴的多个视觉区域进行闭环实验。结果显示，尽管自然图像预测力匹配，模型在神经控制上分歧很大，多数模型编码轴未捕捉精确调谐；其中对抗训练模型表现稳定优势，但控制效果更取决于输入梯度的空间频率结构。这一方法可作为因果测试，评估模型与神经元视觉参数化的一致性。"
source: biorxiv
selection_source: fresh_fetch
motivation: 尽管深度网络模型在自然图像上预测皮层反应几乎同样准确，但其编码轴是否真正反映神经元调谐尚未被因果验证。
method: 提出轴对齐特征强调，将各模型编码轴转化为参数化刺激扰动，并在猕猴多个视觉区进行闭环控制实验。
result: 模型在神经控制上显著分化，对抗训练模型有优势，但输入梯度空间频率结构更能预测控制效果。
conclusion: 轴对齐特征强调可作为因果方法，评估模型与神经元在视觉参数化上的对齐程度。
---

## 摘要
领先的深度神经网络编码模型以几乎无差别的准确率预测视觉皮层反应，这引发了强烈的推断：这些模型已收敛到相同的、与大脑对齐的自然图像空间参数化。在这里，我们证明事实并非如此。我们引入了轴向对齐特征强调，将每个模型的拟合编码轴转换为分级的刺激扰动，这些扰动被预测可在自然图像范围内外参数化控制神经放电。我们从十个领先视觉模型生成了超过27500个控制器刺激，并将其呈现给五只猕猴，在针对早期、中期和高级视觉区域的闭环实验中。尽管自然图像可预测性匹配，模型在通过强调刺激控制神经放电的能力上表现出强烈差异，揭示了大多数模型编码轴未能捕捉其对应神经元的精确调谐。两个对抗训练模型表现出一致的优势，尽管对抗鲁棒性在其他模型中对神经控制的预测仅较弱。相反，控制更好地由输入梯度的空间频率结构预测：影响每个编码轴的像素分布。总体而言，这些结果确立了通过轴向对齐特征强调的神经控制作为一种因果方法，用于评估神经元和模型如何参数化视觉世界之间的一致性。

## Abstract
Leading deep neural network encoding models predict visual cortical responses with nearly indistinguishable accuracy, raising the strong inference that these models have converged on the same underlying brain-aligned parameterization of natural image space. Here we demonstrate that this is not the case. We introduce axis-aligned feature accentuation, which converts each model's fitted encoding axis into graded stimulus perturbations that are predicted to parametrically control neural firing within and beyond the natural-image range. We generated over 27,500 controller stimuli from ten leading vision models and presented them to five macaques in closed-loop experiments targeting early, mid-, and high-level visual areas. Despite matched natural image predictivity, models diverged strongly in their ability to control neural firing using accentuated stimuli, revealing that most model encoding axes failed to capture the precise tuning of their corresponding neurons. The two adversarially trained models showed a consistent advantage, though adversarial robustness was only weakly predictive of neural control across other models. Instead, control was better predicted by the spatial frequency structure of the input gradient: the distribution of pixels influencing each encoding axis. Overall, these results establish neural control via axis-aligned feature accentuation as a causal method to assess the alignment between how neurons and models parameterize the visual world.

---

## 论文详细总结（自动生成）

## 论文总结

### 1. 论文的核心问题与整体含义
- **研究动机**：领先的深度神经网络编码模型在预测灵长类视觉皮层对自然图像的反应时，准确率几乎无法区分。这容易让人以为这些模型已经收敛到同一个与大脑对齐的自然图像空间参数化。作者怀疑这一推断的正确性。
- **核心问题**：尽管模型在自然图像上的预测性能相当，它们拟合出的“编码轴”是否真正与神经元的调谐特性一致？这需要因果验证，而不仅仅是预测相关性。
- **整体含义**：论文提出了一种因果测试方法，用于评估模型与神经元在“如何参数化视觉世界”上的对齐程度，从而区分表面上同等优秀的模型，并为计算神经科学中的模型选择提供新标准。

### 2. 论文提出的方法论
- **核心思想**：将每个模型拟合的编码轴（即模型中与某个神经元响应相关的特征方向）转换为分级的刺激扰动，通过刺激自然图像来参数化地控制神经元放电率。这样可以直接测试模型的编码轴是否对应神经元的真实调谐。
- **关键技术细节**：
  - **轴对齐特征强调**：针对每个模型的某个编码轴，计算该轴对输入像素的梯度，并沿梯度方向生成强调刺激。这些刺激在自然图像范围内或超出现有自然图像分布，以激发更强的目标神经元响应。
  - **闭环实验**：将生成的刺激实时呈现给受试动物，根据实际神经响应调整刺激参数，实现闭环优化。
  - **空间频率结构分析**：分析输入梯度的功率谱或空间频率分布，以确定哪些像素尺度对编码轴的影响最大。
- **算法流程（文字说明）**：
  1. 用自然图像数据拟合各编码模型的编码轴（映射到特定神经元的响应预测）。
  2. 对每个编码轴计算输入梯度，生成轴对齐的扰动信号。
  3. 将扰动叠加在基础自然图像上，生成一系列分级强调刺激。
  4. 在猕猴上进行闭环呈现，记录目标视觉区域的神经放电。
  5. 比较各模型在控制神经元放电上的有效性，并关联输入梯度特征。

### 3. 实验设计
- **数据集/场景**：
  - 受试动物：5只猕猴（macaca mulatta）。
  - 视觉区域：早期（early）、中期（mid-level）、高级（high-level）视觉皮层，覆盖从V1到IT等不同处理层级。
  - 刺激规模：超过27,500个控制器刺激，由10个领先视觉模型生成。
- **Benchmark**：
  - 所有模型在自然图像预测力（predictivity）上匹配，即先确认它们在传统编码任务上表现相当，再比较神经控制能力。
  - 主要基准是“能否通过强调刺激实际控制神经元放电率”。
- **对比方法**：
  - 10个领先视觉模型，其中包括两个对抗训练（adversarially trained）模型，其余为常规训练模型。
  - 比较不同模型之间的神经控制效果，并分析对抗鲁棒性、输入梯度空间频率结构等属性与控制效果的关系。

### 4. 资源与算力
- 论文文本中**未明确说明**使用的GPU型号、数量、训练时长或推理算力。
- 可能涉及大量刺激生成和模型梯度计算，但具体资源未在摘要中披露。如需了解，需查看论文完整正文。

### 5. 实验数量与充分性
- **实验数量**：规模较大——27,500+刺激，10个模型，5只动物，多个视觉区域，闭环实验。
- **消融与对照**：摘要中未提及传统消融实验（如移除某些模型组件），但通过比较多个模型和对照自然图像预测力，实现了模型间的公平比较。
- **充分性评价**：
  - 覆盖面较广，视觉区域分层多，动物数量合理，刺激数量充足。
  - 客观性较高：使用闭环神经控制作为直接因果指标，而非仅依赖相关性。
  - 公平性较好：先在自然图像预测力上匹配，再进行差异比较，降低了性能偏差。
- 不足之处可能在于：没有提及跨物种（如人类）验证，也没有说明是否测试了所有主流模型架构（如最近的大规模基础模型）。

### 6. 论文的主要结论与发现
- 尽管自然图像预测力匹配，模型在神经控制能力上表现出**强烈差异**，说明它们并未收敛到相同的大脑对齐参数化。
- 大多数模型的编码轴**未能捕捉对应神经元的精确调谐**，即通过强调刺激不能有效控制神经元放电。
- **两个对抗训练模型**表现出稳定优势，但对抗鲁棒性在其他模型中对神经控制的预测能力**较弱**，说明鲁棒性不是唯一决定因素。
- **输入梯度的空间频率结构**是更好的预测因子：控制效果的好坏取决于影响每个编码轴的像素在空间频率上的分布（例如，低频 vs 高频结构的匹配程度）。
- 总体确立了一种新的评估范式：**轴对齐特征强调的神经控制**作为因果方法，可区分模型的内部参数化是否与大脑对齐。

### 7. 优点
- **因果验证**：不同于传统编码模型只做预测相关性，该方法用刺激直接驱动神经活动，提供因果证据。
- **闭环设计**：实时调整刺激，增强实验敏感性和生态效度。
- **多层级覆盖**：包含早期到高级视觉区域，能检测模型在不同表征层级的对齐情况。
- **创新性分析**：引入输入梯度的空间频率结构，指出了一种解释模型可解释性的新维度。
- **公平比较**：先匹配自然图像预测力，消除了模型性能差异的干扰。

### 8. 不足与局限
- **资源信息缺失**：未提供算力、训练时长等细节，难以评估计算成本。
- **模型范围有限**：仅10个模型，且未明确列出具体架构，可能缺乏对最新大规模模型的覆盖。
- **物种局限**：实验仅在猕猴上进行，未验证在其他灵长类或人类上的可推广性。
- **刺激生成依赖梯度**：梯度扰动可能受模型输入边界、对抗攻击等因素影响，导致刺激不自然或不可控。
- **未讨论负结果的可解释性**：多数模型编码轴未能控制神经元，可能源于模型容量、训练数据或梯度噪声，但论文未深入分解原因。
- **预印本状态**：尚未经过同行评议，结论可能随审稿意见修改。

（完）
