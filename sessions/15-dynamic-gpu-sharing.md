# Beyond Static Pods: Dynamic GPU Sharing and Low-Latency Model Switching for LLM Inference on K8s

- 时间：2026-09-09，13:45–14:15（UTC+8）
- 地点 / 语言：1F · Mandarin Hall II / 中文
- 讲者：Xining Wang、Jun Duan
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1218005)
- Slides：官方暂未公开 / 待补
- 官方视频：待补

## 官方简介摘要

介绍 llm-d 孵化项目 Fast Model Actuation（FMA）：通过 Dual Pods 解耦 GPU 资源声明与模型执行，结合 vLLM Sleep/Wake 和常驻 Multi-Instance Launcher，将模型切换时间从分钟级降低到秒级，实现 GPU 时间片共享。

## 为什么必须关注

它直接处理大规模 MaaS 平台的核心矛盾：模型数量和流量变化巨大，而 GPU 昂贵。传统 Pod 级模型切换慢、无流量模型仍占用 GPU；FMA 展示了一种提高利用率同时保持 TTFT/TPOT SLO 的 Kubernetes 实现。

- 技术关键词：FMA、llm-d、Dual Pods、GPU Sharing、vLLM Sleep/Wake、Model Switching、TTFT、TPOT
- 学习主线：GPU 配额 → 动态执行 → 快速模型切换 → 利用率与延迟

## 个人笔记

- 

