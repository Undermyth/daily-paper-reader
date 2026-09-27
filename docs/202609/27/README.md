# 日报 · 2026-09-27

- 生成时间：2026-09-27 22:39:27 UTC
- 当次推荐总数：4
- 精读区：0
- 速读区：4

## 今日简报（AI）
今日速读4篇、精读0篇，全部为6.0分，方向集中在KV cache压缩与注意力计算效率。

最值得看的是KV cache这条线：ValueDiff用值几何做淘汰、Shared Global KV提出分层局部历史的共享方案，另一篇FlashBoB则给Softmax注意力做I/O高效的精确backward-over-backward。

普通读者建议先读两篇KV cache短文建立直觉，再按需跟进FlashBoB这类偏工程实现的内容。

## 精读区
- 本次无精读推荐。

## 速读区
1. [ValueDiff: Value-Geometric KV Cache Eviction for Sink-Suppressed LLMs](/202609/27/2609.23314v1-valuediff-value-geometric-kv-cache-eviction-for-sink-suppressed-llms) （6.0/10）
2. [FlashBoB: I/O-Efficient Exact Backward-over-Backward for Softmax Attention](/202609/27/2609.24089v1-flashbob-io-efficient-exact-backward-over-backward-for-softmax-attention) （6.0/10）
3. [Shared Global KV with Layer-Specific Local History](/202609/27/2609.28006v1-shared-global-kv-with-layer-specific-local-history) （6.0/10）
4. [FlashLoop: Fast and Memory-Efficient Looped Transformers via Lazy Updates](/202609/27/2609.29812v1-flashloop-fast-and-memory-efficient-looped-transformers-via-lazy-updates) （6.0/10）

---
使用键盘方向键可在日报/论文之间快速切换。
