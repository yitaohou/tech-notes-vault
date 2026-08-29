---
title: Safety Classifier in Claude
aliases: []
tags:
- concept
summary: Claude 中用于识别请求是否涉及网络安全或生物安全等敏感领域、并据此转交或拒绝处理的安全分类机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# Safety Classifier in Claude

%% ytkb:def %%
Claude 中用于识别请求是否涉及网络安全或生物安全等敏感领域、并据此转交或拒绝处理的安全分类机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- 部分命中网络安全或生物相关内容的请求可能被安全分类器转交给 Opus 处理，在 API 场景下也可能被直接拒绝。（[09:02](https://youtu.be/Lle_EJljIoo?t=542)）
- Anthropic 称该安全机制平均在不到 5% 的会话中触发。（[09:20](https://youtu.be/Lle_EJljIoo?t=560)）
- 该安全机制存在误伤风险，正常开发任务也可能被误判触发，因此正式接入前必须先进行实测。（[09:25](https://youtu.be/Lle_EJljIoo?t=565)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-5]]
%% ytkb:end %%
