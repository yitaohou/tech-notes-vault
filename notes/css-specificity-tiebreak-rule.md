---
title: CSS Specificity Tiebreak Rule
aliases: []
tags:
- concept
summary: CSS specificity 的比较规则是逐位（tie-break）比较而非求和：先比较最高位（ID），只有相同时才继续比较下一位（class/attribute），最后才比较
  element。
created: '2026-08-26'
updated: '2026-08-26'
---

# CSS Specificity Tiebreak Rule

%% ytkb:def %%
CSS specificity 的比较规则是逐位（tie-break）比较而非求和：先比较最高位（ID），只有相同时才继续比较下一位（class/attribute），最后才比较 element。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-css-styling]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 两个选择器比较 specificity 时，只要靠左的位（如 ID 位）出现1比0的差异就直接决定胜负，根本不会再去看后面较低位的数字。（[27:07](https://youtu.be/AMerB8XjfZ0?t=1627)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[css-specificity-calculation]]
%% ytkb:end %%
