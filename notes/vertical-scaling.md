---
title: Vertical Scaling
aliases: []
tags:
- concept
summary: 通过提升单台机器的资源配置（如 CPU、内存）来应对更高负载的扩展方式，区别于增加机器数量的水平扩展。
created: '2026-08-26'
updated: '2026-08-26'
---

# Vertical Scaling

%% ytkb:def %%
通过提升单台机器的资源配置（如 CPU、内存）来应对更高负载的扩展方式，区别于增加机器数量的水平扩展。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 为了支持竞赛期间多达10万甚至百万级用户，可考虑的扩展方式之一是 vertical scaling，即通过提升单台服务器的资源来应对增长的负载。（[39:13](https://youtu.be/QBHTbtWSECg?t=2353)）
%% ytkb:end %%

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- vertical scaling 指不增加机器数量，而是把单台机器换成更强的机器（更多 RAM、CPU、存储），俗称「砸钱解决问题」。（[15:55](https://youtu.be/Qa-7iWxDz1A?t=955)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- vertical scaling（也称scale up）指为现有服务器增加RAM、CPU等资源来提升处理能力，实现简单，适合流量低到中等的应用。（[12:00](https://youtu.be/oYxTTirKY8M?t=720)）
- vertical scaling存在硬性资源上限（resource limits），单台服务器能升级的资源终会达到瓶颈，无法无限扩容。（[12:00](https://youtu.be/oYxTTirKY8M?t=720)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[combined-scaling-strategy]]
- [[horizontal-scaling]]
%% ytkb:end %%
