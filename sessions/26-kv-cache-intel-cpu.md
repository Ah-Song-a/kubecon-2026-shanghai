# KV Cache: Accelerating AI inference on Intel CPU

- 时间：2026-09-09，11:25–11:45（UTC+8）
- 地点 / 语言：5F · 5B + C / 中文
- 讲者：Bin Yang
- 类型：Sponsor Demo
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1303982)
- Slides：[原始 PDF](../slides/kv-cache-intel-cpu.pdf) · [官方下载](https://sessionize.com/download/ijzappeg~GghacyHV9Jff6YjjfU19pa.pdf~intel_accelerating_ai_inference_on_intel_cpu.pdf)
- 官方视频：待补

## 官方简介摘要

介绍 KVShrink 如何把 KV Cache 从固定的 HBM 成本转化为可分层、可压缩的资产：将缓存卸载到 DDR 或存储，并利用 Intel QAT 硬件加速压缩，尽量保留原本会被淘汰的缓存，以提高跨请求复用率并降低重复计算。

## 为什么值得关注

它补足了以 GPU HBM 为中心的 KV Cache 视角，展示 CPU 内存、存储和硬件压缩如何进入缓存层级设计。评估结论时需注意这是 Sponsor Demo，并结合独立基准验证性能数据。

- 技术关键词：KV Cache、HBM、DDR、Storage Offload、Intel QAT、Compression、TTFT
- 学习主线：KV Cache 容量压力 → 分层卸载 → 硬件压缩 → 复用率与并发

## 个人笔记

- 

