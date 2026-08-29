---
title: Uneven Load Distribution Degrades User Experience
aliases: []
tags:
- concept
summary: 在多服务器场景下，如果请求没有被合理分配，导致大部分用户集中打到同一台服务器、而另一台资源空闲，会让被过度请求的服务器上的用户体验变差。
created: '2026-08-26'
updated: '2026-08-26'
---

# Uneven Load Distribution Degrades User Experience

%% ytkb:def %%
在多服务器场景下，如果请求没有被合理分配，导致大部分用户集中打到同一台服务器、而另一台资源空闲，会让被过度请求的服务器上的用户体验变差。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 举例说明：如果大多数用户的请求都涌向其中一台服务器，而另一台还有大量空闲资源，被拥堵的那台服务器上的用户就会遭遇响应变慢等体验下降的问题，原因正是缺少合理的请求分配机制。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[load-balancer-need-multi-server]]
%% ytkb:end %%
