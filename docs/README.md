<div class="dpr-home-notice-card">
  <h3 class="dpr-home-notice-title">🚀 Start Here</h3>
  <ul class="dpr-home-notice-list">
    <li><a href="#/tutorial/README">使用教程</a></li>
  </ul>
</div>

## 每次日报
- 最新运行日期：2026-08-04
- 运行时间：2026-08-04 22:07:57 UTC
- 运行状态：成功
- 本次总论文数：17
- 精读区：7
- 速读区：10

### 今日简报（AI）
今日聚焦高效语言流建模与视觉语言桥接，并延伸至长上下文缓存压缩与记忆机制。  
最值得精读的是《DeltaFlow》与《Linear Multi-Timescale Retention》，分别解决嵌入式语言流自适应与视觉语言记忆瓶颈。  
建议优先关注KV缓存压缩和角色解耦注意力方向，对实际部署成本更友好。
- 详情：[/202608/04/README](/202608/04/README)

### 精读区论文标签
1. [DeltaFlow: Noise-Adaptive Bidirectional Gated Delta Networks for Embedded Language Flows](/202608/04/2608.01240v1-deltaflow-noise-adaptive-bidirectional-gated-delta-networks-for-embedded-language-flows)  
   标签：评分：9.0/10、query:la
   evidence：面向高效序列混合的双向门控Delta网络
2. [Linear Multi-Timescale Retention as a Memory-Efficient Vision-Language Bridge](/202608/04/2608.01614v1-linear-multi-timescale-retention-as-a-memory-efficient-vision-language-bridge)  
   标签：评分：9.0/10、query:la
   evidence：基于ELU的线性注意力与多时间尺度循环衰减，用于记忆高效的序列处理
3. [RING: Retrieval-Internalized Generation for Continual Large-Scale Knowledge Injection](/202608/04/2608.01630v1-ring-retrieval-internalized-generation-for-continual-large-scale-knowledge-injection)  
   标签：评分：9.0/10、query:la
   evidence：通过记忆专家将检索内化到生成中
4. [Bole: Efficient Tree Speculation for Hybrid-Attention Language Models](/202608/04/2608.01651v1-bole-efficient-tree-speculation-for-hybrid-attention-language-models)  
   标签：评分：9.0/10、query:la
   evidence：面向混合注意力模型中线性注意力递归的树形投机解码优化
5. [DART: Decoded Attention over Recurrent States for Efficient Long-Context Sequence Modeling](/202608/04/2608.02032v1-dart-decoded-attention-over-recurrent-states-for-efficient-long-context-sequence-modeling)  
   标签：评分：9.0/10、query:la
   evidence：通过状态空间对偶性直接连接循环状态压缩与注意力风格检索
6. [Mamba with Hierarchical Memory: Solving Representation Bottleneck in Long Sequence Modeling](/202608/04/2608.02347v1-mamba-with-hierarchical-memory-solving-representation-bottleneck-in-long-sequence-modeling)  
   标签：评分：9.0/10、query:la
   evidence：带分层记忆的循环线性注意力模型用于长序列建模
7. [Structured Memory for Edge Language Models: Persistent Context and Corpus Retrieval via O(1) SSM State Injection](/202608/04/2608.02560v1-structured-memory-for-edge-language-models-persistent-context-and-corpus-retrieval-via-o1-ssm-state-injection)  
   标签：评分：9.0/10、query:la
   evidence：SSM作为现代RNN，以O(1)状态注入实现高效序列处理

### 速读区论文标签
1. [S$^4$R: Selective Sampling, Subspaces, and Sparse Reconstruction for Compressed Long-Context KV Caching](/202608/04/2608.00528v1-s4r-selective-sampling-subspaces-and-sparse-reconstruction-for-compressed-long-context-kv-caching)  
   标签：评分：8.0/10、query:la
   evidence：通过选择性采样与稀疏重建实现长上下文KV缓存压缩
2. [Role-Decoupled Attention Residuals: Separating Matching and Content Retrieval Across Depth](/202608/04/2608.01075v1-role-decoupled-attention-residuals-separating-matching-and-content-retrieval-across-depth)  
   标签：评分：8.0/10、query:la
   evidence：将注意力匹配(QK)与内容检索(V)路径分离的注意力机制
3. [Divisive Normalization Shapes Low-Rank Slow Manifolds for Continuous Working Memory](/202608/04/2608.01947v1-divisive-normalization-shapes-low-rank-slow-manifolds-for-continuous-working-memory)  
   标签：评分：8.0/10、query:comp-neuro
   evidence：使用分割归一化建模连续工作记忆，是计算神经科学记忆研究的核心工作
4. [LiveMem: Maintaining Memory State Continuity in Long-Running LLM Inference](/202608/04/2608.02515v1-livemem-maintaining-memory-state-continuity-in-long-running-llm-inference)  
   标签：评分：8.0/10、query:la
   evidence：面向有界KV长上下文的记忆状态连续性
5. [SepPrune:A Separator-based Pruning Framework for Efficient Multimodal Large Language Models](/202608/04/2607.25818v1-sepprunea-separator-based-pruning-framework-for-efficient-multimodal-large-language-models)  
   标签：评分：7.0/10、query:la
   evidence：基于分隔符的高效多模态注意力剪枝
6. [SeDeM: Selective Decompression of Hidden-State Memories for Long-Context Question Answering](/202608/04/2608.00311v1-sedem-selective-decompression-of-hidden-state-memories-for-long-context-question-answering)  
   标签：评分：7.0/10、query:la
   evidence：面向长上下文问答的选择性解压隐状态记忆方法
7. [PMMC: Prospective Multimodal Memory Compilation for Long-Term LVLM Agents](/202608/04/2608.00962v1-pmmc-prospective-multimodal-memory-compilation-for-long-term-lvlm-agents)  
   标签：评分：7.0/10、query:la
   evidence：面向长期记忆的增强型大模型智能体，使用问题条件记忆编译
8. [LongCat Sparse Attention: Taming the Lightning via Streaming-aware Hierarchical Cross-Layer Indexing](/202608/04/2608.01662v1-longcat-sparse-attention-taming-the-lightning-via-streaming-aware-hierarchical-cross-layer-indexing)  
   标签：评分：7.0/10、query:la
   evidence：硬件算法协同设计的稀疏注意力
9. [ReLoop-UME: Recurrent Depth with Learnable Retrieval Registers for Universal Multimodal Embedding](/202608/04/2607.28751v1-reloop-ume-recurrent-depth-with-learnable-retrieval-registers-for-universal-multimodal-embedding)  
   标签：评分：6.0/10、query:la
   evidence：循环深度与可学习检索寄存器探索面向高效多模态嵌入的现代RNN架构
10. [Reproducing LightMem: Naive RAG Is Just as Good for Memory Management](/202608/04/2607.29104v1-reproducing-lightmem-naive-rag-is-just-as-good-for-memory-management)  
   标签：评分：6.0/10、query:la
   evidence：复现面向长期对话的LightMem记忆管理，并发现朴素RAG同样有效，为记忆增强系统设计提供借鉴


<div class="dpr-home-promo-card">
  <h3 class="dpr-home-promo-title">💬 社区与支持</h3>
  <ul class="dpr-home-promo-list">
    <li>欢迎 Star / Fork / Issue / PR</li>
    <li>QQ群：583867967（欢迎交流，已有：1151人）</li>
  </ul>
</div>
