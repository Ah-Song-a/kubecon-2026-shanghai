# KubeCon China 2026 — AI Infra 资料集锦

这是 **KubeCon + CloudNativeCon + OpenInfra Summit + PyTorch Conference China 2026**（上海，2026 年 9 月 8–9 日）的个人学习资料存档。仓库严格依据两天的官方议程整理，重点覆盖 AI 基础设施、GPU 通信与拓扑、Kubernetes 调度、LLM 推理、KV Cache 和可观测性。

## 快速入口

- [9 月 8 日议程](agenda/2026-09-08.md) · [9 月 9 日议程](agenda/2026-09-09.md)
- [Slides 原文件清单](slides/README.md)
- 延伸资料：[Cilium: Up and Running](resources/cilium-up-and-running.md)
- 专题：[NCCL/RDMA](topics/nccl-rdma.md) · [GPU 拓扑](topics/gpu-topology.md) · [LLM 推理](topics/llm-inference.md) · [KV Cache](topics/kv-cache.md) · [GPU 调度](topics/gpu-scheduling.md) · [可观测性](topics/observability.md)

## 学习主线

```text
PyTorch / AI 工作负载
        ├─ 训练 ─ NCCL ─ NVLink / RDMA ─ 容错
        │                    │
        │              GPU / NIC 拓扑
        │                    │
        └─ 推理 ─ PD 分离 / KV Cache
                         │
                Kubernetes DRA / Volcano
                         │
              Token → Runtime → GPU 可观测性
```

## 精选 Session

| 日期 | 官方英文标题 | 为什么值得关注 | Slides |
|---|---|---|---|
| 9 月 8 日 | [Advanced NCCL Tutorial: Beyond Collectives](sessions/01-advanced-nccl-tutorial.md) | 对称内存、GIN、NVLink 域内与跨节点通信 | [PDF](slides/advanced-nccl-tutorial.pdf) |
| 9 月 8 日 | [10 Years of Cilium: Connecting, Securing, and Simplifying the Cloud Native Stack](sessions/02-cilium-10-years.md) | eBPF 网络、可观测性与 AI Agent 安全 | 暂未公开 |
| 9 月 8 日 | [Evolving Argo Workflows for AI: New Features, Tuning, and Multi-Tenant Isolation](sessions/03-argo-workflows-for-ai.md) | 大规模 AI 流水线、调优和租户隔离 | 暂未公开 |
| 9 月 8 日 | [Gravity of Ecosystems: Pollinating the Modern AI Orchestrator](sessions/04-modern-ai-orchestrator.md) | DRA、Workload API、Ray、Slurm 与 PyTorch | 暂未公开 |
| 9 月 9 日 | [Serving AI at Massive Scale: The Cloud-Native Inference Plane Behind Huawei Celia](sessions/05-huawei-celia-inference-plane.md) | 万卡级 PD 分离推理基础设施 | 暂未公开 |
| 9 月 9 日 | [Training Through Failures: How Meta Keeps 100k-GPU Jobs Alive with Open-Source Fault Tolerance](sessions/06-meta-100k-gpu-fault-tolerance.md) | NCCL communicator 恢复与 RDMA checkpoint | 暂未公开 |
| 9 月 9 日 | [Turning Fragmented GPU Clusters Into One Elastic Compute Pool](sessions/07-elastic-gpu-compute-pool.md) | 多集群 DRA/Kueue 与拓扑感知放置 | [PDF](slides/turning-fragmented-gpu-clusters-into-one-elastic-compute-pool.pdf) |
| 9 月 9 日 | [To Cache or Not to Cache? A Tiered KVCache Storage System for Agent Scenarios](sessions/08-tiered-kvcache.md) | Agent 场景的缓存分层与生命周期管理 | 暂未公开 |
| 9 月 9 日 | [End-to-End Observability for LLM Inference: From Token to GPU](sessions/09-llm-observability-token-to-gpu.md) | 将 TTFT/TPOT/ITL 一路关联到 GPU | [PDF](slides/end-to-end-observability-for-llm-inference.pdf) |
| 9 月 9 日 | [vLLM KV Cache Management: From Cache Reuse to Agent Scenario Optimization](sessions/10-vllm-kv-cache.md) | Prefix 复用、Offload、LRU/ARC | 暂未公开 |
| 9 月 9 日 | [Why Your TTFT Lies: Diagnosing PD-Disaggregated LLM Inference with Minimal Cross-Layer Metrics](sessions/11-why-your-ttft-lies.md) | 指标 → 根因 → 调优动作 | [PPTX](slides/why-your-ttft-lies.pptx) |
| 9 月 9 日 | [Kubernetes DRA Architecture: Scheduling, Status, and Topology at Scale](sessions/12-kubernetes-dra.md) | GPU/NIC/NUMA/PCIe/NVLink 拓扑感知分配 | [PDF](slides/kubernetes-dra-architecture-v1.1.pdf) |
| 9 月 9 日 | [Volcano: A Unified Scheduling Platform for Cloud Native AI](sessions/13-volcano-unified-scheduling.md) | 统一调度训练、推理和 Agent | 暂未公开 |
| 9 月 8 日 | [Beyond Model Sharding: Atomic Scheduling and Disaggregated LLM Serving with LeaderWorkerSet](sessions/14-leaderworkerset-disaggregated-serving.md) | LWS、Gang Scheduling 与 PD 分离推理原子调度 | [PDF](slides/beyond-model-sharding-leaderworkerset.pdf) |
| 9 月 9 日 | [Beyond Static Pods: Dynamic GPU Sharing and Low-Latency Model Switching for LLM Inference on K8s](sessions/15-dynamic-gpu-sharing.md) | 动态 GPU 共享与秒级模型切换 | 暂未公开 |
| 9 月 9 日 | [Non-Invasive AI Agent Observability With OBI](sessions/16-obi-agent-observability.md) | eBPF 无侵入观测 MCP 与 Agent 工具调用 | [PDF](slides/non-invasive-ai-agent-observability-with-obi.pdf) |
| 9 月 8 日 | [Zero-Trust Traffic Governance For Kubernetes AI Agent Sandboxes](sessions/17-zero-trust-agent-sandbox-traffic.md) | Agent Sandbox 出站流量、身份、凭据与审计治理 | [PDF](slides/zero-trust-traffic-governance-for-kubernetes-ai-agent-sandboxes.pdf) |
| 9 月 9 日 | [What We Learned Securing AI Agents at Scale on Multi-Tenant Kubernetes Clusters](sessions/18-securing-ai-agents-multi-tenant-kubernetes.md) | 多租户 Agent 的微虚机、身份、网络和准入纵深防御 | [PDF](slides/securing-ai-agents-at-scale-multi-tenant-kubernetes.pdf) |
| 9 月 9 日 | [Pathless First: Redefining runc Container Security Against ProcFS-Based Attacks](sessions/19-pathless-first-runc-security.md) | Agent Sandbox 底层 runc 与 ProcFS 逃逸防护 | [PDF](slides/pathless-first-runc-container-security.pdf) |
| 9 月 9 日 | [A Cloud Native Stack from Bare Metal to Tokens for Large-Scale AI Inference](sessions/20-cloud-native-stack-bare-metal-to-tokens.md) | 从多代异构 GPU、裸机和资源池一路构建 Token-as-a-Service | [PDF](slides/cloud-native-stack-bare-metal-to-tokens.pdf) |
| 9 月 9 日 | [Escaping the Vendor Trap: A Journey for Migrating Legacy Infrastructure to OpenStack and K8s](sessions/21-escaping-vendor-trap-openstack-kubernetes.md) | 从 VMware 迁移至 OpenStack、Ceph 与 Kubernetes 的大规模实践 | [PDF](slides/escaping-vendor-trap-openstack-kubernetes.pdf) |
| 9 月 8 日 | [From Containers to Agents: The Next Cloud Native](sessions/22-from-containers-to-agents.md) | 把 Agent 建模为具备身份、状态、权限和策略的新型云原生工作负载 | [PDF](slides/from-containers-to-agents.pdf) |
| 9 月 8 日 | [8 Million Tasks Daily: Driving Efficiency in Multi-Tenant Data Platforms at Horizon Robotics](sessions/23-horizon-8-million-tasks.md) | 每日 800 万任务下的 Argo、Volcano、Kueue 控制面实践 | [PDF](slides/horizon-8-million-tasks.pdf) |
| 9 月 8 日 | [Declarative Underlays: Scaling Purpose-Built Infrastructure(Clusters) for OpenStack with Cluster API](sessions/24-declarative-underlays-openstack-cluster-api.md) | 用 CAPI 声明式管理 GPU、高速网络和存储专用底层集群 | [PDF](slides/declarative-underlays-openstack-cluster-api.pdf) |
| 9 月 8 日 | [⚡ Before vLLM starts: Preflight Checks for LWS for LLM Inference on K8S](sessions/25-vllm-preflight-lws.md) | 在推理启动前验证 NCCL、拓扑和连通性，尽早阻断隐性故障 | [PPTX](slides/vllm-preflight-lws.pptx) |
| 9 月 9 日 | [KV Cache: Accelerating AI inference on Intel CPU](sessions/26-kv-cache-intel-cpu.md) | 用 DDR、存储卸载和 QAT 压缩扩展 KV Cache 层级 | [PDF](slides/kv-cache-intel-cpu.pdf) |
| 9 月 9 日 | [Secure AI Agent Sandboxing with OpenStack Zun and Kata Container](sessions/27-secure-ai-agent-sandbox-openstack-zun-kata.md) | Zun、Kata、Glance 与 Neutron 组成 Agent 执行安全边界 | [PDF](slides/secure-ai-agent-sandbox-openstack-zun-kata.pdf) |
| 9 月 9 日 | [vLLM-Helion: SOTA LLM Performance by advanced autotuning and fine-grained dispatching](sessions/28-vllm-helion.md) | Kernel 离线自动调优与运行时细粒度配置分派 | [PDF](slides/vllm-helion.pdf) |

## 来源和版权

- 信息来自官方 [9 月 8 日](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?date=tue-sep-8)及[9 月 9 日](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?date=wed-sep-9)议程。
- Session 简介是对官方摘要的合规概括，不是整段复制。
- 只镜像官方议程明确提供下载的 Slides；视频发布前统一标记为“待补”，后续可关注 [CNCF YouTube](https://www.youtube.com/@cncf)。
- Slides 版权归相应讲者及权利人所有。文件仅供学习与资料参考；公开 GitHub 仓库前应逐份确认再分发许可。许可不明确时，请删除二进制文件，仅保留官方下载链接。
- 完整商业书籍不上传到仓库，只记录书目信息、官方入口和推荐阅读路线。

## 后续维护

1. 在各 Session 的“个人笔记”中补充现场收获。
2. 官方录像发布后更新视频链接。
3. 公开前重新检查新增 Slides 和再分发许可。
