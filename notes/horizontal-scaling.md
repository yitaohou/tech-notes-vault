---
title: Horizontal Scaling
aliases: []
tags:
- concept
summary: 通过增加更多服务器实例而非单纯增强单机硬件来应对负载增长的系统扩展方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Horizontal Scaling

%% ytkb:def %%
通过增加更多服务器实例而非单纯增强单机硬件来应对负载增长的系统扩展方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 面对用户数持续增长，单纯升级单机的 CPU 和内存并非长期方案，因为算力堆叠终会无法满足需求，更优做法是水平扩展系统，用多台服务器分摊负载。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
%% ytkb:end %%

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 对无状态服务器做横向扩展（增加实例数量）看似简单，但若数据与实例本地耦合，多实例间会出现数据重复且互不感知的问题。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
- horizontal scaling 指往集群中增加更多机器，每台机器独立运算、拥有独立资源，可以分别服务不同用户或用户集群。（[15:20](https://youtu.be/Qa-7iWxDz1A?t=920)）
- API Gateway 本身也可以像其他服务一样进行水平扩展或垂直扩展，以应对其成为瓶颈的风险。（[21:05](https://youtu.be/Qa-7iWxDz1A?t=1265)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 在负载均衡器的支持下，向系统新增第四台或更多服务器后，负载均衡器会自动把新服务器纳入流量分配范围，确保各实例负载均匀，从而提升系统的可扩展性。（[15:01](https://youtu.be/oYxTTirKY8M?t=901)）
- horizontal scaling（也称scale out）指复制多台相同服务器、将请求负载分摊到这些服务器上，而不是让单台服务器处理全部请求。（[12:00](https://youtu.be/oYxTTirKY8M?t=720)）
- horizontal scaling具备更高的容错能力（fault tolerance）：即使某台服务器宕机，其余服务器仍可继续为用户提供服务，同时故障服务器可以恢复。（[12:00](https://youtu.be/oYxTTirKY8M?t=720)）
- horizontal scaling具备更好的可扩展性：可以根据需要随时增加服务器数量（如从三台增至四台）来承接新增流量。（[12:00](https://youtu.be/oYxTTirKY8M?t=720)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-gateway]]
- [[autoscaling]]
- [[data-coupled-server-scaling-problem]]
- [[data-synchronization-problem-scaling]]
- [[fault-tolerance-requirement]]
- [[load-balancer]]
- [[per-language-runtime-containers]]
- [[runtime-service-capacity-estimation]]
- [[single-point-of-failure]]
- [[vertical-scaling]]
%% ytkb:end %%
