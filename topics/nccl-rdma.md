# NCCL 与 RDMA

NCCL 是连接 GPU 本地计算与大规模训练、MoE 推理的通信层。本次学习主线为：

```text
对称 GPU 内存 → GPU-Initiated Networking → NVLink 域
       → NIC / RDMA Fabric → Communicator 容错
```

建议依次阅读：[Advanced NCCL](../sessions/01-advanced-nccl-tutorial.md)、[Meta 超大规模训练容错](../sessions/06-meta-100k-gpu-fault-tolerance.md)、[TTFT 诊断](../sessions/11-why-your-ttft-lies.md)。

