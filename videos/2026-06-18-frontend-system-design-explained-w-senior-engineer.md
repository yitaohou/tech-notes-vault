---
video_id: KuClyhvSzXk
url: https://www.youtube.com/watch?v=KuClyhvSzXk
title: Frontend System Design Explained w/ Senior Engineer (Microfrontends, Monorepo,
  MCP UI, Reactjs)
channel: theSeniorDev
published: '2026-06-18'
duration: '38:02'
transcript_origin: subs
tags:
- video
---

# Frontend System Design Explained w/ Senior Engineer (Microfrontends, Monorepo, MCP UI, Reactjs)

摘要: [[2026-06-18-frontend-system-design-explained-w-senior-engineer-summary|完整摘要]]

## 知识点

- [[ai-context-scope-reduction-via-modularization]] — 当开发者只在更小的模块内工作时，AI coding 工具需要处理的 context 更少，因此效率更高、风险更低。（[06:02](https://youtu.be/KuClyhvSzXk?t=362)）
- [[ai-verification-time-tradeoff]] — Claude Code 等 coding agent 能把功能实现时间降到几乎为零，但会显著增加验证时间，因此 AI 时代前端系统设计的目标转变为降低验证时间、减少架构漂移，同时最大化开发速度，而不是单纯追求实现速度。（[00:00](https://youtu.be/KuClyhvSzXk?t=0)）
- [[api-edge-functions]] — micro-frontend 与 backend service 通信时都需要处理一组称为 edge functions 的重复性功能，包括 caching、HTTPS、authentication、content negotiation 和 rate limiting。（[06:02](https://youtu.be/KuClyhvSzXk?t=362)）
- [[api-gateway]] — 如果每次都要在前端和后端两侧分别重复实现 caching、认证、限流等 edge functions，会造成大量重复劳动，这正是引入 API gateway 集中处理这些功能的动机。（[06:02](https://youtu.be/KuClyhvSzXk?t=362)）
- [[api-gateway-https-http-boundary]] — 客户端到 API gateway 用 HTTPS，gateway 到微服务之间用 HTTP，因为内部环境已是封闭网络、不再需要额外的传输安全保障，从而提升整体性能。（[09:03](https://youtu.be/KuClyhvSzXk?t=543)）
- [[architectural-drift]] — AI 时代优秀的前端系统设计应当最小化架构漂移，让代码演进始终贴合既定架构，从而降低后续人工验证代码的成本。（[00:00](https://youtu.be/KuClyhvSzXk?t=0)）
- [[atomic-css]] — Tailwind CSS 是 Atomic CSS 架构风格的一种具体实现。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
- [[backend-for-frontend]] — BFF 模式下每个客户端都有自己专属的 backend for frontend，客户端团队可以独立开发，同时与真正的后端服务完全解耦。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
- [[backend-for-frontend-pattern]] — BFF 接收前端请求后转发给对应微服务，前端团队借此可以整合改造微服务接口，自行实现新功能，端到端拥有客户端侧的整个特性交付。（[09:03](https://youtu.be/KuClyhvSzXk?t=543)）
- [[backend-team-backlog-bottleneck]] — 大公司里前端工程师常因为需要联系多个不同的后端团队、受制于对方各自的 backlog 和优先级排期，而难以快速推进功能交付。（[09:03](https://youtu.be/KuClyhvSzXk?t=543)）
- [[cache-busting]] — cache busting是module bundler采用的机制，用来在部署新版本时强制让用户拿到最新资源，避免误用CDN中还未失效的旧版本静态资源。（[19:20](https://youtu.be/KuClyhvSzXk?t=1160)）
- [[cache-hit-cache-invalidation-terminology]] — 在CDN语境下，从边缘节点拿到资源叫作cache hit；服务器推送新版本资源、让旧缓存失效的动作叫作cache invalidation。（[19:05](https://youtu.be/KuClyhvSzXk?t=1145)）
- [[cdn-cost-effective-optimization]] — 现代CDN在就近分发资源的基础上，还会自动压缩资产并处理好的缓存策略，开箱即用地解决大多数性能问题，是投入产出比很高的性能优化方式。（[19:45](https://youtu.be/KuClyhvSzXk?t=1185)）
- [[cdn-edge-asset-caching]] — CDN（内容分发网络）用于在客户端-服务器模型中，把静态的 JavaScript、CSS、HTML 等资源缓存到离用户更近的边缘节点，从而减少跨地域访问带来的延迟。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
- [[cdn-point-of-presence]] — CDN通过在全球部署大量edge location（PoP）服务器，把静态资源提前推送到这些节点；用户发起请求时会被重定向到离自己最近的edge location，从而缩短物理距离、降低延迟。（[18:20](https://youtu.be/KuClyhvSzXk?t=1100)）
- [[chatgpt-claude-sse-observability]] — 在浏览器开发者工具 Network 面板中找到 ChatGPT 或 Claude 的对话请求，可以看到响应是以 event stream 形式一块块（chunk）返回的，这正是构建 LLM 聊天 UI 的技术基础。（[36:09](https://youtu.be/KuClyhvSzXk?t=2169)）
- [[client-side-rendering-white-screen]] — 在 client-side rendering 下，浏览器加载的初始 HTML 是空的，只有当框架的渲染函数真正执行后页面才会显示内容，这导致用户短暂看到白屏。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
- [[code-splitting-dynamic-import]] — 传统 module bundler 会把所有 JavaScript 打包进单个大文件，一次性加载这种大文件会严重拖慢 Core Web Vitals，因为加载了远超当前页面所需的代码量。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
- [[component-library-accessibility]] — 设计系统组件库可以统一处理组件的 accessibility，避免每个团队各自重复投入精力实现无障碍能力。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
- [[container-orchestration-services]] — DevOps 团队可以把打包好的 Docker image 推送到容器编排系统的部署管线中运行，编排系统负责处理负载均衡、并行运行多个容器实例，以及容器故障后快速拉起新实例等复杂工作。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
- [[conways-law]] — 根据 Conway's law，如果想让开发团队保持小型且独立，就需要把系统拆分成小型独立的 vertical slice。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
- [[core-web-vitals]] — Core Web Vitals 是前端工程师岗位描述中最常被提及的性能模式，由三项指标构成，分别衡量网站的加载速度、交互速度和视觉稳定性，并由 Google 给出合格数值标准。（[27:59](https://youtu.be/KuClyhvSzXk?t=1679)）
- [[critical-rendering-path]] — critical rendering path 的具体步骤依次为：构建 DOM、构建 CSSOM、生成 render tree、计算 layout tree（各节点的位置与宽度）、转换为交给 GPU 处理的 paint 操作，最后进入 composite 阶段；组件框架引起的重新渲染会在这些步骤完成后反复触发。（[29:07](https://youtu.be/KuClyhvSzXk?t=1747)）
- [[csr-loading-waterfall]] — 在采用 client-side rendering 的 SPA 架构中，加载顺序依次是获取静态文件、再获取动态数据、最后才执行渲染，这一整套流程会耗费较长时间。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
- [[csr-seo-performance-limitation]] — 如果目标是打造高性能网站，或者希望页面内容能被搜索引擎爬虫顺利抓取收录，那么 client-side rendering 通常不是最佳选择。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
- [[cumulative-layout-shift]] — CLS 衡量页面加载过程中 UI 发生位移变化的程度，浏览器会截取页面前后的快照来判断元素是否移动过多。（[28:29](https://youtu.be/KuClyhvSzXk?t=1709)）
- [[design-system]] — 在 feature team / platform team 组织架构中，设计系统（design system）通常由 platform team 构建并维护，供各 feature team 复用。（[00:00](https://youtu.be/KuClyhvSzXk?t=0)）
- [[design-tokens]] — 构建设计系统的第一步是定义design tokens，即团队的品牌色、border定义、字体家族等视觉基础信息；现代做法是把这些值定义为CSS custom properties。（[20:35](https://youtu.be/KuClyhvSzXk?t=1235)）
- [[docker]] — Docker 通过 Dockerfile 定义打包步骤，把应用代码打包成 Docker image，从而无论底层技术栈是什么，都能用统一方式完成部署。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
- [[docker-compose]] — 理想情况下前端工程师应具备用 Nginx 和 Docker Compose 在本地机器上手动搭建一个小型负载均衡器的能力，以此证明自己能推理清楚其工作原理。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
- [[docker-environment-consistency]] — 只要宿主机支持运行 Docker，就可以直接运行任意 Docker image，无需关心目标机器是否安装了正确版本的 Node.js、PHP 或其他依赖，因为运行环境已随镜像一并打包。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
- [[docker-image-structure]] — 以 Next.js 应用为例，其 Docker image 会包含应用代码本身、Next.js 所需的 Node.js runtime，以及底层操作系统（通常是 Linux）。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
- [[dockerfile]] — 开发者在 Dockerfile 中声明打包步骤，Docker 据此生成对应的 Docker image。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
- [[dry-principle]] — 设计系统的组件复用本质上是在架构层面践行 DRY 原则，避免不同前端团队重复造轮子。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
- [[feature-team-platform-team-split]] — 理想情况下应把单体开发团队拆分为多个全栈的 feature team，各自使用 coding agent 独立负责并交付特定功能，同时依赖 platform team 提供的共享基础设施来支撑整体产品推进。（[00:00](https://youtu.be/KuClyhvSzXk?t=0)）
- [[figma-mcp-design-to-code]] — 当设计团队最初在 Figma 中构建设计系统、随后前端团队在组件库中实现它时，可以用 Figma MCP server 配合 coding agent，快速把设计系统装配进各 feature team 的垂直切片功能中，这是多数公司正在转向的工作流。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
- [[frontend-backend-skill-expectation]] — 在大公司里，条件最好、工作最有意思的前端岗位通常都要求工程师至少在高层面上懂得如何扩展 microservice、构建 BFF 并掌握 API 设计。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
- [[frontend-devops-awareness]] — 前端工程师不需要因为职位描述中出现 Kubernetes 或容器系统字样就被吓退，也不必立刻转型成 DevOps 工程师，但应能从架构层面说明这些系统在部署流程中处于什么位置。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
- [[frontend-engineering-bifurcation-speculation]] — 前端工程正走向两个极端：一是成为在 vertical slice 上工作的 full-stack 工程师；二是深耕前端本身，加入 infra 团队构建应用外壳或 design system，为 feature team 提供可复用的构建模块。（[06:02](https://youtu.be/KuClyhvSzXk?t=362)）
- [[frontend-monolith]] — 前端应用最初都是 monolith，团队规模扩大后（例如40人团队每日 standup 要开1.5小时）单体架构在开发层面变得不可持续，这正是引入 micro-frontends 的动因。（[00:00](https://youtu.be/KuClyhvSzXk?t=0)）
- [[geographic-latency-example]] — 以美国用户访问部署在欧洲的应用为例：若没有 CDN，获取 JavaScript、CSS、HTML 等静态资源需要跨越大西洋一个往返，这段物理距离直接带来额外的网络延迟。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
- [[graphql]] — GraphQL 被认为是构建 backend for frontend 的优秀技术选择之一。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
- [[https-handshake-performance-cost]] — HTTPS 通常比 HTTP 性能差，因为需要更多的 round trip 来完成 handshake，这是内部微服务间通信改用 HTTP 的直接原因。（[09:03](https://youtu.be/KuClyhvSzXk?t=543)）
- [[hydration]] — SSR 返回的 HTML 页面虽然避免了白屏，但此时页面还不可交互，因为浏览器尚未构建 virtual DOM 并将其附加到已渲染好的 DOM 上，这一过程称为 hydration。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
- [[incremental-static-generation]] — incremental static generation 只重新生成发生变化的页面，例如 CMS 新增一篇博客文章会触发 build pipeline，仅重建静态文件中变化的那部分，而不是全量重建整个网站。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
- [[interaction-to-next-paint]] — INP 衡量的是用户发生交互后到界面完成重新绘制（repaint）所需的时间，与页面初次渲染无关，而是关注后续的重新渲染过程，这对使用组件框架的应用尤为重要。（[28:35](https://youtu.be/KuClyhvSzXk?t=1715)）
- [[kubernetes-container-orchestration]] — Kubernetes 是知名的容器编排系统，AWS 的 ECS 是与之对应的替代方案，两者都常出现在前端相关职位的招聘描述中。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
- [[largest-contentful-paint]] — LCP 指从用户按下回车到页面中最大元素渲染完成所花费的时间，与页面初次渲染相关。（[28:18](https://youtu.be/KuClyhvSzXk?t=1698)）
- [[lazy-loading-vs-eager-loading]] — lazy loading 与 eager loading 相对：前者按需（滚动、跳转、点击等用户交互）逐步加载内容，后者在用户落地页面时就一次性加载全部内容。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
- [[llm-response-communication-asymmetry]] — AI 场景中确实需要实时通信，但方向是单向的：客户端只发送一次查询，之后服务端持续推送 token 回来，这种客户端与服务端消息量的不对称正是 SSE 适用的原因。（[36:09](https://youtu.be/KuClyhvSzXk?t=2169)）
- [[load-balancer]] — 当单台服务器的并发处理能力达到上限时，最简单的扩展方式是创建多个相同的服务器实例，并引入一个应用负载均衡器（application load balancer）在这些实例之间分配流量。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
- [[managed-load-balancer-provisioning]] — 实际工作中很少需要手动搭建负载均衡器，因为 AWS 或 Google Cloud 等主流云服务商都能在几秒钟内自动配置好一个负载均衡器。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
- [[mcp-connectors]] — 前端工程师应掌握如何使用 MCP server，并针对团队所用的设计工具搭建对应连接器（若尚无现成连接器则需自行开发），再接入 Claude Code（企业中使用最广）或 Codex 等 coding agent。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
- [[mcp-ui]] — MCP UI 使聊天应用中 LLM 的回答不再局限于纯文本，还能渲染出实际的 UI 组件，例如产品卡片或地图。（[24:07](https://youtu.be/KuClyhvSzXk?t=1447)）
- [[mcp-ui-resource-declaration]] — MCP UI 的实现方式是在协议层声明 resource，说明其使用场景和 LLM 应给出的回答格式，再由前端解析该声明并渲染出对应界面。（[27:07](https://youtu.be/KuClyhvSzXk?t=1627)）
- [[micro-frontend-independent-deployment]] — 各个 micro-frontend 可以独立部署，例如 header 应用可以托管在 header.theseniordev.com 这样单独的域名下并独立加载，product 页和 cart 页同理，最终由 shell 把它们整合在一起。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
- [[micro-frontend-shell]] — micro-frontend shell 负责处理 auth、routing、language 和 global state（如用户是否登录）等全局功能，并将这些全局状态传递给其内部加载的各个 micro-frontend 应用。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
- [[micro-frontend-team-scaling]] — 即使后端已拆分为微服务、团队变小变快，若前端仍是 monolith，会因太多人向同一客户端推送代码而容易出错，甚至有人改动全局 CSS 规则影响所有人，最终导致前端团队因沟通协调开销过大而无法继续扩展。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
- [[micro-frontend-visual-divergence]] — 当product团队和payment团队各自独立开发发布micro-frontend时，容易出现代码重复和视觉divergence，例如产品页面按钮和支付页面按钮样式不同，用户会察觉这其实是彼此独立的前端。（[20:00](https://youtu.be/KuClyhvSzXk?t=1200)）
- [[micro-frontends]] — 解决前端团队规模瓶颈的方法是仿照后端从 monolith 拆分为 microservices 的思路，把前端 monolith 拆分成多个可独立部署的 micro-frontend 应用。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
- [[microservice-api-inconsistency-frontend-complexity]] — 在没有 BFF 的情况下，客户端要对多个形态各异的微服务分别发起 fetch 调用，各自需要不同的 client/SDK，造成大量前端复杂度。（[09:03](https://youtu.be/KuClyhvSzXk?t=543)）
- [[microservice-blueprint-layers]] — 一个典型的 microservice blueprint 由 API、business logic layer、persistence layer 和数据库（如 Postgres 或 NoSQL DB）组成，是构建大型应用的基本单元。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
- [[microservices]] — micro-frontends 这一前端架构概念的思想源头来自后端的 microservices 架构风格，二者都是为解决单体应用团队协作难以扩展的问题。（[00:00](https://youtu.be/KuClyhvSzXk?t=0)）
- [[microservices-architecture]] — 微服务拆分通常从 back-end 开始，把 monolith 拆分成各自暴露独立 API、可独立部署的 micro back-end，代码库和团队彼此独立，只通过 API 相互通信。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
- [[microservices-suited-for-large-organizations]] — 大型应用在生产环境中可能运行上千个 microservices，例如讲者曾就职的一家金融公司在生产环境中大约有1000个微服务，不同团队各自拥有一部分微服务，讲者所在团队拥有其中13个。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
- [[model-context-protocol]] — 「design to code MCP」中的 MCP 全称是 Model Context Protocol，即一种协议服务器标准。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
- [[monorepo]] — monorepo 通过让所有子项目共享同一套代码规范、依赖和构建工具链，能够有效避免 architectural drift。（[24:07](https://youtu.be/KuClyhvSzXk?t=1447)）
- [[monorepo-ai-cross-boundary-context]] — monorepo 能为 coding agent 提供跨服务边界进行修改所需的完整上下文，使其可以在单次会话中完成原本涉及多个仓库的复杂修改任务。（[24:07](https://youtu.be/KuClyhvSzXk?t=1447)）
- [[nodejs-server-capacity]] — 一台经过良好优化的 Node.js 服务器通常可以支撑 2000 到 10000 个并发请求，超过这个范围就需要考虑扩展方式。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
- [[openai-sdk-streaming-iterator]] — 在 React 应用中用 OpenAI NPM package 构建聊天应用时，底层实际使用的就是 server-sent events 来接收 token 流。（[36:09](https://youtu.be/KuClyhvSzXk?t=2169)）
- [[over-fetching-under-fetching]] — 如果把 desktop 和 mobile 的数据需求都塞进同一个 API：接口做大会导致 mobile 端 over-fetch 到不需要的数据，接口做小又会导致 desktop 端需要多次请求才能拿到同样的数据，即 under-fetching。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
- [[polling-technique]] — polling 通过反复调用某个接口（如用 setTimeout 不断请求交易状态接口，直到状态变为 completed）来实现类实时效果，用纯 JavaScript 即可轻松实现，但会对服务器造成过多请求、扩展性差，还可能引发 race condition。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
- [[real-time-communication-alternatives]] — 实现不遵循传统请求-响应循环的实时通信，通常有三种可选技术方案：polling、WebSocket 和 Server-Sent Events。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
- [[reusable-components]] — 设计系统可以进一步升级为可复用组件库（如 input、button），供各 feature team 在装配功能时直接消费，从而保证跨多个 micro frontend 的 UI 一致性，并避免代码重复。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
- [[server-sent-events-llm]] — 使用 SSE 时客户端发送一条消息建立会话，之后在该 endpoint 上持续接收服务端推送的更新（token），大多数 LLM 应用采用这种方式而非 WebSocket 或 polling。（[36:09](https://youtu.be/KuClyhvSzXk?t=2169)）
- [[server-side-rendering]] — 在 server-side rendering 中，front-end server 会先向 back-end server 请求数据、在服务端完成渲染，再把预渲染好的完整 HTML 页面返回给客户端，因此客户端不会遇到白屏问题。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
- [[static-site-generation-limitation]] — 静态站点预渲染方案仅适用于内容变化不频繁的场景，例如博客这类需要经常发布新内容的站点就不适合采用这种方式。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
- [[static-site-pre-rendering]] — 对交互性较弱的静态网站，可以在服务器端预先渲染（pre-render）页面，客户端请求静态文件时即可直接拿到已渲染好的 HTML 和 CSS，从而省去大量 JavaScript 执行开销。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
- [[two-pizza-team]] — 引入 agentic coding 后，原本的两个披萨团队规模进一步缩小为一个披萨团队，因为同样的工作量可以由更少的人配合 AI 完成。（[00:00](https://youtu.be/KuClyhvSzXk?t=0)）
- [[ui-relevance-in-llm-chat-era]] — 尽管有观点认为聊天界面普及后不再需要传统 UI，作者认为 UI 依然是高效传达信息的方式，前端开发者仍然不可或缺，未来趋势是把 LLM 聊天能力与传统 Web UI 结合起来。（[24:07](https://youtu.be/KuClyhvSzXk?t=1447)）
- [[verification-time-reduction]] — 变更的 surface area 越小，团队做质量把关所需的 verification time 就越短，这也是 AI 高频提交代码场景下更适合采用 micro-frontends 和 microservices 的原因。（[06:02](https://youtu.be/KuClyhvSzXk?t=362)）
- [[vertical-slicing]] — 当 micro-frontend 与同一业务领域内的一个或多个 microservices 组合在一起时，就形成了 vertical slice，可以由独立团队扩展和维护。（[06:02](https://youtu.be/KuClyhvSzXk?t=362)）
- [[vertically-integrated-engineer]] — 只做前端或只做后端的工程师应尽快转型为 vertically integrated engineer，即能借助 coding agent 独立跨全栈工作的工程师，这被认为是在当前市场生存下去的必经转型。（[06:02](https://youtu.be/KuClyhvSzXk?t=362)）
- [[vibe-coding]] — 如果不先提取设计系统喂给 AI，coding agent 会自行编造样式，导致 UI 风格不一致，一眼就能看出这段代码是 vibe coded 出来的。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
- [[vpc-private-network-isolation]] — 有了 API gateway 后，后端微服务通常部署在 VPC（虚拟私有云）内，外部唯一能进入的入口就是 API gateway，从而保证安全性。（[09:03](https://youtu.be/KuClyhvSzXk?t=543)）
- [[websocket-communication]] — WebSocket 非常适合双向通信场景，例如聊天应用中客户端和服务端都需要不断发送消息片段，但代价是 overhead 较大，且对服务端资源消耗很高，多数场景并不需要。（[36:09](https://youtu.be/KuClyhvSzXk?t=2169)）
