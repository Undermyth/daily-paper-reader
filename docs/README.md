<div class="dpr-home-notice-card">
  <h3 class="dpr-home-notice-title">🚀 Start Here</h3>
  <ul class="dpr-home-notice-list">
    <li><a href="#/tutorial/README">使用教程</a></li>
  </ul>
</div>

## 每次日报
- 最新运行日期：2026-09-01
- 运行时间：2026-09-01 23:04:23 UTC
- 运行状态：成功
- 本次总论文数：13
- 精读区：7
- 速读区：6

### 今日简报（AI）
今日聚焦注意力机制与记忆增强，精读两篇9分论文，另含视频理解与语义分割速读。  
最值得关注《Tail-Replay》突破混合LLM前缀缓存线性注意力瓶颈，以及《Kathleen Remembers》实现免注意力长度不变的回忆。  
建议优先精读这两篇，并留意速读中的Liquid门控注意力对动态记忆的补充启发。
- 详情：[/202609/01/README](/202609/01/README)

### 精读区论文标签
1. [Tail-Replay: Escaping the Curse of Linear Attention in Prefix Caching for Hybrid LLMs](/202609/01/2608.30310v1-tail-replay-escaping-the-curse-of-linear-attention-in-prefix-caching-for-hybrid-llms)  
   标签：评分：9.0/10、query:la
   evidence：针对混合大模型中线性注意力循环状态导致前缀缓存受限的问题
2. [Kathleen Remembers: Length-Invariant One-Shot Recall Without Attention](/202609/01/2608.30376v1-kathleen-remembers-length-invariant-one-shot-recall-without-attention)  
   标签：评分：9.0/10、query:la
   evidence：为免注意力递归主干添加固定键全息(HRR)关联存储，实现长度不变的一次性回忆
3. [DASC: Decay-Aware State Compression for Hybrid Linear-Attention Serving](/202609/01/2608.30386v1-dasc-decay-aware-state-compression-for-hybrid-linear-attention-serving)  
   标签：评分：9.0/10、query:la
   evidence：混合线性注意力架构，利用衰减结构实现状态压缩
4. [Event-Driven Language Models with Sparse Neural Activity for Neuromorphic Hardware](/202609/01/2608.30439v1-event-driven-language-models-with-sparse-neural-activity-for-neuromorphic-hardware)  
   标签：评分：9.0/10、query:la
   evidence：直接面向线性注意力/状态空间模型的稀疏激活与高效序列处理
5. [Beyond Static and Linear: What Attention Constraints Best Fit Human Reading Times?](/202609/01/2608.23818v1-beyond-static-and-linear-what-attention-constraints-best-fit-human-reading-times)  
   标签：评分：8.0/10、query:la
   evidence：系统比较Transformer中基于注意力的记忆约束与人类阅读时间的拟合
6. [RouteSparse: Input-Conditional Pattern Routing for Budgeted Long-Context Prefilling](/202609/01/2608.29058v1-routesparse-input-conditional-pattern-routing-for-budgeted-long-context-prefilling)  
   标签：评分：8.0/10、query:la
   evidence：输入条件的稀疏注意力路由用于长上下文预填充，与高效注意力主题高度契合
7. [LoGo: Token-Level Dynamic Local-Global Attention](/202609/01/2608.29539v1-logo-token-level-dynamic-local-global-attention)  
   标签：评分：8.0/10、query:la
   evidence：令牌级动态局部-全局注意力高效分配注意力预算以处理长序列

### 速读区论文标签
1. [Liquid Gated Attention](/202609/01/2608.30695v1-liquid-gated-attention)  
   标签：评分：8.0/10、query:la
   evidence：输入驱动门控与快速权重隐状态，属于线性注意力风格的高效序列处理
2. [nnMNet: Baseline for Martian Terrain Semantic Segmentation](/202609/01/2608.29609v1-nnmnet-baseline-for-martian-terrain-semantic-segmentation)  
   标签：评分：7.0/10、query:la
   evidence：将线性注意力整合进火星地形分割基线以捕捉全局上下文
3. [Dynamic Hub-and-Spoke Memory for Streaming Video Understanding](/202609/01/2608.30294v1-dynamic-hub-and-spoke-memory-for-streaming-video-understanding)  
   标签：评分：7.0/10、query:la
   evidence：提出用于流式视频问答的动态hub-and-spoke记忆，是一种带注意力检索的记忆增强网络
4. [CateKV: On Sequential Consistency for Long-Context LLM Inference Acceleration](/202609/01/2608.30295v1-catekv-on-sequential-consistency-for-long-context-llm-inference-acceleration)  
   标签：评分：7.0/10、query:la
   evidence：面向长上下文推理的混合KV缓存加速
5. [State-Conditioned Visual Evidence Retrieval for Fine-Grained Perception in Document Vision-Language Models](/202609/01/2608.28698v1-state-conditioned-visual-evidence-retrieval-for-fine-grained-perception-in-document-vision-language-models)  
   标签：评分：6.0/10、query:la
   evidence：解码时按状态检索局部视觉证据，减少全局表示重复访问
6. [All You Need Is Non-Commutative Words](/202609/01/2608.29314v1-all-you-need-is-non-commutative-words)  
   标签：评分：6.0/10、query:la
   evidence：提出一种非交换矩阵乘积的注意力机制，无需QKV投影并降低注意力成本


<div class="dpr-home-promo-card">
  <h3 class="dpr-home-promo-title">💬 社区与支持</h3>
  <ul class="dpr-home-promo-list">
    <li>欢迎 Star / Fork / Issue / PR</li>
    <li>QQ群：583867967（欢迎交流，已有：1151人）</li>
  </ul>
</div>
