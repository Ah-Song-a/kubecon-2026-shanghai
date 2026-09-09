# Cilium: Up and Running

## 书目信息

- 官方英文书名：**Cilium: Up and Running**
- 作者：Nico Vibert、Filip Nikolic、James Laverack
- 出版社：O’Reilly Media
- 出版时间：2026 年 2 月
- 页数：官方页面标注 372 页；本地 PDF 文件为 373 页（包含封面等页面）
- 难度：Intermediate to Advanced
- ISBN：9798341622982
- [O’Reilly 官方阅读与购买页面](https://www.oreilly.com/library/view/cilium-up-and/9798341622982/)

## 为什么值得加入这份资料集锦

这本书比单场大会分享更适合作为 Cilium 的系统参考资料。它从 Kubernetes 网络和 Cilium 架构开始，继续覆盖 Datapath、Service Networking、Gateway API、性能优化、多集群、出口流量、安全策略和 Hubble 可观测性。

它与大会 Session **10 Years of Cilium: Connecting, Securing, and Simplifying the Cloud Native Stack** 形成互补：Session 用于了解项目最新方向和生产案例，本书用于补齐原理、配置与日常运维细节。

## 推荐阅读顺序

针对网络 → Kubernetes → AI Infra 的学习路线，建议优先阅读：

1. **Why Cilium?**：建立 Cilium 使用场景全景。
2. **Inside Cilium**：理解 Agent、Operator、eBPF Maps、Envoy 和 Hubble 的关系。
3. **The Cilium Datapath**：理解节点内与节点间的数据路径。
4. **Service Networking**：理解 kube-proxy replacement 与 Service 转发。
5. **Performance Networking and Traffic Optimization**：重点关注吞吐、延迟、Jitter 与高性能数据路径。
6. **Multicluster Networking**：连接跨集群 AI 平台和 GPU 资源池场景。
7. **Observability with Hubble**：连接网络可观测性与 AI Infra 排障。

## 与 AI Infra 的关联

```text
Cilium / eBPF Datapath
        │
        ├─ Kubernetes Service / Gateway
        ├─ Network Policy / Agent Sandbox Security
        ├─ Hubble Observability
        └─ Multicluster Networking
                    │
            分布式训练与推理流量
                    │
              GPU / RDMA 基础设施
```

## 版权说明

本仓库不收录整本 PDF。该书版权归作者及 O’Reilly Media 等权利人所有，请通过官方页面阅读或购买。用户本地持有的文件仅作为个人学习资料，不代表可以在公开 GitHub 仓库中再次分发。

