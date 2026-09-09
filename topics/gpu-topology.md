# GPU 拓扑

仅满足设备数量并不够。性能取决于 GPU↔GPU 和 GPU↔NIC 在 NUMA、PCIe、NVLink 与外部 Fabric 上的关系。

```text
工作负载申请 → 选择 GPU + NIC → NUMA/PCIe Locality
             → NVLink/RDMA 路径 → NCCL 性能
```

建议阅读：[Kubernetes DRA](../sessions/12-kubernetes-dra.md)、[弹性 GPU 计算池](../sessions/07-elastic-gpu-compute-pool.md)、[Advanced NCCL](../sessions/01-advanced-nccl-tutorial.md)。

