# Serving AI at Massive Scale: The Cloud-Native Inference Plane Behind Huawei Celia

- 时间：2026-09-09，11:00–11:30
- 地点 / 语言 / 难度：1F · Mandarin Hall I / 中文 / Intermediate
- 讲者：Kevin Wang
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1224671)
- Slides：官方暂未公开 / 待补
- 官方视频：[CNCF 官方大会录像播放列表](https://www.youtube.com/playlist?list=PLGcxfZT6qI-w)

## 官方简介摘要

介绍数万加速器规模下的多模态 PD 分离推理架构和生产结果，包括 PodGroup/SubGroup gang scheduling、Token-aware routing，以及 Prefill 与 Decode 的独立扩缩容。

## 为什么值得关注

它具体说明普通 Kubernetes Workload、Router 和 HPA 的假设为什么会在计算与带宽特征完全不同的 Prefill/Decode 阶段失效。

- 技术关键词：PD Disaggregation、TTFT、Token Routing、Gang Scheduling、Autoscaling、Inference Plane
- 学习主线：LLM 工作负载 → 推理平面 → 调度/路由 → 加速器

## 个人笔记

- 

