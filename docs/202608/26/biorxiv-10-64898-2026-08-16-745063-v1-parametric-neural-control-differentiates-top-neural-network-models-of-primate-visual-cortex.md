---
title: Parametric neural control differentiates top neural network models of primate visual cortex
title_zh: 参数化神经控制区分灵长类视觉皮层的前沿神经网络模型
authors: "Prince, J. S., Wang, B., Fel, T., Jagadeesh, A. V., Vaziri, P. A., Alvarez, G. A., Livingstone, M. S., Konkle, T."
date: 2026-08-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.16.745063v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 参数化神经控制区分视觉皮层深度网络模型
tldr: 深度神经网络编码模型对视觉皮层反应的预测精度相近，但未必共享相同的脑对齐参数化。本文提出轴对齐特征强调方法，将模型编码轴转化为刺激扰动，在猕猴闭环实验中测试神经控制。结果显示模型间控制能力差异显著，对抗训练模型占优，且控制力与输入梯度的空间频率结构相关。这为评估模型与神经元的参数化一致性提供了因果方法。
source: biorxiv
selection_source: fresh_fetch
motivation: 尽管各模型自然图像预测精度相似，但其编码轴是否真正匹配神经元调谐尚不清楚，需要因果测试。
method: 提出轴对齐特征强调，将编码轴转化为分级刺激扰动，在猕猴视觉区域进行闭环实验。
result: 模型控制神经放电能力差异显著，对抗训练模型占优，且控制力与输入梯度空间频率结构相关。
conclusion: 轴对齐特征强调可作为因果方法，揭示模型与神经元参数化视觉世界的对齐程度。
---

## 摘要
领先的深度神经网络编码模型以几乎无法区分的精度预测视觉皮层反应，这强烈暗示这些模型已经收敛到相同的、与大脑对齐的自然图像空间参数化。在此我们证明情况并非如此。我们引入了轴对齐特征强调方法，将每个模型的拟合编码轴转换为分级的刺激扰动，这些扰动被预测能在自然图像范围内外参数化地控制神经放电。我们从十个前沿视觉模型生成了超过27,500个控制器刺激，并在针对早期、中期和高级视觉区域的闭环实验中将其呈现给五只猕猴。尽管自然图像预测性匹配，模型在使用强调刺激控制神经放电的能力上表现出巨大差异，揭示大多数模型的编码轴未能捕捉其对应神经元的精确调谐。两个对抗训练模型表现出一致的优势，尽管对抗鲁棒性在其他模型中对神经控制的预测性较弱。相反，控制效果更好地由输入梯度的空间频率结构预测：即影响每个编码轴的像素分布。总体而言，这些结果确立了通过轴对齐特征强调进行的神经控制作为一种因果方法，用于评估神经元和模型如何参数化视觉世界之间的对齐程度。

## Abstract
Leading deep neural network encoding models predict visual cortical responses with nearly indistinguishable accuracy, raising the strong inference that these models have converged on the same underlying brain-aligned parameterization of natural image space. Here we demonstrate that this is not the case. We introduce axis-aligned feature accentuation, which converts each model's fitted encoding axis into graded stimulus perturbations that are predicted to parametrically control neural firing within and beyond the natural-image range. We generated over 27,500 controller stimuli from ten leading vision models and presented them to five macaques in closed-loop experiments targeting early, mid-, and high-level visual areas. Despite matched natural image predictivity, models diverged strongly in their ability to control neural firing using accentuated stimuli, revealing that most model encoding axes failed to capture the precise tuning of their corresponding neurons. The two adversarially trained models showed a consistent advantage, though adversarial robustness was only weakly predictive of neural control across other models. Instead, control was better predicted by the spatial frequency structure of the input gradient: the distribution of pixels influencing each encoding axis. Overall, these results establish neural control via axis-aligned feature accentuation as a causal method to assess the alignment between how neurons and models parameterize the visual world.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 一、核心问题与整体含义（研究动机与背景）

- **核心问题**：当前多款领先的深度神经网络编码模型在预测灵长类视觉皮层神经反应上均有极高且几乎无法区分的精度，这容易让人误以为这些模型已经收敛到相同的、与大脑对齐的自然图像空间参数化。然而，预测精度相同并不能保证模型的内部参数化方式（编码轴）与真实神经元调谐一致。
- **研究动机**：需要一种因果性的测试方法，直接检验模型“如何参数化视觉世界”是否与神经元一致，而不只是比较预测分数。
- **整体含义**：本文提出并验证了一种新的因果评估方法——通过“轴对齐特征强调”（axis-aligned feature accentuation）产生的刺激来驱动神经放电，从而区分预测精度相似的模型，揭示模型与神经元在参数化视觉世界上的真实对齐程度。

## 二、方法论：核心思想、关键技术细节与流程

- **核心思想**：将每个模型拟合的编码轴（encoding axis）转化为分级的刺激扰动，这些扰动被预测能在自然图像范围之内和之外参数化地控制神经放电。
- **技术细节**：
  1. 首先为每个被试神经元的反应拟合一个线性映射（编码轴），将高维视觉刺激映射到预测的神经响应；
  2. 然后将这个编码轴的方向直接用于生成刺激扰动：在自然图像基础上沿编码轴方向逐步加强（或减弱）特征，得到一组“强调刺激”；
  3. 这组刺激被设计为能在预定方向上有参数化（graded）地改变神经放电率；
  4. 最终在猕猴的闭环实验中进行验证，即先预测、再施加刺激、再测量神经响应。
- **流程简述**：模型编码轴 → 生成控制器刺激（强调/减弱特征） → 闭环神经实验 → 比较预测与实际控制效果 → 评估模型与神经元的参数化一致性。

## 三、实验设计：数据集、场景与对比方法

- **控制器刺激生成**：从十个前沿视觉模型生成了超过 **27,500 个控制器刺激**。
- **实验对象与场景**：在 **五只猕猴** 上进行闭环实验，目标覆盖 **早期（early）、中期（mid-）和高级（high-level）视觉区域**。
- **Benchmark 设定**：以各模型在自然图像上的预测精度为基线（matched natural image predictivity），再比较它们在使用强调刺激时的神经控制能力。
- **对比方法**：
  - 五个模型之间相互对比控制能力；
  - 特别考察了 **对抗训练模型**（adversarially trained models）与其他模型的差异；
  - 进一步比较了“对抗鲁棒性”和“输入梯度空间频率结构”两个因素对神经控制效果的预测力。

## 四、资源与算力

- **原文未明确披露**：论文文本中没有给出具体的 GPU 型号、数量、训练时长、推理开销等算力信息。
- 仅可推测生成 27,500+ 控制器刺激和运行闭环实验需要相当的计算资源，但具体细节无法从本文内容获得。

## 五、实验数量与充分性

- **实验数量**：
  - 生成刺激：27,500+；
  - 实验对象：5 只猕猴；
  - 模型数量：10 个前沿视觉模型；
  - 覆盖脑区：早期、中期、高级视觉区域。
- **充分性评估**：
  - 实验规模较大，模型数量、刺激数量、被试数量和脑区覆盖均较充分；
  - 闭环实验设计提供了因果性证据，这是单纯预测性比较无法提供的；
  - 论文中涉及了对多种解释变量（对抗鲁棒性 vs 梯度空间频率）的比较，增加了结论的客观性；
  - 但从文本来看，没有提及详细的消融实验（如移除某一环节的影响），因此“充分性”上还有提升空间。

## 六、主要结论与发现

- **预测精度相似 ≠ 神经控制能力相似**：尽管在自然图像预测上表现几乎一样，模型在“用强调刺激控制神经放电”上的能力差异巨大。
- **大多数模型的编码轴未能捕捉神经元的精确调谐**：多数模型生成的控制器刺激不能有效驱动对应神经元。
- **两个对抗训练模型表现出一致性优势**：它们在神经控制上明显优于其他模型。
- **对抗鲁棒性并非关键预测因子**：对抗训练带来的优势并不能推广到其他模型的预测中，即对抗鲁棒性本身不能普遍预测神经控制效果。
- **真正预测控制效果的因素是输入梯度的空间频率结构**：即影响每个编码轴的像素分布（spatial frequency structure of the input gradient），而非简单的鲁棒性指标。
- **方法学贡献**：轴对齐特征强调被确立为一种因果性评估工具，可用于衡量神经元与模型间参数化视觉世界的对齐程度。

## 七、优点

- **因果性测试方法**：突破了传统仅依赖预测精度的评估范式，直接测试模型编码轴是否能因果性地驱动神经活动。
- **闭环实验设计**：在活体猕猴上验证预测，结论具有较高的生物学可信度。
- **多模型、多样化比较**：同时比较 10 个模型，覆盖面较广，并在多个视觉层次上进行评估。
- **引入了新的解释变量**：将输入梯度的空间频率结构作为预测变量，提供了更本质的机制性解释。

## 八、不足与局限

- **算力信息缺失**：未提供任何关于计算资源、训练时长等信息，可复现性和成本评估受限。
- **未提及消融实验**：对各设计要素（如刺激生成参数、编码轴拟合方法等）的影响缺乏系统分析。
- **物种与应用范围有限**：实验仅在猕猴上进行，是否能推广到人类或其他物种尚未验证。
- **对抗训练的优势机制仍未完全解释**：虽然发现对抗训练模型一致占优，但文中也承认对抗鲁棒性不能普遍预测控制效果，其优势的内在机制可能需要进一步研究。
- **刺激空间与自然图像的差异**：虽然刺激被设计为在自然图像范围内外均有效，但“范围外”刺激可能引入非自然特征，其生物学意义需谨慎解读。

（完）
