---
title: Status Code Selection Best Practice
aliases: []
tags:
- concept
summary: RESTful API 设计中要求根据请求的实际处理结果精确匹配对应状态码的最佳实践。
created: '2026-08-26'
updated: '2026-08-26'
---

# Status Code Selection Best Practice

%% ytkb:def %%
RESTful API 设计中要求根据请求的实际处理结果精确匹配对应状态码的最佳实践。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 设计 REST API 时应根据每个操作的实际结果选用最贴切的状态码（如创建用 201、查询成功用 200、未找到用 404），而不是笼统地都返回同一个状态码。（[72:17](https://youtu.be/oYxTTirKY8M?t=4337)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[http-status-code-categories]]
- [[restful-api-design]]
%% ytkb:end %%
