# GPU 调度

调度栈涉及多个层次：

```text
设备分配：Kubernetes DRA
工作负载与队列语义：Workload API、Kueue、Volcano
全局容量：Federation 与多集群弹性计算池
应用层：训练、PD 推理、Agent Runtime
```

建议阅读：[Modern AI Orchestrator](../sessions/04-modern-ai-orchestrator.md)、[Kubernetes DRA](../sessions/12-kubernetes-dra.md)、[Volcano](../sessions/13-volcano-unified-scheduling.md)。

