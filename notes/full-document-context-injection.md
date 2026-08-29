---
title: 直接输入完整文档作为上下文
aliases: []
tags:
- concept
summary: 直接把完整文档一次性作为上下文输入给模型的方法，是构建知识客服时最直观但存在缺陷的思路。
created: '2026-08-26'
updated: '2026-08-26'
---

# 直接输入完整文档作为上下文

%% ytkb:def %%
直接把完整文档一次性作为上下文输入给模型的方法，是构建知识客服时最直观但存在缺陷的思路。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 构建产品知识客服时，若把整本产品手册直接随问题一起发送给模型，当手册内容超过模型的上下文窗口大小时，模型会出现读取不全、'读了后面忘了前面'的问题，导致回答准确率无法保障。（[00:00](https://youtu.be/WWdlme1EAGI?t=0)）
- 直接把完整文档作为输入的方式会显著推高模型的推理成本，因为输入内容越多，推理成本越高。（[00:00](https://youtu.be/WWdlme1EAGI?t=0)）
- 直接把完整文档作为输入还会拖慢模型的推理速度，模型需要消化的内容越多，输出速度就越慢。（[00:00](https://youtu.be/WWdlme1EAGI?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[retrieval-augmented-generation]]
%% ytkb:end %%
