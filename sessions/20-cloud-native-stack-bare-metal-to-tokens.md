# A Cloud Native Stack from Bare Metal to Tokens for Large-Scale AI Inference

- 时间：2026-09-09，10:00–10:05（UTC+8）
- 地点 / 语言：7F · Grand Ballroom II + III / 英文
- 讲者：Trong Vinh Nguyen
- 类型：Keynote Session
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1308448)
- Slides：[原始 PDF](../slides/cloud-native-stack-bare-metal-to-tokens.pdf) · [官方下载](https://sessionize.com/download/iwvabbeb~JtLQi6m8kTTM9XEAGaKDgz.pdf~viettel-ai-platform-2026.pdf)
- 官方视频：待补

## 官方简介摘要

介绍如何将多个采购周期积累的 T4、L40S、A100、H200、B200 等异构 GPU，整合为统一的大规模推理平台。整体架构分为三层：使用 OpenInfra Foundation 生态管理裸机，使用 CNCF 工具完成 GPU Pooling 与多租户切分，再利用 PyTorch Foundation 项目优化模型服务，最终形成 Token-as-a-Service 平台。

## 为什么值得关注

这场虽然只有五分钟，却提供了从物理硬件到 Token 服务的完整纵向视角。它讨论的不是理想化同构集群，而是现实中多代 GPU、不同显存容量、算力特征和驱动要求并存时，如何提高存量设备利用率。

- 技术关键词：Bare Metal、OIF、CNCF、PyTorch、GPU Pooling、Multi-tenancy、T4、L40S、A100、H200、B200、Token-as-a-Service
- 学习主线：异构 GPU → 裸机资源层 → 云原生资源池 → 推理优化 → Token 服务

## 与其他 Session 的关系

建议结合 [Turning Fragmented GPU Clusters Into One Elastic Compute Pool](07-elastic-gpu-compute-pool.md)、[Kubernetes DRA Architecture](12-kubernetes-dra.md) 和 [Huawei Celia Inference Plane](05-huawei-celia-inference-plane.md) 阅读。

## 个人笔记

- 

