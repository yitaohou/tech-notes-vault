---
title: VPC Private Network Isolation
aliases: []
tags:
- concept
summary: 将系统内部所有服务部署在私有虚拟网络（VPC）中、不对外暴露端口，从而阻止外部直接访问服务的架构方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# VPC Private Network Isolation

%% ytkb:def %%
将系统内部所有服务部署在私有虚拟网络（VPC）中、不对外暴露端口，从而阻止外部直接访问服务的架构方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 引入 API Gateway 后，所有内部服务被部署在私有虚拟网络（VPC）中，不再对外暴露端口，其 IP 仅在网络内部可达。（[21:05](https://youtu.be/Qa-7iWxDz1A?t=1265)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 有了 API gateway 后，后端微服务通常部署在 VPC（虚拟私有云）内，外部唯一能进入的入口就是 API gateway，从而保证安全性。（[09:03](https://youtu.be/KuClyhvSzXk?t=543)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-gateway]]
- [[gateway-single-entry-point]]
%% ytkb:end %%
