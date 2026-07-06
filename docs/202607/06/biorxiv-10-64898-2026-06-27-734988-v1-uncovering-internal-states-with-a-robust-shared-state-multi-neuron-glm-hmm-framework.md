---
title: Uncovering internal states with a robust shared-state multi-neuron GLM-HMM framework
title_zh: 使用鲁棒的共享状态多神经元GLM-HMM框架揭示内部状态
authors: "Lawrence, A., Yezerets, E., Janak, P. H., Charles, A."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.27.734988v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 多神经元GLM-HMM框架用于神经状态推断
tldr: 神经群体活动存在反映内部状态的多个发放状态，但传统GLM-HMM难以适应神经数据的高稀疏性和共线性。本文构建了一个鲁棒的多神经元GLM-HMM框架，采用神经元自适应惩罚和信任区域算法改进EM估计，稳定获取Poisson GLM系数。在灵长类和啮齿类决策任务电生理数据上，模型收敛稳定，并揭示了与行为相关的潜在状态。该框架为从神经群体活动推断内部状态提供了可靠方法。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有GLM-HMM通常仅用于行为数据，难以直接拟合高稀疏、低试验次数的神经数据，缺乏鲁棒的参数估计方法。
method: 构建多神经元GLM-HMM，在EM最大化步骤中加入神经元自适应惩罚处理共线性，采用信任区域算法确保Hessian病态时稳定收敛。
result: 在三个灵长类和啮齿类决策任务电生理数据集上，模型稳定收敛，推断的状态具有行为相关性。
conclusion: 提出的鲁棒拟合框架有效克服了神经数据稀疏性和共线性挑战，能够从群体活动中提取有意义的内部状态。
---

## 摘要
神经系统表现出多种放电状态，这些状态反映了生物体的内部状态，并调节外部环境刺激与行为之间的关系。已有研究通过在传统隐马尔可夫模型（HMM）中补充广义线性模型（GLM）并引入非泊松行为观测，推断这些潜在状态。然而，理解大脑内部状态与行为之间的关系还需要对神经活动进行建模。尽管如此，由于神经数据集的高度稀疏性、共线性和低试验次数，拟合多神经元GLM-HMM并非易事。因此，我们构建了一个鲁棒的多神经元GLM-HMM框架，该框架从群体活动中揭示潜在状态，同时纳入带时间戳的任务变量和尖峰历史的影响。为了获得可靠的模型参数，我们采用了一种改进的期望最大化程序。具体而言，我们表明在最大化步骤中引入神经元自适应惩罚能够克服时间戳事件和稀疏放电典型存在的协变量共线性问题，从而获得泊松GLM系数的稳定估计。此外，我们引入信赖域算法，以确保在病态海森矩阵可能导致牛顿-拉夫逊更新不稳定的情况下，M步能够稳定收敛。我们还展示了留一法交叉验证分析在评估低试验次数数据集模型性能且不破坏其时间结构方面的实用性。我们在灵长类和啮齿类动物执行决策任务时的三个电生理数据集上评估了我们的框架，证明了模型的稳定收敛，并讨论了推断状态的行为相关性。

作者总结：神经系统随时间演化：不仅单个神经元在整个网络中相互影响，而且当动物进入不同行为（例如专注 vs. 游离）或状态（例如饥饿或疲劳）时，网络及其连接本身也会发生变化。因此，分析指导行为的神经活动必须考虑大脑的时变特性。最近的建模工作扩展了流行的广义线性模型（该模型可将任务和行为与记录的神经动作电位联系起来），纳入了一个隐马尔可夫模型。这种扩展使得生成的GLM-HMM能够表现出多种不同的关系（不同的GLM），这些关系随时间切换，以解释动物的变化模式。尽管GLM-HMM已广泛用于行为数据（例如决策范式中的任务选择），但由于神经数据样本量更小、活动更稀疏、参数空间更大，其应用困难得多。我们的工作提出了一种新的拟合方法和最佳实践，以鲁棒地将GLM-HMM拟合到神经数据。通过将GLM-HMM鲁棒地拟合到多种神经数据集的众多应用，我们证明可以识别神经活动的重要特征，从而更好地理解其与行为的关系。

## Abstract
Neural systems exhibit multiple firing states that reflect an organisms internal state and modulate the relationship between external environmental stimuli and behavior. Several studies have inferred these latent states by supplementing the traditional hidden Markov Model (HMM) with generalized linear models (GLMs) with non-Poisson behavioral observations. However, understanding the relationship between internal brain states and behavior also requires modeling the neural activity. Nonetheless, fitting multi-neuron GLM-HMMs is non-trivial due to high sparsity, collinearity, and low trial counts in neuronal datasets. Therefore, we built a robust multi-neuron GLM-HMM framework that uncovers latent states from population activity while incorporating the influence of time-stamped task variables and spike histories. To obtain reliable model parameters, we employ a modified expectation-maximization procedure. Specifically, we show that incorporating neuron-adaptive penalization in the maximization step overcomes the covariate co-linearity issues typical of time-stamped events and sparse spiking, yielding stable estimates of Poisson GLM coefficients. Furthermore, we incorporate a trust-region algorithm to ensure stable M-step convergence in the presence of ill-conditioned Hessians that can lead to unstable Newton-Raphson updates. We further demonstrate the utility of leave-one-out cross-validation analysis for evaluating model performance on datasets with low trial counts and without breaking their temporal structure. We evaluate our framework on three electrophysiological datasets from primates and rodents as they perform a decision-making task, demonstrate stable model convergence, and discuss the behavioral relevance of the inferred states.

Author SummaryNeural systems evolve over time: not only do the individual neurons influence each other across the network, but the network and interconnections themselves change as an animal enters different behaviors (e.g., attentive vs. disengaged) or states (e.g., hungry or tired). Analyzing the neural activity that guides behavior thus must incorporate the time-varying nature of the brain. Recent modeling work has extended the popular Generalized Linear Model, a model that can connect task and behavior to recorded neural action potentials, to incorporate a latent Hidden Markov Model. This extension allows the resulting GLM-HMM to exhibit several different relationships (different GLMs) that are switched between over time to account for the animals changing patterns. While GLM-HMMs have been applied extensively on behavioral data (e.g., task choice in a decision making paradigm), neural data is much more difficult due to the smaller sample sizes, sparser activity, and larger parameter space. Our work presents a new fitting approach and best practices to robustly fit GLM-HMMs to neural data. We demonstrate through numerous applications to a variety of neural datasets that by robustly fitting GLM-HMMs to data, we can identify important features of neural activity that let us better understand its relationship to behavior.