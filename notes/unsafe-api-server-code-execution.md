---
title: Unsafe Code Execution on API Server
aliases: []
tags:
- concept
summary: 直接在承载核心业务逻辑的 API 服务器上执行用户提交代码的做法，存在多重安全与稳定性风险。
created: '2026-08-26'
updated: '2026-08-26'
---

# Unsafe Code Execution on API Server

%% ytkb:def %%
直接在承载核心业务逻辑的 API 服务器上执行用户提交代码的做法，存在多重安全与稳定性风险。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 直接在 API 服务器上运行用户提交的代码是很危险的做法，恶意用户可能在提交的代码中植入 malware，导致系统数据被删除。（[24:07](https://youtu.be/QBHTbtWSECg?t=1447)）
- 在 API 服务器直接执行用户提交代码还可能被利用发起 DDoS 攻击，即大量重复请求涌入服务器意图使其宕机。（[24:07](https://youtu.be/QBHTbtWSECg?t=1447)）
- 在 API 服务器上直接执行用户代码容易造成 CPU 或内存的过度占用（resource hog）。（[24:07](https://youtu.be/QBHTbtWSECg?t=1447)）
- 由于缺乏隔离性（isolation）和容错能力（fault tolerance），如果 API 服务器因执行用户代码而崩溃，会导致整个系统出现较长时间的 downtime。（[24:07](https://youtu.be/QBHTbtWSECg?t=1447)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[vm-based-code-execution]]
%% ytkb:end %%
