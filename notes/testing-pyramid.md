---
title: Testing Pyramid
aliases: []
tags:
- concept
summary: 一种按测试类型分层组织测试策略的经典模型，用于评估团队测试结构是否合理。
created: '2026-08-26'
updated: '2026-08-26'
---

# Testing Pyramid

%% ytkb:def %%
一种按测试类型分层组织测试策略的经典模型，用于评估团队测试结构是否合理。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[career-industry-engineering-practices]] · [[career-industry]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 除了看覆盖率数字，senior 工程师还应该对照传统的 testing pyramid 模型，判断团队当前的测试结构处于金字塔的哪个位置。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- 很多人使用 AI 写代码时容易陷入误区，认为 unit tests 和 integration tests 不重要，只需要写 end-to-end tests，因为 AI 能把中间细节处理好。（[12:02](https://youtu.be/AMerB8XjfZ0?t=722)）
- 如果只依赖 end-to-end tests，一旦前端出错，只能知道 end-to-end test 失败，却无法确定大代码库中具体哪里出了问题，用 debugger 或 LLM 排查需要花费大量时间或 token。（[12:02](https://youtu.be/AMerB8XjfZ0?t=722)）
- 如果有 unit tests 覆盖各部分代码，可以通过逐一排除已通过的 unit tests 所覆盖的代码范围，更快更省成本地定位 bug 所在位置。（[12:02](https://youtu.be/AMerB8XjfZ0?t=722)）
- 利用 unit tests 快速排查缩小 bug 范围的前提是代码库要模块化、结构相对清晰。（[12:02](https://youtu.be/AMerB8XjfZ0?t=722)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[test-coverage-target-range]]
- [[test-driven-development]]
%% ytkb:end %%
