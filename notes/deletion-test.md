---
title: Deletion Test
aliases: []
tags:
- concept
summary: 一种判断模块是深模組还是淺模組的测试方法：想象把该模块直接移除、让主程式自己处理其逻辑，观察代码库结果是变乱还是变整洁。
created: '2026-08-26'
updated: '2026-08-26'
---

# Deletion Test

%% ytkb:def %%
一种判断模块是深模組还是淺模組的测试方法：想象把该模块直接移除、让主程式自己处理其逻辑，观察代码库结果是变乱还是变整洁。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-code-quality-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:aR97E7aKEgg %%
### 来自 [[2026-07-22-700-萬人下載的-grill-mematt-pocock-到底寫了什麼]]
- 如果拔掉某模块后天下大乱、原本隐藏的复杂逻辑全部炸回主程式，说明这是真正有在做事的深模組；如果拔掉后代码反而变清爽、原本要跳着看的两个文件合并到一处，说明这个模块只是没有隐藏任何细节的淺模組空壳，应该清理掉。（[12:00](https://youtu.be/aR97E7aKEgg?t=720)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deep-module]]
- [[improve-codebase-architecture-skill]]
- [[shallow-module]]
%% ytkb:end %%
