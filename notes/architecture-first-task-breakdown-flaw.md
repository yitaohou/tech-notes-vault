---
title: 按技术架构拆分任务的缺陷
aliases: []
tags:
- concept
summary: AI 自行规划任务时倾向于按技术层（先建数据库、再写后端逻辑、最后做前端画面）拆分，导致在最后一步做出画面前完全无法测试任何东西，早期出错要等到很后面才被发现。
created: '2026-08-26'
updated: '2026-08-26'
---

# 按技术架构拆分任务的缺陷

%% ytkb:def %%
AI 自行规划任务时倾向于按技术层（先建数据库、再写后端逻辑、最后做前端画面）拆分，导致在最后一步做出画面前完全无法测试任何东西，早期出错要等到很后面才被发现。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:aR97E7aKEgg %%
### 来自 [[2026-07-22-700-萬人下載的-grill-mematt-pocock-到底寫了什麼]]
- 举例来说，如果让 AI 自己规划一个电商网站的任务，它会先把全部资料库建好，再把处理资料的后端逻辑写完，最后才画出前端画面；这样拆分最可怕的盲点是，在最后一步画面出来之前完全没办法测试任何东西，如果第一步资料库建错了，要等到做前端画面时才会发现，前面的心血就全毁了。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-task-planning-weakness]]
- [[feature-based-task-breakdown]]
%% ytkb:end %%
