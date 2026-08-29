---
title: AI 会话结束后的上下文失忆
aliases: []
tags:
- concept
summary: AI 对话一旦被关闭就会立即失忆，此前在对话中好不容易达成的共识会直接消失，无法保留到下一次会话。
created: '2026-08-26'
updated: '2026-08-26'
---

# AI 会话结束后的上下文失忆

%% ytkb:def %%
AI 对话一旦被关闭就会立即失忆，此前在对话中好不容易达成的共识会直接消失，无法保留到下一次会话。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-prompt-engineering]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:aR97E7aKEgg %%
### 来自 [[2026-07-22-700-萬人下載的-grill-mematt-pocock-到底寫了什麼]]
- 用户被 grill-me 拷问完达成共识后，只要一关掉对话，AI 就会立刻失忆，刚才吵出来的共识直接蒸发，因此需要额外一步把共识写下来保存。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
%% ytkb:end %%

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 大模型有一个本质特点：每次运行之间不会记住之前的内容，所以记忆不能只存在于对话上下文里，必须落到磁盘文件等持久化存储上。（[13:35](https://youtu.be/KgiwIEBeOHw?t=815)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[file-system-persistent-memory]]
- [[grill-me-skill]]
- [[to-spec-skill]]
%% ytkb:end %%
