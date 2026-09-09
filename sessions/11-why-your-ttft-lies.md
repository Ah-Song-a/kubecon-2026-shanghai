# Why Your TTFT Lies: Diagnosing PD-Disaggregated LLM Inference with Minimal Cross-Layer Metrics

- 时间：2026-09-09，16:15–16:45
- 地点 / 语言 / 难度：1F · Mandarin Hall II / 中文 / Intermediate
- 讲者：Nicole Li、Kebe Liu
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1220647)
- Slides：[原始 PPTX](../slides/why-your-ttft-lies.pptx) · [官方下载](https://sessionize.com/download/idyatweu~QMcLoJtAyViBA2cZx3Mwny.pptx~kubecon-china-2026-why-your-ttft-lies.pptx)
- 官方视频：待补

## 官方简介摘要

提出一套面向 PD 分离推理的精简诊断方法，将 Gateway、Engine 内部、KV Cache、Batching/Scheduler、基础设施、GPU 和网络指标串联起来，再映射到 P:D 比例、Batch Size、KV 策略和 RDMA/拓扑等调优动作。

## 为什么值得关注

TTFT 本身无法指出慢在哪个阶段。这场分享把跨层指标真正变成可执行的生产排障流程。

- 技术关键词：TTFT、PD Disaggregation、KV Transfer、Batching、GPU、RDMA、Topology
- 学习主线：现象 → 阶段感知指标 → 根因 → 调优动作

## 个人笔记

- 

