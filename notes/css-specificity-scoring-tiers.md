---
title: CSS Specificity Three-Tier Scoring (A, B, C)
aliases: []
tags:
- concept
summary: CSS specificity 采用 A、B、C 三层计分体系，初始值均为 0，根据 selector 类型（ID、class/attribute、元素类型等）分别递增对应层级的分数。
created: '2026-08-26'
updated: '2026-08-26'
---

# CSS Specificity Three-Tier Scoring (A, B, C)

%% ytkb:def %%
CSS specificity 采用 A、B、C 三层计分体系，初始值均为 0，根据 selector 类型（ID、class/attribute、元素类型等）分别递增对应层级的分数。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-css-styling]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- CSS specificity 的计分方式是一个三段式分数 A-B-C，起始都是 000：selector 中每出现一个 ID 就让 A 加一，每出现一个 class 或 attribute 选择器就让 B 加一。（[24:07](https://youtu.be/AMerB8XjfZ0?t=1447)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[css-specificity]]
%% ytkb:end %%
