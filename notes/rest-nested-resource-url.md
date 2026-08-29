---
title: REST Nested Resource URL
aliases: []
tags:
- concept
summary: 用于表达资源间从属关系的 URL 设计方式，把子资源路径嵌套在父资源 ID 之后。
created: '2026-08-26'
updated: '2026-08-26'
---

# REST Nested Resource URL

%% ytkb:def %%
用于表达资源间从属关系的 URL 设计方式，把子资源路径嵌套在父资源 ID 之后。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 要获取某个特定产品的评论，可以设计嵌套路径 /products/{id}/reviews，请求该路径即可返回该产品对应的评论集合。（[63:13](https://youtu.be/oYxTTirKY8M?t=3793)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rest-collection-vs-item-resource]]
%% ytkb:end %%
