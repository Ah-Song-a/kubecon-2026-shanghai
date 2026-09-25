# vLLM-Helion: SOTA LLM Performance by advanced autotuning and fine-grained dispatching

- 时间：2026-09-09，16:15–16:45（UTC+8）
- 地点 / 语言：1F · Mandarin Hall I / 英文
- 讲者：Sean Chen
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1214156)
- Slides：[原始 PDF](../slides/vllm-helion.pdf) · [官方下载](https://sessionize.com/download/impaldey~Lu9nPHGesXnMGADsrTkByA.pdf~vllm-helion-pytorch-conference-china-2026.pdf)
- [GitHub Repository](https://github.com/redhat-et/vllm-helion)
- 官方视频：[CNCF YouTube](https://www.youtube.com/watch?v=5Uhe4aGb5YA)

## 官方简介摘要

介绍 vLLM 与 PyTorch Helion Kernel DSL 的集成。离线自动调优系统针对生产输入形状搜索配置空间，并随平台分发预调优结果；运行时再根据每次调用的实际输入维度进行细粒度配置分派，避免单一平台配置覆盖所有工作负载。

## 为什么值得关注

这场把 vLLM 性能优化下沉到 Kernel 层，清楚展示离线搜索与运行时 Dispatch 的职责边界，适合理解“模型服务框架性能”如何最终落到算子生成、硬件适配和真实输入形状。

- 技术关键词：vLLM、Helion、PyTorch、Kernel DSL、Autotuning、Runtime Dispatch、Shape Specialization
- 学习主线：LLM Serving → Kernel 实现 → 离线自动调优 → 运行时细粒度分派

## 个人笔记

- 
