---
title: REST API Explicit Versioning
aliases: []
tags:
- concept
summary: RESTful API 通过在 URL 路径中包含版本号（如 V1、V2）来提供明确版本控制，重大升级时推出新版本号。
created: '2026-08-26'
updated: '2026-08-26'
---

# REST API Explicit Versioning

%% ytkb:def %%
RESTful API 通过在 URL 路径中包含版本号（如 V1、V2）来提供明确版本控制，重大升级时推出新版本号。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- RESTful API 通常在 URL 中包含版本号如 /v1/，进行重大升级时会推出 /v2/ 等新版本，提供明确的版本控制（explicit versioning）。（[36:06](https://youtu.be/oYxTTirKY8M?t=2166)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[graphql-schema-evolution-without-versioning]]
- [[restful-api-design]]
%% ytkb:end %%
