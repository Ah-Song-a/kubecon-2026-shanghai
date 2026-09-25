# Zero-Trust Traffic Governance For Kubernetes AI Agent Sandboxes

- 时间：2026-09-08，13:45–14:15（UTC+8）
- 地点 / 语言 / 难度：1F · Mandarin Hall II / 中文 / Intermediate
- 讲者：Bingshen Wang、Bo Kang Li
- Track：Networking + Edge + Distributed Systems
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1221856)
- Slides：[原始 PDF](../slides/zero-trust-traffic-governance-for-kubernetes-ai-agent-sandboxes.pdf) · [官方下载](https://sessionize.com/download/ioyjayxe~SGt9nR1NtS54hTts9Bb8dy.pdf~zero-trust_traffic_governance_for_kubernetes_ai_agent_sandboxes.pdf)
- 官方视频：[CNCF YouTube](https://www.youtube.com/watch?v=E2GxX4VeWD8)

## 官方简介摘要

将 Kubernetes 中的 AI Agent Sandbox 出站访问视为零信任流量治理问题：每个请求都需要明确的目标、身份、凭据边界和审计记录。内容涵盖按域名、服务和网络目标限制流量，将平台级 Guardrail 与租户 Allowlist 结合，并处理 DNS 变化、首包时序和短生命周期 Sandbox 带来的挑战。

同一控制路径还承担身份注入、Token 替换、LLM 请求审计，以及强制经由内部模型网关转发等能力，同时避免为每个 Sandbox 部署重量级 Sidecar。

## 为什么值得关注

Agent 会执行动态生成的代码、运行时选择工具、访问外部模型/API，并使用不应直接暴露给 Sandbox 的凭据。传统静态网络 Allowlist 无法完整处理这些风险。这场分享将网络治理、身份、Secret 隔离、模型网关和审计整合成一条生产控制路径。

- 技术关键词：Zero Trust、AI Agent Sandbox、Egress、Allowlist、Identity Injection、Token Replacement、LLM Audit、Model Gateway、DNS
- 学习主线：Agent Sandbox → 出站流量治理 → 身份/凭据边界 → 审计与模型网关

## 与其他 Session 的关系

```text
Agent Runtime / Sandbox
        ├─ Cilium / eBPF 网络数据面
        ├─ Zero-Trust Egress 治理
        ├─ 身份与凭据注入
        └─ OBI / OpenTelemetry 可观测性
```

建议结合 [10 Years of Cilium](02-cilium-10-years.md) 和 [Non-Invasive AI Agent Observability With OBI](16-obi-agent-observability.md) 一起阅读。

## 个人笔记

- 
