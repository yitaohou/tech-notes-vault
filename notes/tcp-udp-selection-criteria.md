---
title: TCP vs UDP Selection Criteria
aliases: []
tags:
- concept
summary: 根据应用对可靠性与速度的不同需求，在 TCP 与 UDP 之间做选择的判断标准。
created: '2026-08-26'
updated: '2026-08-26'
---

# TCP vs UDP Selection Criteria

%% ytkb:def %%
根据应用对可靠性与速度的不同需求，在 TCP 与 UDP 之间做选择的判断标准。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-networking-protocols]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 选择协议时的核心判断标准是：若需要连接安全可靠则选 TCP；若需要快速轻量、可以接受一定数据丢失则选 UDP。（[60:11](https://youtu.be/oYxTTirKY8M?t=3611)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[tcp-protocol]]
- [[udp-protocol]]
%% ytkb:end %%
