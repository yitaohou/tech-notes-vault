---
video_id: AMerB8XjfZ0
title: Top 15 Frontend Interview Questions for 2026 (wa/ Senior Engineer)
source: '[[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: 2624fdcd387d6328138a9198692821355fe349124c200529044da2d16746117b
  schema_version: 1
  model: sonnet
  generated_at: '2026-08-26T20:06:37+00:00'
---

## 一句话总结

这是一场模拟高级前端工程师面试的深度技术串讲，覆盖了 15 道问题，从浏览器渲染机制、CSS box model、AI 辅助编码的质量陷阱，到 JavaScript event loop、React 性能优化、缓存扩展策略与实时通信协议选型，核心主线是：AI 编码时代，真正区分 senior 与 junior 的不是会不会用 AI，而是能否用底层原理去审查、约束和修复 AI 产出的代码。

## 核心内容

### 渲染机制：reflow 与 compositor thread

开场问题围绕一个常见 AI 实现——用 JS 修改 button 的 width 来做悬停放大效果。这种做法会触发 [[browser-reflow]]（00:00），浏览器需要重新扫描区域内所有元素、重算布局属性,进而跑一遍完整渲染流程；而且因为改动是在 JS 里执行的，还额外占用了 [[main-thread-vs-compositor-thread|main thread]]（00:00），比纯 CSS 触发的 reflow 更差（[[js-triggered-animation-cost]]，00:00）。更优方案是用 [[css-transform-compositor-thread|CSS transform/scale]]，把元素提升为独立 layer 后交给 [[compositor-thread-layer-promotion|compositor thread]] 处理（03:00），因为这是纯数学变换、不触碰布局树，能让 main thread 空闲去执行其他逻辑。视频强调，[[interview-senior-depth-signaling|senior 的回答方式]]应该是先质疑实现是否高效，再从底层机制展开分析（00:00）。

### AI 编码工作流与设计系统集成

多数初级工程师的 AI workflow 只是直接甩 prompt 给 Claude Code 或 Copilot（[[ai-coding-workflow-maturity-gap]]，03:00），但这类单条 prompt 输出效果好，是因为模型对视觉效果做了过度优化（[[ai-prompt-to-ui-overoptimization]]，03:00），代价是大量重复代码、硬编码数值（[[ai-hardcoded-values-vs-design-tokens]]，03:00）而不遵循 design token。高级工程师的做法是先进入 [[plan-mode-design-system-integration|plan mode]]，要求 Agent 在规划阶段就基于已有 [[design-system|design system]] 展开（03:00），并可以借助 [[figma-mcp-design-to-code|Figma MCP]]（03:00）等 [[design-to-code-mcp|design-to-code MCP]]（18:04）让 Agent 直接对照 Figma 中的设计定义工作。约束 AI 的具体规则包括：要求使用 [[relative-css-units-ai-constraint|相对 CSS 单位]]（03:00）、遵循 [[single-record-principle|single record principle]] 避免 [[state-duplication-performance-risk|state 重复]]（03:00）。

设计系统本身分四步构建：先提炼 [[design-tokens|design tokens]]（15:02），再搭建 [[reusable-components|可复用组件]]，可以用 [[radix-ui|Radix]] 这类 headless 框架获得 [[component-library-accessibility|无障碍能力]]（15:02/18:04），然后用 [[composition-pattern-design-system|composition pattern]] 组合出高阶组件（18:04），最后用 [[storybook-component-tooling|Storybook]] 做工具化渲染部署（18:04）。这套体系形成 [[design-system-self-service-tiers|自助式分层接入]]（18:04），也呼应了视频提到的一种行业猜测——[[frontend-engineering-bifurcation-speculation|前端工程正在分化]]为全栈方向与设计系统专精方向（18:04）。

### 代码审查：static 与 dynamic 质量测量

审查 AI 生成的前端代码应分为两类：[[static-code-quality-measures|static 测量]]（不运行代码，确定性强、速度快）与 [[dynamic-code-quality-measures|dynamic 测量]]（实际执行，主要靠测试）（[[frontend-code-quality-static-dynamic-split]]，06:00）。审查重点应放在 [[component-props-state-shape-priority|组件的 props 类型与 state shape]]（06:00），因为依赖或全局配置改动的 [[blast-radius-dependency-change|blast radius]] 远大于某个组件写得不够优（06:00）；[[manual-review-trigger-config-changes|凡涉及 config、测试、linter、package.json 的改动都必须人工审查]]（06:00）。[[programming-to-interfaces-frontend|面向接口编程]]在前端体现为给 AI 清晰的边界（06:00）。

static 分析工具链除 [[linter-tooling|ESLint/Oxlint]]（09:01）外，还应引入 [[static-code-analysis-beyond-linting|新一代静态分析工具]]（09:01），重点检测 [[cyclomatic-complexity-analysis|cyclomatic complexity]]（09:01）、[[code-duplication-analysis|代码重复]]（09:01，对应 [[ai-code-duplication-tendency|AI 倾向于局部优化导致重复]]，09:01）和 [[component-file-length-analysis|文件长度]]（09:01），因为 [[ai-monolithic-component-antipattern|AI 常把多个子组件逻辑塞进单一巨型文件]]（09:01），而 [[static-analysis-bloat-blindspot|静态分析本身检测不出这种臃肿]]（09:01），需要靠写单元测试倒逼拆分。dynamic 侧要警惕 [[ai-fake-test-coverage|AI 制造虚假覆盖率]]（09:01），[[test-coverage-target-range|覆盖率目标建议 65%-85%]]（09:01），并对照 [[testing-pyramid|testing pyramid]] 检查测试结构（09:01），用 [[aaa-pattern|AAA pattern]]（arrange/act/assert）让 AI 写出的测试更易读（12:02）。此外应优先引入 [[typescript-for-large-scale-projects|TypeScript]] 以划定模块边界（09:01）。

### Token 经济学与最小化改动

LLM 计费中 [[llm-input-output-token-cost-asymmetry|input token 比 output token 便宜]]（12:02），因此 [[minimal-diff-token-cost-reduction|最简单的省 token 方式是减少改动量]]（12:02），这也解释了为何 [[testing-pyramid|unit test]] 比只依赖 end-to-end test 更省 debug 成本（12:02）。目前订阅制模型是高度补贴的（[[token-based-pricing-trend-coding-agents]]，12:02），但讲者预测未来会 [[ai-pricing-shift-token-to-compute|从按 token 计费转向按 GPU 计算时间计费]]（15:02），届时省 token 的意义会下降，重点转向通过 [[hexagonal-architecture|hexagonal architecture]]、[[solid-principles|SOLID principles]]、[[micro-frontends|micro-frontends]]、[[atomic-css|atomic CSS]] 等手段 [[minimize-change-size-ai-coding|最小化实现功能所需的代码改动范围]]（15:02），micro-frontends 还能通过 [[ai-context-scope-reduction-via-modularization|缩小 AI 读取的上下文范围]]进一步省 token（15:02）。像 [[caveman-skill|caveman skill]] 这类省 token 小技巧的长期价值存疑（15:02）。

### CSS box model 与响应式设计

[[css-box-model|CSS box model]] 由内到外是 content box、padding box、border（[[css-border-box]]）、margin box（[[css-margin-box]]）四层（18:04/21:06），[[css-outline-box-shadow-rendering-position|outline 和 box-shadow 渲染在 border 之后、margin box 之前]]（21:06）。[[css-box-sizing-property|box-sizing]] 默认 content-box，可切换为 border-box，二者在 [[extrinsic-width-concept|宽度计算逻辑]]上完全不同：content-box 是先算内容宽度再叠加 padding，border-box 则把 width 当总宽度去挤压内容（21:06）。[[box-model-knowledge-for-ai-bug-fixing|掌握 box model 能显著提升修复 AI 布局 bug 的速度]]，也是很多十年经验工程师说不清楚的考点（21:06）。

AI 常见的响应式失误是 [[ai-hardcoded-width-breaks-responsive-design|硬编码固定宽度]]（21:06），出问题后又倾向于用 [[ai-breakpoint-hack-vs-native-css-solution|堆砌大量断点]]去补救，而不是用一行原生 CSS 解决（21:06）。[[responsive-design-core-principles|响应式设计第一原则]]是优先用 [[relative-sizing-units|相对单位]]（27:07），组件级用 [[rem-vs-em-units|em]]、应用级用 rem（27:07），[[css-layout-algorithm-choice|布局算法选择]]上 flex 最通用、block 适合简单场景、grid 适合复杂布局（27:07），断点值应直接复用 [[css-breakpoints-reuse-existing-framework|Tailwind 等成熟框架]]而非重新造轮子（30:08）。[[ai-coding-productivity-illusion|资历浅的工程师用 AI 往往前期快、后 20% 卡在 bug 上反而更慢]]（24:07）。

顺带涉及的 CSS 优先级机制：[[css-cascade-algorithm|cascade algorithm]]（24:07）、[[css-specificity|specificity]] 的 A-B-C 三段计分（[[css-specificity-scoring-tiers]]，24:07；[[css-specificity-calculation]]，27:07）、[[css-specificity-tiebreak-rule|靠左位数一旦分出高低即直接判定胜负]]（27:07）、[[css-margin-collapsing|margin collapsing]] 这一历史遗留规则（24:07），以及在 [[chrome-devtools-computed-style-strikethrough|Chrome DevTools 中查看被覆盖样式的删除线标记]]（27:07）。

### Event loop 与 JS 单线程模型

[[js-single-threaded-design-reason|JS 被设计为单线程]]是为了让 DOM 渲染结果可预测（30:08），[[js-call-stack|调用栈]]、[[js-microtask-macrotask-queue|microtask/macrotask 队列]]都存在于 V8 引擎内，而 [[js-engine-vs-browser-runtime-split|event loop 本身是浏览器用 C++ 实现的]]，不属于 V8（30:08）。[[event-loop-mechanism|事件循环机制]]：先清空调用栈，再检查 microtask 队列，每处理完一个 microtask 就检查是否需要渲染（30:08）。可以把 [[event-loop|event loop]] 类比成两条并行传送带交替处理 JS 执行与渲染（33:08），因为 [[dom-modification-during-render-risk|浏览器不允许边渲染边改 DOM]]（33:08），[[main-thread-blocking|JS 执行和渲染共享同一主线程互斥执行]]（33:08）。生产环境最常见的相关 bug 是 [[event-handler-overload-performance-bug|表单绑定过多事件处理器导致输入卡顿]]（33:08），排查「应用很慢」类模糊反馈时第一步要区分 [[loading-speed-vs-input-reactiveness-diagnosis|是加载慢还是响应慢]]（33:08）。

### React 性能优化

加载慢问题：先用 [[react-bundle-size-analysis|bundle analyzer]] 查体积（36:08），检查是否用了 [[react-server-components|SSR/server components]]（36:08）减少 JS 发送量（[[critical-rendering-path]]，36:08），并通过 [[code-splitting-dynamic-import|dynamic import 做代码分割]]（36:08）。响应慢问题：思路只有让重渲染更快或避免其发生（[[rerender-optimization-strategies]]，36:08），手段包括检查 [[react-memoization-layer|memoization layer]]（36:08）、用 [[react-memo-prevents-rerender|React.memo]] 结合 [[use-callback-use-memo-purpose|useCallback/useMemo]]（36:08）、做 [[state-colocation|state colocation]] 避免不必要的 state 上提（36:08）、把非 state 依赖逻辑做 [[component-logic-extraction|组件外抽离]]（36:08）。有 [[react-compiler|React Compiler]] 时手动 memoization 会更轻松但仍建议多用（36:08），本质上都是 [[memoization-react-performance|把大任务拆成小颗粒度工作]]交给主线程（33:08）。

### Map/WeakMap 与垃圾回收

垃圾回收依据 [[garbage-collection-reachability|reachability]] 判断对象是否可回收（39:09）。[[map-vs-object-key-types|Map 支持任意类型 key]]、[[map-vs-object-iteration|自带 iterator]]，但生产中不如 Object 常用，主因是 [[map-adoption-syntax-comfort|语法舒适度不足]]（39:09），且 [[map-garbage-collection-limitation|Map 的 key 不会被自动垃圾回收]]，可能导致内存泄漏（39:09）。[[weakmap-garbage-collection|WeakMap 的 key 一旦不可达会被自动清除]]（39:09），因此更适合 [[weakmap-memoization-use-case|做 memoization 缓存]]（39:09），代价是 [[weakmap-no-iterator|不支持遍历]]（39:09）。

### 缓存、扩展性与实时通信

区分资深与初级工程师的不只是「用 CDN」，而是能解释 [[frontend-bundle-splitting|bundle 拆分]]如何影响 [[selective-caching-policy-frontend|差异化缓存策略]]（[[cdn-usage-sophistication-signal]]，42:09）：[[stable-vendor-chunk-long-max-age|稳定第三方库设长 max-age]]（如7天）、[[app-logic-chunk-short-max-age|业务逻辑设短 max-age]]（如5分钟）（42:09，[[max-age-http-cache-directive]]）。[[csr-frontend-scaling-simplicity|纯 CSR 单体架构本身可支撑到10万日活]]（42:09），[[micro-frontend-team-scaling|micro-frontend 的引入理由是团队规模而非用户量]]（42:09）。[[ssr-scaling-bottleneck|SSR 存在渲染请求集中回源的扩展瓶颈]]（45:09），现代方案是用 [[edge-computing-ssr|边缘计算做 SSR]]（45:09）配合 [[edge-database-replica|边缘只读数据库副本]]（45:09），但这带来 [[edge-architecture-write-consistency-tradeoff|写一致性代价]]（45:09）和 [[cap-theorem|CAP 定理]]下的最终一致性（45:09），[[edge-architecture-complexity-cost|整体是一种代价高昂、值不值得投入存疑的理想架构]]（45:09）。

实时通信选型上，[[polling-technique|polling]] 简单但易过载（45:09），[[long-polling-scalability-limit|long polling 扩展性差]]（48:09），[[websocket-communication|WebSocket]] 适合双向实时但后端开销大、实现复杂（48:09）。由于 [[llm-response-communication-asymmetry|LLM 输出是单向流式的不对称通信]]（48:09），[[server-sent-events-llm|SSE]] 是更合适的方案，浏览器原生支持、无需第三方库（48:09），[[openai-sdk-streaming-iterator|OpenAI SDK 底层用 SSE 但对外暴露迭代器接口]]（48:09），可在 [[chatgpt-claude-sse-observability|ChatGPT/Claude 的 Network 面板 event stream 中直接观察到]]（48:09）。

## 值得记住的细节

- 00:00 用 CSS transform/scale 而非 JS 改 width 实现 hover 放大，可避开 reflow、交给 compositor thread。
- 06:00 依赖、全局 config、linter/type checker、package.json 的改动必须人工审查；组件级改动若有规范把关可不逐个查。
- 09:01 test coverage 建议目标区间 65%–85%，过高反而可能混入 AI 生成的低质量测试。
- 09:01 可用 NPM 工具（如"follow"）自动检测组件文件长度，识别过度臃肿的文件。
- 21:06 box-sizing 默认是 content-box；border-box 下 width 是总宽度，会挤压内容导致 overflow。
- 24:07 CSS specificity 三段式计分 A-B-C：ID 加 A，class/attribute 加 B，元素类型加 C；靠左位一旦 1 比 0 直接决出胜负。
- 27:07 组件复用用 em（相对父元素），应用级统一观感用 rem（相对根字体大小）。
- 30:08 断点值建议直接复用 Tailwind 等成熟框架的既有方案，而非自己重新设计。
- 39:09 WeakMap 适合做 memoization 缓存，因为其 key 不可达时会被自动垃圾回收，但不支持遍历（无 forEach）。
- 42:09 稳定第三方库 chunk 建议 max-age 设为约 7 天，业务逻辑 chunk 建议约 5 分钟。
- 42:09 纯 client-side rendering 的单体前端架构本身可支撑到约 10 万日活用户，无需引入 micro-frontend。
- 45:09 边缘架构下只有一个主库负责写入，写操作成本更高，只能实现 eventual consistency（受 CAP 定理约束）。
- 48:09 可在浏览器 DevTools Network 面板的 event stream 标签中直接观察 ChatGPT/Claude 的 SSE token 流。

## 这个视频适合谁 / 可以跳过什么

适合已有一定前端经验、正在准备高级/资深前端面试，并且日常使用 AI coding agent（Claude Code、Copilot 等）的工程师，尤其是想系统了解「如何用底层原理审查和约束 AI 生成代码」的人。内容横跨渲染机制、CSS、JS 运行时、React 优化、缓存架构、实时通信协议，覆盖面广、深度足够支撑面试追问。如果已经非常熟悉 box model、event loop、CSS specificity 等基础前端八股，可以跳过 18:04–30:08 这段偏基础知识回顾的部分，直接看 03:00–18:04（AI workflow 与设计系统集成）和 42:09 之后（缓存、边缘架构、实时通信选型）这些更偏架构决策与 AI 协作策略的内容。
