---
title: Docker Compose
aliases: []
tags:
- concept
summary: 用于通过单一命令定义并启动由多个容器组成的应用（如多个 Golang 服务加一个 Nginx 反向代理）的工具。
created: '2026-08-26'
updated: '2026-08-26'
---

# Docker Compose

%% ytkb:def %%
用于通过单一命令定义并启动由多个容器组成的应用（如多个 Golang 服务加一个 Nginx 反向代理）的工具。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-containerization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 该演示使用 docker compose up 一次性启动三个完全相同代码的 Golang 服务和一个作为负载均衡器的 Nginx，用于直观展示不同负载均衡算法的效果。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 理想情况下前端工程师应具备用 Nginx 和 Docker Compose 在本地机器上手动搭建一个小型负载均衡器的能力，以此证明自己能推理清楚其工作原理。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[load-balancer]]
- [[nginx-upstream-block]]
%% ytkb:end %%
