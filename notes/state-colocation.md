---
title: State Colocation
aliases: []
tags:
- concept
summary: 把 state 尽量放在靠近其实际被使用的组件层级，而不是不必要地提升到组件树上层，以减少重新渲染范围的实践原则。
created: '2026-08-26'
updated: '2026-08-26'
---

# State Colocation

%% ytkb:def %%
把 state 尽量放在靠近其实际被使用的组件层级，而不是不必要地提升到组件树上层，以减少重新渲染范围的实践原则。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-state-management]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 如果把 state 不必要地提升到组件树较高层级（lift state up），该 state 变化时会导致其下所有组件自动重新渲染；把 state 保持在靠近使用它的地方，可以避免这种不必要的重新渲染。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rerender-optimization-strategies]]
%% ytkb:end %%
