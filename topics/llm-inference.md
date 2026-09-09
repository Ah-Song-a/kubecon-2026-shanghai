# LLM 推理

核心服务形态是 PD 分离：Prefill 与 Decode 的计算、内存和扩缩容特征不同，因此基础设施需要 Token-aware Routing、阶段感知扩缩容、KV Locality 与跨层诊断。

建议阅读：[Huawei Celia](../sessions/05-huawei-celia-inference-plane.md)、[vLLM KV Cache](../sessions/10-vllm-kv-cache.md)、[TTFT 诊断](../sessions/11-why-your-ttft-lies.md)。

