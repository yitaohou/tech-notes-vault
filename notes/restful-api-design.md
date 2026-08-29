---
title: RESTful API Design
aliases: []
tags:
- concept
summary: 使用符合 REST 规范的 HTTP 方法与资源化 URL 来设计系统对外查询与操作接口的实践。
created: '2026-08-26'
updated: '2026-08-26'
---

# RESTful API Design

%% ytkb:def %%
使用符合 REST 规范的 HTTP 方法与资源化 URL 来设计系统对外查询与操作接口的实践。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 系统的 API 路由被设计为 RESTful API 端点，用于定义获取题目列表、过滤题目等各类查询操作。（[13:10](https://youtu.be/QBHTbtWSECg?t=790)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 一个典型的 REST 风格接口示例是 GET /product/{id}，用于获取某个产品的详情，服务端返回的 JSON 中通常包含 ID、名称、描述、价格等元数据字段供客户端展示。（[03:00](https://youtu.be/oYxTTirKY8M?t=180)）
- REST（Representational State Transfer）是一种以资源为中心，并借助 HTTP 方法作为通信协议的 API 风格，是目前最常用的 API 风格。（[30:03](https://youtu.be/oYxTTirKY8M?t=1803)）
- REST 是三种主流 API 风格中最常用的一种，通常被用在 Web 和移动应用（mobile applications）中。（[33:05](https://youtu.be/oYxTTirKY8M?t=1985)）
- REST 使用标准 HTTP 方法（如 GET）来定义具体操作类型，且其响应结构（response structure）是固定的。（[33:05](https://youtu.be/oYxTTirKY8M?t=1985)）
- HTTP 协议自带的 status code 机制天然适合搭配 RESTful API 中的 CRUD 操作，因此 RESTful API 通常选择 HTTP 作为底层协议。（[41:20](https://youtu.be/oYxTTirKY8M?t=2480)）
- REST 是系统间通过标准 HTTP 方法通信的架构风格，是当前开发者构建和消费 API 最常见的方式。（[63:13](https://youtu.be/oYxTTirKY8M?t=3793)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-protocol-design-influence]]
- [[graphql]]
- [[grpc-rpc-framework]]
- [[http-methods-crud-mapping]]
- [[mobile-api-json-response]]
- [[pagination-api-design]]
- [[rest-noun-based-url-design]]
- [[rest-statelessness]]
%% ytkb:end %%
