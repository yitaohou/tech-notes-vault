---
title: Static Site Pre-rendering
aliases: []
tags:
- concept
summary: 针对交互性不强的静态网站，在服务器端预先把页面渲染好再发送给客户端，使客户端在获取静态文件时就已直接得到渲染完成的 HTML 和 CSS，无需再运行大量
  JavaScript。
created: '2026-08-26'
updated: '2026-08-26'
---

# Static Site Pre-rendering

%% ytkb:def %%
针对交互性不强的静态网站，在服务器端预先把页面渲染好再发送给客户端，使客户端在获取静态文件时就已直接得到渲染完成的 HTML 和 CSS，无需再运行大量 JavaScript。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-rendering-strategies]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 对交互性较弱的静态网站，可以在服务器端预先渲染（pre-render）页面，客户端请求静态文件时即可直接拿到已渲染好的 HTML 和 CSS，从而省去大量 JavaScript 执行开销。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[client-side-rendering-white-screen]]
%% ytkb:end %%
