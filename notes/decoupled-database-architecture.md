---
title: Decoupled Database Architecture
aliases: []
tags:
- concept
summary: 把数据库从服务器实例中解耦出来、作为独立的单一关系型数据库供所有服务器实例共享访问的架构方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Decoupled Database Architecture

%% ytkb:def %%
把数据库从服务器实例中解耦出来、作为独立的单一关系型数据库供所有服务器实例共享访问的架构方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-service-architecture-patterns]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 解决数据耦合问题的方法是把数据库独立出来，作为一个统一的关系型数据库集中存放用户表、文件表等所有数据，用户请求落到哪台服务器实例都能访问到同一份数据。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[data-coupled-server-scaling-problem]]
- [[separation-of-concerns-server-database]]
%% ytkb:end %%
