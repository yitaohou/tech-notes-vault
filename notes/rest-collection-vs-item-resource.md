---
title: REST Collection vs Item Resource
aliases: []
tags:
- concept
summary: REST 资源可分为集合资源（返回多个项，如 /products）和单个资源（返回具体一项，如 /products/{id}）两种形式。
created: '2026-08-26'
updated: '2026-08-26'
---

# REST Collection vs Item Resource

%% ytkb:def %%
REST 资源可分为集合资源（返回多个项，如 /products）和单个资源（返回具体一项，如 /products/{id}）两种形式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 请求 /api/products 返回整个产品集合，而请求 /products/{id} 则返回该 ID 对应的单个产品项，二者共用同一资源名但语义不同。（[63:13](https://youtu.be/oYxTTirKY8M?t=3793)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rest-noun-based-url-design]]
%% ytkb:end %%
