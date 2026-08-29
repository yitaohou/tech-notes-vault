---
title: Container Orchestration Services
aliases: []
tags:
- concept
summary: 云服务商提供的用于管理和编排 container 集群的托管服务，例如 AWS 的 ECS、EKS 以及 Google 主导开发的 Kubernetes。
created: '2026-08-26'
updated: '2026-08-26'
---

# Container Orchestration Services

%% ytkb:def %%
云服务商提供的用于管理和编排 container 集群的托管服务，例如 AWS 的 ECS、EKS 以及 Google 主导开发的 Kubernetes。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-containerization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- AWS 提供 ECS、EKS 等 elastic container service，而 Kubernetes 则是由 Google 主导开发的另一款流行容器编排系统，二者都能用于管理 container 化的部署。（[27:08](https://youtu.be/QBHTbtWSECg?t=1628)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- DevOps 团队可以把打包好的 Docker image 推送到容器编排系统的部署管线中运行，编排系统负责处理负载均衡、并行运行多个容器实例，以及容器故障后快速拉起新实例等复杂工作。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[container-elastic-scaling]]
- [[docker]]
- [[kubernetes-container-orchestration]]
%% ytkb:end %%
