# ⚡ Before vLLM starts: Preflight Checks for LWS for LLM Inference on K8S

- 时间：2026-09-08，17:04–17:09（UTC+8）
- 地点 / 语言：7F · Pearl Hall / 英文
- 讲者：Peter Pan
- 类型 / 难度：Lightning Talk / Intermediate
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1220735)
- Slides：[原始 PPTX](../slides/vllm-preflight-lws.pptx) · [官方下载](https://sessionize.com/download/ipcabzec~pCjHasFF5EvMw5K29jsEgj.pptx~kubecon-2026-peter-preflight-and-lws.pptx)
- 相关实现：[LWS PR #813](https://github.com/kubernetes-sigs/lws/pull/813)
- 官方视频：待补

## 官方简介摘要

为基于 LeaderWorkerSet 的分布式 vLLM 推理设计启动前检查门禁：在 init container 中验证 NCCL、拓扑和节点连通性，异常时尽早失败，并依据故障类型决定重试、重新调度或停止。重点讨论 init 阶段节点发现、无限重建循环和终止失败边界。

## 为什么值得关注

分布式推理最昂贵的问题往往不是无法启动，而是启动后才暴露吞吐抖动、P99 延迟和跨节点性能退化。这份检查清单将 NCCL/RDMA、拓扑和 LWS 生命周期真正连接到生产发布门禁。

- 技术关键词：vLLM、LeaderWorkerSet、Init Container、NCCL、Topology、Preflight、Failure Policy
- 学习主线：GPU/网络拓扑 → 启动前验证 → LWS 生命周期 → 推理可靠性

## 个人笔记

- 

