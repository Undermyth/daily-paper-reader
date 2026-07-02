---
title: Uncovering internal states with a robust shared-state multi-neuron GLM-HMM framework
title_zh: 使用鲁棒的共享状态多神经元GLM-HMM框架揭示内部状态
authors: "Lawrence, A., Yezerets, E., Janak, P. H., Charles, A."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.27.734988v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 属于计算神经科学主题核心
tldr: 神经群体活动中的状态推断因数据稀疏和共线性极具挑战。本研究提出一种鲁棒的多神经元GLM-HMM框架，通过引入神经元自适应惩罚和信赖域算法改进EM过程，稳定地从群体尖峰序列中提取潜在状态。在多个灵长类和啮齿类决策任务数据集上验证，模型收敛且推断的状态具有行为相关性。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有状态推断方法未同时建模神经活动和行为，多神经元GLM-HMM面临稀疏、共线性和低试验次数的挑战。
method: 构建多神经元GLM-HMM，采用神经元自适应惩罚和信赖域算法的改进EM过程，并利用留一法交叉验证评估模型。
result: 在灵长类和啮齿类决策任务电生理数据上实现稳定收敛，推断状态具有行为相关性。
conclusion: 本框架克服了神经数据稀疏和共线性问题，能有效揭示内部状态与行为的关联。
---

## 摘要
神经系统表现出多种放电状态，这些状态反映生物体的内部状态，并调节外部环境刺激与行为之间的关系。已有研究通过使用带有非泊松行为观测的广义线性模型（GLM）补充传统隐马尔可夫模型（HMM）来推断这些潜在状态。然而，理解大脑内部状态与行为之间的关系还需要对神经活动进行建模。尽管如此，由于神经元数据集的高度稀疏性、共线性以及低试验次数，拟合多神经元GLM-HMM并非易事。因此，我们构建了一个鲁棒的多神经元GLM-HMM框架，该框架从群体活动中揭示潜在状态，同时纳入带有时间戳的任务变量和尖峰历史的影响。为了获得可靠的模型参数，我们采用了一种改进的期望最大化程序。具体而言，我们证明在最大化步骤中加入神经元自适应罚项能够克服时间戳事件和稀疏尖峰中典型的协变量共线性问题，从而得到泊松GLM系数的稳定估计。此外，我们引入信赖域算法，以确保在病态Hessian矩阵可能导致不稳定的牛顿-拉夫森更新的情况下实现稳定的M步收敛。我们进一步展示了留一交叉验证分析在评估低试验次数且不破坏时间结构的模型性能方面的实用性。我们通过对灵长类和啮齿类动物在执行决策任务时的三个电生理数据集进行评估，展示了稳定的模型收敛性，并讨论了推断状态的行为相关性。

## Abstract
Neural systems exhibit multiple firing states that reflect an organism's internal state and modulate the relationship between external environmental stimuli and behavior. Several studies have inferred these latent states by supplementing the traditional hidden Markov Model (HMM) with generalized linear models (GLMs) with non-Poisson behavioral observations. However, understanding the relationship between internal brain states and behavior also requires modeling the neural activity. Nonetheless, fitting multi-neuron GLM-HMMs is non-trivial due to high sparsity, collinearity, and low trial counts in neuronal datasets. Therefore, we built a robust multi-neuron GLM-HMM framework that uncovers latent states from population activity while incorporating the influence of time-stamped task variables and spike histories. To obtain reliable model parameters, we employ a modified expectation-maximization procedure. Specifically, we show that incorporating neuron-adaptive penalization in the maximization step overcomes the covariate co-linearity issues typical of time-stamped events and sparse spiking, yielding stable estimates of Poisson GLM coefficients. Furthermore, we incorporate a trust-region algorithm to ensure stable M-step convergence in the presence of ill-conditioned Hessians that can lead to unstable Newton-Raphson updates. We further demonstrate the utility of leave-one-out cross-validation analysis for evaluating model performance on datasets with low trial counts and without breaking their temporal structure. We evaluate our framework on three electrophysiological datasets from primates and rodents as they perform a decision-making task, demonstrate stable model convergence, and discuss the behavioral relevance of the inferred states.