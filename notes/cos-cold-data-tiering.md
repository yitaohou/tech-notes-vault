---
title: COS Object Storage for Cold Data Tiering
aliases: []
tags:
- concept
summary: 腾讯云 ES 企业版支持把不常访问的历史日志和冷数据从高性能磁盘迁移到成本更低的 COS 对象存储中，需要时依然可以搜索。
created: '2026-09-02'
updated: '2026-09-02'
---

# COS Object Storage for Cold Data Tiering

%% ytkb:def %%
腾讯云 ES 企业版支持把不常访问的历史日志和冷数据从高性能磁盘迁移到成本更低的 COS 对象存储中，需要时依然可以搜索。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-data-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:ky7_1K3wfAY %%
### 来自 [[2026-08-26-agent搜索和记忆的基础设施腾讯云-elastichsearch-service-企业版详细攻略]]
- 大量历史日志和冷数据不需要一直放在昂贵的高性能磁盘里，可以放到成本更低的 COS 对象存储里，需要时依然能够搜索。（[03:00](https://youtu.be/ky7_1K3wfAY?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[object-storage]]
- [[snapshot-archive-recovery-optimization]]
%% ytkb:end %%
