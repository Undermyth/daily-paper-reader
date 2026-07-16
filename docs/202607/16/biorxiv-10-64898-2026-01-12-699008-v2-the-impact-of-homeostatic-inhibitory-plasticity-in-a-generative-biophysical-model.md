---
title: The impact of homeostatic inhibitory plasticity in a generative biophysical model
title_zh: 稳态抑制可塑性在生成性生物物理模型中的影响
authors: "Mindlin, I., Coronel-Oliveros, C., Llabres, M., Sitt, J. D., Cofre, R., Luppi, A., Andrillon, T., Sanz Perl, Y., Herzog, R."
date: 2026-07-16
pdf: "https://www.biorxiv.org/content/10.64898/2026.01.12.699008v2.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 生物物理模型中的稳态抑制性可塑性
tldr: 大脑通过突触可塑性和稳态调节动态适应环境。该研究将抑制性稳态可塑性规则嵌入动态平均场模型，构建稳态动态平均场模型，动态调节局部兴奋-抑制平衡。模型能复现脑活动统计特征，无需额外计算即可承受神经调节扰动，并产生类似睡眠的慢波活动及与清醒异步动力学共存的状态，可用于研究局部适应过程如何塑造全脑动态。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-12-699008-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1608, \"height\": 931, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-12-699008-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1648, \"height\": 1317, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-12-699008-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1622, \"height\": 1788, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-12-699008-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1622, \"height\": 1981, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-12-699008-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1614, \"height\": 1737, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-01-12-699008-v2/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1646, \"height\": 1796, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-01-12-699008-v2/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1333, \"height\": 1765, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-01-12-699008-v2/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1354, \"height\": 778, \"label\": \"Table\"}]"
motivation: 现有生成性生物物理模型缺乏稳态可塑性，难以捕捉大脑的动态自适应能力。
method: 将抑制性稳态可塑性规则嵌入动态平均场模型，构建稳态动态平均场模型，动态调节兴奋-抑制平衡。
result: 模型复现脑活动统计特征，产生睡眠样慢波活动，并能与清醒异步动力学共存。
conclusion: 单一稳态规则扩展了动态平均场模型的稳定性和表现力，为研究局部适应过程塑造全脑动态提供统一平台。
---

## 摘要
生物系统的一个主要特征是它们能够动态适应环境变化。在大脑中，突触可塑性使神经元之间的连接得以增强或减弱，从而使神经回路能够根据经验、学习和环境变化进行调整。然而，这种可塑性受到稳态调节，以避免突触连接的过度增殖。这些机制可以通过大规模的大脑活动模型进行研究。在这里，我们将一个生物学基础的抑制性稳态可塑性规则嵌入动态平均场（DMF）模型中，创建了一个稳态动态平均场（HDMF）模型，该模型动态调节局部兴奋-抑制平衡。通过将大范围的耦合强度映射到抑制性突触的参数上，实现了兴奋性发放率的收敛。HDMF再现了大脑活动的统计观测值以及原始DMF，并且可以在没有额外计算的情况下维持神经调节扰动。HDMF可以产生前所未有的类似睡眠的慢波活动，这种活动也可以与类似清醒的异步动态共存，从而可以模拟分离的意识状态，如异态睡眠。这些结果共同表明，单一的稳态规则拓宽了DMF的稳定性和表现力，为研究局部适应过程如何塑造人脑多样化的全局动态提供了一个统一的平台。

## Abstract
A main characteristic of biological systems is their capacity to dynamically adapt to environmental changes. In the brain, synaptic plasticity enables the strengthening or weakening of connections between neurons, allowing neural circuits to adapt based on experience, learning, and environmental changes. Yet, it is homeostatically regulated such that it avoids excessive proliferation of synaptic contacts. These mechanisms can be studied with large-scale models of brain activity. Here, we embed a biologically grounded inhibitory homeostatic plasticity rule into the Dynamic Mean Field (DMF) model, creating a Homeostatic Dynamic Mean Field (HDMF) model that dynamically tunes local excitation-inhibition balance. Convergence of excitatory firing rates is reached by mapping a large range of coupling strength to parameters of inhibitory synapses. The HDMF reproduces statistical observables of brain activity as well as the original DMF, and can sustain neuromodulatory perturbations without overhead computations. The HDMF can generate unprecedented sleep-like slow-wave activity, which can also coexist with wake-like asynchronous dynamics, permitting to model dissociated states of consciousness such as parasomnias. Together, these results show that a single homeostatic rule broadens the stability and expressiveness of the DMF, providing a unified platform for studying how local adaptive processes shape the diverse global dynamics of the human brain.

---

## 论文详细总结（自动生成）

好的，作为一名资深学术论文分析助手，以下是对您提供的论文的详细、结构化与深入的中文总结。

---

### **论文核心总结：《稳态抑制性可塑性在生成性生物物理模型中的影响》**

#### **1. 论文的核心问题与整体含义（研究动机和背景）**

*   **研究动机**：大脑的显著特征之一是其能够适应环境变化，这种适应性部分源于突触可塑性。然而，这种可塑性必须受到稳态调节，以防止神经活动过度亢进或抑制，从而维持健康的兴奋-抑制（E/I）平衡。现有的全脑模型，如动态平均场（DMF）模型，虽然能模拟多种脑状态，但其通常依赖于静态的反馈抑制控制（FIC）参数或繁复的参数搜索，缺乏一个统一的、动态的、生物合理的稳态调节机制。
*   **核心问题**：如何在一个生物物理生成模型中嵌入一种稳态机制，使其不仅能维持稳定的神经活动，还能自发地产生更广泛的、包括睡眠样慢波在内的不同脑动态，并能够模拟多种动态共存的复杂状态（如分离意识状态）？
*   **整体含义**：本研究通过将一种生物学基础的抑制性稳态可塑性规则嵌入到DMF模型中，创建了稳态动态平均场（HDMF）模型。该模型不仅解决了原DMF模型在稳定性上的固有限制，更重要的是，它通过一个统一的局部适应机制，能够解释和复现从清醒到睡眠、从异步到同步、甚至多种动态共存的广泛脑活动模式，为理解大脑的全局动态如何从局部适应过程中涌现提供了一个统一而强大的平台。

#### **2. 论文提出的方法论：核心思想与关键技术细节**

*   **核心思想**：在基于脑网络的大规模神经质量模型（DMF）中，用**动态的、具有遗忘机制的稳态抑制性可塑性规则**，来替代传统的**静态的**反馈抑制控制（FIC）参数。该规则允许每个脑区根据其当前的兴奋性活动和预设的目标发放率，自主地、持续地调整局部抑制性突触权重（\(J_i\)）。
*   **关键技术细节**：
    *   **基础模型**：使用动态平均场（DMF）模型，其中每个脑区由相互连接的兴奋性（E）和抑制性（I）神经元群组成，脑区间仅通过E群连接。
    *   **稳态可塑性规则**：该规则动态调整从抑制性到兴奋性神经元群的突触权重 \(J_i\)，其微分方程为：

        \[
        \frac{dJ_i}{dt} = -\frac{J_i}{\tau_{decay}} + LR \cdot r_i^{(I)} (r_i^{(E)} - \rho)
        \]
        *   **\(LR\)（学习率）**：控制突触权重更新的速度。
        *   **\(\tau_{decay}\)（衰减时间常数）**：强制“遗忘”旧的权重值，防止其无限增长，使规则成为一个持续的动态过程。
        *   **\(r_i^{(E)}\) 与 \(r_i^{(I)}\)**：分别是兴奋性和抑制性神经群的发放率。
        *   **\(\rho\) (目标发放率)**：系统期望维持的兴奋性发放率（本研究中设为3.44 Hz）。
    *   **核心发现一：参数间的幂律关系**：研究发现，只有在学习率（\(LR\)）和衰减时间常数（\(\tau_{decay}\)）满足特定的**幂律关系**时，系统才能实现最佳稳态，即：
        \[
        \tau_{decay} = \chi \cdot LR^{\epsilon}
        \]
        这个关系由网络特性决定，意味着**学习越快，遗忘也需要越快**，以保证系统能动态适应输入变化。
    *   **核心发现二：动态FIC的必要性**：通过将HDMF与静态FIC的DMF、“混合模型”（使用HDMF的时均FIC但固定不变）对比，证明了**持续的动态调整**是系统在不同全局耦合强度（G）下维持稳定的关键，尤其在临界点附近。静态或简单平均的FIC无法处理该点附近的快速波动，会导致系统失稳。

#### **3. 实验设计**

*   **数据集**：
    1.  **理论分析用数据**：来自丹麦奥胡斯大学16名健康被试的弥散加权MRI数据，用以构建AAL模板的90个皮层区域的结构连接矩阵。
    2.  **静息态fMRI实证数据**：来自人类连接组计划（HCP-YA）S1200公开数据集中的99名无关健康被试的静息态fMRI数据。预处理后，使用Schaefer-100图谱将数据划分到100个皮层区域。
    3.  **PET受体密度图**：来自Hansen等人2022年发布的神经递质图谱，本文使用了5-HT2A血清素受体密度图来模拟神经调节。
*   **Benchmark与对比方法**：
    *   **对比模型**：
        *   原始DMF模型，使用启发式线性解计算静态FIC。
        *   “混合”DMF模型，使用HDMF模型的时均FIC值，但将其固定。
    *   **对比任务**：
        1.  **稳态性能**：比较三种模型在不同全局耦合强度（G）下的发放率稳定性。
        2.  **神经调节稳健性**：模拟神经调节（*即*，增加5-HT2A受体介导的增益），比较DMF与HDMF的发放率变化和对数据的拟合能力。
        3.  **慢波生成能力**：研究HDMF在高低LR和G值下的频谱特性，确认其能否生成慢波。
        4.  **静息态数据拟合**：比较DMF和HDMF在拟合HCP静息态fMRI数据的静态功能连接（FC）和动态功能连接（FCD）时的表现。
        5.  **异质性动态**：通过在**局部改变学习率**，验证HDMF能否在同一网络中同时产生不同的动态（如慢波与异步活动）。

#### **4. 资源与算力**

*   论文中**未明确说明**所使用的具体GPU型号、数量或训练时长。文中提到使用了一个包含31个G值和11个\(\alpha\)值（DMF）以及51个G值和41个LR值（HDMF）的参数网格搜索，每个条件运行了20次模拟，这暗示了计算需求不小，但未提供具体硬件和耗时细节。

#### **5. 实验数量与充分性**

*   **实验数量**：论文进行了非常系统和详尽的实验，主要包括：
    *   **参数空间扫描**：扫描了LR和\(\tau_{decay}\)的二维空间（图2A，B）以及G-LR空间（图4C-F），以确定最优稳态区域和慢波生成条件。
    *   **模型性能对比**：对DMF、混合模型和HDMF在稳定性方面进行了多组对比（图2C, D）。
    *   **神经调节实验**：测试了动态和静态增益、不同受体类型，以及动态时间变化的增益，并复现了LSD药理数据拟合（图3，补充图3, 4, 5）。
    *   **异质性动态实验**：采用三种不同的选择标准（节点强度STR，强度核S-CORE，随机RANDOM）和多组不同数量（9, 10个区域）的子网络进行了实验（图5）。
    *   **静息态数据拟合实验**：在网格搜索基础上，筛选出FC和FCD拟合的最优参数，并对100个不同随机种子进行了统计对比分析（图6）。
*   **充分性与公平性**：
    *   **充分**：实验的覆盖范围非常广泛，涉及了模型验证、参数探索、鲁棒性测试、应用拓展（慢波生成）、异质性复杂状态模拟以及与实证数据的拟合，逻辑链条完整。
    *   **客观公平**：研究对比了HDMF与标准DMF在相同条件下的性能，并指出了HDMF的优势和局限（如并非完美保持目标发放率，而是在小幅波动中稳定）。在静息态拟合实验中，通过从交叉验证的“最优重叠区域”选取参数，并比较了100对模拟结果，增加了结论的统计可靠性。

#### **6. 论文的主要结论与发现**

1.  **实现了稳健的全脑稳态**：HDMF通过动态FIC，在广泛的全局耦合强度范围内成功将兴奋性发放率稳定在目标值附近，克服了原始DMF在高耦合下易发散、FIC需要复杂优化的局限。
2.  **动态FIC优于静态FIC**：证明了动态FIC是稳定性的关键，即使是同样数值的静态FIC也无法复现。FIC的动态特性对于补偿网络输入的快速波动至关重要。
3.  **增强了神经调节下的鲁棒性与预测性**：在接受神经调节扰动时，HDMF能维持发放率在生物合理范围内，而原始DMF则会出现超兴奋。这使得受体密度图和发放率变化之间的关系更加明确和可预测。
4.  **生成了前所未有的慢波活动**：仅通过调节学习率（LR）和全局耦合（G），HDMF就能产生类似睡眠的1-4 Hz慢波活动。这为DMF模型家族增添了一种全新的、重要的脑状态生成能力。
5.  **实现了“类嵌合体”的共存动态**：通过在不同脑区赋予不同的学习率，HDMF能够在一个网络中同时支持慢波活动和异步活动，这为模拟分离意识状态（如异态睡眠）提供了机制上的解释和计算模型。
6.  **保持了与实证数据拟合的能力**：在与HCP静息态fMRI数据的拟合中，HDMF在保持与DMF相当的静态功能连接（FC）拟合度的同时，显著改进了对动态功能连接（FCD）的拟合，捕捉到了更丰富的时变脑动态结构。

#### **7. 优点**

1.  **高生物合理性**：所采用的稳态可塑性规则直接来源于神经科学中对抑制性突触调节E/I平衡的研究。增加了模型的“遗忘机制”（\(\tau_{decay}\)）使其更像一个持续的、真实的生物过程。
2.  **解决核心难题**：成功解决了DMF模型的一大瓶颈——对静态FIC的依赖和不稳定性。该方法提供了一种无需额外复杂计算就能自适应的解决方案。
3.  **扩展动态表现力**：通过一个统一的机制，模型不仅保持了原有的表现力，还显著扩展了其动态活动图谱，特别是能够生成慢波活动。
4.  **可解释性强**：该模型为“局部”适应过程（可塑性）如何导致“全局”状态变化（慢波、清醒等）提供了清晰的机制性解释，例如局部慢波的产生源于对全局高耦合力输入的延迟抑制补偿。
5.  **实用性改善**：该HDMF模型可以轻松集成到开源框架（如fastDMF）中，降低了使用门槛，便于其他研究者复现和应用。

#### **8. 不足与局限**

1.  **单一目标发放率假设**：模型假设所有皮层区域都维持同一个目标发放率（\( \rho \)），但这在生物学上并不完全准确，不同脑区具有不同的代谢需求和活动水平。文章在末尾进行了初步探索，但并未完全解决此问题。
2.  **仅考虑抑制性稳态可塑性**：文中只考虑了抑制性（I->E）的稳态，而真实的稳态调节同时涉及兴奋性可塑性、内在兴奋性调控等多种机制。未来的工作可以扩展到这些机制。
3.  **缺乏对其他可塑性的交互研究**：未探讨该稳态规则与赫布型学习（Hebbian learning）等其他形式的突触可塑性的相互作用，这对于理解学习和记忆形成至关重要。
4.  **皮层中心主义**：主要基于皮层结构连接进行建模，对皮层下结构（如丘脑、脑干）和长程反馈的贡献考虑不足。这些结构在调节睡眠-觉醒周期和全局脑状态中扮演关键角色。
5.  **参数依赖**：虽然引入了自调节，但模型表现依然依赖于内部参数（如学习率）的设置，且在改变目标发放率或连接矩阵时，需要重新校准LR与\( \tau_{decay} \)的幂律关系。

（完）
