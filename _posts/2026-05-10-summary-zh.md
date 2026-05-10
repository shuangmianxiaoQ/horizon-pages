---
layout: default
title: "Horizon Summary: 2026-05-10 (ZH)"
date: 2026-05-10
lang: zh
---

> From 32 items, 9 important content pieces were selected

---

1. [AI 推动 R(3,17)下界提升](#item-1) ⭐️ 8.0/10
2. [OpenCode v1.14.46 新增技能并修复安全问题](#item-2) ⭐️ 7.0/10
3. [macOS ARM64 汇编网页服务器](#item-3) ⭐️ 7.0/10
4. [Mac 软件分发越来越难](#item-4) ⭐️ 7.0/10
5. [NASA 推进火星旋翼技术](#item-5) ⭐️ 7.0/10
6. [Claude 代理灰产曝光](#item-6) ⭐️ 7.0/10
7. [opencode v1.14.42 增加压缩和工作区同步](#item-7) ⭐️ 6.0/10
8. [Gemini API 文件搜索支持多模态](#item-8) ⭐️ 6.0/10
9. [FCC 拟要求开号前核验身份](#item-9) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [AI 推动 R(3,17)下界提升](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247889542&idx=1&sn=5ccec8ac583f5112d169e360152c1baf) ⭐️ 8.0/10

浙江大学校友团队借助 AI 辅助方法，将拉姆齐数 R(3,17) 的下界从 92 推进到 93。这个结果打破了该下界长达 32 年没有变化的纪录。 这是一项有意义的组合数学进展，因为提升拉姆齐数下界，意味着要证明更大的图构造仍然可以避免被禁止的结构。对于拉姆齐理论来说，哪怕只前进一步也很重要，因为这类精确值通常极难求出。 这条新闻提升的是下界，而不是 R(3,17) 的精确值，所以这个拉姆齐数本身仍然未知。按照拉姆齐记号，R(3,17) 表示从某个顶点规模开始，任意图中都必然出现一个三角形，或者一个大小为 17 的独立集。

rss · 量子位 · May 10, 03:52

**背景**: 拉姆齐理论研究的是：当结构足够大时，即使它们看起来是任意安排的，也一定会出现某种有序模式。拉姆齐数 R(m,n) 指的是在任意图中都能保证出现大小为 m 的团，或者大小为 n 的独立集所需的最小顶点数。实际研究中，证明下界通常意味着构造出在某个规模以下仍然能同时避开这两种模式的例子。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mathworld.wolfram.com/RamseyNumber.html">Ramsey Number - from Wolfram MathWorld</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ramsey's_theorem">Ramsey's theorem - Wikipedia</a></li>
<li><a href="https://math.mit.edu/~apost/courses/18.204_2018/ramsey-numbers.pdf">Ramsey Numbers - MIT Mathematics Ramsey Theory | Jacob's Math Academy Key Ramsey Numbers to Know for Ramsey Theory - fiveable.me \ (R (3,3,3) = 17\text {:}\) Before Your Eyes Ramsey Number R (3, 3, 3) - Alexander Bogomolny</a></li>

</ul>
</details>

**标签**: `#Ramsey理论`, `#组合数学`, `#AI辅助研究`, `#数学突破`, `#学术研究`

---

<a id="item-2"></a>
## [OpenCode v1.14.46 新增技能并修复安全问题](https://github.com/anomalyco/opencode/releases/tag/v1.14.46) ⭐️ 7.0/10

OpenCode v1.14.46 新增了内置的 `customize-opencode` 技能，并修复了 HTTP API、OpenAPI/SDK 生成、旧数据加载、MCP 工具发现以及 Plan Mode 安全性方面的一系列问题。此次发布特别修正了数值和布尔查询参数处理、旧会话数据兼容性，以及 Plan Mode 子代理的安全绕过问题。 这次发布提升了使用 OpenCode 的 API、SDK 和代理工作流时的日常可靠性，尤其影响到仍在使用旧会话数据或 MCP 集成的开发者。最重要的是修复了 Plan Mode 绕过问题，因为它堵住了一个可能让子代理无视父代理拒绝规则的安全漏洞。 这些 API 修复让生成的 OpenAPI 规范和 SDK 类型与运行时行为保持一致，涉及 session、file 以及 workspace 路由的端点。此次发布还增强了加载的容错性，能够接受旧会话、diff 和重试事件中的旧数值以及负 token 计数，并且在 MCP 服务器发布损坏的 `outputSchema` 引用时也不会直接失败。

github · opencode-agent[bot] · May 10, 02:34

**背景**: OpenCode 的技能是可复用的指令，代理可以按需发现并加载，因此内置 `customize-opencode` 技能有助于更安全地修改配置。MCP，即 Model Context Protocol，会用模式定义工具，让模型以结构化方式发现并调用外部能力，所以损坏的模式引用会影响工具发现。Plan Mode 是只读阶段，拒绝规则非常重要，而子代理应该继承这些限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opencode.ai/docs/skills/">Agent Skills | OpenCode</a></li>
<li><a href="https://opencode.ai/docs/agents/">Agents | OpenCode</a></li>
<li><a href="https://modelcontextprotocol.io/specification/2025-06-18/server/tools">Tools - Model Context Protocol</a></li>

</ul>
</details>

**标签**: `#release`, `#security`, `#bugfix`, `#openapi`, `#developer-tools`

---

<a id="item-3"></a>
## [macOS ARM64 汇编网页服务器](https://github.com/imtomt/ymawky) ⭐️ 7.0/10

一位开发者发布了 ymawky，这是一个完全用 ARM64 汇编编写的 macOS 静态文件网页服务器。它支持 GET、PUT、DELETE、HEAD、OPTIONS、字节范围请求、目录列表、URL 百分号解码、严格的 docroot 限制、自定义错误页，并带有部分针对 slowloris 的缓解措施。 这是一个少见的、把实用网络服务完全放到极低层实现的例子，说明汇编不仅能写演示程序，也能承担真实 HTTP 服务。对于系统程序员来说，它具体展示了在 macOS/Apple Silicon 上不依赖更高层运行时也能直接构建完整的 HTTP 功能。 该服务器支持 Range: bytes 请求，这通常用于部分下载和视频拖动定位，并且会严格将访问限制在文档根目录内。它还提供目录列表、自定义错误响应，以及用于降低 slowloris 式不完整请求攻击影响的保护措施。

hackernews · imtomt · May 10, 03:01 · [社区讨论](https://news.ycombinator.com/item?id=48080587)

**背景**: HTTP 范围请求允许客户端只获取文件的一部分，而不是一次下载整个资源，这对媒体播放和断点续传很有用。slowloris 攻击会通过非常缓慢或不完整地发送 HTTP 请求来长期占用连接，从而耗尽服务器的连接处理能力。macOS 上的 ARM64 汇编尤其底层，因为开发者是在接近机器接口的层面工作，而不是使用常见的应用框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/Range_requests">HTTP range requests - MDN Web Docs - Mozilla</a></li>
<li><a href="https://www.cloudflare.com/learning/ddos/ddos-attack-tools/slowloris/">Slowloris DDoS attack - Cloudflare</a></li>
<li><a href="https://github.com/below/HelloSilicon">GitHub - below/HelloSilicon: An introduction to ARM64 assembly on Apple Silicon Macs · GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍称赞了这份手工能力和迎难而上的态度。也有人借此讨论 LLMs 对这类工作的影响：一位评论者把它看作旧时代技能价值的提醒，另一位则指出，写大型汇编程序虽然更啰嗦，但本质上并不比更高层语言难到哪里去。

**标签**: `#assembly`, `#web server`, `#systems programming`, `#macOS`, `#hacker news`

---

<a id="item-4"></a>
## [Mac 软件分发越来越难](https://blog.kronis.dev/blog/apple-is-increasing-my-cortisol-levels) ⭐️ 7.0/10

一位独立开发者发布文章，称 Mac 软件分发变得越来越痛苦且成本更高，尤其是在 Apple 代码签名、软件公证和 Gatekeeper 限制方面。文章及其评论区把这件事描述为实际的发版难题，而不只是抽象的安全争论。 这件事很重要，因为这些要求会影响所有在 Mac App Store 之外发布 Mac 应用的人，尤其是预算和时间都有限的独立开发者与小团队。它也反映出平台安全控制与软件分发摩擦之间日益明显的矛盾。 Mac 软件分发通常需要 Developer ID 证书、代码签名和软件公证，而且 Apple 的公证服务自 2023 年 11 月 1 日起不再接受来自 altool 或 Xcode 13 及更早版本的上传。Gatekeeper 默认会检查下载的软件是否含有恶意内容，但用户可以在自己的机器上覆盖或放宽这些策略。

hackernews · LorenDB · May 9, 14:40 · [社区讨论](https://news.ycombinator.com/item?id=48075366)

**背景**: 代码签名是 Apple 为应用附加加密身份的一种方式，这样 macOS 就能在发布后检测应用是否被篡改。软件公证是一个独立于 Mac App Store 的 Apple 审核流程，目的是让用户更有信心，确认应用已经过恶意组件检查。Gatekeeper 是 macOS 在首次打开软件时执行这些检查的保护层，因此开发者通常是在分发阶段而不是开发阶段最强烈地感受到它的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/developer-id/">Signing Mac Software with Developer ID - Apple Developer</a></li>
<li><a href="https://developer.apple.com/documentation/security/notarizing-macos-software-before-distribution">Notarizing macOS software before distribution | Apple ...</a></li>
<li><a href="https://support.apple.com/guide/security/gatekeeper-and-runtime-protection-sec5599b66df/web">Gatekeeper and runtime protection in macOS - Apple Support</a></li>

</ul>
</details>

**社区讨论**: 评论区整体上对作者的抱怨表示理解，不少开发者认为 Apple 的分发规则和向后兼容性问题已经很难处理。有人主张不喜欢 Gatekeeper 的用户可以在本机关闭它，但也有人反驳说，这并不能解决开发者面向所有用户发软件时承担的额外负担。

**标签**: `#macOS`, `#software distribution`, `#code signing`, `#Gatekeeper`, `#developer tooling`

---

<a id="item-5"></a>
## [NASA 推进火星旋翼技术](https://arstechnica.com/space/2026/05/engineers-at-nasas-jet-propulsion-lab-make-a-breakthrough-in-rotor-technology/) ⭐️ 7.0/10

NASA 喷气推进实验室表示，工程师在下一代火星直升机的旋翼技术上取得了突破。3 月的测试显示，新旋翼叶片可以突破音障而不会解体，这为更高速的火星飞行设计打开了空间。 更快、效率更高的旋翼，可能让未来火星旋翼飞行器携带比“机智号”更重的载荷并飞得更远。这将扩大火星空中探测的能力，例如覆盖更大区域并携带更多科学仪器。 NASA 表示，这些旋翼叶片面向火星稀薄大气中的飞行器，因为在那里升力很难获得，而旋翼转速至关重要。JPL 的报告指出，火星直升机的旋翼转得越快，就越能携带更重的载荷并飞得更远。

telegram · zaihuapd · May 9, 14:21

**背景**: 火星旋翼飞行器要解决的空气动力学问题，比地球直升机困难得多，因为火星大气极其稀薄。NASA 的先驱火星直升机“机智号”使用了异常大的叶片和很高的旋翼转速来实现飞行，它的飞行方案也成了后续设计的参考。如今，工程师如果想在火星上实现更重、能力更强的飞行器，就必须把旋翼性能继续推高。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.jpl.nasa.gov/news/nasa-pushes-next-gen-mars-helicopter-rotor-blades-past-mach-1/">NASA Pushes Next-Gen Mars Helicopter Rotor Blades Past Mach 1</a></li>
<li><a href="https://rotorcraft.arc.nasa.gov/Publications/files/1699_Koning_TM_020224.pdf">NASA/TM-20240001510 Mars Helicopter Ingenuity Rotor Geometry</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ingenuity_(helicopter)">Ingenuity (helicopter) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#NASA`, `#rotorcraft`, `#Mars exploration`, `#aerospace engineering`, `#planetary science`

---

<a id="item-6"></a>
## [Claude 代理灰产曝光](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinese-grey-market-sells-claude-api-access-at-90-percent-off-through-proxy-networks-that-harvest-user-data) ⭐️ 7.0/10

一份报告称，部分中国 API 中转站正在以官方约一成的价格转售 Anthropic 的 Claude 访问权限。报告还指称，这些服务通过盗用或滥用账号、偷换模型，以及收集用户提示词和输出结果来牟利。 如果属实，这会给依赖第三方 API 网关的开发者和企业带来直接的安全与合规风险。它也说明灰市低价接入会如何在压低官方价格的同时，放大数据泄露和模型冒充的风险。 报告称，这类“中转站”可能通过盗刷信用卡、批量注册、拆分订阅，甚至外包实名认证来获取权限。报告还指出，用户看到的结果可能来自更便宜的模型或国产模型，却被伪装成 Claude Opus，同时被采集的提示词还可能用于蒸馏。

telegram · zaihuapd · May 10, 01:48

**背景**: API 中转站或代理服务位于用户和模型提供方之间，允许客户通过一个转售商调用多个 AI 模型。它们在 AI 社区里常被宣传为以更低成本接入 Claude、GPT 或 Gemini 的方式，但也会带来信任问题，因为用户要依赖代理方如实转发请求并安全处理数据。模型蒸馏是一种把大模型知识迁移给小模型的技术，而在这份报告里，它被描述为一种潜在滥用场景：提示词和输出在未经同意的情况下被收集并用于训练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/2018044893910552640">AI API中转站推荐与评测 - 知乎</a></li>
<li><a href="https://github.com/qixing-jk/all-api-hub">GitHub - qixing-jk/all-api-hub: 一站式 New-API/Sub2API 等中转站账号管理：余额/用量看板、自动签到、密钥一键使用、价格对比、可用性测试，另提供高级渠道管理 | All-in-one New-API/Sub2API account hub: balance/usage dashboard, auto check-in, one-click keys, price comparison, health checks, plus advanced channel management</a></li>
<li><a href="https://cloud.tencent.com/developer/article/2517760">一文读懂到底什么是“模型蒸馏（Model Distillation）”技术？-腾讯云开...</a></li>

</ul>
</details>

**标签**: `#AI security`, `#Claude API`, `#data leakage`, `#grey market`, `#model spoofing`

---

<a id="item-7"></a>
## [opencode v1.14.42 增加压缩和工作区同步](https://github.com/anomalyco/opencode/releases/tag/v1.14.42) ⭐️ 6.0/10

anomalyco/opencode 发布了 v1.14.42，新增了 HTTP API 响应压缩、Scout 调研代理，以及用于自动发现适配器驱动工作区的同步功能。该版本还加入了 `opencode run` 的交互式分割页脚模式，简化了 TUI 快捷键配置，并将桌面端更新改为静默的按用户安装流程。 这些改动提升了 CLI 的日常可用性：大响应的传输开销更低，工作区配置更自动化，开发者还多了一个用于仓库和文档检索的研究代理。与此同时，API 可靠性、认证处理和信号转发也得到修复，这对将 opencode 接入脚本、包装层或自动化流程的人尤其重要。 HTTP API 的修复包括：空的认证/共享错误保持原有线格式、返回结构化校验错误、拒绝无效的权限和问题 ID，以及在带类型的 `401` 响应中附带认证挑战信息。该版本还修正了 OpenAPI 文档路由、保持工具顺序稳定，并针对 Gemini、Anthropic Opus 4.5、OpenAI deep research 模型和 GPT-5 变体调整了各自支持的推理选项。

github · opencode-agent[bot] · May 9, 16:54

**背景**: opencode 是一个面向命令行的开发者工具，包含 TUI、HTTP API 和桌面端支持，因此一次小版本更新可能同时影响交互使用和自动化场景。新加入的 Scout 代理用于外部调研任务，例如仓库文档检索和依赖源码检查，而工作区同步则帮助工具在无需手动配置的情况下发现并注册工作区。OpenAPI 是描述 HTTP API 的标准方式，因此修复文档路由有助于客户端生成和 API 使用方集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.claudekit.cc/docs/marketing/agents/scout">Scout Agent - ClaudeKit Documentation</a></li>
<li><a href="https://learn.openapis.org/specification/paths.html">API Endpoints - OpenAPI Documentation Paths and Operations | Swagger Docs Customize OpenAPI documents - GitHub OpenAPI Document Generation in .NET 9 APIs - C# Corner python-openapi · PyPI Modern API Development with TypeSpec and OpenAPI</a></li>
<li><a href="https://developer.chrome.com/docs/devtools/automatic-workspaces">Automatic Workspace connection in Chrome DevTools | Chrome for...</a></li>

</ul>
</details>

**标签**: `#release`, `#CLI tools`, `#developer-tools`, `#HTTP API`, `#workspace management`

---

<a id="item-8"></a>
## [Gemini API 文件搜索支持多模态](https://blog.google/innovation-and-ai/technology/developers-tools/expanded-gemini-api-file-search-multimodal-rag/) ⭐️ 6.0/10

Google 宣布 Gemini API 的 File Search 工具现在支持多模态检索，因此开发者可以在不止文本的数据上构建 RAG 系统。此次更新还为 File Search 工作流加入了自定义元数据支持。 这扩展了 Gemini 面向开发者的工具能力，适合需要从包含图片或其他非文本内容的文件中检索信息的应用。它也让 Gemini 的 RAG 方案更接近整个行业向多模态 RAG 发展的趋势，即让模型能够搜索并推理多种数据类型。 根据 Google 的 File Search 文档，该工具会导入、分块并索引数据，以便根据提示快速检索，而这次更新把这一流程扩展到了多模态输入。此次公告更像是一次能力增强，而不是新产品线或重大模型发布。

hackernews · gmays · May 10, 03:22 · [社区讨论](https://news.ycombinator.com/item?id=48080702)

**背景**: RAG，即检索增强生成，是一种先检索相关外部信息，再利用这些信息生成答案的技术。传统 RAG 通常主要处理文本，而多模态 RAG 则把同样的思路扩展到图片、视频等其他格式。实际应用中，这能让 AI 系统利用比纯文本更丰富的来源材料来回答问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/expanded-gemini-api-file-search-multimodal-rag/">Gemini API File Search is now multimodal</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/file-search">Gemini generateContent API | Google AI for Developers</a></li>
<li><a href="https://www.ibm.com/think/topics/multimodal-rag">What is multimodal RAG? - IBM</a></li>

</ul>
</details>

**社区讨论**: 讨论整体偏怀疑，重点更多放在 Gemini 的产品体验，而不是这次技术更新本身。评论者批评了 AI Studio 的搜索和滚动体验，询问是否支持按 API key 设置消费上限，并讽刺 Google 虽然搜索技术强，但自家 AI 产品的搜索体验却不佳。

**标签**: `#Gemini`, `#LLM APIs`, `#RAG`, `#multimodal`, `#developer tools`

---

<a id="item-9"></a>
## [FCC 拟要求开号前核验身份](https://reclaimthenet.org/the-fcc-wants-your-id-before-you-get-a-phone-number) ⭐️ 6.0/10

美国 FCC 一致通过了一项提案，拟要求运营商在开通电话服务前核验用户身份。该草案将覆盖传统运营商、移动运营商和 VoIP 服务，可能要求提供政府签发证件、法定姓名、住址以及现有号码信息；目前仍在征求公众意见。 如果最终落地，这项规则会让用户更难在不暴露真实身份的情况下获取电话号码，影响重视隐私的用户、预付费手机购买者和 VoIP 用户。它也反映出监管机构正把反欺诈、反骚扰措施进一步延伸到电信开户注册环节。 该提案还在考虑要求运营商在用户离网后至少保存身份资料 4 年，并核查执法观察名单。由于规则也会覆盖预付费手机和 SIM 卡，而这类产品通常是按购买方式办理的，实际影响最大的将是开户注册时匿名性的下降。

telegram · zaihuapd · May 10, 04:12

**背景**: VoIP 指的是通过互联网提供的电话服务，不同于传统固定电话线路。预付费 SIM 卡通常以购买式套餐出售，往往不需要长期合约，因此历史上比需要完整实名核验的后付费服务更容易获得。在这个背景下，FCC 的提案就是要把更多电话服务纳入身份核验模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anttone.com/cn/voip-virtual-phone-number.htm">VoIP 电 话 服 务 | AntTone.com</a></li>
<li><a href="https://povo.jp/zh-CHS/consider/library/detail/article_099/">什么是预付费SIM卡？讲解其优缺点、使用场景和激活流程！| au智能手机...</a></li>

</ul>
</details>

**标签**: `#FCC`, `#privacy`, `#telecom policy`, `#identity verification`, `#VoIP`

---
