---
title: Attribute-Based Access Control (ABAC)
aliases: []
tags:
- concept
summary: 一种超越角色划分、基于用户属性、资源属性和环境条件的组合来动态决定访问权限的授权模型。
created: '2026-08-26'
updated: '2026-08-26'
---

# Attribute-Based Access Control (ABAC)

%% ytkb:def %%
一种超越角色划分、基于用户属性、资源属性和环境条件的组合来动态决定访问权限的授权模型。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-authentication-authorization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- ABAC 通过检查用户模型或资源模型中的具体属性（而非固定角色）来决定允许或拒绝访问，例如仅当用户部门为 HR 时才授予某项访问权限。（[1:49:15](https://youtu.be/oYxTTirKY8M?t=6555)）
- ABAC 的判定条件可以组合用户属性（如部门、年龄）、资源属性（如机密级别、所有者、分类）和环境属性（如时间、地点、设备类型）三类信息。（[1:49:40](https://youtu.be/oYxTTirKY8M?t=6580)）
- ABAC 可以与 RBAC 结合使用，在角色基础上叠加属性条件来进一步细化授权粒度。（[1:49:35](https://youtu.be/oYxTTirKY8M?t=6575)）
- ABAC 比 RBAC 更灵活，但需要良好的策略管理，整体更复杂，且容易出现属性条件之间相互冲突的问题。（[1:50:05](https://youtu.be/oYxTTirKY8M?t=6605)）
- ABAC 根据用户或资源的属性（而非固定角色）来决定访问权限，比 RBAC 更灵活，但设计和维护也更复杂。（[1:45:30](https://youtu.be/oYxTTirKY8M?t=6330)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[access-control-list]]
- [[role-based-access-control]]
%% ytkb:end %%
