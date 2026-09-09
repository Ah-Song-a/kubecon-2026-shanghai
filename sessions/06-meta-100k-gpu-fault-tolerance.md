# Training Through Failures: How Meta Keeps 100k-GPU Jobs Alive with Open-Source Fault Tolerance

- 时间：2026-09-09，11:45–12:15
- 地点 / 语言 / 难度：1F · Mandarin Hall I / 英文 / Intermediate
- 讲者：Tristan Rice、Amir Afzali
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1223450)
- Slides：官方暂未公开 / 待补
- 官方视频：待补

## 官方简介摘要

介绍 Meta 如何让超大规模训练任务在日常硬件故障下持续运行，包括 torchcomms 的 NCCL/MCCL/Gloo 后端、新的 communicator 恢复原语，以及基于 GPU Peer Memory 或本地磁盘的快速 checkpoint。

## 为什么值得关注

它把 NCCL 从通信性能问题延伸到故障恢复：动态缩减、扩展或撤销 communicator，并用 GPU Peer RDMA 加速恢复。

- 技术关键词：torchcomms、NCCL、MCCL、Gloo、ncclShrink、ncclGrow、ncclCommRevoke、RDMA
- 学习主线：集合通信 → 故障检测 → 恢复 → 弹性训练

## 个人笔记

- 

