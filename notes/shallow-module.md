---
title: Shallow Module
aliases: []
tags:
- concept
summary: 淺模組指模块虽然存在拆分，却没有提供统一简单的入口来隐藏内部实现细节，导致外部调用者必须了解并直接处理其内部结构的模块设计。
created: '2026-08-26'
updated: '2026-08-26'
---

# Shallow Module

%% ytkb:def %%
淺模組指模块虽然存在拆分，却没有提供统一简单的入口来隐藏内部实现细节，导致外部调用者必须了解并直接处理其内部结构的模块设计。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-code-quality-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:aR97E7aKEgg %%
### 来自 [[2026-07-22-700-萬人下載的-grill-mematt-pocock-到底寫了什麼]]
- 结帐系统被拆成计算折扣、验证信用卡、建立订单、扣除库存、寄信五个小模块，却没有为这五个模块建立统一的大门来隐藏细节，导致主程式必须亲自处理五个模块间的资料传递，这是典型的淺模組设计。（[12:00](https://youtu.be/aR97E7aKEgg?t=720)）
- 淺模組架构对 AI 维护极不友好，因为 AI 的 context window 有限，修 bug 时逻辑散落在多个房间里，AI 必须在文件间跳转拼凑上下文，一旦瑣碎逻辑超过其记忆范围就会开始瞎猜，甚至把原本正常的代码也一起改坏。（[12:00](https://youtu.be/aR97E7aKEgg?t=720)）
- 浅模块就像一栋分好了厨房、客厅、卧室的房子，房间分得很干净，却没有大门——要进厨房得爬窗户，进客厅得爬烟囱。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
- 浅模块设计的溝通成本极高，就像进自己的房子却被迫记住五个房间各自独立的密码和路线。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
- AI 在写购物车结帐这类逻辑时，最容易蓋出浅模块这种有隐患的设计。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-lacks-global-view-coding]]
- [[context-window-limits-large-models]]
- [[deep-module]]
%% ytkb:end %%
