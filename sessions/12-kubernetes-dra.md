# Kubernetes DRA Architecture: Scheduling, Status, and Topology at Scale

- 时间：2026-09-09，16:15–16:45
- 地点 / 语言 / 难度：7F · Pearl Hall / 中文 / Intermediate
- 讲者：Paco Xu、Kang Zhang
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1223308)
- Slides：[原始 PDF](../slides/kubernetes-dra-architecture-v1.1.pdf) · [官方下载](https://sessionize.com/download/kqaxyec~47fBae5CA846z2Fj7Xfbwx.pdf~kubernetes-dra-architecture-v1.1.pdf)
- 代码：[NVIDIA Kubernetes DRA GPU Driver](https://github.com/NVIDIA/k8s-dra-driver-gpu)
- 官方视频：待补

## 官方简介摘要

系统介绍 Kubernetes v1.36 中的 DRA 架构，包括资源建模、Scheduler 分配、Binding、Kubelet 准备、状态、健康度和访问边界；重点讨论 NUMA、PCIe、NVLink、Fabric 感知放置，以及千设备规模的 IMEX 分配案例。

## 为什么值得关注

AI/HPC 任务需要拓扑匹配的 GPU 和 NIC，而不是只满足设备数量。DRA 正是连接工作负载意图与物理通信拓扑的桥梁。

- 技术关键词：Kubernetes DRA、GPU、NIC、NUMA、PCIe、NVLink、Fabric、IMEX
- 学习主线：设备需求 → 拓扑感知分配 → NCCL/RDMA 性能

## 个人笔记

- 

