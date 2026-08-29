---
title: Incremental Static Generation (ISG)
aliases: []
tags:
- concept
summary: 一种静态站点生成策略，仅重新生成内容发生变化的页面（如CMS新增博客文章后触发的部分构建），而非重建整个网站。
created: '2026-08-26'
updated: '2026-08-26'
---

# Incremental Static Generation (ISG)

%% ytkb:def %%
一种静态站点生成策略，仅重新生成内容发生变化的页面（如CMS新增博客文章后触发的部分构建），而非重建整个网站。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-rendering-strategies]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- incremental static generation 只重新生成发生变化的页面，例如 CMS 新增一篇博客文章会触发 build pipeline，仅重建静态文件中变化的那部分，而不是全量重建整个网站。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
- ISG 的优势不仅在于构建速度更快，客户端如果已下载过部分 CSS/JS，也无需重新下载未发生变化的部分，只需下载变化的部分。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
- ISG 通常已内置在 Next.js 这类框架中，开发者一般不需要自己手动实现这套机制。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[code-splitting-dynamic-import]]
%% ytkb:end %%
