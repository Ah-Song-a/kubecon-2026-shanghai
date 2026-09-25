# Pathless First: Redefining runc Container Security Against ProcFS-Based Attacks

- 时间：2026-09-09，11:00–11:30（UTC+8）
- 地点 / 语言 / 难度：1F · Mandarin Hall II / 中文 / Intermediate
- 讲者：Fubang Li
- Track：Security + Privacy + Trusted Computing
- [官方 Session 页面](https://www.lfopensource.cn/kubecon-cloudnativecon-openinfra-summit-pytorch-conference-china/program/schedule/?id=1224844)
- Slides：[原始 PDF](../slides/pathless-first-runc-container-security.pdf) · [官方下载](https://sessionize.com/download/powuy~ReFLDezCLCUwpTkPzRqtMo.pdf~kubecon2026-pathless-first.pdf)
- 代码：[opencontainers/runc](https://github.com/opencontainers/runc)
- 讲者网站：[lifubang.github.io/acm](https://lifubang.github.io/acm/)
- 官方视频：[CNCF YouTube](https://www.youtube.com/watch?v=nH2fwO0WyFg)

## 官方简介摘要

回顾 runc 中从 TOCTOU 符号链接劫持到 Bind Mount Escape 的 ProcFS 路径攻击，并介绍 Pathless Container Setup（PCS）的 File Descriptor-Centric 设计。PCS 使用 `fsopen`、`fsmount` 等现代 Linux Pathless Mount API，减少依赖攻击者可控的环境路径解析。

## 为什么值得关注

这场不直接讨论 AI 推理，但属于 Agent Sandbox 的底层可信计算基础。其设计已经进入 runc，并用于缓解已知路径相关 CVE，适合作为容器 Runtime 安全的扩展阅读。

- 技术关键词：runc、ProcFS、TOCTOU、Bind Mount Escape、PCS、fsopen、fsmount、Container Runtime
- 学习主线：Agent Sandbox → 容器 Runtime → Mount/Path Resolution → 逃逸防护

## 个人笔记

- 
