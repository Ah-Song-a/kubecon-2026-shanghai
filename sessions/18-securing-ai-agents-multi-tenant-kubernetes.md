# What We Learned Securing AI Agents at Scale on Multi-Tenant Kubernetes Clusters

- 时间：2026-09-09，16:15–16:45（UTC+8）
- 地点 / 语言：7F · Grand Ballroom II + III / 中文
- 讲者：Pengfei Ni
- Track：AI + ML + Agentic AI + Data Systems
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1218010)
- Slides：[原始 PDF](../slides/securing-ai-agents-at-scale-multi-tenant-kubernetes.pdf) · [官方下载](https://sessionize.com/download/ilzawiv~4MTg7dwnN4m6TLkGTZpAu7.pdf~what-we-learned-securing-ai-agents-at-scale-on-multi-tenant-kubernetes-clusters.pdf)
- 官方视频：[CNCF YouTube](https://www.youtube.com/watch?v=Iio1IklYFi4)

## 官方简介摘要

分享一个服务数百名工程师的多租户 Agent 平台如何建立纵深防御：使用 Kata Containers 为 Agent 提供独立内核；通过 OIDC Federation 为每个 Agent 实例分配与所有者绑定的云身份；利用 NetworkPolicy 阻断 IMDS 与横向移动；用 ValidatingAdmissionPolicy 防止 Exec 逃逸，并通过治理规则、爆炸半径限制和完整审计控制风险。

## 为什么值得关注

Namespace、RBAC 和 NetworkPolicy 原本主要面向相互协作的工作负载，而 Agent 会执行任意代码、调用 MCP 工具、持有云凭据并自主作出网络决策。这场展示了把微虚机隔离、身份、网络策略、准入控制和审计组合为完整 Agent 安全边界的方法。

- 技术关键词：Kata Containers、OIDC Federation、Agent Identity、NetworkPolicy、IMDS、ValidatingAdmissionPolicy、MCP、Audit
- 学习主线：多租户 Agent → 运行时隔离 → 独立身份 → 网络与准入策略 → 审计

## 个人笔记

- 
