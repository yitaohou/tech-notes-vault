---
title: DeepSeek Harness Data Offsite Risk
aliases: []
tags:
- concept
summary: 使用 DeepSeek Harness 时，由于语言模型运行在 DeepSeek 服务器上，本地文件内容必须通过网络发送到远端服务器才能被模型读取和处理，构成数据离开本地设备的固有架构代价。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Data Offsite Risk

%% ytkb:def %%
使用 DeepSeek Harness 时，由于语言模型运行在 DeepSeek 服务器上，本地文件内容必须通过网络发送到远端服务器才能被模型读取和处理，构成数据离开本地设备的固有架构代价。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 只要用户在 Harness 上让 AI 读取本地文件，该文件内容就必须经网络传输到 DeepSeek 服务器由远端模型处理后再返回结果，数据一旦离开本机就只能依赖对方的服务条款承诺，出问题也无法自行审计。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-provider-control-risk]]
- [[data-privacy-model-hosting-factor]]
%% ytkb:end %%
