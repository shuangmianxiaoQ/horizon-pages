---
layout: default
title: "Horizon Summary: 2026-05-25 (ZH)"
date: 2026-05-25
lang: zh
---

> From 32 items, 11 important content pieces were selected

---

1. [从 Go 迁移到 Rust](#item-1) ⭐️ 8.0/10
2. [微粗糙度挑战光滑机翼定律](#item-2) ⭐️ 8.0/10
3. [Grok V9-Medium 训练完成](#item-3) ⭐️ 8.0/10
4. [HN 用户比较谷歌替代搜索](#item-4) ⭐️ 7.0/10
5. [教宗警告 AI 并非中立。](#item-5) ⭐️ 7.0/10
6. [神舟二十三号乘组公布](#item-6) ⭐️ 7.0/10
7. [Epic 公布虚幻引擎 6，Rocket League 率先展示](#item-7) ⭐️ 7.0/10
8. [在 AI 开发转变中感到被落下](#item-8) ⭐️ 6.0/10
9. [Audiomass 把多轨音频编辑带到网页](#item-9) ⭐️ 6.0/10
10. [Jira 被证明图灵完备](#item-10) ⭐️ 6.0/10
11. [人工智能时代网络安全专家需求激增](#item-11) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [从 Go 迁移到 Rust](https://corrode.dev/learn/migration-guides/go-to-rust/) ⭐️ 8.0/10

这篇新文章给出了一份从 Go 迁移到 Rust 的指南，并把这一选择描述为两个生态之间的一组权衡。文章同时兼具实用迁移建议和对 Rust 采用的倡导意味。 这篇指南对正在评估是否采用 Rust 的后端和系统工程师很有参考价值，因为他们需要判断 Rust 更强的编译期保证是否值得额外的复杂度。它也反映了业界更广泛的讨论：团队究竟是更看重托管运行时和更简单的使用体验，还是更看重对内存和性能的细粒度控制。 围绕这篇文章的讨论主要集中在 Rust 的所有权模型、借用检查器以及由编译期强制执行的内存安全保证。评论者还提出了很多实际问题，比如 Go 的错误处理是否过于啰嗦、包管理差异，以及 Rust 是否适合做 Web 后端。

hackernews · jabits · May 24, 18:31 · [社区讨论](https://news.ycombinator.com/item?id=48259808)

**背景**: Rust 不依赖垃圾回收来管理内存，而是使用所有权和借用规则，并由借用检查器在编译期验证这些规则。Rust 官方文档说明，引用可以借用数据而不取得所有权，而生命周期标注则帮助编译器确保引用不会比其指向的数据活得更久。这些特性是 Rust 常被用于系统编程的重要原因，也解释了为什么从 Go 迁移到 Rust 往往意味着编程模型上的明显变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://doc.rust-lang.org/1.8.0/book/references-and-borrowing.html">Rust borrow checker</a></li>
<li><a href="https://doc.rust-lang.org/book/ch10-03-lifetime-syntax.html">Validating References with Lifetimes - The Rust Programming Language</a></li>
<li><a href="https://samolusola.me/posts/borrow-checker-scope-and-ownership/">Rust Ownership 3: The Borrow Checker, Scope, and Ownership · Sam Olusola</a></li>

</ul>
</details>

**社区讨论**: 评论总体上是有分歧但讨论很热烈的。有人认为 Go 仍然更适合 Web 后端，也有人指出真正的关键往往在于是否需要托管运行时；还有几位评论者批评了 Rust 的包管理，并认为这篇文章更像是在为 Rust 做倡导，而不是完全中立的迁移指南。

**标签**: `#Rust`, `#Go`, `#migration-guide`, `#systems-programming`, `#backend-development`

---

<a id="item-2"></a>
## [微粗糙度挑战光滑机翼定律](https://www.wired.com/story/a-fundamental-principle-of-aeronautical-engineering-has-been-overturned/) ⭐️ 8.0/10

《Wired》报道称，一项新研究表明，对于翼型来说，极微小的表面粗糙度可能会降低阻力，而不一定像传统观点认为的那样增加阻力。这颠覆了“表面越光滑，空气动力学性能就一定越好”的长期假设。 如果这一结果经得起验证，它可能会改变飞机和其他气动表面的设计与加工方式，并影响燃油效率以及改装思路。它还挑战了航空工程中的一条核心经验法则，因此影响不只限于某一篇论文。 这里讨论的是翼型表面的微尺度粗糙度，而不是普通可见缺陷，实际收益很可能取决于表面处在边界层转捩的什么位置。评论者还提出了一个重要提醒：即使局部阻力系数更低，也不一定意味着整体阻力会大幅下降。

hackernews · littlexsparkee · May 24, 19:10 · [社区讨论](https://news.ycombinator.com/item?id=48260117)

**背景**: 在空气动力学中，边界层是紧贴物体表面的一层薄薄空气，它的行为会显著影响升力和阻力。层流边界层通常具有更低的表面摩擦阻力，而湍流边界层的表现不同，也会改变流动分离的方式。表面粗糙度之所以重要，是因为它会影响边界层如何发展，所以工程师通常会非常重视翼型表面的加工质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eaglepubs.erau.edu/introductiontoaerospaceflightvehicles/chapter/boundary-layers/">Boundary Layer Flows – Introduction to Aerospace Flight Vehicles</a></li>
<li><a href="https://www.kitplanes.com/laminar-vs-turbulent-flow-airfoils/">Laminar- vs. Turbulent-Flow Airfoils - KITPLANES Laminar and turbulent boundary layers | Aerodynamics Class ... Boundary Layer Flows – Introduction to Aerospace Flight Vehicles Boundary Layer - Glenn Research Center | NASA Laminar vs Turbulent Flow Over Airfoils - Symscape 7.3. Separation - Stanford University Laminar vs Turbulent Boundary Layer’s: Understanding Fluid ...</a></li>
<li><a href="https://link.springer.com/chapter/10.1007/978-981-99-6874-9_6">Effect of Surface Roughness Size on the Skin Friction Drag for...</a></li>

</ul>
</details>

**社区讨论**: 讨论整体上以惊讶和好奇为主：一些评论者说，这与帆船和翼板竞速者长期观察到的现象相符，还有人拿高尔夫球凹坑减少阻力作类比。也有人追问实际收益到底有多大、文中提到的改善是否只发生在转捩区，以及这种方法能否低成本改装到现有飞机上。

**标签**: `#aerodynamics`, `#fluid dynamics`, `#aerospace engineering`, `#research`, `#drag reduction`

---

<a id="item-3"></a>
## [Grok V9-Medium 训练完成](https://x.com/elonmusk/status/2058787384364265734) ⭐️ 8.0/10

马斯克表示，Grok V9-Medium 这一 1.5T 基础模型已经完成训练，评估结果看起来不错。团队目前正在进行微调，并计划在几天后启动强化学习，预计两三周后向公众发布。 如果这次发布如预期进行，Grok 在代码能力上可能会有明显提升，尤其是在复杂编程任务上。对于依赖 AI 助手进行软件开发的用户和开发者来说，这会带来直接影响，也会进一步加大对其他前沿聊天和编程模型的竞争压力。 这次补充训练中加入了大量 Cursor 数据，说明模型更强调编程工作流。文中将其与当前线上运行的 v8-small（0.5T）对比，意味着新模型被定位为一个规模更大、能力更强的继任版本。

telegram · zaihuapd · May 25, 07:07

**背景**: Grok 是与马斯克相关的 AI 模型家族，这次更新提到的是基础模型，也就是先进行大规模预训练、再用于后续任务适配的模型。完成预训练后，团队通常会通过微调来提升特定任务表现，再通过强化学习进一步优化输出。Cursor 是一款 AI 编程代理和编辑器，因此加入 Cursor 数据说明这次训练明显偏向软件开发场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/teortaxesTex">Teortaxes▶️ (DeepSeek 推特 铁粉 2023 – ∞) (@teortaxesTex) / Posts / X</a></li>
<li><a href="https://cursor.com/">Cursor : The best coding agent</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1953263345906984145">大模型的训练与调优，SFT (监督微调)和RLHF (基于人类反馈的强化学习)...</a></li>

</ul>
</details>

**标签**: `#Grok`, `#大模型`, `#Elon Musk`, `#代码生成`, `#强化学习`

---

<a id="item-4"></a>
## [HN 用户比较谷歌替代搜索](https://techcrunch.com/2026/05/21/six-search-engines-worth-trying-now-that-google-isnt-really-google-anymore/) ⭐️ 7.0/10

一场 Hacker News 讨论集中介绍了几种谷歌替代方案，参与者分享了他们对注重隐私、无广告以及可自托管搜索工具的亲身体验。讨论重点包括 Kagi、Searx/SearXNG、Brave Search，以及像 Hister 这样的新自托管项目。 搜索是互联网最重要的入口之一，因此谷歌产品行为的变化会促使用户去寻找替代方案。这个讨论显示，人们对隐私、控制权以及更贴近实际需求的搜索结果越来越感兴趣。 评论者称赞 Kagi 的相关性和可选 AI 功能，而 Searx 则被讨论为一种可减少对单一提供商依赖的元搜索方式。帖子还提到了像 Hister 这样的自托管方案，它旨在索引网页和本地文件，同时对 Google 的 AI Overview 和 Brave Search 的 AI 回复也存在不同看法。

hackernews · elorant · May 25, 12:27 · [社区讨论](https://news.ycombinator.com/item?id=48266051)

**背景**: 元搜索引擎并不是从零开始建立自己的索引，而是向其他搜索服务发起查询并汇总结果。讨论中提到的 SearXNG 是一个可自托管的免费元搜索引擎，目标是不跟踪用户也不建立用户画像。自托管之所以重要，是因为它允许用户自己运行搜索服务，而不是完全依赖商业提供商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.searxng.org/">SearXNG Documentation (2026.5.23+323ce7600)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Metasearch_engine">Metasearch engine - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 整体情绪偏务实，但用户优先级不同：一些人强烈偏好 Kagi 或 Brave Search 的便利性，而另一些人则更看重隐私、无广告体验或自托管。评论还显示，AI 辅助搜索对部分用户来说已不再新鲜，有人喜欢 AI 答案，也有人完全不想使用它。

**标签**: `#search engines`, `#privacy`, `#Hacker News`, `#Google alternatives`, `#open source`

---

<a id="item-5"></a>
## [教宗警告 AI 并非中立。](https://www.vatican.va/content/leo-xiv/en/encyclicals/documents/20260515-magnifica-humanitas.html) ⭐️ 7.0/10

梵蒂冈发布了通谕《Magnifica Humanitas》，其中指出技术和 AI 从来都不是中立的，开发者必须考虑它们对人类和文明的影响。该文件认为，设计、融资、监管和使用方式都会塑造技术最终呈现的样子。 这件事重要在于，它把 AI 伦理从抽象讨论推进到对构建者的直接责任要求。它在 AI 日益集中化的背景下尤其相关，因为工具的设计方式会影响可及性、权力分配和社会结果。 这份通谕强调，每一个设计选择都体现了对人类的某种理解，并警告不要把 AI 当作没有道德重量的纯技术工具。评论中也提到了权力集中、同质化风险，以及广泛计算资源可及性与中心化控制之间的张力。

hackernews · theletterf · May 25, 10:11 · [社区讨论](https://news.ycombinator.com/item?id=48265206)

**背景**: 通谕是天主教会的一种正式文件，通常用来讨论教义、道德或社会问题。这里，它被用来讨论技术和 AI 伦理，追问开发者是在做有利于还是有害于人类繁荣的选择。该话题默认读者了解一个更广泛的技术政策争论：工具是否价值中立，还是不可避免地反映制造者和部署者的意图与激励。

**社区讨论**: 讨论整体上比较认真，但立场略有分化：一些评论者认同核心警告，认为 AI 会放大既有的经济和制度权力；另一些人则指出，这其实是早期计算时代就已经出现的老问题。也有人赞赏通谕中关于多样性与同质化的表述，而一条较怀疑的评论认为，这份文件仍然陷在它所批评的结构性前提之中。

**标签**: `#AI ethics`, `#technology policy`, `#Hacker News discussion`, `#philosophy of technology`, `#society`

---

<a id="item-6"></a>
## [神舟二十三号乘组公布](https://t.me/zaihuapd/41554) ⭐️ 7.0/10

中国公布了神舟二十三号航天员乘组，由指令长朱杨柱、航天驾驶员张志远和载荷专家黎家盈组成。飞船计划于 5 月 24 日 23 时 08 分发射，乘组中将迎来首位港籍航天员执行任务。 这标志着中国载人航天进入新的阶段，因为它不仅公布了新乘组，还将首次由港籍航天员执行飞行任务。它也体现出中国航天员队伍在不同批次、不同分工上的持续扩充，并包含一年期飞行安排。 报道提到，这还是我国首个由第三批和第四批航天员共同组成的乘组，其中一名航天员将执行一年期飞行任务。朱杨柱此前执行过神舟十六号任务，此次首次担任指令长；黎家盈则被描述为面向港澳选拔的首位女性载荷专家。

telegram · zaihuapd · May 24, 15:13

**背景**: 在中国载人航天任务中，指令长负责带领乘组、接收地面指令并保障飞行安全。航天驾驶员主要负责飞船操控，载荷专家则更侧重于特定实验和载荷操作。报道还提到一年期飞行任务，这通常指长时间在轨驻留，用于研究人体和心理在微重力环境下的适应情况。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cmse.gov.cn/xwzx/202305/t20230531_53675.html">总师有话说｜为什么是“航天驾驶员+航天飞行工程师+载荷专家”？_中国载...</a></li>
<li><a href="https://baike.baidu.com/item/指令长/9584343">指令长_百度百科</a></li>
<li><a href="https://zh.wikipedia.org/wiki/载荷专家">载荷专家 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**标签**: `#载人航天`, `#神舟二十三号`, `#航天员`, `#中国航天`, `#港籍航天员`

---

<a id="item-7"></a>
## [Epic 公布虚幻引擎 6，Rocket League 率先展示](https://www.pcgamer.com/gaming-industry/epic-reveals-first-unreal-engine-6-game-and-its-not-fortnite/) ⭐️ 7.0/10

Epic Games 在巴黎《Rocket League》冠军系列赛上首次公开虚幻引擎 6，并确认《Rocket League》将成为首个展示 UE6 的游戏。该作将直接从虚幻引擎 3 升级到 UE6，这意味着一次跨越多个世代的大幅引擎迁移。 一款仍在运营的高知名度游戏从 UE3 直接跃迁到 UE6，说明 Epic 正把 Unreal 视为长期平台而不只是一次版本迭代。若 UE6 在工具链、性能或内容流程上带来改进，可能会影响大量游戏工作室和相关内容制作团队的技术规划。 这次公布更像是一次早期展示，而不是完整的技术发布；在现有信息里，Epic 并没有披露 UE6 的具体规格或发布时间。与此同时，UE5 虽然已经使用了四年并被广泛采用，但在 PC 端的优化问题也一直受到玩家批评。

telegram · zaihuapd · May 25, 02:20

**背景**: 游戏引擎是负责渲染、物理、AI、网络和文件管理等核心系统的软件层，这样开发者就不必从零实现这些底层能力。虚幻引擎是业内最知名的引擎之一，常被用作跨平台开发的技术基础，也会被视为一种中间件。这里的“中间件”指的是位于游戏与底层硬件或操作系统之间、可复用的技术层。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/游戏引擎">游戏引擎 - 维基百科，自由的百科全书</a></li>
<li><a href="https://zh.wikipedia.org/zh-hans/虚幻引擎">虚幻引擎 - 维基百科，自由的百科全书</a></li>
<li><a href="https://learn.microsoft.com/zh-cn/shows/windows-store-developer-solutions/game-development-middleware-it-do-i-need-it">游戏开发中间件：它是什么？ 我需要它吗？ | Microsoft Learn</a></li>

</ul>
</details>

**标签**: `#Unreal Engine 6`, `#Epic Games`, `#Rocket League`, `#game engine`, `#game development`

---

<a id="item-8"></a>
## [在 AI 开发转变中感到被落下](http://androidessence.com/leave-me-behind/) ⭐️ 6.0/10

这篇《Leave Me Behind》文章反思了在 AI 快速改变软件开发时，人们想被“留在原地”的情绪。它把这种变化描述为不仅是工具层面的转变，更是对旧有学习方式、工作方式和工匠感的一种失落。 这篇文章反映了许多开发者在 AI 重塑日常工作流和职业认同时所感受到的普遍焦虑。它在 Hacker News 上的高关注度说明，这个话题已经超出一篇博客文章本身，触及了工匠精神、生产力以及什么才算“真正的开发工作”等更广泛的问题。 这篇文章不是技术发布，而是一篇观点文章，因此它的价值主要在于视角，而不是新工具或基准结果。讨论中强调了“追求深度理解”与“接受客户更关心支持、成本和可预测性而不是实现方式”之间的张力。

hackernews · mooreds · May 25, 12:03 · [社区讨论](https://news.ycombinator.com/item?id=48265876)

**社区讨论**: 评论整体上对文章的情绪核心表示理解，不少读者说自己也对 AI 时代的变化和更传统、更动手的工作方式消失有同样感受。也有人提出反对意见，认为怀旧情绪可能掩盖软件工作的现实，客户需求和长期可维护性比“真正的编程”这种浪漫化想象更重要。

**标签**: `#AI`, `#software development`, `#developer experience`, `#industry change`, `#Hacker News`

---

<a id="item-9"></a>
## [Audiomass 把多轨音频编辑带到网页](https://audiomass.co/?multitrack=1) ⭐️ 6.0/10

Audiomass 在 Hacker News 上亮相，它是一个运行在浏览器中的免费开源多轨音频编辑器，网址为 audiomass.co。这个 Show HN 之所以引起强烈关注，是因为它把直观的编辑流程和可离线使用的网页应用体验结合在了一起。 这件事重要在于它展示了浏览器音频工具已经发展到足以承载较严肃的多轨编辑，用户不必安装桌面软件也能完成工作。它也反映出人们越来越关注那种像本地应用一样可用、还能离线运行的网页应用，以及未来可能延伸出的协作式工作流。 它的技术基础是 Web Audio API，这套接口专门用于在浏览器里构建复杂的音频路由图和效果处理。离线体验则符合 PWA 的常见模式，也就是通过 service worker 缓存资源，让应用在网络不可用时仍然可以继续工作。

hackernews · pantelisk · May 24, 15:25 · [社区讨论](https://news.ycombinator.com/item?id=48258015)

**背景**: 多轨音频编辑器允许你在同一时间轴上处理多条音轨，这对于叠加人声、乐器或效果非常有用。网页端通常依赖 Web Audio API 来完成播放和处理，因为它为开发者提供了处理音源、路由和效果的底层积木。PWA 是一种行为更像已安装应用的网页应用，借助缓存资源甚至可以支持离线使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.google.com/codelabs/pwa-training/pwa03--going-offline">Progressive Web Apps: Going Offline | Google for Developers</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API">Web Audio API - Web APIs | MDN - MDN Web Docs Code sample</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Tutorials/js13kGames/Offline_Service_workers">js13kGames: Making the PWA work offline with service workers - Progressive web apps | MDN</a></li>

</ul>
</details>

**社区讨论**: 讨论整体上是积极而热情的，几位评论者称赞了它的 UX、实现质量和带有怀旧感的界面风格。最突出的需求是云端协作功能，大家希望能像共享即兴创作一样分支、叠加音轨并“提交”修改。

**标签**: `#open source`, `#web audio`, `#multitrack editing`, `#PWA`, `#Hacker News`

---

<a id="item-10"></a>
## [Jira 被证明图灵完备](https://seriot.ch/computation/jira.html) ⭐️ 6.0/10

一篇文章提出，Jira 是图灵完备的，并展示了它的工作流和工单机制如何被组合起来模拟计算。文章把 Jira 的状态流转视为这一结论的核心。 这个观点主要是一种有趣的技术奇观，但它也说明了一个广泛使用的企业工具中的自动化能力可以被延伸到多么夸张的程度。对于长期使用 Jira 的开发者和团队来说，这也提醒人们，工作流可能会变得非常有表现力，尽管这并不等于实用。 这个论证依赖于 Jira 的工作流，而工作流由状态和转换组成，控制工单在生命周期中的流转。换句话说，这篇文章把工单状态变化当成一种计算系统，而不只是项目跟踪功能。

hackernews · vinhnx · May 25, 03:54 · [社区讨论](https://news.ycombinator.com/item?id=48263253)

**背景**: 图灵完备是指一个系统在理论上可以模拟任意图灵机，因此能够表达通用计算。Jira 是一个项目管理工具，它的工作流描述了工作项如何通过不同状态和转换，从创建走向完成。这篇文章利用这种结构，带着戏谑意味提出 Jira 也可以被当作一种计算系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Turing_completeness">Turing completeness - Wikipedia</a></li>
<li><a href="https://www.atlassian.com/software/jira/guides/workflows/overview">Introduction to Jira Workflows | Atlassian</a></li>

</ul>
</details>

**社区讨论**: 讨论整体上偏幽默和讽刺，很多人开玩笑说可以在 Jira 里玩 Doom，或者拿 Azure Boards 之类更糟的工具来对比。较认真的观点则提到，Jira 的普及度和 API 让高级用户很容易进行大量自动化，甚至可以把 Jira 反过来“用来对付它自己”。

**标签**: `#Jira`, `#Turing-completeness`, `#developer tools`, `#software satire`, `#productivity automation`

---

<a id="item-11"></a>
## [人工智能时代网络安全专家需求激增](https://www.nytimes.com/2026/05/24/technology/one-job-that-is-growing-in-the-ai-era-cybersecurity-experts.html) ⭐️ 6.0/10

AI-driven code growth and new attack capabilities are sharply increasing demand for cybersecurity experts, especially senior leaders who can combine security and AI expertise.

telegram · zaihuapd · May 25, 06:21

**标签**: `#cybersecurity`, `#artificial intelligence`, `#labor market`, `#software security`, `#AI security`

---
