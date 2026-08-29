---
title: improve-codebase-architecture Skill
aliases: []
tags:
- concept
summary: Matt Pocock 开发的一款 Claude Skill，用于扫描并清理代码库中的淺模組，帮助代码库向深模組架构演进。
created: '2026-08-26'
updated: '2026-08-26'
---

# improve-codebase-architecture Skill

%% ytkb:def %%
Matt Pocock 开发的一款 Claude Skill，用于扫描并清理代码库中的淺模組，帮助代码库向深模組架构演进。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:aR97E7aKEgg %%
### 来自 [[2026-07-22-700-萬人下載的-grill-mematt-pocock-到底寫了什麼]]
- improve-codebase-architecture 这个 skill 不是单纯检查语法，而是对代码库中每一个模块执行「刪除测试」，以此判断该模块究竟是深模組还是多余的淺模組空壳。（[12:00](https://youtu.be/aR97E7aKEgg?t=720)）
- Matt 建议把该 skill 当成日常保养，每隔几天在终端机跑一次，让它扫描整个专案并在本机生成一份 HTML 诊断报告，附上重构前后的架构对比图，使用者不需要看代码，只要挑一个最急迫的建议告诉 AI 照此方案重构即可。（[12:00](https://youtu.be/aR97E7aKEgg?t=720)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-skills]]
- [[deep-module]]
- [[deletion-test]]
- [[shallow-module]]
%% ytkb:end %%
