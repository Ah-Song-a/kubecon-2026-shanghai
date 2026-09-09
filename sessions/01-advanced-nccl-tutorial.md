# Advanced NCCL Tutorial: Beyond Collectives

- 时间：2026-09-08，13:45–15:00（UTC+8）
- 地点：7F · Pearl Hall
- 语言 / 难度：英文 / Advanced；官方说明教学资料计划提供中英文版本
- 讲者：Jeff Hammond、Hanyue He、Ke Wen
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1224567)
- Slides：[原始 PDF](../slides/advanced-nccl-tutorial.pdf) · [官方下载](https://sessionize.com/download/okugpa~ErvMRkjRjLFiWksGeRKUuR.pdf~pytorch-china-2026-tutorial.pdf)
- 官方代码仓库：[jeffhammond/pytorch-china-2026-nccl-tutorial](https://github.com/jeffhammond/pytorch-china-2026-nccl-tutorial)
- 官方视频：待补

## 官方简介摘要

动手介绍 NCCL 的对称内存和 GPU-Initiated Networking（GIN），包括如何在 NVLink 域内扩展通信，以及如何通过 GIN 跨互联 GPU 节点扩展。这些能力与 DeepEP v2 等现代 MoE 通信方案直接相关。

## 为什么值得关注

这是整个资料集锦最底层的知识锚点：GPU 通信原语与内存模型会继续影响 MoE 推理、拓扑放置、DRA 和网络性能排障。

- 技术关键词：NCCL、Symmetric Memory、GIN、NVLink、DeepEP、MoE
- 学习主线：GPU 通信 → GPU/NIC 拓扑 → 调度放置 → AI 工作负载性能

## 个人笔记

- 
