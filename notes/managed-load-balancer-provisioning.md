---
title: Managed Load Balancer Provisioning
aliases: []
tags:
- concept
summary: AWS、Google Cloud 等云服务商提供的能力，可在几秒钟内自动配置好一个负载均衡器，无需工程师手动搭建。
created: '2026-08-26'
updated: '2026-08-26'
---

# Managed Load Balancer Provisioning

%% ytkb:def %%
AWS、Google Cloud 等云服务商提供的能力，可在几秒钟内自动配置好一个负载均衡器，无需工程师手动搭建。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 实际工作中很少需要手动搭建负载均衡器，因为 AWS 或 Google Cloud 等主流云服务商都能在几秒钟内自动配置好一个负载均衡器。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 相比自行搭建配置软件或硬件负载均衡器，AWS Elastic Load Balancing 这类云托管负载均衡器配置更为简便，若服务器本身也部署在 AWS 上则更加方便。（[24:03](https://youtu.be/oYxTTirKY8M?t=1443)）
- 除 AWS 外，Azure 和 Google Cloud 也提供与 Elastic Load Balancing 类似的云托管负载均衡服务。（[24:03](https://youtu.be/oYxTTirKY8M?t=1443)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[autoscaling]]
- [[health-check-load-balancing]]
- [[load-balancer]]
%% ytkb:end %%
