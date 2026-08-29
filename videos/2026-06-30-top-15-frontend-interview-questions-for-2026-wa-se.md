---
video_id: AMerB8XjfZ0
url: https://www.youtube.com/watch?v=AMerB8XjfZ0
title: Top 15 Frontend Interview Questions for 2026 (wa/ Senior Engineer)
channel: theSeniorDev
published: '2026-06-30'
duration: '50:40'
transcript_origin: subs
tags:
- video
---

# Top 15 Frontend Interview Questions for 2026 (wa/ Senior Engineer)

摘要: [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se-summary|完整摘要]]

## 知识点

- [[aaa-pattern]] — 无论测试或 UI 多复杂，都可以用 AAA pattern 拆分：arrange 阶段准备 mocks 和 test doubles，act 阶段触发/渲染组件或点击按钮，assert 阶段做断言，这样让 AI 写出的测试更易读。（[12:02](https://youtu.be/AMerB8XjfZ0?t=722)）
- [[ai-breakpoint-hack-vs-native-css-solution]] — AI 出现响应式问题后的典型补救方式是添加大量断点并为每个断点单独指定宽度，而如果遵循浏览器引擎内置的标准写法，往往只需一行 CSS 代码就能解决，无需大量断点堆砌。（[21:06](https://youtu.be/AMerB8XjfZ0?t=1266)）
- [[ai-code-duplication-tendency]] — AI 倾向于做局部优化，经常会在代码库的不同位置重复写出功能相同的函数或组件。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- [[ai-coding-agent-dependency-bloat]] — 使用 AI coding agent 做前端开发时常见的问题是它们不仅会产生重复代码，还会安装实际上不需要的依赖（dependencies）。（[06:00](https://youtu.be/AMerB8XjfZ0?t=360)）
- [[ai-coding-productivity-illusion]] — 资历较浅的工程师用 AI 编程往往先获得很大的效率提升、快速完成 80% 的任务，但剩余 20% 会卡在各种 bug 上，最终发现用 AI 反而比自己动手写耗时更长，也没有学到多少东西。（[24:07](https://youtu.be/AMerB8XjfZ0?t=1447)）
- [[ai-coding-workflow-maturity-gap]] — 大多数初级前端开发者的 AI workflow 就是直接用 Claude Code，顶多再加上 Copilot 或 ChatGPT，但高级工程师想要高质量产出需要远不止于此。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
- [[ai-context-scope-reduction-via-modularization]] — 把前端 monolith 拆分为 micro-frontend 后，AI 理想情况下只需读取该特定 micro-frontend 的代码，而非整个代码库，从而减少输入 token 数量。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
- [[ai-fake-test-coverage]] — AI 几乎可以为任何代码写出测试，但除非人工核实，否则这些测试很可能只是制造出虚假的覆盖率（fake coverage），并未真正验证代码行为是否正确。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- [[ai-hardcoded-values-vs-design-tokens]] — AI 模型即便使用了 Tailwind，也常常不用 font-xs 这类原子 CSS class，而是直接写死 font-11px 这样的硬编码数值。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
- [[ai-hardcoded-width-breaks-responsive-design]] — AI coding model 经常直接给元素硬编码固定宽度（如 300px），这会完全破坏响应式设计，导致页面在桌面端看起来正常，但在移动端显示效果很差。（[21:06](https://youtu.be/AMerB8XjfZ0?t=1266)）
- [[ai-monolithic-component-antipattern]] — AI 编程最常见的问题之一是生成体积巨大的组件，把多个子组件的逻辑全部合并进单一文件里。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- [[ai-pricing-shift-token-to-compute]] — 讲者预测 AI 提供商未来会停止按 token 计费，转而按 GPU 计算时间收费，因此从长期看省多少 token 并不重要，重要的是占用了多少 GPU 时间。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
- [[ai-prompt-to-ui-overoptimization]] — Claude Code、GPT-4.8 之所以单条 prompt 输出效果惊艳，是因为它们针对 prompt 和视觉效果做了过度优化，代价是产生大量重复代码、不遵循已有 design token。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
- [[app-logic-chunk-short-max-age]] — 由于应用的业务逻辑和组件代码会频繁部署，这部分应该单独打包，并设置很短的 max-age（例如5分钟），以保证用户总能拿到最新的 JavaScript。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
- [[atomic-css]] — 采用 atomic CSS 等标准化样式方案可以减少前端开发新功能时需要新增的 CSS 改动量。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
- [[blast-radius-dependency-change]] — 代码审查时应优先检查依赖或全局配置的改动，因为这类改动一旦出错的影响范围（blast radius）远大于某个组件写得不够优（sub-optimal）的情况，后者通常够用且问题不大。（[06:00](https://youtu.be/AMerB8XjfZ0?t=360)）
- [[box-model-knowledge-for-ai-bug-fixing]] — 即使在 AI 编程盛行的当下，掌握 box model 仍然很重要，因为它能让开发者更快速地修复 AI 生成代码带来的布局 bug。（[21:06](https://youtu.be/AMerB8XjfZ0?t=1266)）
- [[browser-reflow]] — 用 JavaScript 直接修改 button 的 width 属性会触发 reflow，浏览器需要重新扫描该区域所有元素、重新计算宽高等布局属性，进而触发从布局到 GPU 生成像素的完整渲染流程。（[00:00](https://youtu.be/AMerB8XjfZ0?t=0)）
- [[cap-theorem]] — 根据 CAP 定理，边缘分布式数据库架构必然会出现一定程度的不一致状态，以换取系统在大部分情况下的可扩展性。（[45:09](https://youtu.be/AMerB8XjfZ0?t=2709)）
- [[caveman-skill]] — 很多人推荐 caveman skill 之类让 LLM 少说废话以省 token 的技巧，但讲者认为这类做法的长期价值存疑。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
- [[cdn-usage-sophistication-signal]] — 许多初中级前端工程师面对扩展性问题时只会回答「用 CDN」，但真正区分资深工程师的是能进一步说明应用的构建方式和 bundle 拆分策略如何影响可选择性的缓存能力。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
- [[chatgpt-claude-sse-observability]] — 打开ChatGPT或Claude的浏览器开发者工具Network面板，在对应请求的event stream标签中可以直接看到token一个个被推送过来，验证了这些主流聊天应用底层确实采用SSE传输模型输出。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
- [[chrome-devtools-computed-style-strikethrough]] — 在 Chrome DevTools 的元素样式面板里，被覆盖的 CSS 属性（如 background-color white）会显示为带删除线的文本，鼠标悬停在选择器上还能看到其 specificity 数值。（[27:07](https://youtu.be/AMerB8XjfZ0?t=1627)）
- [[code-duplication-analysis]] — code duplication analysis 能够量化代码库中有多少行代码、多少功能是完全重复的，用来发现 AI 造成的冗余代码。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- [[code-splitting-dynamic-import]] — 为了减少首屏加载的 JavaScript 量，应该使用 dynamic import 来延迟加载非必需代码，并可以按路径（path）或用户操作（user actions）进行 code splitting。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
- [[component-file-length-analysis]] — 可以用自动化工具（例如 NPM 上名为 follow 的工具）来检测文件长度，识别出过长、过度臃肿的组件文件。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- [[component-library-accessibility]] — 自己实现并做到 accessible 的组件（如 dropdown）成本很高，直接复用现成的 accessible 组件库能避免重复造轮子。（[18:04](https://youtu.be/AMerB8XjfZ0?t=1084)）
- [[component-logic-extraction]] — 让组件保持精简的做法是把不直接需要 state 的逻辑抽离成组件外部的独立函数，这样这部分逻辑只在应用加载时创建一次，不会随组件重新渲染而重复创建。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
- [[component-props-state-shape-priority]] — 审查 AI 生成的前端组件时，最应关注的是组件接收的 props 类型和 state 的 shape，这是决定其余代码质量的最关键因素。（[06:00](https://youtu.be/AMerB8XjfZ0?t=360)）
- [[composition-pattern-design-system]] — composition pattern 指把 button、input field 等基础组件组合起来，构建出更高阶的可复用组件，例如一个完整的表单。（[18:04](https://youtu.be/AMerB8XjfZ0?t=1084)）
- [[compositor-thread-layer-promotion]] — 把按钮提升到独立 layer 后，浏览器可以交给 compositor thread 处理像放大这样简单的变换，而不必经过主线程。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
- [[critical-rendering-path]] — 页面加载慢的根本原因通常是发送了过多 JavaScript：critical rendering path 中的大体积 CSS 和 JS 文件需要先被解析、解释后才能进行实际渲染。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
- [[csr-frontend-scaling-simplicity]] — 如果前端只做纯客户端渲染（client-side rendering），即使不引入 micro-frontend，单体前端应用架构本身也完全可以支撑到10万日活用户的规模。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
- [[css-border-box]] — border box 是 margin box 内部的下一层盒子，代表元素的 border，border 的厚度可以调整。（[18:04](https://youtu.be/AMerB8XjfZ0?t=1084)）
- [[css-box-model]] — CSS box model 由内到外依次是 content box、padding box、border、margin box 四个层级。（[21:06](https://youtu.be/AMerB8XjfZ0?t=1266)）
- [[css-box-sizing-property]] — box-sizing 属性默认值是 content-box，也可以设置为 border-box，这是一个常见的面试考点，因为很多人无法解释二者区别。（[21:06](https://youtu.be/AMerB8XjfZ0?t=1266)）
- [[css-breakpoints-reuse-existing-framework]] — 设计 breakpoint 和 media query 时不需要重新造轮子，可以直接使用像 Tailwind 这类大型框架已经过大量测试的断点值，既可以直接使用 Tailwind，也可以让 coding agent 在项目中全局实现 Tailwind 的断点方案。（[30:08](https://youtu.be/AMerB8XjfZ0?t=1808)）
- [[css-cascade-algorithm]] — 当多条 CSS 规则的 selector 都指向同一个元素时，浏览器会收集这些规则并执行 cascade algorithm 来确定最终样式；若这些规则处于同一 layer，其中一步就是比较各 selector 的 specificity 得分。（[24:07](https://youtu.be/AMerB8XjfZ0?t=1447)）
- [[css-layout-algorithm-choice]] — flex 通常是实现响应式布局最简单的方式，block（浏览器默认布局，段落纵向排列、单词横向排列）也适合非常简单的布局；grid 适合复杂布局，但只有在熟练掌握 grid 或大量配合媒体查询时才能用好。（[27:07](https://youtu.be/AMerB8XjfZ0?t=1627)）
- [[css-margin-box]] — margin box 是 CSS box model 中最外层的盒子，包含元素本身及其 margin 和 outline。（[18:04](https://youtu.be/AMerB8XjfZ0?t=1084)）
- [[css-margin-collapsing]] — margin collapsing 是 CSS box model 中内建的一个例外规则，起源于早期 Web 以段落（paragraph）排版为主的时代，用来让相邻元素间的外观更美观，也是高级前端工程师面试中的常见考点。（[24:07](https://youtu.be/AMerB8XjfZ0?t=1447)）
- [[css-outline-box-shadow-rendering-position]] — outline 和 box-shadow 这类效果被渲染在 padding box 与 margin box 之间，也就是紧跟在 border 之后的位置。（[21:06](https://youtu.be/AMerB8XjfZ0?t=1266)）
- [[css-specificity]] — 要理解 CSS specificity，需要先理解每条 CSS 声明（declaration）都包含一个 selector，例如可以先用泛化的元素选择器（如 form），再逐步细化为带 class 或 ID 的更具体选择器。（[24:07](https://youtu.be/AMerB8XjfZ0?t=1447)）
- [[css-specificity-calculation]] — 计算 specificity 时，引用 element 类型（如 form）记一分，class 或 attribute 选择器记一分，ID 选择器单独记一分，三者分属不同位次而非同一累加值。（[27:07](https://youtu.be/AMerB8XjfZ0?t=1627)）
- [[css-specificity-scoring-tiers]] — CSS specificity 的计分方式是一个三段式分数 A-B-C，起始都是 000：selector 中每出现一个 ID 就让 A 加一，每出现一个 class 或 attribute 选择器就让 B 加一。（[24:07](https://youtu.be/AMerB8XjfZ0?t=1447)）
- [[css-specificity-tiebreak-rule]] — 两个选择器比较 specificity 时，只要靠左的位（如 ID 位）出现1比0的差异就直接决定胜负，根本不会再去看后面较低位的数字。（[27:07](https://youtu.be/AMerB8XjfZ0?t=1627)）
- [[css-transform-compositor-thread]] — 用 CSS transition 配合 scale 这类 CSS transform 实现按钮悬停变大效果，可以绕开 reflow，直接交给 compositor thread 处理，因为这是纯数学变换、不需要修改布局树。（[00:00](https://youtu.be/AMerB8XjfZ0?t=0)）
- [[cyclomatic-complexity-analysis]] — cyclomatic complexity 分析特别适合发现哪些函数逻辑分支过多、嵌套过深，从而提示需要拆分重构的位置。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- [[design-system]] — 构建一个好的设计系统能让 AI 辅助开发更快，并为界面提供视觉一致性（visual cohesion），其第一步是提炼出 design tokens。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
- [[design-system-self-service-tiers]] — 设计系统可提供多层级自助式使用方式——直接用 design tokens、使用现成可用组件，或使用满足特定功能的完整组合组件，LLM 或其他开发者可按需选择合适层级接入。（[18:04](https://youtu.be/AMerB8XjfZ0?t=1084)）
- [[design-to-code-mcp]] — design-to-code MCP 让 LLM 能连接 Figma 作为 source of truth，编码 agent 实现功能时可以自动对照 Figma 中的设计系统定义进行优化调整。（[18:04](https://youtu.be/AMerB8XjfZ0?t=1084)）
- [[design-token]] — 把可复用组件库（component library）与自己的 design tokens 结合使用，就能获得开箱即用的 accessible 组件。（[18:04](https://youtu.be/AMerB8XjfZ0?t=1084)）
- [[design-tokens]] — 设计系统的第一步是定义 design tokens，通常以 CSS custom properties 形式存储在根元素上（如品牌色变量），供所有组件复用，使全局样式变更（如换品牌色）只需一行代码即可完成。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
- [[dom-modification-during-render-risk]] — 浏览器不允许在渲染的同时修改 DOM，因为这会破坏 UI 状态、且让编程模型难以处理，所以刻意把 JS 执行与渲染设计为互斥的两个阶段。（[33:08](https://youtu.be/AMerB8XjfZ0?t=1988)）
- [[dynamic-code-quality-measures]] — dynamic 质量测量指实际执行应用代码，主要形式是测试，前端里以 unit test 为主，也包括 end-to-end test 和 integration test。（[06:00](https://youtu.be/AMerB8XjfZ0?t=360)）
- [[edge-architecture-complexity-cost]] — 这种边缘分布式 SSR + 边缘数据库的方案是一种非常假设性的理想架构，大多数场景不值得投入，因为它涉及大量 cache invalidation，一旦出问题会非常难以调试。（[45:09](https://youtu.be/AMerB8XjfZ0?t=2709)）
- [[edge-architecture-write-consistency-tradeoff]] — 边缘架构中只有一个主版本数据库负责实际写入，所有写操作都要回到这个主 DB；写操作因此成本更高，且写入的数据需要传播到各只读副本，导致只能实现 eventual consistency。（[45:09](https://youtu.be/AMerB8XjfZ0?t=2709)）
- [[edge-computing-ssr]] — 现代解决 SSR 延迟问题的做法是使用类似 Cloudflare Workers 的边缘系统，把分布式后端部署在全球各地，在靠近用户的位置完成 server-side rendering。（[45:09](https://youtu.be/AMerB8XjfZ0?t=2709)）
- [[edge-database-replica]] — 一旦后端被分布式部署到边缘 worker，数据库也必须随之下沉到边缘，通常做法是通过 Prisma 等服务提供的分布式只读数据库副本，把数据放在靠近用户的位置。（[45:09](https://youtu.be/AMerB8XjfZ0?t=2709)）
- [[event-handler-overload-performance-bug]] — 最常见的与 event loop 相关的生产环境 bug 是表单里绑定了过多事件处理器，用户打字时触发大量重渲染任务被推入栈中，导致输入出现明显卡顿（lagging）。（[33:08](https://youtu.be/AMerB8XjfZ0?t=1988)）
- [[event-loop]] — event loop 可以类比为两条并行传送带，把 JS 执行（microtask）和渲染工作交替推送给同一个 CPU：先处理一段 JS，再检查是否有渲染任务要做，处理完再回来处理下一段 JS，如此循环。（[33:08](https://youtu.be/AMerB8XjfZ0?t=1988)）
- [[event-loop-mechanism]] — 事件循环会先检查主线程是否空闲，空闲时执行调用栈中的所有任务；调用栈清空后再检查 microtask 队列，若队列中有任务就将其压入栈底执行；一个 microtask 执行完毕后不会立刻连续处理下一个，而是先检查主线程是否需要进行渲染。（[30:08](https://youtu.be/AMerB8XjfZ0?t=1808)）
- [[extrinsic-width-concept]] — 当元素设为 border-box 并指定 width: 300px 时，浏览器会把这个值当作固定总宽度去挤压内容，内容过多则产生溢出（overflow）。（[21:06](https://youtu.be/AMerB8XjfZ0?t=1266)）
- [[figma-mcp-design-to-code]] — 通过 Figma MCP 这类 design-to-code MCP，可以让 Coding Agent 在做功能规划时基于已有的设计 blocks 和现有功能来展开，而不是凭空生成。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
- [[frontend-bundle-splitting]] — 对纯 client-rendered 前端应用做扩展时，第一步通常是把静态资源（JS、HTML、CSS）推送到 CDN，并在此基础上做 bundle splitting，而不是简单地整体推送单一 bundle。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
- [[frontend-code-quality-static-dynamic-split]] — 前端代码质量保障可分为两大类：static 测量（不运行代码、只检查代码结构）和 dynamic 测量（实际执行应用），面试中应清晰地展示这种分类思路而非笼统提及 linter 或测试。（[06:00](https://youtu.be/AMerB8XjfZ0?t=360)）
- [[frontend-engineering-bifurcation-speculation]] — 前端生态最近流传一种猜测——前端工程正在消失，未来前端工程师要么转向 full stack（因为有 AI 辅助全栈开发变得更容易），要么专精于构建可供其他工程师复用的设计系统。（[18:04](https://youtu.be/AMerB8XjfZ0?t=1084)）
- [[garbage-collection-reachability]] — 垃圾回收算法判断一个对象是否可回收，依据是它是否仍然"可达"（reachable），即是否与 DOM 或事件处理器等保持关联；若不再关联，垃圾回收器会将其标记为可重新分配的内存。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
- [[hexagonal-architecture]] — 一旦计费模式转向按计算时间而非按 token，工程重点会转向通过 decoupling、hexagonal architecture 等设计手段最小化实现一个功能所需改动的代码范围。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
- [[interview-senior-depth-signaling]] — 面对『AI agent 通过修改 width 实现按钮悬停变大』这一问题，senior 工程师的回答方式是先质疑该实现是否高效，再从 reflow、compositor thread 等底层渲染机制展开分析，而不只是描述现象本身。（[00:00](https://youtu.be/AMerB8XjfZ0?t=0)）
- [[js-call-stack]] — 每当执行一个函数时，会将其压入调用栈（call stack）形成一个栈帧（stack frame），栈帧内保存该函数的闭包（closures）和所有会用到的变量，用于实际执行该函数。（[30:08](https://youtu.be/AMerB8XjfZ0?t=1808)）
- [[js-engine-vs-browser-runtime-split]] — 调用栈、microtask 队列和 macrotask 队列这些结构都存在于 V8 引擎内部，而事件循环（event loop）本身并不属于 V8 引擎，而是由浏览器用 C++ 实现的。（[30:08](https://youtu.be/AMerB8XjfZ0?t=1808)）
- [[js-microtask-macrotask-queue]] — JavaScript 运行时除了调用栈外还维护 microtask 队列和 macrotask 队列：Promise resolve 后的回调（如 .then）不会直接压入调用栈，而是先进入 microtask 队列；浏览器事件（如 click）触发的事件处理函数或定时器（timer）回调则会进入 macrotask 队列。（[30:08](https://youtu.be/AMerB8XjfZ0?t=1808)）
- [[js-single-threaded-design-reason]] — JavaScript 被设计为单线程，主要是为了让 DOM 的渲染结果更容易预测；虽然浏览器本身大多是多线程的，但如果让 JS 也变成多线程执行，会因并行化带来难以预料且危险的 bug，尤其是因为每次修改 JavaScript 都会影响 DOM 这个唯一的单例结构。（[30:08](https://youtu.be/AMerB8XjfZ0?t=1808)）
- [[js-triggered-animation-cost]] — 如果动画效果是通过 JavaScript 在 mouseenter 事件里修改 width 实现的，比单纯用 CSS 触发 reflow 更差，因为它还额外占用了 main thread 去执行 JavaScript 逻辑。（[00:00](https://youtu.be/AMerB8XjfZ0?t=0)）
- [[linter-tooling]] — 静态分析的第二步是引入 linter，例如 ESLint 或性能更优的 Oxlint，这是保证代码质量的基础工具。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- [[llm-input-output-token-cost-asymmetry]] — LLM 的基本工作方式是给模型一个 input 得到一个 output，如果把代码库改动拆分为 input 和 output token，通常 input token 比 output token 便宜很多。（[12:02](https://youtu.be/AMerB8XjfZ0?t=722)）
- [[llm-response-communication-asymmetry]] — 在 LLM 场景下，客户端发送一次查询后，模型会依次返回第一个token、第二个token、第三个token直到最终完整句子，这种高度不对称的通信模式是选择流式传输方案而非轮询或WebSocket的关键原因。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
- [[loading-speed-vs-input-reactiveness-diagnosis]] — 面对产品经理反馈「应用很慢」这类模糊问题时，第一步应先厘清究竟是加载速度慢，还是对用户输入的响应迟钝，两者排查方向完全不同。（[33:08](https://youtu.be/AMerB8XjfZ0?t=1988)）
- [[long-polling-scalability-limit]] — 轮询方式虽然易于实现且很健壮，但如果有上万个客户端同时轮询，请求量会成倍叠加，容易把后端打垮，本质上是自己对自己发起了DDOS，因此扩展性不好。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
- [[main-thread-blocking]] — JS 执行和 DOM 渲染共享同一个主线程（CPU）处理空间，任意时刻只能执行其中一项，这是浏览器有意为之的设计，而不是拆分成两个可并行的独立线程。（[33:08](https://youtu.be/AMerB8XjfZ0?t=1988)）
- [[main-thread-reflow-dom-modification]] — 修改 DOM 会触发主线程 reflow，这个改动要先压入调用栈、被解释执行，因此应尽量避免频繁触发。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
- [[main-thread-vs-compositor-thread]] — compositor thread 被设计用来高效处理滚动这类操作而不占用 main thread，只要避免触发 reflow，main thread 就能保持空闲去处理 JavaScript 或其他任务，实现动画与逻辑执行互不阻塞。（[00:00](https://youtu.be/AMerB8XjfZ0?t=0)）
- [[manual-review-trigger-config-changes]] — 只要 AI 改动了全局 config、测试、linter、type checker 或 package.json（即新增依赖）等文件，就必须进行人工手动审查；其余组件级改动若已有合适的规范（widgets）把关则无需逐个检查。（[06:00](https://youtu.be/AMerB8XjfZ0?t=360)）
- [[map-adoption-syntax-comfort]] — Map 在生产环境中不如 Object 常用的主要原因是其语法不如 Object 那样普及和舒适，只有当 key 需要超出字符串/symbol 范畴时才会考虑用 Map。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
- [[map-garbage-collection-limitation]] — Map 中的 key 即使指向已不再需要的对象，也不会被垃圾回收，如果持续往 Map 添加内容而不手动清理，会导致内存泄漏（memory leak）。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
- [[map-vs-object-iteration]] — 遍历 Object 需要借助 Object.entries() 或 Object.keys()，而 Map 直接内置了 iterator，可以直接被遍历。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
- [[map-vs-object-key-types]] — Map 适合用作需要任意类型 key（包括对象）的存储结构，因为它天生擅长构建以对象为 key 的内存映射。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
- [[max-age-http-cache-directive]] — max-age 本质上是决定客户端多久应该重新检查并刷新某个资源的参数，可以针对不同类型的资源设置不同数值。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
- [[memoization-react-performance]] — 主线程的任务栈被设计为擅长处理大量微小的独立工作单元，因此应尽量使用 memoization、把每次更新拆成小颗粒度的工作，而不要一次性推送大块任务，尤其在大型组件框架中。（[33:08](https://youtu.be/AMerB8XjfZ0?t=1988)）
- [[micro-frontend-team-scaling]] — 只有当有大量开发者同时在同一个前端应用上工作时，才有必要考虑引入 micro-frontend 架构，目的是获得更好的故障隔离模式和更小的爆炸半径，而不是单纯为了应对用户量增长。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
- [[micro-frontends]] — 当很多人共同贡献同一个前端代码库时，采用 micro-frontends 架构可以缩小单次改动出错的影响范围（blast radius），便于控制损害。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
- [[minimal-diff-token-cost-reduction]] — 降低 token 花费最简单的方法是在实现一个 feature 时尽量减少代码库中的改动量，这与传统软件工程中追求以最小改动交付功能的理念是一致的。（[12:02](https://youtu.be/AMerB8XjfZ0?t=722)）
- [[minimize-change-size-ai-coding]] — 面对 AI 大量参与代码编写，团队应优先追求小改动，通过统一使用 design tokens、atomic CSS 等标准化手段减少每次开发新功能所需的代码变更量。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
- [[openai-sdk-streaming-iterator]] — OpenAI 的官方包底层使用SSE来传输数据，但对开发者暴露的是一个迭代器接口，使开发者可以直接遍历获取每个生成的token，而无需自己处理原始的SSE事件流。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
- [[plan-mode-design-system-integration]] — 高级前端工程师使用 AI 编码时会先进入 plan mode，并要求 Agent 在规划阶段就使用已有的 design system。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
- [[polling-technique]] — 实现类似实时通信最简单的方式是 polling：使用 setInterval 等定时器函数每隔几秒调用一次后端接口，检查是否有新数据并更新界面。（[45:09](https://youtu.be/AMerB8XjfZ0?t=2709)）
- [[programming-to-interfaces-frontend]] — 把面向接口编程应用到前端时，关键是在 data layer 遵循清晰接口，同时更关注组件代码的边界（boundaries），因为 AI 一旦被给定明确边界就能很好地执行任务。（[06:00](https://youtu.be/AMerB8XjfZ0?t=360)）
- [[radix-ui]] — Radix 是一个 headless 组件框架，内置了无障碍性等基础交互能力，团队可以直接在其上应用自己的样式，而无需从零实现底层交互逻辑。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
- [[react-bundle-size-analysis]] — 当 React 应用出现加载慢的问题时，第一步应该用 module bundle analyzer 检查 bundle size，找出可以消除或延迟加载的库。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
- [[react-compiler]] — 如果项目使用了 React Compiler，手动做 memoization 会更容易，但仍然建议尽可能多地使用 memo、useCallback 等手段。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
- [[react-memo-prevents-rerender]] — React.memo 会比较组件的 props，如果收到的 props 没有变化，就不会仅因为父组件重新渲染而重新渲染该子组件。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
- [[react-memoization-layer]] — 排查加载慢问题时，除了 bundle size，还要检查项目的 memorization layer，即是否合理使用了 memo、useCallback、useMemo 来加快渲染、避免重新渲染。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
- [[react-server-components]] — 排查加载性能时要检查项目是否使用了 SSR 和 server components，因为尽量减少或延迟发送 JavaScript 是让页面加载更快的关键手段。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
- [[relative-css-units-ai-constraint]] — 为约束 AI 编码行为，需要明确要求它在 CSS 中使用相对单位，而不是像 AI 默认那样硬编码具体像素值。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
- [[relative-sizing-units]] — 响应式设计第一原则是尽量做到自适应（adaptive），具体做法是避免使用 pixel 这类绝对单位，改用百分比、rem 或 em 等相对单位。（[27:07](https://youtu.be/AMerB8XjfZ0?t=1627)）
- [[rem-vs-em-units]] — 构建可复用组件时适合用 em（相对父元素），而构建整个应用范围内统一观感时更适合用 rem（相对根元素字体大小）。（[27:07](https://youtu.be/AMerB8XjfZ0?t=1627)）
- [[rerender-optimization-strategies]] — 在 React 中处理用户输入引发的重新渲染问题，思路只有两种：要么让重新渲染更快，要么直接避免它发生。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
- [[responsive-design-core-principles]] — 在用 AI 生成代码前就应遵循响应式设计原则，否则 AI 生成的界面往往只在开发者自己的电脑上好看，在手机等其他设备上无法正常显示。（[27:07](https://youtu.be/AMerB8XjfZ0?t=1627)）
- [[reusable-components]] — 设计系统的第二个支柱是构建可复用组件（如 input、button），团队可以从零开发，也可以使用像 Radix 这样的 headless 组件框架来获得无障碍能力后再自行套样式。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
- [[selective-caching-policy-frontend]] — 前端应用中变化很少的部分（如设计系统、核心逻辑、稳定的第三方库）应该和经常变化的部分分开打包，从而可以对它们分别设置不同的缓存策略。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
- [[server-sent-events-llm]] — 使用SSE时，客户端发起一个携带完整对话内容的POST请求，然后在该端点上持续监听，随着模型逐步生成内容不断收到对应的token chunk，是目前最健壮的LLM流式传输方式之一。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
- [[single-record-principle]] — 为约束 AI 生成的 state 架构，需要明确要求其遵循 single record principle：一份数据在整个状态中只表示一次。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
- [[solid-principles]] — SOLID principles 与 design patterns 被认为是在 AI 编码成本模型转向按计算时间收费后，用于降低改动范围、控制影响半径的关键设计手段。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
- [[ssr-scaling-bottleneck]] — SSR 的复杂性在于，用户拿到静态资源后仍需回源请求服务器完成渲染，所有用户的渲染请求都集中打到同一服务器，形成 scaling bottleneck。（[45:09](https://youtu.be/AMerB8XjfZ0?t=2709)）
- [[stable-vendor-chunk-long-max-age]] — 像 React、ReactDOM 这类几乎每年都不会变的稳定第三方库，应该被打包进单独的 chunk 文件，并设置较长的 max-age（例如7天），减少客户端重复下载。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
- [[state-colocation]] — 如果把 state 不必要地提升到组件树较高层级（lift state up），该 state 变化时会导致其下所有组件自动重新渲染；把 state 保持在靠近使用它的地方，可以避免这种不必要的重新渲染。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
- [[state-duplication-performance-risk]] — AI 生成前端代码时容易把同一份数据在 state 中重复表示，这类 state 重复常常会在后期变成性能瓶颈。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
- [[static-analysis-bloat-blindspot]] — 静态分析（static analysis）即便代码文件极度臃肿庞大也可能全部检查通过，因此不能仅依赖它来发现过大文件的问题，还需要通过为其编写单元测试来倒逼拆分。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- [[static-code-analysis-beyond-linting]] — 由于 AI 编程的普及，出现了一批超越传统 linting 的静态代码分析新工具，重点检测 cyclomatic complexity 和代码重复。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- [[static-code-quality-measures]] — static 质量测量因为不需要执行代码、只检查结构，所以是确定性的（deterministic）且速度很快，相比之下让 LLM 生成代码通常较慢且消耗大量 token。（[06:00](https://youtu.be/AMerB8XjfZ0?t=360)）
- [[storybook-component-tooling]] — Storybook 是构建设计系统的第四步（tooling）中的核心工具，用于渲染和部署组件，使团队所有人都能访问、渲染组件并与其交互。（[18:04](https://youtu.be/AMerB8XjfZ0?t=1084)）
- [[test-coverage-target-range]] — 作为 senior 工程师应关注 test coverage 指标，建议目标定在 65% 以上但不超过 85%，因为过高的覆盖率容易掺入 AI 生成的低质量测试。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- [[testing-pyramid]] — 除了看覆盖率数字，senior 工程师还应该对照传统的 testing pyramid 模型，判断团队当前的测试结构处于金字塔的哪个位置。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- [[token-based-pricing-trend-coding-agents]] — 目前如 Claude Code 这类模型在普通订阅方案下是高度补贴的，用户通常不直接按 token 付费，但行业正朝着按 token 计费的方向发展。（[12:02](https://youtu.be/AMerB8XjfZ0?t=722)）
- [[typescript-for-large-scale-projects]] — 在前端项目中优先引入 TypeScript，因为它天生适合大规模代码、多人协作的场景，能更容易地划定模块边界。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
- [[unit-integration-test-boundary-ambiguity-frontend]] — 在前端场景下，unit test 和 integration test 之间的边界比较模糊，很难明确界定一个组件测试应该算 unit test 还是 integration test。（[06:00](https://youtu.be/AMerB8XjfZ0?t=360)）
- [[use-callback-use-memo-purpose]] — 当组件确实需要重新渲染时，使用 useCallback 和 useMemo 可以确保组件内声明的变量和函数不会被不必要地重新计算。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
- [[weakmap-garbage-collection]] — 与 Map 不同，WeakMap 中一旦某个 key 不再被引用（不可达），垃圾回收算法会自动将其从 WeakMap 中移除，从而避免内存泄漏。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
- [[weakmap-memoization-use-case]] — 当需要为函数做 memoization（结果缓存）时，使用 WeakMap 比普通 Map 或 Object 更安全、更省内存，因为不再使用的缓存 key 会被自动垃圾回收。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
- [[weakmap-no-iterator]] — WeakMap 不支持 forEach 或直接遍历其所有 key，必须自己单独保存曾经访问过的 key 才能再次取用，因此编程上使用起来比 Map 更繁琐。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
- [[websocket-communication]] — WebSocket 让每个客户端与后端建立一条双向通信通道，消息可以双向实时推送，非常适合聊天类应用中点对点即时通讯的场景。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
