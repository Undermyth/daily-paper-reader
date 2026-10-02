<div class="dpr-home-notice-card">
  <h3 class="dpr-home-notice-title">🚀 Start Here</h3>
  <ul class="dpr-home-notice-list">
    <li><a href="#/tutorial/README">使用教程</a></li>
  </ul>
</div>

## 每次日报
- 最新运行日期：2026-10-02
- 运行时间：2026-10-02 23:29:01 UTC
- 运行状态：成功
- 本次总论文数：18
- 精读区：7
- 速读区：11

### 今日简报（AI）
今日精读7篇、速读11篇共18篇，重点聚焦线性序列建模与长上下文记忆。最值得看的是CyFA与Triadic Linear Attention双双拿下9.0分，分别用相对时间分区记忆和三维循环状态攻克长序列建模。普通读者可优先从这两篇入手，再顺带浏览LOCI的空间线性记忆思路。
- 详情：[/202610/02/README](/202610/02/README)

### 精读区论文标签
1. [CyFA: Linear Sequence Modeling with Relative-Time-Partitioned Memory](/202610/02/2609.36259v1-cyfa-linear-sequence-modeling-with-relative-time-partitioned-memory)  
   标签：评分：9.0/10、query:la
   evidence：带相对时间分区记忆的线性RNN，组织键值关联
2. [Triadic Linear Attention: Three-Dimensional Recurrent States for Long-Context Sequence Modeling](/202610/02/2609.36529v1-triadic-linear-attention-three-dimensional-recurrent-states-for-long-context-sequence-modeling)  
   标签：评分：9.0/10、query:la
   evidence：三元外积写入三维记忆状态的线性注意力
3. [LeapQuant: Efficient Linear Attention with Accurate Recurrent State Quantization](/202610/02/2609.38166v1-leapquant-efficient-linear-attention-with-accurate-recurrent-state-quantization)  
   标签：评分：9.0/10、query:la
   evidence：面向长上下文推理的线性注意力循环状态精确量化
4. [Switching Linear Attention](/202610/02/2609.39034v1-switching-linear-attention)  
   标签：评分：9.0/10、query:la
   evidence：基于测试时回归推导的固定状态线性注意力序列层
5. [Intrinsic Associative Memory on Riemannian Manifolds: Curvature, Capacity, and Emergent Modes](/202610/02/2609.35948v1-intrinsic-associative-memory-on-riemannian-manifolds-curvature-capacity-and-emergent-modes)  
   标签：评分：8.0/10、query:la
   evidence：黎曼流形上的联想记忆与容量分析
6. [SMat-Attention: Structured Long-Context Sequence Modeling](/202610/02/2609.36062v1-smat-attention-structured-long-context-sequence-modeling)  
   标签：评分：8.0/10、query:la
   evidence：结构化因果掩码连接Softmax注意力与线性注意力
7. [The Evolution of Attention in Large Language Models: Mechanisms, Trade-offs, and Emerging Trends](/202610/02/2609.39661v1-the-evolution-of-attention-in-large-language-models-mechanisms-trade-offs-and-emerging-trends)  
   标签：评分：8.0/10、query:la
   evidence：将注意力视为模型内部上下文记忆，涵盖记忆压缩与循环状态

### 速读区论文标签
1. [LOCI: Spatial Linear Memory for Streaming World Models](/202610/02/2609.40222v1-loci-spatial-linear-memory-for-streaming-world-models)  
   标签：评分：8.0/10、query:la
   evidence：在transformer块中结合循环线性注意力记忆与键值缓存
2. [A neural network that maintains and retrieves memories based on context](/202610/02/2609.37791v1-a-neural-network-that-maintains-and-retrieves-memories-based-on-context)  
   标签：评分：7.0/10、query:comp-neuro
   evidence：带情景记忆缓冲的RNN建模情境调制的记忆并匹配人类fMRI响应
3. [Retrieval Capacity of Self-Attention Under Competition](/202610/02/2609.37879v1-retrieval-capacity-of-self-attention-under-competition)  
   标签：评分：7.0/10、query:la
   evidence：自注意力的有效注意力集合规模与检索容量
4. [Progressive Memory Transformer: Memory-Aware Attention for Time-Series](/202610/02/2609.31351v1-progressive-memory-transformer-memory-aware-attention-for-time-series)  
   标签：评分：6.0/10、query:la
   evidence：面向多尺度时间序列的记忆感知注意力
5. [ALLOT: Budgeted Hybrid-Memory Routing for Knowledge Updates in LLMs](/202610/02/2609.32344v1-allot-budgeted-hybrid-memory-routing-for-knowledge-updates-in-llms)  
   标签：评分：6.0/10、query:la
   evidence：外部记忆与检索结合的记忆感知路由
6. [MemEvo: Automatic Discovery of Streaming Video Memory Mechanisms](/202610/02/2609.36581v1-memevo-automatic-discovery-of-streaming-video-memory-mechanisms)  
   标签：评分：6.0/10、query:la
   evidence：自动发现带表示与检索原语的有界流式记忆机制
7. [Efficiently Approximating Attention Is Hard](/202610/02/2609.37261v1-efficiently-approximating-attention-is-hard)  
   标签：评分：6.0/10、query:la
   evidence：复杂性下界表明不存在具有均匀近似保证的高效注意力算法
8. [Scaling Parameter and Context in Attention: Native Sparse Attention from Mixture-of-Head](/202610/02/2609.38832v1-scaling-parameter-and-context-in-attention-native-sparse-attention-from-mixture-of-head)  
   标签：评分：6.0/10、query:la
   evidence：每token激活部分头的架构固有稀疏注意力
9. [CommunityKV: Efficient Long-Context Decoding via Graph Partitioning](/202610/02/2610.00418v1-communitykv-efficient-long-context-decoding-via-graph-partitioning)  
   标签：评分：6.0/10、query:la
   evidence：基于图划分的稀疏注意力与令牌检索
10. [Decision Titan: Test-Time Training for Long-Term Memory in Offline Reinforcement Learning](/202610/02/2610.01513v1-decision-titan-test-time-training-for-long-term-memory-in-offline-reinforcement-learning)  
   标签：评分：6.0/10、query:la
   evidence：以测试时训练记忆框架缓解RNN与Transformer的长期记忆局限
11. [In-context Learning of Single-index Targets: Comparing Kernel and Feature Learners](/202610/02/2610.01712v1-in-context-learning-of-single-index-targets-comparing-kernel-and-feature-learners)  
   标签：评分：6.0/10、query:la
   evidence：核学习器先做非线性特征映射再施加线性注意力


<div class="dpr-home-promo-card">
  <h3 class="dpr-home-promo-title">💬 社区与支持</h3>
  <ul class="dpr-home-promo-list">
    <li>欢迎 Star / Fork / Issue / PR</li>
    <li>QQ群：583867967（欢迎交流，已有：1151人）</li>
  </ul>
</div>
