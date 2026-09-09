# End-to-End Observability for LLM Inference: From Token to GPU

- 时间：2026-09-09，14:30–15:00
- 地点 / 语言 / 难度：1F · Mandarin Hall II / 中文 / Intermediate
- 讲者：Jared Tan、Murphy Chen、Nicole Li
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1223860)
- Slides：[原始 PDF](../slides/end-to-end-observability-for-llm-inference.pdf) · [官方下载](https://sessionize.com/download/ifiymay~Dur7z1Dbqz7DLEgf5TnNjJ.pdf~end-to-end-observability-for-llm-inference-from-token-to-gpu-en.pdf)
- 官方视频：待补

## 官方简介摘要

介绍贯穿 Ingress、Inference Gateway、vLLM/SGLang、模型 Runtime 和 GPU 硬件的生产可观测性方案，并使用 OpenTelemetry GenAI 语义规范统一 Token 指标与流式 Trace。案例包括 P99 延迟突增、GPU“忙而不做功”和 KV Cache OOM。

## 为什么值得关注

传统请求级 RED/USE 指标无法解释 TTFT、TPOT 和 ITL。这场分享提供了 LLM 生产运维真正需要的跨层诊断模型。

- 技术关键词：TTFT、TPOT、ITL、OpenTelemetry、vLLM、SGLang、GPU、KV Cache OOM
- 学习主线：用户请求 → Token 指标 → Runtime → GPU → 根因

## 个人笔记

- 

