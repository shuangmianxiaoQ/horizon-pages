---
layout: default
title: "Horizon Summary: 2026-05-15 (ZH)"
date: 2026-05-15
lang: zh
---

> From 65 items, 21 important content pieces were selected

---

1. [Calif 宣称首个公开的 M5 macOS 内核漏洞利用](#item-1) ⭐️ 9.0/10
2. [移除 2024 款 RAV4 混动的调制解调器和 GPS](#item-2) ⭐️ 8.0/10
3. [英国政府改用自建难民系统](#item-3) ⭐️ 8.0/10
4. [DS4 面向本地 LLM 推理](#item-4) ⭐️ 8.0/10
5. [中国与波音磋商至多 500 架 737 MAX](#item-5) ⭐️ 8.0/10
6. [arXiv 严惩未核查 LLM 内容](#item-6) ⭐️ 8.0/10
7. [苹果与 OpenAI 联盟出现裂痕，OpenAI 考虑法律行动](#item-7) ⭐️ 8.0/10
8. [OxCaml 进入太空系统](#item-8) ⭐️ 7.0/10
9. [RTX 5090 在 M4 MacBook Air 上能玩吗](#item-9) ⭐️ 7.0/10
10. [多尺度 Transformer 缓解气象误差累积](#item-10) ⭐️ 7.0/10
11. [🐶 京东上线 AI 硬件京东自营专区 多款遭受制裁硬件现可恢复购买  京东开设“AI 硬件京东自营专区”，首批上架 NVIDIA GeForce RTX 509](#item-11) ⭐️ 7.0/10
12. [♻️ 英伟达盘中市值首次突破 5.5 万亿美元，高于第三大经济体德国 GDP](#item-12) ⭐️ 7.0/10
13. [加州集体诉讼指控 OpenAI 未经同意向 Meta 和 Google 分享用户数据](#item-13) ⭐️ 7.0/10
14. [anomalyco/opencode released v1.14.51](#item-14) ⭐️ 6.0/10
15. [openclaw/openclaw released v2026.5.14-beta.2](#item-15) ⭐️ 6.0/10
16. [Show HN: Find the best local LLM for your hardware, ranked by benchmarks](#item-16) ⭐️ 6.0/10
17. [Kimi WebBridge](#item-17) ⭐️ 6.0/10
18. [科技爱好者周刊（第 396 期）：互联网通信的替代方案](#item-18) ⭐️ 6.0/10
19. [🤖 ChatGPT Android 版拆解发现 Codex 手机远控桌面会话功能  ChatGPT Android 版 1.2026.125 的 APK 被拆解](#item-19) ⭐️ 6.0/10
20. [开源项目分享：Anima——20 亿参数动漫风文生图模型](#item-20) ⭐️ 6.0/10
21. [Surge 官方回应 VLESS 协议支持请求：因非标准设计增加维护风险，暂不合并至正式版  知名网络工具 Surge 开发者近日就用户长期请求支持 VLESS](#item-21) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Calif 宣称首个公开的 M5 macOS 内核漏洞利用](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 9.0/10

Calif 表示，他们与 AI 系统 Mythos Preview 合作，在 5 天内为运行 macOS 26.4.1 的 Apple M5 硬件构建了一条本地内核提权链，时间范围是 4 月 25 日到 5 月 1 日。该链据称从非特权本地用户开始，仅使用普通系统调用即可获得 root shell，并绕过了 Apple 的 Memory Integrity Enforcement（MIE）。 如果属实，这将是首个公开的 Apple M5 macOS 内核内存破坏漏洞利用，也是 Apple 最新平台上本地提权的一个明确案例。它还说明 AI 辅助工作流可能显著加速漏洞发现和利用开发，这对防御方、Apple 以及依赖 MIE 作为安全边界的用户都很重要。 Calif 将该利用链描述为“数据型”内核本地提权链，而不是内核代码执行，并表示其中涉及两个漏洞和多项技术。该团队称会在 Apple 修复后发布一份 55 页的技术报告，因此目前信息仍主要来自研究人员的表述，而非完整公开报告。

telegram · zaihuapd · May 15, 02:15

**背景**: Apple 的 Memory Integrity Enforcement（MIE）是一种基于硬件的内存安全防护，结合了 Apple silicon 和操作系统保护机制。Apple 表示，这项技术凝聚了长达五年的工程投入，旨在保护内核——也就是在软件与硬件之间充当高权限核心的部分。内核内存破坏漏洞有时可以被转化为本地提权，也就是攻击者从普通用户起步，最终获得同一台机器上的 root 级控制权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.calif.io/p/first-public-kernel-memory-corruption">First public macOS kernel memory corruption exploit on Apple M5</a></li>
<li><a href="https://security.apple.com/blog/memory-integrity-enforcement/">Memory Integrity Enforcement : A complete vision for memory safety...</a></li>
<li><a href="https://cyberinsider.com/researchers-claim-the-first-macos-kernel-exploit-on-apple-m5-chips/">Researchers claim the first macOS kernel exploit on Apple M5 ...</a></li>

</ul>
</details>

**标签**: `#security`, `#macOS`, `#exploit`, `#Apple M5`, `#kernel vulnerability`

---

<a id="item-2"></a>
## [移除 2024 款 RAV4 混动的调制解调器和 GPS](https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/) ⭐️ 8.0/10

一篇详细文章描述了从一辆 2024 款丰田 RAV4 混动中拆除调制解调器和 GPS。作者将这一改装定位为以隐私为导向，试图减少车辆的遥测和联网能力。 联网汽车越来越依赖远程信息处理硬件来传输车辆数据，因此关闭这条路径会实质性改变车辆向外发送什么信息。对于重视隐私的车主，以及关注车企和车机系统对遥测控制权的人来说，这篇文章都很有参考价值。 社区讨论指出，拆掉调制解调器可能并不是唯一的数据通道：有人提到可以通过 Toyota Techstream 编码、调整 Denso 车机设置，而且蓝牙连接还可能借助手机继续传输遥测数据。也有人指出，USB 连接的 CarPlay 可能避开这条路径，但 CarPlay 和 Android Auto 本身仍可能收集车辆遥测信息。

hackernews · arkadiyt · May 14, 17:08 · [社区讨论](https://news.ycombinator.com/item?id=48138136)

**背景**: 远程信息处理控制单元（TCU）是让汽车具备蜂窝联网能力的嵌入式系统，它负责与外部服务通信。对于现代联网汽车来说，这条连接可以支持定位、远程功能，以及向厂商回传数据。文章中拆除调制解调器和 GPS，正是针对支持这些功能的硬件，因此会直接涉及隐私和车辆破解话题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Telematic_control_unit">Telematic control unit - Wikipedia</a></li>
<li><a href="https://www.valeo.com/en/connectivity-systems/">Connectivity for connected cars | Valeo</a></li>

</ul>
</details>

**社区讨论**: 讨论整体上支持这种隐私取向，但重点集中在实际权衡和隐藏的数据通道上。有人建议用 Techstream 等软件方式替代，而另一些人则担心，即使拆掉硬件，蓝牙、通过 USB 连接的手机集成功能以及车机系统仍然可能泄露数据。

**标签**: `#privacy`, `#automotive hacking`, `#embedded systems`, `#telemetry`, `#reverse engineering`

---

<a id="item-3"></a>
## [英国政府改用自建难民系统](https://www.bbc.com/news/articles/c2l2j1lxdk5o) ⭐️ 8.0/10

据报道，英国政府正用内部自建系统替换用于难民案件管理的 Palantir 软件。BBC 报道了这一变化后，围绕公共部门技术策略和对供应商的依赖问题引发了讨论。 这显示出政府正在尝试减少对强势供应商在敏感公共服务上的依赖。它也凸显了政府 IT 中关于厂商锁定、成本以及数据主权的更广泛担忧。 Palantir Foundry 是一个同时用于商业和政府场景的数据平台，因此替换它影响的可能不只是前端界面。评论者重点讨论了跨系统数据集成的复杂性，并认为真正的难点往往在底层数据管道和工作流程。

hackernews · cdrnsf · May 14, 22:44 · [社区讨论](https://news.ycombinator.com/item?id=48142251)

**背景**: Palantir 是一家以数据平台著称的软件公司，其中 Foundry 用于跨系统汇总和分析大量信息。厂商锁定是指由于客户的数据和工作流程深度绑定某一家供应商的软件，导致更换供应商代价很高或非常困难。数据主权指数据由其存储或处理所在国家的法律和政策来约束。对于公共部门 IT 来说，这些问题尤为重要，因为政府系统通常处理敏感个人数据，而且还要长期稳定运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Palantir">Palantir - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vendor_lock-in">Vendor lock - in - Wikipedia</a></li>
<li><a href="https://www.contentguru.com/en-us/resources/blogs/internet-of-things-data/">The Boundaries of Data are Expanding... - Content Guru</a></li>

</ul>
</details>

**社区讨论**: 评论区整体上对 Palantir 持批评态度，许多人认为它价格很高，而且并不特别好用。也有人指出，政府团队本来就经常构建这类数据集成系统，真正的问题在于公共部门能否自己把系统做好并掌握主导权。

**标签**: `#government IT`, `#Palantir`, `#vendor lock-in`, `#public-sector software`, `#data sovereignty`

---

<a id="item-4"></a>
## [DS4 面向本地 LLM 推理](https://antirez.com/news/165) ⭐️ 8.0/10

Antirez 发布了一篇关于 DS4 的简短文章，介绍这是一款轻量级 LLM 推理运行时，并强调它面向本地部署以及对硬件的要求。文章也把 DS4 放在“小模型越来越能胜任编码任务”这个背景下来看待。 本地运行时可以减少对云端 API 的依赖，这对延迟、隐私、离线使用和成本可预测性都很重要。若更小的模型确实已经接近足够用于编码，那么像 DS4 这样的工具会让自托管硬件上的代理式工作流更可行。 社区评论指出，DS4 以 Metal 为主要后端，也支持 NVIDIA CUDA，并且特别考虑了 DGX Spark；AMD ROCm 则放在单独的 rocm 分支中。项目还依赖 llama.cpp 和 GGML，而且有评论者提到，目前使用它可能需要 96GB 的 VRAM。

hackernews · caust1c · May 14, 22:29 · [社区讨论](https://news.ycombinator.com/item?id=48142108)

**背景**: 轻量级 LLM 推理运行时指的是在本地硬件上加载模型并提供推理服务的软件层，而不是通过远程 API。这样做的重要性在于，本地部署可以减少供应商锁定，并让代码补全或私有文档处理更接近数据本身。通常会借助量化模型和 GGUF 这类紧凑格式来适配更小的机器，但性能仍然高度依赖可用的 GPU 或统一内存。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/topics/llm-local">llm -local · GitHub Topics · GitHub</a></li>
<li><a href="https://www.sitepoint.com/local-llms-complete-guide/">The Complete Developer's Guide to Running LLMs Locally</a></li>
<li><a href="https://aiobserver.co/comparing-the-top-6-inference-runtimes-for-llm-serving-in-2025/">Comparing the Top 6 Inference Runtimes for LLM ... - aiobserver.co</a></li>

</ul>
</details>

**社区讨论**: 讨论整体偏积极，而且技术味很浓，很多人对这样一个聚焦的运行时出现感到兴奋。主要话题是硬件门槛，尤其是有人提到的 96GB 要求，以及关于编码模型何时会“足够好”、从而改变代理工作流和 AI 服务采购方式的更大范围猜测。

**标签**: `#LLM inference`, `#local AI`, `#developer tools`, `#AI infrastructure`, `#machine learning`

---

<a id="item-5"></a>
## [中国与波音磋商至多 500 架 737 MAX](https://t.me/zaihuapd/41389) ⭐️ 8.0/10

据报道，波音正与中国方面磋商一笔最多可达 500 架 737 MAX 的潜在订单，相关方希望在本月底或下月初特朗普访华期间对外公布。若交易最终落地，这将是中国近 10 年来首笔面向波音的大型飞机订单。 一笔 500 架的订单将是波音的重要商业利好，也可能表明在多年放缓后，中国航空采购正在回暖。它还会成为中美贸易和航空关系中的一个重要信号，因为大型飞机采购往往同时具有商业和政治含义。 报道称，双方还在洽谈约 100 架宽体机，具体为 787 和 777X，但这些订单更可能在稍后单独宣布。交易尚未最终敲定，公告形式以及是否会形成具有约束力的正式承诺仍待协商。

telegram · zaihuapd · May 15, 01:09

**背景**: 737 MAX 是波音的窄体客机系列，主要用于中短程航线，并通过更高效的发动机和气动改进提升燃油效率。787 梦想客机和 777X 属于宽体机，适合长航线和更大的客流量，因此通常会与 737 MAX 这类单通道客机分开讨论。近年来，在更广泛的中美紧张关系背景下，波音来自中国的大额订单明显放缓，因此任何新的采购都格外重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Boeing_737_MAX">Boeing 737 MAX - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Boeing_777X">Boeing 777X - Wikipedia Boeing 787 vs 777X: Examining Features, Efficiency, and Impact Boeing 777X vs Boeing 787-8: What is the difference? Boeing 777X Explained Comparing Boeing’s Giants: 777 vs 787 Twinjet Showdown</a></li>

</ul>
</details>

**标签**: `#Aviation`, `#Boeing`, `#U.S.-China trade`, `#737 MAX`, `#Reuters`

---

<a id="item-6"></a>
## [arXiv 严惩未核查 LLM 内容](https://x.com/tdietterich/status/2055000956144935055) ⭐️ 8.0/10

arXiv 已明确：如果稿件中出现明显未核查的 LLM 生成内容，作者可能会被禁止投稿 1 年。处罚示例包括幻觉引用、模型留下的元注释，以及“请把示例数据替换为真实实验数据”这类提示语。 这提高了 LLM 在学术写作中的使用门槛，尤其影响依赖它来起草、润色或生成引用的研究者。它表明 arXiv 把 AI 辅助下的疏漏视为研究诚信问题，而不只是排版错误。 该政策适用于有明确证据表明作者没有检查模型输出的情况，而且禁投期结束后还有附加限制：之后的新投稿必须先被可信的同行评审发表场所接收。arXiv 同时强调，作者署名就意味着要对整篇论文负责，不管内容是如何生成的。

telegram · zaihuapd · May 15, 04:30

**背景**: arXiv 是一个预印本平台，研究者会在正式同行评审前先发布论文。由于 LLM 可能生成流畅但错误的文本，如果作者不仔细检查，就可能带来伪造引用、残留指令或其他痕迹。更广泛的担忧是，未经核查的模型使用会削弱研究流程和引用质量的可信度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aihola.com/article/arxiv-llm-author-ban">arXiv Bans Authors One Year Over Unchecked LLM Output</a></li>
<li><a href="https://the-decoder.com/arxiv-tightens-penalties-for-ai-bungling-in-scientific-papers/">Arxiv cracks down on unchecked AI-generated content in ...</a></li>
<li><a href="https://arxiv.org/abs/2605.07723">[2605.07723] LLM hallucinations in the wild: Large-scale evidence from non-existent citations</a></li>

</ul>
</details>

**标签**: `#arXiv`, `#LLM policy`, `#academic publishing`, `#AI safety`, `#research integrity`

---

<a id="item-7"></a>
## [苹果与 OpenAI 联盟出现裂痕，OpenAI 考虑法律行动](https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight) ⭐️ 8.0/10

彭博报道显示苹果与 OpenAI 的合作出现裂痕，OpenAI 认为苹果推广不足并考虑法律行动，而苹果则可能在 iOS 27 中进一步引入 Claude、Gemini 等模型。

telegram · zaihuapd · May 15, 12:59

**标签**: `#Apple`, `#OpenAI`, `#AI合作`, `#iOS`, `#法律纠纷`

---

<a id="item-8"></a>
## [OxCaml 进入太空系统](https://gazagnaire.org/blog/2026-05-14-borealis.html) ⭐️ 7.0/10

这篇文章介绍了 OxCaml 在航天相关软件中的一次部署，并展示了通过添加栈注解可以显著优化一个高频数据包分发路径。在文中的基准测试里，p99.9 延迟从每包 29 纳秒降到 9 纳秒，而且在 2500 万个数据包的处理过程中，minor GC 从 394 次降到了 0 次。 这说明 OCaml 的类型和模式系统不仅能用于微基准优化，也能在真实系统负载中直接提升性能。对于卫星和嵌入式风格的软件来说，更低的尾延迟和更少的 GC 压力，意味着更可预测的行为以及更少的运行时停顿。 OxCaml 的栈分配依赖局部注解和 `stack_` 关键字，编译器可以据此证明某些值可以放在栈上而不是堆上。文章强调的权衡很明确：通过增加更多类型注解，程序仍然保留 OCaml 默认的 GC，但可以在热点路径上消除堆分配。

hackernews · yminsky · May 15, 10:55 · [社区讨论](https://news.ycombinator.com/item?id=48147058)

**背景**: OCaml 通常使用垃圾回收器来管理内存，这简化了编程，但如果程序频繁分配对象，就可能带来额外开销。OxCaml 在这一模型上增加了模式和栈分配能力，使程序员可以更明确地表达分配行为，并在某些情况下让编译器在栈帧结束时立即回收这些值。文档还指出，要让栈分配在高阶函数中顺利工作，通常需要添加局部注解。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://oxcaml.org/documentation/stack-allocation/intro/">OxCaml | Stack allocation | Intro</a></li>
<li><a href="https://oxcaml.org/documentation/stack-allocation/reference/">OxCaml | Stack allocation | Reference</a></li>
<li><a href="https://ocaml.org/docs/garbage-collector">Understanding the Garbage Collector · OCaml Documentation</a></li>

</ul>
</details>

**社区讨论**: 评论区整体对性能结果持积极态度，其中一位评论者特别强调，减少 GC 压力是最大的收益。社区还补充了更多背景：有人声称自己早在 2016 年就把 OCaml 用到了太空任务中；另外一些人则讨论了卫星软件选型、CCSDS 的复杂性，以及与其自定义加密，不如使用 TLS 这类成熟安全协议。

**标签**: `#OCaml`, `#OxCaml`, `#systems programming`, `#performance optimization`, `#satellite software`

---

<a id="item-9"></a>
## [RTX 5090 在 M4 MacBook Air 上能玩吗](https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/) ⭐️ 7.0/10

这篇文章测试了将 RTX 5090 以外接显卡式方案连接到 M4 MacBook Air 上，同时用于游戏和本地 LLM 工作负载。结果表明，这种配置在技术上可以实现，但 macOS 的图形支持和性能瓶颈仍然非常明显。 这件事之所以重要，是因为很多人想用 Apple Silicon 笔记本做本地 AI，同时又希望获得独立显卡的性能和更好的游戏兼容性。文章凸显了苹果硬件能力与 eGPU 式工作流所需软件支持之间的落差。 苹果官方支持页面仍然写明，eGPU 只支持带 Thunderbolt 3 的 Intel Mac，这也说明 M4 MacBook Air 上的这种方案非常不寻常。讨论还指出，macOS 的图形限制，尤其是对 OpenGL 的支持不足，以及 LLM 的提示词处理瓶颈，是主要的实际问题。

hackernews · allenleee · May 14, 15:47 · [社区讨论](https://news.ycombinator.com/item?id=48137145)

**背景**: eGPU 是通过 Thunderbolt 连接到笔记本上的外接图形处理器，让电脑使用桌面级 GPU 硬件。过去的 Intel Mac 支持这种功能，但 Apple Silicon Mac 已经不在官方 eGPU 路径之内。GPU passthrough 是一种相关的虚拟化技术，它可以让虚拟机直接访问一块物理 GPU，所以在讨论 Mac 如何更好地利用独立显卡时经常会被提到。LLM inference 指的是在本地运行语言模型，而速度不仅取决于 GPU 算力，也取决于内存行为和提示词处理吞吐量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/en-us/102363">Use an external graphics processor with your Mac - Apple Support</a></li>
<li><a href="https://medium.com/macoclock/why-dont-macs-with-apple-silicon-support-egpu-db13a705512c">Why Don’t Macs With Apple Silicon Support eGPU ? | Medium</a></li>
<li><a href="https://github.com/BigAnteater/MacOS-KVM-GPU-Passthrough">GitHub - BigAnteater/ MacOS -KVM- GPU - Passthrough : Run macOS ...</a></li>

</ul>
</details>

**社区讨论**: 评论者整体上对这种方案能跑起来感到很惊讶，也有不少人表示自己长期希望 Apple Silicon 能支持 GPU passthrough 或原生外接 NVIDIA 显卡。另一些人更关注实际的 AI 使用场景，指出 Mac 上提示词处理速度往往才是真正瓶颈；还有人提醒，苹果官方文档至今仍把 eGPU 限制在 Intel Mac 和 AMD 显卡上。

**标签**: `#Apple Silicon`, `#eGPU`, `#GPU passthrough`, `#LLM inference`, `#PC gaming`

---

<a id="item-10"></a>
## [多尺度 Transformer 缓解气象误差累积](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247890898&idx=4&sn=d075b46de39b2318be648f978a45257e) ⭐️ 7.0/10

这篇文章介绍了一种与 ICML 2026 相关的方法，使用高效的多尺度 Transformer 来缓解气象预测中的长期误差累积问题。它还声称同一套架构可以适配气象与视觉两类任务。 长时程预测最容易出现小误差不断累积的问题，因此如果这种方法能降低累积误差，就可能提升实际天气预报的可靠性。一个能在气象和视觉之间迁移的共享架构也很重要，因为它暗示了一种更可复用的序列与图像建模设计。 其核心技术思路是多尺度 Transformer，通常意味着在不同分辨率上处理信息，从而同时捕捉局部模式和更大范围的上下文。给出的摘要没有提供具体基准、数据集或消融结果，因此无法仅凭这段材料核实真实的性能提升幅度。

rss · 量子位 · May 15, 02:10

**背景**: Transformer 模型通过注意力机制来关联输入序列中的不同部分，已经成为许多 AI 系统中的基础骨干网络。对于气象预测来说，尤其是在更长时间跨度上，误差会一步一步累积，导致预报时间越长，预测质量越容易下降。多尺度架构会尝试以多种粒度表示同一份数据，让模型既能看到细节，也能把握整体趋势。这里提到视觉任务，是因为同样的多尺度设计除了时间序列预测之外，也可能适用于图像处理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://colab.research.google.com/github/d2l-ai/d2l-zh-tensorflow-colab/blob/master/chapter_attention-mechanisms/transformer.ipynb">transformer .ipynb - Colab</a></li>
<li><a href="https://www.weather.com.cn/weather15d/101250401.shtml">衡阳 天 气 预 报 ,衡阳7 天 天 气 预 报 ,衡阳15 天 天 气 预 报 ,衡阳 天 气 查询</a></li>
<li><a href="https://www.researchgate.net/publication/342976544_2019-jiyujiqixuexideshuzhitianqiyubaofengsudingzhengyanjiu">(PDF) 2019-基于 机 器 学 习 的数值 天 气 预 报 风速订正研究</a></li>

</ul>
</details>

**标签**: `#weather forecasting`, `#transformer`, `#ICML`, `#machine learning`, `#multiscale architecture`

---

<a id="item-11"></a>
## [🐶 京东上线 AI 硬件京东自营专区 多款遭受制裁硬件现可恢复购买  京东开设“AI 硬件京东自营专区”，首批上架 NVIDIA GeForce RTX 509](https://t.me/zaihuapd/41386) ⭐️ 7.0/10

京东开设 AI 硬件自营专区，上架 RTX 5090、RTX PRO 6000 Blackwell 和 H100 等高端硬件，引发对受限 AI 算力设备重新可购的关注。

telegram · zaihuapd · May 14, 16:22

**标签**: `#AI硬件`, `#NVIDIA`, `#GPU`, `#中国市场`, `#供应链`

---

<a id="item-12"></a>
## [♻️ 英伟达盘中市值首次突破 5.5 万亿美元，高于第三大经济体德国 GDP](https://www.ithome.com/0/950/303.htm) ⭐️ 7.0/10

英伟达盘中市值首次突破 5.5 万亿美元，创下全球上市公司市值新纪录，并超过德国名义 GDP。

telegram · zaihuapd · May 14, 16:43

**标签**: `#NVIDIA`, `#AI infrastructure`, `#market cap`, `#semiconductors`, `#tech industry`

---

<a id="item-13"></a>
## [加州集体诉讼指控 OpenAI 未经同意向 Meta 和 Google 分享用户数据](https://futurism.com/artificial-intelligence/openai-personal-information-meta-google) ⭐️ 7.0/10

A California class-action lawsuit alleges OpenAI shared user chat queries and personal identifiers with Meta and Google without proper consent.

telegram · zaihuapd · May 15, 03:45

**标签**: `#OpenAI`, `#privacy`, `#class-action lawsuit`, `#data sharing`, `#AI policy`

---

<a id="item-14"></a>
## [anomalyco/opencode released v1.14.51](https://github.com/anomalyco/opencode/releases/tag/v1.14.51) ⭐️ 6.0/10

opencode v1.14.51 adds experimental background subagents and MCP connect while fixing several session, API, and compatibility bugs.

github · opencode-agent[bot] · May 15, 00:39

**标签**: `#release-notes`, `#developer-tools`, `#ai-agents`, `#bugfixes`, `#mcp`

---

<a id="item-15"></a>
## [openclaw/openclaw released v2026.5.14-beta.2](https://github.com/openclaw/openclaw/releases/tag/v2026.5.14-beta.2) ⭐️ 6.0/10

openclaw/openclaw v2026.5.14-beta.2 adds command-turn support, per-agent bootstrap overrides, dependency simplification, lazy-loaded Canvas modules, and updated maintainer tooling.

github · steipete · May 15, 11:11

**标签**: `#release`, `#SDK`, `#agent-framework`, `#performance`, `#dependency-management`

---

<a id="item-16"></a>
## [Show HN: Find the best local LLM for your hardware, ranked by benchmarks](https://github.com/Andyyyy64/whichllm) ⭐️ 6.0/10

A Show HN project that recommends the best local LLM for your hardware by ranking models against benchmarks and system specs.

hackernews · andyyyy64 · May 15, 09:19 · [社区讨论](https://news.ycombinator.com/item?id=48146369)

**标签**: `#local-llms`, `#benchmarking`, `#ai-tools`, `#gpu`, `#hacker-news`

---

<a id="item-17"></a>
## [Kimi WebBridge](https://www.producthunt.com/products/kimi-ai-assistant) ⭐️ 6.0/10

Kimi WebBridge is a tool that connects AI agents to the live web.

rss · Product Hunt · May 15, 05:16

**标签**: `#AI agents`, `#web automation`, `#product launch`, `#agent tooling`, `#Product Hunt`

---

<a id="item-18"></a>
## [科技爱好者周刊（第 396 期）：互联网通信的替代方案](http://www.ruanyifeng.com/blog/2026/05/weekly-issue-396.html) ⭐️ 6.0/10

This issue of Tech Enthusiast Weekly highlights alternative approaches to internet communication and curates noteworthy technology content for the week.

rss · ruanyifeng · May 15, 00:01

**标签**: `#networking`, `#internet communication`, `#tech newsletter`, `#systems`, `#alternative protocols`

---

<a id="item-19"></a>
## [🤖 ChatGPT Android 版拆解发现 Codex 手机远控桌面会话功能  ChatGPT Android 版 1.2026.125 的 APK 被拆解](https://t.me/zaihuapd/41388) ⭐️ 6.0/10

ChatGPT Android 版 APK 拆解显示，OpenAI 正在为 Codex 添加手机远程管理和重连桌面会话的功能。

telegram · zaihuapd · May 14, 21:48

**标签**: `#OpenAI`, `#Codex`, `#APK拆解`, `#Android`, `#远程控制`

---

<a id="item-20"></a>
## [开源项目分享：Anima——20 亿参数动漫风文生图模型](https://civitai.com/models/2458426/anima) ⭐️ 6.0/10

Anima is a 2B-parameter open anime-focused text-to-image model trained on millions of anime images and hundreds of thousands of non-anime art images for generating anime concepts, characters, and stylized artwork.

telegram · zaihuapd · May 15, 03:00

**标签**: `#text-to-image`, `#generative AI`, `#anime model`, `#open source`, `#computer vision`

---

<a id="item-21"></a>
## [Surge 官方回应 VLESS 协议支持请求：因非标准设计增加维护风险，暂不合并至正式版  知名网络工具 Surge 开发者近日就用户长期请求支持 VLESS](https://t.me/zaihuapd/41396) ⭐️ 6.0/10

Surge’s developers said they have an experimental VLESS implementation but will not ship it in the stable release because its non-standard TLS-layer design would increase maintenance and security risk.

telegram · zaihuapd · May 15, 05:36

**标签**: `#Surge`, `#VLESS`, `#networking`, `#TLS`, `#proxy protocols`

---
