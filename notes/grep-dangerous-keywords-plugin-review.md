---
title: grep 危险关键词插件代码审查
aliases: []
tags:
- concept
summary: 对解压后的插件代码用 grep 搜索 child_process/spawn、fetch、.ssh、credential、process.env
  这 6 类关键词，用于快速定位潜在危险调用的审查方法。
created: '2026-09-03'
updated: '2026-09-03'
---

# grep 危险关键词插件代码审查

%% ytkb:def %%
对解压后的插件代码用 grep 搜索 child_process/spawn、fetch、.ssh、credential、process.env 这 6 类关键词，用于快速定位潜在危险调用的审查方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 解压插件包后用 grep 搜索 child_process 和 spawn（启动子进程，是攻击链拿到执行能力的最后一步）、fetch（发网络请求，用于数据外传）、.ssh（密钥目录）、credential（凭证字段）、process.env（读环境变量，密钥常存于此），命中哪条就翻到对应代码看它具体在干什么。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[npm-pack-safe-inspection]]
%% ytkb:end %%
