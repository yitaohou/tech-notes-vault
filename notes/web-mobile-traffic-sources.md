---
title: Web and Mobile Traffic Sources
aliases: []
tags:
- concept
summary: 系统流量通常来自 web 应用和 mobile 应用两大来源，服务器对二者承担的职责有所不同。
created: '2026-08-26'
updated: '2026-08-26'
---

# Web and Mobile Traffic Sources

%% ytkb:def %%
系统流量通常来自 web 应用和 mobile 应用两大来源，服务器对二者承担的职责有所不同。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 对 web 用户，服务器需要同时处理业务逻辑、数据存储，以及用 HTML、CSS、JavaScript 完成的页面呈现；而对 mobile 用户，服务器主要通过 HTTP API 调用返回数据，界面渲染由客户端自行完成。（[03:00](https://youtu.be/oYxTTirKY8M?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[restful-api-design]]
%% ytkb:end %%
