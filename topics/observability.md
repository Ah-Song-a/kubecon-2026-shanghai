# 可观测性

LLM 运维需要把用户看到的 Token 延迟，与 Engine 调度、Cache 状态、GPU 行为和 Network/RDMA 拓扑关联起来：

```text
TTFT / TPOT / ITL → 判断 Prefill 或 Decode 阶段
→ 检查 Queue、Batch 和 KV 状态 → 关联 GPU 与网络
→ 调整 P:D 比例、Batch Size、KV 策略或设备放置
```

建议阅读：[Token-to-GPU 可观测性](../sessions/09-llm-observability-token-to-gpu.md)、[Why Your TTFT Lies](../sessions/11-why-your-ttft-lies.md)、[Cilium](../sessions/02-cilium-10-years.md)。

