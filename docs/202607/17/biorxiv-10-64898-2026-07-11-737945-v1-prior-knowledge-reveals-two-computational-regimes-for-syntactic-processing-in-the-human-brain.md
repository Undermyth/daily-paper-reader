---
title: Prior knowledge reveals two computational regimes for syntactic processing in the human brain
title_zh: 先验知识揭示人脑句法加工的两种计算模式
authors: "Iaia, C., Tavano, A."
date: 2026-07-11
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.11.737945v1.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 大脑中句法处理的计算机制
tldr: 人脑将连续语音转化为结构化语言表征，需依赖先验知识，但其神经机制未知。本研究结合MEG与语料库句法转移概率，比较短语与依存语法下的神经动态。结果发现：先验知识仅增强记忆相关特征（局部上下文），而对整合特征无益；长上下文导致解码性能下降。结论揭示两个并行计算机制：面向未完成结构的前瞻性本地预测与结构完成时的整合编码，为神经语言模型提供重要约束。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737945-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1649, \"height\": 897, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737945-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1499, \"height\": 1260, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737945-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1624, \"height\": 1492, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737945-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1628, \"height\": 1572, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737945-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1579, \"height\": 1040, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737945-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 361, \"height\": 851, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737945-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 328, \"height\": 246, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-11-737945-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1091, \"height\": 195, \"label\": \"Table\"}]"
motivation: 探究先验知识如何影响人脑对连续语音的句法加工，揭示其神经计算机制。
method: 结合脑磁图记录与语料库句法转移概率，在短语结构和依存语法框架下分析神经表征。
result: 先验知识仅增强局部上下文中的记忆相关特征，对整合特征无影响，解码性能随上下文长度先升后降。
conclusion: 发现两个并行机制：面向未完成结构的前瞻性局部预测和结构完成时的整合编码，约束神经语言模型理论。
---

## 摘要
人脑能够快速将连续言语转化为结构化的、有意义的语言表征，然而先验知识如何约束这一过程仍不清楚。为刻画这种影响，我们将听有声书时采集的脑磁图（MEG）记录与基于短语结构和依存语法的句法特征上的语料库派生转移概率相结合。跨语法形式体系，先验知识选择性地增强了与记忆相关特征的神经表征，这些特征索引了必须保持开放以待未来完成的句法结构。这种增强严格局限于局部：紧邻的前文语境改善了单词起始和结束时的神经解码，而更长的历史则要么导致单词水平恢复基线，要么导致解码性能下降。相反，索引句法操作完成的整合相关特征未从先验知识中获益，且在单词结束时表征最强，这与它们依赖于单词级结构解析相一致。这些可分离的动态揭示了句法加工的两种并行神经计算模式：一种面向未来的、局部维持的待定结构预测编码，以及一种在结构解析时参与的整合编码。更广泛地说，我们的发现为语言加工的神经理论以及将人类语言理解中的预测与大语言模型（LLM）相对无约束的操作等同起来的观点施加了机制性约束。

## Abstract
The human brain rapidly transforms continuous speech into structured, meaningful linguistic representations, yet how prior knowledge constrains this process remains unclear. To characterize this influence, we combined MEG recordings acquired during audiobook listening with corpus-derived transition probabilities over syntactic features defined within both phrase-structure and dependency-based grammars. Across grammatical formalisms, prior knowledge selectively sharpened the neural representation of memory-related features indexing syntactic structures that must remain open for future completion. This enhancement was strictly local: immediately preceding contexts improved neural decoding at both word onset and offset, whereas longer histories produced either a return to baseline at the word level or a deterioration in decoding performance. By contrast, integration-related features indexing the completion of syntactic operations showed no benefit from prior knowledge and were represented most strongly at word offset, consistent with their dependence on word-level structural resolution. These dissociable dynamics reveal two concurrent neural computational regimes for syntactic processing: a forward-looking, locally maintained predictive code for pending structure and an integrative code engaged when structure is resolved. More broadly, our findings impose a mechanistic constraint on neural theories of language processing and on accounts that equate prediction in human language comprehension with the comparatively unconstrained operations of large language models (LLMs).