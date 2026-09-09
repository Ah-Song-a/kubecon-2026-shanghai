# Beyond Model Sharding: Atomic Scheduling and Disaggregated LLM Serving with LeaderWorkerSet

- 时间：2026-09-08，13:45–14:15（UTC+8）
- 地点 / 语言：5F · 5B + C / 中文
- 讲者：Kay Yan、Chen Zicong
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1222146)
- Slides：[原始 PDF](../slides/beyond-model-sharding-leaderworkerset.pdf) · [官方下载](https://sessionize.com/download/vgayseh~7WqizQY5Mfk3vudj2dh8Bh.pdf~beyond-model-sharding-atomic-scheduling-and-disaggregated-llm-serving-with-leaderworkerset.pdf)
- 官方视频：待补

## 官方简介摘要

介绍如何使用 LeaderWorkerSet（LWS）把跨节点、跨 GPU 的多个 Pod 作为一个完整推理工作单元管理。重点包括 Gang Scheduling、PodGroup 与 Volcano、scheduler-plugins、YuniKorn 的集成，以及使用 DisaggregatedSet 协调 Prefill 和 Decode 两组 LWS 资源。

## 为什么必须关注

普通 Deployment 不理解分布式推理副本的整体性。只调度部分 Pod 会占用加速器却无法提供服务；PD 分离后，滚动升级、扩缩容和拓扑错配还会进一步影响延迟与 GPU 利用率。这场正好连接 vLLM/SGLang、Kubernetes 调度与 GPU 网络拓扑。

- 技术关键词：LeaderWorkerSet、LWS、Gang Scheduling、PodGroup、DisaggregatedSet、Prefill/Decode、Volcano
- 学习主线：分布式推理 → 工作负载原子性 → Gang Scheduling → GPU/网络拓扑

## 个人笔记

- 

