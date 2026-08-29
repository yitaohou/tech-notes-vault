---
title: Web Tier and Data Tier Separation
aliases: []
tags:
- concept
summary: 随着用户量增长，把处理 web/mobile 流量的 web tier 与负责管理数据库的 data tier 拆分开，使每一层可以根据各自的负载独立扩展的架构方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Web Tier and Data Tier Separation

%% ytkb:def %%
随着用户量增长，把处理 web/mobile 流量的 web tier 与负责管理数据库的 data tier 拆分开，使每一层可以根据各自的负载独立扩展的架构方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 将单体服务器拆分为 web tier 和 data tier 后，可以根据各层各自的负载分别进行扩展（scale），而不必整体一起扩容。（[06:00](https://youtu.be/oYxTTirKY8M?t=360)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[horizontal-scaling]]
- [[vertical-scaling]]
%% ytkb:end %%
