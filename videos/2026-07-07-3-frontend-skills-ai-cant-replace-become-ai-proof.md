---
video_id: hA_XnzB1Ef8
url: https://www.youtube.com/watch?v=hA_XnzB1Ef8
title: 3 Frontend Skills AI Can't Replace (become AI-proof)
channel: theSeniorDev
published: '2026-07-07'
duration: '15:15'
transcript_origin: subs
tags:
- video
---

# 3 Frontend Skills AI Can't Replace (become AI-proof)

摘要: [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof-summary|完整摘要]]

## 知识点

- [[accessibility-non-functional-business-deprioritization]] — 可访问性是一种非功能性需求，不直接产生核心商业价值，因此业务方通常会催着团队做完就转到下一个任务，而不愿投入更多资源。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
- [[accessibility-semantic-html-instruction]] — 让 AI agent 处理可访问性（accessibility）需求时，第一条指令是要求其使用 semantic HTML，这是一项定义清晰、可被自动化执行的规则。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
- [[ai-accessibility-automation-speedup]] — 过去团队常常要专门安排为期两周的 accessibility sprint 来处理无障碍问题，而现在这类粒度化、组件级别的工作大部分可以交给 AI agent 自动完成。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
- [[ai-automated-test-writing]] — 写测试是被 AI 自动化程度最高的工作之一，只要工程师清楚自己想要的测试覆盖率和 testing pyramid 结构，就能借助 AI 大幅提速。（[03:01](https://youtu.be/hA_XnzB1Ef8?t=181)）
- [[ai-clear-objective-performance]] — 只要任务有明确的成功标准（例如把 core web vitals 压到某个指标以下），LLM 在这类问题上表现就相当不错。（[03:01](https://youtu.be/hA_XnzB1Ef8?t=181)）
- [[ai-code-duplication-tendency]] — 内联声明的组件因作用域被局限在父组件内部而无法被复用，导致 AI 每次遇到相似的小问题时都要重新写一遍类似代码，造成大量代码重复。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
- [[ai-code-quality-needs-explicit-prompting]] — code quality 是 LLM 在没有被明确要求时最容易做不好的一环，属于生成代码中普遍存在的问题。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
- [[ai-context-scope-reduction-via-modularization]] — 拥有清晰模块边界的前端架构，能让 AI agent 在扩展代码时用更少的 token 实现同等价值的功能增量，这是从 context engineering 角度出发选择模块化架构的重要理由。（[00:00](https://youtu.be/hA_XnzB1Ef8?t=0)）
- [[ai-feature-overfitting-architecture]] — 用 LLM 编码的第二个问题是：每实现一个新功能，AI 都容易让整个架构向该功能过拟合，因为模型的目标是用单条 prompt 展示尽可能惊艳的效果，却以牺牲此前架构的稳定性为代价。（[00:00](https://youtu.be/hA_XnzB1Ef8?t=0)）
- [[ai-generated-ui-maintainability-illusion]] — AI 生成的前端代码表面上能正常运行、没有明显 bug，但实际上维护和扩展成本极其高昂。（[00:00](https://youtu.be/hA_XnzB1Ef8?t=0)）
- [[ai-hardcoded-values-vs-design-tokens]] — 即使项目已经配置好设计系统（如 Tailwind），AI 在还原用户提供的截图时仍可能写死具体数值（如 text-28px），而不是复用已有的预定义原子样式类。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
- [[ai-increases-test-coverage]] — 讲者观察到，现在用 AI 辅助构建的项目普遍比过去手写测试时拥有更高的测试覆盖率。（[03:01](https://youtu.be/hA_XnzB1Ef8?t=181)）
- [[ai-performance-architecture-prompting]] — 较新一代模型在做性能优化时不再单纯抄近路，而是会反过来就架构决策向用户提问。（[03:01](https://youtu.be/hA_XnzB1Ef8?t=181)）
- [[ai-prompt-to-ui-overoptimization]] — 包括最新开源模型在内的大多数 AI coding agent 都被高度优化为「从 prompt 直出 UI」，因此用它们写出的前端代码往往视觉效果漂亮，但内部各实体边界定义不清、相互纠缠交互。（[00:00](https://youtu.be/hA_XnzB1Ef8?t=0)）
- [[ai-target-hyperoptimization-root-cause]] — AI 编码模型的一大通病根源在于它被构建为要不惜一切满足用户给定的具体目标（如截图还原度），因此会倾向于走捷径产生代码坏味道，而不是遵循已有的设计系统。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
- [[ai-tedious-performance-fix-automation]] — 只要明确了优化方向，压缩图片、重构组件等繁琐的性能实现工作现在可以用一条 prompt 交给 AI 完成，不再需要每天手动去做。（[03:01](https://youtu.be/hA_XnzB1Ef8?t=181)）
- [[ai-test-coverage-effort-reduction]] — 过去写测试要自己想清楚怎么 mock、如何 mount component，非常耗时；现在这些繁琐工作可以交给 LLM 完成，只需给出测试目标和测试对象即可，几小时就能完成过去需要数天的工作。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
- [[aria-label-fallback-instruction]] — 当必须走捷径使用大量 div 而无法采用语义化元素时，应指示 AI 使用 area/ARIA label 来标示该元素的用途。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
- [[atomic-css]] — 像 TXL 这样预先定义好的原子化 CSS 类之所以存在，部分原因是为了在整个应用中向用户呈现一致的视觉体验。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
- [[code-duplication-analysis]] — 一个真实生产系统的静态分析结果显示代码库中有 9% 的代码片段完全重复（而非仅有部分共享逻辑），这是缺乏代码质量审查的 vibe coding 所导致的典型后果。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
- [[component-extraction-for-reuse-testability]] — 解决内联组件问题的方法是把该组件提取到单独文件，必要时配合 memoization，这样组件既可复用，也可以在需要时为其单独编写 unit test。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
- [[component-library-accessibility]] — 如果公司级设计系统（design system）已经把组件的无障碍性（accessibility）做好，AI 在生成组件时可以直接复用该设计系统的能力，工程师只需做一次轻量复核（soft check），而不必从零验证 accessibility。（[12:03](https://youtu.be/hA_XnzB1Ef8?t=723)）
- [[context-dilution]] — 把整个代码库都丢给 AI 去查找已实现的可复用功能，会因为上下文过大而稀释注意力，让模型进入表现下降的「dumb zone」，最终结果反而更差。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
- [[deep-module]] — 优秀的前端架构应具备清晰的模块边界，由多个各自承担明确职责的服务组成，并向外界隐藏大量实现细节，只暴露清晰的接口。（[00:00](https://youtu.be/hA_XnzB1Ef8?t=0)）
- [[design-to-code-elimination]] — 过去占前端工作80%的设计稿转代码（design to code）机械性工作，已经基本被 AI 取代而消失。（[03:01](https://youtu.be/hA_XnzB1Ef8?t=181)）
- [[design-to-code-skill]] — design-to-code（把设计稿转成 HTML 或可用组件）是受 AI 影响最大的前端技能领域之一，未来工程师的工作将主要变成审查 AI 生成的实现结果，而非亲手实现。（[00:00](https://youtu.be/hA_XnzB1Ef8?t=0)）
- [[essential-state]] — 构建组件时最重要的底层技能之一，是能看着 UI 判断出最合适的数据结构，把状态收敛为「essential state」，而不是照搬 UI 呈现出的每个细节去建模。（[12:03](https://youtu.be/hA_XnzB1Ef8?t=723)）
- [[front-end-system-design]] — 面对AI冲击，前端工程师应优先投资的第一项技能是前端系统设计（front-end system design），聚焦前端本身，不需要深入数据库分片、负载均衡等后端知识。（[00:00](https://youtu.be/hA_XnzB1Ef8?t=0)）
- [[front-end-team-size-reduction-ai]] — 原本需要五个人做的『把设计稿贴成按钮、改样式』这类机械性工作，现在可以压缩为一个人配合 AI coding agent 和 design system 完成。（[03:01](https://youtu.be/hA_XnzB1Ef8?t=181)）
- [[frontend-job-ai-proofing-depth]] — 若担心 AI 取代前端工作，工程师应同时修炼两项能力：高层次的 system design 视角，以及能够深入检视代码库具体构成的细粒度（granular）分析能力。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
- [[inline-component-declaration-antipattern]] — AI 生成的前端代码中常见把一个如 text 渲染这样的子组件直接内联声明在父组件内部，而不是拆分出去，导致其在每次父组件重新渲染时都被重复创建。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
- [[interview-senior-depth-signaling]] — 同时具备系统设计的宏观视野，以及对浏览器、React 等框架、JavaScript 底层机制的深入理解，是候选人在面试中被认定为具备 senior 水平的关键因素。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
- [[manual-code-review-necessity-ai-output]] — 使用 agent 生成代码后，工程师需要打开对应 pull request 亲自做 code review（而非让 AI 做 code review），这被类比为工厂大量产出蛋糕后，你必须亲口尝一尝才能知道好不好吃。（[12:03](https://youtu.be/hA_XnzB1Ef8?t=723)）
- [[picasso-ball-metaphor]] — 作者用「毕加索的球」作比喻：先画出细节繁复的球，再逐步简化为最精简的轮廓抽象；对应到编码中，就是从堆满冗余 state 的「意大利面」实现，收敛成只保留核心抽象的最小状态模型。（[12:03](https://youtu.be/hA_XnzB1Ef8?t=723)）
- [[programming-to-interfaces-frontend]] — 在良好的前端架构中，各实体应只通过既定的清晰接口与其他模块交互和扩展，而不是直接依赖对方的内部实现。（[00:00](https://youtu.be/hA_XnzB1Ef8?t=0)）
- [[relative-sizing-units]] — 硬编码像素值会导致 UI 难以做响应式适配，而使用 REM 等相对单位可以让界面在不同设备上自动调整。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
- [[shared-library-module-extraction]] — 为避免 AI 每次都要在整个代码库里重新查找或实现重复功能，可以把可复用功能抽取到 modules 间共享的 library 中，这本身就是前端工程中模块化设计的工作。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
- [[single-record-principle]] — essential state 设计应遵循 single record principle：系统中任何一份数据都必须只被存储一次，不能有冗余状态，也不能有可以从其他状态推导出来的 derived state，state 应尽量最小化。（[12:03](https://youtu.be/hA_XnzB1Ef8?t=723)）
- [[skill-priority-by-system-scale]] — 选择优先精进哪项技能取决于所在系统的规模：如果工作在具有 micro-frontend、有一定规模的系统上，应优先投入 system design；如果只负责某个具体 feature、不掌控系统全局，则更应该在 code quality 和 state/data 这类细粒度技能上下功夫。（[12:03](https://youtu.be/hA_XnzB1Ef8?t=723)）
- [[state-duplication-performance-risk]] — 如果用 AI 独立地在各处生成组件而不做架构层面的沟通协调，很容易出现 local state 遍地开花且相互冗余，同一份数据被在两个不同地方分别从后端 fetch，造成重复请求。（[12:03](https://youtu.be/hA_XnzB1Ef8?t=723)）
- [[tab-index-visual-order-match]] — 可访问性设计中还需确保 tab index 中元素被聚焦的顺序，与它们在屏幕上实际显示的视觉顺序保持一致。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
- [[ui-consistency-reduces-cognitive-load]] — 保持 UI 一致性的意义在于，当用户看到一致的界面时大脑处理负担更小，只有真正变化的部分才需要被注意，这也是使用统一样式规范的核心原因。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
- [[unsupervised-agent-tech-debt-accumulation]] — 让 agent 无人监督地工作而不审查代码质量，应用可能看起来实现了预期功能，但实际上是坐在一堆技术债之上，一旦想挪动某个小部件，整个结构就会一起崩塌。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
- [[unused-file-detection]] — 同一份静态分析报告显示该代码库中存在 153 个未使用的文件（unused files），这会显著恶化 AI 的 context management 并降低 AI 给出的结果质量。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
- [[web-performance-diagnosis-implementation-ratio]] — 传统 web performance 工作里只有约5%的时间花在诊断问题上，剩下约90%花在压缩图片、重构组件、加 memoization 等繁琐的实现环节。（[03:01](https://youtu.be/hA_XnzB1Ef8?t=181)）
- [[web-performance-knowledge-diagnostic-value]] — web performance 相关知识本质上被并入了系统设计知识范畴，其价值在于帮助判断问题是设计层面还是优化层面，而不再是需要每天亲自动手实现的核心差异化技能。（[03:01](https://youtu.be/hA_XnzB1Ef8?t=181)）
