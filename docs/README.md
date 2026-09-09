<div class="dpr-home-notice-card">
  <h3 class="dpr-home-notice-title">🚀 Start Here</h3>
  <ul class="dpr-home-notice-list">
    <li><a href="#/tutorial/README">使用教程</a></li>
  </ul>
</div>

## 每次日报
- 最新运行日期：2026-09-09
- 运行时间：2026-09-09 22:10:51 UTC
- 运行状态：成功
- 本次总论文数：19
- 精读区：7
- 速读区：12

### 今日简报（AI）
今日精读7篇、速读12篇，共19篇推荐论文，聚焦记忆机制与高效注意力两大方向。  
最值得关注：Kalman Delta Networks用不确定性感知关联记忆拿下满分，以及SVD压缩下注意力秩坍缩的相位反转分析，揭示效率与表达的深层权衡。  
建议从速读入手，优先“Memory in Deep Time-Series Models”建立基础，再深入精读两篇高分组文。
- 详情：[/202609/09/README](/202609/09/README)

### 精读区论文标签
1. [Kalman Delta Networks: Uncertainty-aware Associative Memory](/202609/09/2609.07816v1-kalman-delta-networks-uncertainty-aware-associative-memory)  
   标签：评分：10.0/10、query:la
   evidence：将循环联想记忆建模为线性高斯状态空间模型并用卡尔曼滤波估计
2. [Linear Algebra Foundations of Efficient Attention: A Phase Reversal in Rank Collapse Under SVD Compression](/202609/09/2609.06341v1-linear-algebra-foundations-of-efficient-attention-a-phase-reversal-in-rank-collapse-under-svd-compression)  
   标签：评分：9.0/10、query:la
   evidence：以线性注意力、半可分矩阵对偶与KV缓存压缩为核心，关联高效序列处理
3. [RoLA: Rotary-Positioned Low-Rank Linear Attention for Efficient Diffusion Transformers](/202609/09/2609.06712v1-rola-rotary-positioned-low-rank-linear-attention-for-efficient-diffusion-transformers)  
   标签：评分：9.0/10、query:la
   evidence：旋转位置低秩线性注意力用于高效扩散Transformer
4. [Storing Infinite Dynamical Attractors in Nonreciprocal Associative Neural Networks](/202609/09/2609.07341v1-storing-infinite-dynamical-attractors-in-nonreciprocal-associative-neural-networks)  
   标签：评分：9.0/10、query:la
   evidence：联想神经网络存储大量动态吸引子，并给出容量与检索理论
5. [On the Recall Scaling Laws in Mamba: A Theoretical and Mechanistic Study via Hashing](/202609/09/2609.07681v1-on-the-recall-scaling-laws-in-mamba-a-theoretical-and-mechanistic-study-via-hashing)  
   标签：评分：9.0/10、query:la
   evidence：针对Mamba这一现代RNN/状态空间模型的关联记忆召回机制进行理论拆解，揭示其隐式线性哈希实现方式
6. [Do Dynamic Routers Need Memory? HeRo: History-Aware Routing for Efficient LLM Inference](/202609/09/2609.08189v1-do-dynamic-routers-need-memory-hero-history-aware-routing-for-efficient-llm-inference)  
   标签：评分：9.0/10、query:la
   evidence：用线性注意力构造跨层路由器记忆以提升LLM推理效率
7. [Dual-Latent Memory Routing for Vision-Language Reasoning](/202609/09/2609.05539v1-dual-latent-memory-routing-for-vision-language-reasoning)  
   标签：评分：8.0/10、query:la
   evidence：用视觉与推理双隐记忆及动态路由器增强多模态大模型的长程推理能力

### 速读区论文标签
1. [Memory in Deep Time-Series Models](/202609/09/2609.06006v1-memory-in-deep-time-series-models)  
   标签：评分：8.0/10、query:la
   evidence：将深度序列模型中的记忆问题统一到现代RNN与状态空间模型等架构之上，贴合线性注意力主题
2. [CEDAR: Error-Bounded Residual Routing for Efficient Long-Context Attention](/202609/09/2609.07237v1-cedar-error-bounded-residual-routing-for-efficient-long-context-attention)  
   标签：评分：8.0/10、query:la
   evidence：基于残差键值摘要与误差感知的由粗到细注意力路由，用于高效长上下文检索
3. [SequenceO1: End-to-End Ultra-Long (100K) Sequence Modeling in Recommendation with Low-Rank Caching](/202609/09/2609.08443v1-sequenceo1-end-to-end-ultra-long-100k-sequence-modeling-in-recommendation-with-low-rank-caching)  
   标签：评分：8.0/10、query:la
   evidence：利用低秩缓存在严格延迟约束下进行高效超长序列建模
4. [Query-Oblivious Coresets for Softmax Attention: Improved Bounds and Efficient Constructions](/202609/09/2609.06327v1-query-oblivious-coresets-for-softmax-attention-improved-bounds-and-efficient-constructions)  
   标签：评分：7.0/10、query:la
   evidence：查询无关注意力核集用少量键值对近似所有查询的注意力输出，是面向记忆检索的高效注意力近似机制
5. [RouteRelay: Event-Triggered Cross-Layer Route Reuse for Efficient Dynamic Sparse Attention](/202609/09/2609.07306v1-routerelay-event-triggered-cross-layer-route-reuse-for-efficient-dynamic-sparse-attention)  
   标签：评分：7.0/10、query:la
   evidence：复用路由元数据加速动态稀疏注意力，面向长上下文的高效检索注意力机制。
6. [Jacap: Robust KV Cache Eviction via Jacobian-Based Nonlinear Information Capacity Preservation](/202609/09/2609.08131v1-jacap-robust-kv-cache-eviction-via-jacobian-based-nonlinear-information-capacity-preservation)  
   标签：评分：7.0/10、query:la
   evidence：用雅可比信息容量指导KV缓存淘汰，为长上下文注意力的键值记忆管理提供理论目标
7. [Sample-Guided Exact Top-K Selection for Long-Context Sparse Attention](/202609/09/2609.08450v1-sample-guided-exact-top-k-selection-for-long-context-sparse-attention)  
   标签：评分：7.0/10、query:la
   evidence：基于样本引导的精确Top-K选择提升长上下文稀疏注意力的检索效率
8. [GaLe: memory-efficient Global Approximate and Local Exact features](/202609/09/2609.02689v1-gale-memory-efficient-global-approximate-and-local-exact-features)  
   标签：评分：6.0/10、query:la
   evidence：全局近似与局部精确特征为受限设备上的视觉模型提供内存高效且支持注意力机制的全局处理
9. [Intra-Prompt Parallel Decoding for Common-Context Question Answering](/202609/09/2609.05707v1-intra-prompt-parallel-decoding-for-common-context-question-answering)  
   标签：评分：6.0/10、query:la
   evidence：在共同上下文问题间共享KV缓存与注意力计算，降低记忆读取开销
10. [Towards Enabling Distance-Based Memory Addressing](/202609/09/2609.06270v1-towards-enabling-distance-based-memory-addressing)  
   标签：评分：6.0/10、query:la
   evidence：面向距离式记忆寻址的数据并行内存相似性搜索机制，可作为联想记忆的硬件支撑
11. [Where to Look and What to Use: Retrieve-Localize-Generate for Long-Term Conversational Memory Question Answering](/202609/09/2609.07093v1-where-to-look-and-what-to-use-retrieve-localize-generate-for-long-term-conversational-memory-question-answering)  
   标签：评分：6.0/10、query:la
   evidence：多粒度记忆单元与基于内部记忆图的查询路由，用于长程对话记忆问答
12. [Separating Stream Stability from Long-Term Recall in Language Models](/202609/09/2609.07282v1-separating-stream-stability-from-long-term-recall-in-language-models)  
   标签：评分：6.0/10、query:la
   evidence：提出稳定、访问与效用跨度来评测缓存外内容可达性，与线性注意力的记忆评估高度相关


<div class="dpr-home-promo-card">
  <h3 class="dpr-home-promo-title">💬 社区与支持</h3>
  <ul class="dpr-home-promo-list">
    <li>欢迎 Star / Fork / Issue / PR</li>
    <li>QQ群：583867967（欢迎交流，已有：1151人）</li>
  </ul>
</div>
