---
title: API Abstraction / Implementation Hiding
aliases: []
tags:
- concept
summary: API 作为一种抽象机制，对调用方隐藏内部实现细节，只对外暴露可用的功能接口。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Abstraction / Implementation Hiding

%% ytkb:def %%
API 作为一种抽象机制，对调用方隐藏内部实现细节，只对外暴露可用的功能接口。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 调用方通过 API 发起请求（例如保存用户数据）时完全不需要了解服务端内部的实现逻辑，只需使用提供好的 endpoint 即可完成操作。（[30:03](https://youtu.be/oYxTTirKY8M?t=1803)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-definition]]
%% ytkb:end %%
