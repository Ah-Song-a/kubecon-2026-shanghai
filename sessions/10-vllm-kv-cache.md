# vLLM KV Cache Management: From Cache Reuse to Agent Scenario Optimization

- 时间：2026-09-09，15:30–16:00
- 地点 / 语言：1F · Mandarin Hall I / 中文
- 讲者：Mengqing Cao、Xiyuan Wang
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1222763)
- Slides：官方暂未公开 / 待补
- 官方视频：待补

## 官方简介摘要

介绍 vLLM 在长上下文和高并发场景中的缓存管理实践：基于 Block Hash 的 Prefix Cache 复用、CPU Offloading、LRU/ARC 策略和 Prefix Cache Hit Rate，以及面向语义压缩、任务依赖调度和跨 Session 共享的后续方向。

## 为什么值得关注

它把 KV Cache 理论连接到具体的 vLLM 机制和运行指标，尤其适合多轮 Agent 与工具调用场景。

- 技术关键词：vLLM、Prefix Caching、KV Offload、LRU、ARC、Cache Hit Rate、Agent
- 学习主线：Prompt/History 复用 → 显存压力 → Offload 与淘汰

## 个人笔记

- 

