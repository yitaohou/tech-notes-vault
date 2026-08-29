---
title: Separation of Concerns Between Server and Database
aliases: []
tags:
- concept
summary: 服务器负责响应用户请求，数据库负责存储数据，两者各自只关心自己的职责范围，是软件工程中经典的separation of concerns原则在后端架构中的体现。
created: '2026-08-26'
updated: '2026-08-26'
---

# Separation of Concerns Between Server and Database

%% ytkb:def %%
服务器负责响应用户请求，数据库负责存储数据，两者各自只关心自己的职责范围，是软件工程中经典的separation of concerns原则在后端架构中的体现。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-data-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 服务器与数据库解耦后，服务器挂掉或被移除不会影响数据库（数据库不知道服务器的存在），体现了服务器关心服务用户、数据库关心存储数据的关注点分离。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
- 但如果数据库本身宕机，情况就不同了：没有数据库整个系统就无法为用户提供服务，不过某些不需要访问数据库的请求仍可能被处理，说明这里的解耦并不彻底。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[decoupled-database-architecture]]
%% ytkb:end %%
