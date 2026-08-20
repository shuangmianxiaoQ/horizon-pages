---
layout: default
title: "Horizon Summary: 2026-08-20 (ZH)"
date: 2026-08-20
lang: zh
---


> 从 45 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [恶意 Rust crate arrayref 在构建时执行载荷](#item-tech-news-1) ⭐️ 8.0/10
2. [AliExpress 静默 WebAudio 指纹识别干扰蓝牙多设备连接](#item-tech-news-2) ⭐️ 8.0/10
3. [Stripe 收购 OpenRouter，整合 AI 模型网关](#item-tech-news-3) ⭐️ 8.0/10
4. [陶哲轩警告：AI 或引发数学界最大危机](#item-tech-news-4) ⭐️ 8.0/10
5. [爱快路由系统曝高危漏洞：无线 AC 远程命令注入](#item-tech-news-5) ⭐️ 8.0/10
6. [125M 参数 Transformer 实现 iPhone 端钢琴自动续奏](#item-tech-news-6) ⭐️ 7.0/10
7. [阿里发布 Qwen-UI-Agent，让模型真正会用每一块屏幕](#item-tech-news-7) ⭐️ 7.0/10
8. [FastMetal 让 Mac 本地 30 秒生成视频](#item-tech-news-8) ⭐️ 7.0/10
9. [H20 上优化 DeepSeek-V4-Pro 服务性能](#item-tech-news-9) ⭐️ 7.0/10
10. [OpenAI 预览零数据留存与私密安全处理](#item-tech-news-10) ⭐️ 7.0/10
11. [AI 助中国学生作业提分 18% 却致考试降 20%](#item-tech-news-11) ⭐️ 7.0/10
12. [美国 CFTC 就 AI 算力期货公开征求意见](#item-tech-news-12) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [恶意 Rust crate arrayref 在构建时执行载荷](https://safedep.io/arrayref-proc-macro1-rust-build-time-malware/) ⭐️ 8.0/10

流行的 Rust crate &\#x27;arrayref&\#x27; 的一个恶意版本被发现会在构建时执行载荷，引发了对 Cargo 沙箱和供应链安全的紧急讨论。该事件涉及一个广泛使用的 crate，其被攻破后运行了构建时恶意代码，凸显了 Cargo 构建脚本沙箱的关键缺口。社区讨论热烈，有 146 个点赞和 94 条评论，并附有官方 Rust 博客和安全厂商的分析链接。此事件对软件工程和安全专业人士高度相关，但并非范式转变或新技术发布。

hackernews · abhisek · 8月20日 13:23 · [社区讨论](https://news.ycombinator.com/item?id=49374269)

**「背景」** arrayref 是一个广泛使用的 Rust 库，用于在切片和数组之间进行安全的引用转换，其 0.3.10 版本被恶意篡改，注入了一个名为 proc-macro1 的恶意依赖包。该恶意包在构建时（通过 build script）下载并执行远程载荷，属于典型的供应链攻击。Rust 官方安全响应团队于 2026 年 8 月 20 日确认了该事件，并已发布相关公告。

**「影响」** 受影响用户可能面临 CI 密钥泄露或构建环境被破坏的风险，因为恶意构建脚本可访问网络和文件系统。此事件可能促使 Rust 社区加速推进 Cargo 构建脚本沙箱化，以限制类似攻击的爆炸半径。

**「社区讨论」** 社区评论强调 Cargo 迫切需要为 build.rs 脚本提供沙箱，并指出此前尝试未果。有观点认为，在严格容器化之外进行软件开发风险日益增大，且 Rust 生态与 JS 生态一样面临依赖链攻击的威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.stepsecurity.io/blog/arrayref-rust-crate-supply-chain-attack">Rust Supply - Chain Attack : arrayref 0.3.10 and the... - StepSecurity</a></li>
<li><a href="https://blog.rust-lang.org/2026/08/20/supply-chain-attack-on-arrayref/">Supply chain attack on arrayref | Rust Blog</a></li>
<li><a href="https://www.aikido.dev/blog/two-popular-rust-crates-arrayref-and-append-only-vec-compromised-in-supply-chain-attack">Two popular Rust crates arrayref and append-only-vec compromised...</a></li>

</ul>
</details>

**标签**: `#security`, `#rust`, `#supply-chain`, `#cargo`, `#malware`

---

<a id="item-tech-news-2"></a>
### [AliExpress 静默 WebAudio 指纹识别干扰蓝牙多设备连接](https://blog.laserphile.com/2026/08/aliexpress-webpage-keeping-multipoint.html) ⭐️ 8.0/10

一篇博客文章披露，阿里巴巴旗下的电商平台 AliExpress 在其网页中使用了静默的 WebAudio 指纹识别技术，该技术会干扰蓝牙多设备连接（multipoint）功能。文章指出，这种指纹识别通过无声的音频处理来收集设备特征，但副作用是可能导致蓝牙耳机或助听器在连接多个设备时出现异常，例如环境噪音放大变化或音频命令误触发。社区评论中，多位用户报告了类似问题，涉及 AliExpress 的 iOS 应用、Wolt 应用以及某些新闻网站，表明该问题可能并非个例。该技术引发了对隐私侵犯的担忧，因为用户可能在不知情的情况下被追踪，同时其副作用也影响了正常设备功能。

hackernews · emctech · 8月20日 10:08 · [社区讨论](https://news.ycombinator.com/item?id=49372583)

**「背景」** WebAudio 指纹识别是一种通过浏览器音频处理 API 提取设备特征的技术，通常利用音频处理链的微小差异来生成唯一标识，用于跨站点追踪用户。蓝牙多点连接（Bluetooth multipoint）允许一副耳机同时连接多个设备（如电脑和手机），并根据音频播放状态自动切换。AliExpress 首页静默运行的两个 WebAudio 指纹识别脚本（collina.js 和 fireyejs.js）创建了零增益音频图并连接到系统输出，即使静音也会被浏览器处理，从而干扰了耳机的多点切换功能。

**「影响」** 对于使用蓝牙多设备连接功能的用户（如佩戴助听器或使用车载音频系统的人），访问 AliExpress 网站或使用其应用可能导致音频异常或连接中断，且用户可能因静默指纹识别而面临隐私风险。

**「社区讨论」** 用户评论证实了该问题的影响范围：有用户报告在访问多种网站时助听器环境噪音放大变化，另有用户发现 AliExpress 应用在后台时导致车载音频误触发，而其他用户则推测类似行为可能存在于 Wolt 等应用中，并怀疑是指纹识别所致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.laserphile.com/2026/08/aliexpress-webpage-keeping-multipoint.html">laserphile: AliExpress webpage keeping multipoint Bluetooth ...</a></li>
<li><a href="https://zeli.app/en/story/49372583">AliExpress runs silent WebAudio fingerprinting that breaks ...</a></li>

</ul>
</details>

**标签**: `#privacy`, `#web-audio`, `#fingerprinting`, `#bluetooth`, `#security`

---

<a id="item-tech-news-3"></a>
### [Stripe 收购 OpenRouter，整合 AI 模型网关](https://stripe.com/en-jp/newsroom/news/stripe-agrees-to-acquire-openrouter) ⭐️ 8.0/10

Stripe 于 2026 年 8 月 19 日宣布已同意收购 AI 模型网关与路由平台 OpenRouter。OpenRouter 能够根据任务复杂度、价格、速度和可靠性，在 80 多家提供商的 400 多个模型之间动态分配请求，帮助企业优化 Token 使用。此次收购标志着支付巨头 Stripe 进军 AI 基础设施领域，可能对依赖模型路由的 AI 开发者和企业产生广泛影响。目前交易的具体条款和后续技术整合细节尚未披露。

telegram · zaihuapd · 8月20日 07:00

**「背景」** OpenRouter 是一个 AI 模型网关与路由平台，允许开发者通过统一接口访问 80 多家提供商的 400 多个模型，并根据任务复杂度、价格、速度和可靠性动态分配请求，以优化 Token 使用。Stripe 是一家主要提供在线支付处理服务的公司，近年来正积极扩展其 AI 基础设施业务。此次收购是 Stripe 在 AI 基础设施领域的重要布局，据多家媒体报道，交易金额超过 70 亿美元，但官方未披露具体条款。

**「影响」** 对于使用 OpenRouter 的 AI 开发者和企业，此次收购可能带来更紧密的支付与模型路由集成，但具体技术变化和定价影响尚不明确，需关注后续公告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/08/19/business/stripe-openrouter-ai.html">Stripe Buys A.I. Start-Up OpenRouter for $7.5 Billion - The ...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/stripe-acquires-ai-model-gateway-124818504.html?fr=sycsrp_catchall">Stripe acquires AI model gateway OpenRouter for $7 billion</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-19/stripe-agrees-to-buy-ai-firm-openrouter-no-terms-disclosed">Stripe to Acquire AI Startup OpenRouter, Expanding Artificial ...</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#acquisition`, `#model routing`, `#Stripe`, `#OpenRouter`

---

<a id="item-tech-news-4"></a>
### [陶哲轩警告：AI 或引发数学界最大危机](https://the-decoder.com/terence-tao-says-ai-could-trigger-maths-biggest-crisis-since-godel/) ⭐️ 8.0/10

陶哲轩在为 2026 年国际数学家大会撰写的文章中警告，AI 可能引发数学界自哥德尔以来最大的危机，即证明过剩导致无人能懂。他呼吁数学界停止争论 AI 能做什么，转而正视研究目标这一被回避的问题，并将当下比作 1900 至 1930 年间由罗素悖论和哥德尔不完备定理引发的基础危机。他援引 First-Proof 项目的数据：第二轮中 10 道未发表研究题由 4 个 AI 系统测试，其中 7 道至少被一个系统判为合格，每题成本仅数十至数百美元。陶哲轩指出，数学可能从证明稀缺转向证明过剩，并强调即使通过形式验证，无人能清晰讲解的证明也应视为不完整。

telegram · zaihuapd · 8月20日 13:19

**「背景」** 陶哲轩是菲尔兹奖得主，他在为 2026 年国际数学家大会撰写的论文《Mathematics in the age of AI》中，将当前 AI 对数学的影响比作 20 世纪初由罗素悖论和哥德尔不完备定理引发的基础危机。他主张数学界应停止争论 AI 能做什么，转而正视研究目标这一被回避的问题。

**「影响」** 对数学研究者、AI 开发者和学术出版体系而言，这一警告意味着未来需要建立新的验证和沟通标准，否则大量 AI 生成的证明可能因无人理解而无法被有效利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.16753">Abstract page for arXiv paper 2608.16753: Mathematics in the age of AI</a></li>
<li><a href="https://the-decoder.com/terence-tao-says-ai-could-trigger-maths-biggest-crisis-since-godel/">Terence Tao says AI could trigger math &#x27;s biggest crisis since Gödel</a></li>

</ul>
</details>

**标签**: `#AI in Mathematics`, `#Terence Tao`, `#Proof Verification`, `#Mathematical Research`, `#AI Impact`

---

<a id="item-tech-news-5"></a>
### [爱快路由系统曝高危漏洞：无线 AC 远程命令注入](https://telegram.me/xhqcankao/31509) ⭐️ 8.0/10

安全研究人员通过固件逆向与比对，确认爱快 iKuai 路由系统的无线 AC 服务存在严重远程命令注入漏洞。在网络可达的情况下，未经身份认证的攻击者可利用该漏洞向设备注入任意 Shell 命令，并直接获取系统的 root 最高控制权限。该漏洞影响 iKuai8 3.7.23 及以下版本（暂无 CVE 编号），触发条件为启用无线 AC 功能（或通过 Mesh 路径拉起服务），且设备的 UDP/1234 端口暴露于 WAN 侧或非可信网络。漏洞根因在于 AC 控制协议使用固定密钥加密、缺少设备绑定的唯一认证机制，且系统在解析 Join 消息时将外部可控的 element 44 字段（上限 63 字节）直接拼接到 Shell 执行路径（调用 popen 执行脚本），未做参数过滤与转义。由于 AC 服务以 root 身份运行且未进行权限降级，注入成功后可执行任意高权限命令或拉取二阶段恶意载荷。建议受影响用户尽快将固件升级至 iKuai8 3.7.24 或更高版本，暂无法升级的用户应立即关闭“无线 AC 智能控制”功能，并配置防火墙阻断 UDP/1234 端口对外暴露。

telegram · xhqcankao · 8月20日 04:32

**「背景」** 爱快 iKuai 是一款面向企业、网吧及家庭场景的国产路由操作系统，其无线 AC（接入控制器）功能用于集中管理多个无线接入点（AP），通过 UDP/1234 端口与 AP 通信。该功能在启用时，若设备暴露于不可信网络，攻击者可能利用协议缺陷实施攻击。

**「影响」** 使用爱快 iKuai8 3.7.23 及以下版本且启用了无线 AC 功能、并将 UDP/1234 端口暴露于不可信网络的路由器用户，面临被远程完全控制的风险，攻击者可执行任意命令并获取 root 权限。

**标签**: `#security`, `#vulnerability`, `#router`, `#command injection`, `#iKuai`

---

<a id="item-tech-news-6"></a>
### [125M 参数 Transformer 实现 iPhone 端钢琴自动续奏](https://simedw.com/2026/08/20/midi-autocomplete/) ⭐️ 7.0/10

开发者 simedw 训练了一个 125M 参数的 Transformer 模型，用于在设备端实时自动续奏钢琴演奏，并在 iPhone 15 上实现了约每秒 108 个音符的处理速度。该模型类似于 GitHub Copilot 或 Tabnine，但以 MIDI 钢琴演奏的少量音符作为提示，模型会继续生成音乐，整个过程完全在设备端运行，无需联网。配套的免费 iPhone 应用已发布，供用户体验。项目展示了 Transformer 在音乐生成领域的实际应用，并涉及 Core ML 部署和训练数据的相关问题。

hackernews · simedw · 8月20日 12:04 · [社区讨论](https://news.ycombinator.com/item?id=49373456)

**「背景」** MIDI（乐器数字接口）是一种让电子乐器、计算机和其他设备之间交换音乐演奏数据的标准协议，它记录的是音符、力度和时长等指令，而非音频波形。自动续写钢琴演奏的想法并非全新：早在 2003 年，François Pachet 就开发了 Continuator 系统，它使用增强的马尔可夫模型来学习用户的演奏风格，并实时生成风格连贯的续奏，与用户进行交互式即兴演奏。与这些早期基于统计模型的方法不同，本项目采用现代 Transformer 架构，在设备端（通过 Core ML）运行，实现了更强大的序列建模能力。

**「影响」** 该演示为音乐软件和边缘 AI 领域提供了实用的参考，表明在移动设备上运行中等规模 Transformer 模型进行实时音乐生成是可行的，可能启发更多音乐创作工具采用类似技术。

**「社区讨论」** 社区评论中，有用户将其与 2003 年的 Continuator 项目（使用层次马尔可夫模型）进行比较，也有用户提到一个生成所有旋律以对抗音乐版权诉讼的项目。开发者被问及训练数据规模，但未在评论中直接回答。有用户反馈应用运行良好，并建议增加将 AI 生成的音频作为 MIDI 输出到外部设备的功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.francoispachet.fr/wp-content/uploads/2021/01/pachet-03d.pdf">The Continuator: Musical Interaction With Style</a></li>
<li><a href="https://www.researchgate.net/publication/261686495_The_Continuator_Musical_Interaction_With_Style">(PDF) The Continuator: Musical Interaction With Style continuator_interactive_music_instrument_style_AI The Continuator: Musical Interaction With Style Presented by Ching-Hua Chuan François Pachet: The Continuato fpachet (François Pachet) · GitHub Continuator – Library of Mixed-Initiative Creative Interfaces</a></li>
<li><a href="https://www.francoispachet.fr/continuator/">continuator_interactive_music_instrument_style_AI</a></li>

</ul>
</details>

**标签**: `#transformer`, `#MIDI`, `#on-device AI`, `#Core ML`, `#music generation`

---

<a id="item-tech-news-7"></a>
### [阿里发布 Qwen-UI-Agent，让模型真正会用每一块屏幕](https://aihot.virxact.com/items/cmt1di48c04vuro1q95i06dby) ⭐️ 7.0/10

阿里巴巴正式推出 Qwen-UI-Agent，这是一个以真实世界为中心的 GUI 智能体基座模型，旨在让模型能够真正“会用”每一块屏幕。该模型覆盖移动端、电脑端、网页端以及深度搜索（DeepSearch）环境，适用于多种平台上的实际屏幕交互场景。作为基座模型，Qwen-UI-Agent 为后续针对特定界面或任务的微调与部署提供了基础能力。此次发布标志着阿里在 GUI 智能体领域的重要布局，但官方尚未公布具体的技术细节、性能数据或基准测试结果。

rss · AI HOT 精选 · 8月20日 09:45

**「背景」** GUI 智能体（图形用户界面智能体）是一种能够像人类一样操作屏幕界面的人工智能模型，通过理解界面元素并执行点击、输入等操作来完成用户任务。此前，多数 GUI 智能体在真实设备上的表现有限，往往依赖模拟环境训练，难以应对真实世界的复杂界面。阿里巴巴推出的 Qwen-UI-Agent 是一个以真实世界为中心的 GUI 智能体基座模型，覆盖移动端、电脑端、网页端及深度搜索（DeepSearch）环境，其技术报告指出该模型在获得强大 GUI 能力的同时，并未退化为仅限 GUI 的窄模型，而是保留了基础模型的通用推理和智能体能力，以支持更广泛的任务。

**「影响」** 对于开发 GUI 智能体应用的研究人员与工程师而言，Qwen-UI-Agent 提供了一个覆盖多端环境的基座模型，可能降低从零构建屏幕交互智能体的门槛，并推动跨平台自动化操作与深度搜索等场景的落地。不过，由于缺乏公开的性能基准和对比数据，其实际效果与相对优势仍有待验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tongyi-mai.github.io/Qwen-UI-Agent/">Qwen-UI-Agent — Technical Report</a></li>
<li><a href="https://arxiv.org/abs/2607.28227">[2607.28227] Qwen-UI-Agent Technical Report: Toward Next ...</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#GUI`, `#Alibaba`, `#Qwen`, `#Foundation models`

---

<a id="item-tech-news-8"></a>
### [FastMetal 让 Mac 本地 30 秒生成视频](https://aihot.virxact.com/items/cmt0kxcuu07f2ro2owuqpbjc8) ⭐️ 7.0/10

FastMetal 项目将 FastWan-QAD 系列视频生成模型移植到 Apple Silicon，通过 MLX 和 Metal 实现完全本地的视频生成，无需 CUDA 或云端支持。在 Mac 上生成一段 5 秒 480P 视频仅需 30 秒，内存占用约 3.9 GiB，默认使用 INT8 量化。该项目提供三个模型：1.3B 支持 480P，5B 支持 720P，14B 追求更高画质。相关博客、代码和模型已分别发布在 haoailab.com、GitHub 和 Hugging Face 上。

rss · AI HOT 精选 · 8月19日 20:42

**「背景」** FastWan-QAD 是此前发布的视频生成模型系列，通过 DMD2 蒸馏和量化技术（如 NVFP4 精度）在 NVIDIA GPU 上实现了极快的推理速度，例如在 RTX 5090 上生成 5 秒 480P 视频仅需 1.8 秒。FastMetal 是 FastVideo 项目为 Apple Silicon 新增的 MLX 运行时，使原本依赖 CUDA 的模型、流水线和训练代码能够通过 Metal 在 Mac 上本地运行，并利用统一内存架构进行优化。

**「影响」** 对于使用 Apple Silicon Mac 的开发者，FastMetal 使得在本地快速生成视频成为可能，降低了视频生成的门槛，并减少了对云端 GPU 的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://haoailab.com/blogs/fastmetal/">FastMetal - QAD : Fast Local Video Generation on Apple Silicon</a></li>
<li><a href="https://gigazine.net/gsc_news/en/20260624-fastwan-qad-video-generation-ai/">A video generation AI model called &#x27; FastWan - QAD &#x27; has... - GIGAZINE</a></li>

</ul>
</details>

**标签**: `#Apple Silicon`, `#MLX`, `#Video Generation`, `#On-device AI`, `#Open Source`

---

<a id="item-tech-news-9"></a>
### [H20 上优化 DeepSeek-V4-Pro 服务性能](https://aihot.virxact.com/items/cmt0e7sxo01eiro2o4l4y9jmh) ⭐️ 7.0/10

LMSYS 团队针对 1.6 万亿参数的 MoE 模型 DeepSeek-V4-Pro，在 H20 GPU 上通过场景化服务配置优化性能。单节点 H20-141GB 参考实现达到 271 output tokens/s，与 B300 的 383.7 tokens/s 相比，性能差距缩小至 1.42 倍。该优化方法涉及针对不同场景调整服务配置，以逼近高端 GPU 的性能表现。这一成果对 AI 基础设施部署具有实际意义，但原始内容为摘要性描述，缺乏深入的技术细节。

rss · AI HOT 精选 · 8月19日 17:56

**「背景」** DeepSeek-V4-Pro 是 DeepSeek 于 2026 年 4 月发布的 1.6 万亿参数 MoE 模型，采用 Liquid MoE 架构，并针对 NVIDIA H200 进行了优化。其官方 vLLM 推理方案需要约 960 GB 的混合精度显存，通常需要 8 卡 H200 或 B300 集群，或升级到多节点集群。LMSYS 团队此前已针对该模型在 SGLang 等引擎上进行了推理优化，本次报道则聚焦于在显存较小的 H20 GPU 上通过场景化配置提升服务性能。

**「影响」** 使用 H20 GPU 部署 DeepSeek-V4-Pro 的开发者和组织，可通过场景化配置显著提升输出吞吐量，降低与 B300 等高端硬件的性能差距，从而在成本受限环境中更高效地运行大规模 MoE 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepseek.ai/blog">DeepSeek AI Blog: Model Updates, API Pricing &amp; Guides (2026)</a></li>
<li><a href="https://www.runpod.io/blog/deepseek-v4-in-the-wild-and-how-to-run-it-on-runpod">DeepSeek V4 in the wild, and how to run it on Runpod</a></li>
<li><a href="https://www.lmsys.org/blog/2026-04-25-deepseek-v4/">DeepSeek-V4 on Day 0: From Fast Inference to Verified RL with SGLang and Miles - LMSYS Org</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#GPU optimization`, `#LLM serving`, `#MoE`, `#H20`

---

<a id="item-tech-news-10"></a>
### [OpenAI 预览零数据留存与私密安全处理](https://openai.com/index/offering-zero-data-retention-for-frontier-models/) ⭐️ 7.0/10

OpenAI 宣布面向符合条件的 API 客户重申「零数据留存」（ZDR）承诺，即在请求处理完毕后不保留提示词与回复。同时，公司预览了「私密安全处理」机制，该机制可在不向 OpenAI 人员暴露原始内容的前提下，跨多次模型交互识别潜在滥用，并仅回传有限的安全信号。客户内容将使用由客户控制的密钥加密存储，即使被标记，OpenAI 员工也无法查看原文。该功能目前正与早期客户测试，计划于 9 月逐步上线，并发布技术白皮书。此举旨在突破以往 AI 安全系统只能单独监控单次交互的局限，在提升安全性的同时保障企业客户数据隐私。

telegram · zaihuapd · 8月20日 02:33

**「背景」** OpenAI 此前已为符合条件的 API 客户提供“零数据留存”（ZDR）选项，即请求处理完毕后不保留提示词与模型回复。但传统 AI 安全系统通常需要保留部分客户数据，才能跨多次交互识别滥用模式，这限制了零数据留存方案在安全监控上的能力。此次预览的“私密安全处理”机制旨在解决这一矛盾，在不保留原始内容的前提下，通过客户控制的密钥加密存储数据，并仅向 OpenAI 回传有限的安全信号，从而兼顾隐私保护与滥用检测。

**「影响」** 对于使用 OpenAI 前沿模型的企业 API 客户，这一举措将显著降低数据留存风险，使敏感数据在推理后不被存储，同时仍能获得跨交互的安全监控，从而可能推动金融、医疗等高度合规行业更放心地采用 OpenAI 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/offering-zero-data-retention-for-frontier-models/">Offering Zero Data Retention for frontier models | OpenAI</a></li>
<li><a href="https://www.medianama.com/2026/08/223-openai-zero-retention-frontier-models/">OpenAI tests private safety processing for Zero - Retention AI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#privacy`, `#security`, `#API`, `#data retention`

---

<a id="item-tech-news-11"></a>
### [AI 助中国学生作业提分 18% 却致考试降 20%](https://www.economist.com/graphic-detail/2026/08/18/does-ai-stop-children-from-learning) ⭐️ 7.0/10

《经济学人》报道的一项研究追踪了中国 2.7 万名 12 至 18 岁学生，其中约 80% 使用豆包等常见 AI 模型。六个月后，使用 AI 的学生各科作业平均分数上升 18%，每项作业耗时从 64 分钟降至 45 分钟；但考试时成绩比不用 AI 的同学低 20%，且成绩下滑集中在赶作业的学生中。研究认为，将 AI 当作私人辅导、花同样时间理解概念的学生成绩未受损。另一项研究也发现，借助聊天机器人学习的大学生测试得分更高，且优势在一周后仍保持。

telegram · zaihuapd · 8月20日 03:58

**「背景」** 该研究基于中国 7 至 12 年级（约 12 至 18 岁）学生 30 个月的追踪数据，样本量为 26,811 人，由经济政策研究中心（CEPR）发布。研究将学生使用生成式 AI（如豆包等常见模型）完成作业的情况与闭卷考试成绩进行对比，以考察 AI 对学习效果的影响。此前，作业成绩通常被视为预测考试成绩的指标，而该研究试图检验在 AI 介入后这一关联是否仍然成立。

**「影响」** 对于依赖 AI 快速完成作业的学生，其考试表现可能显著下降，而将 AI 用于辅助理解的学生则可能受益，这提示教育者和家长需关注 AI 使用方式对学习效果的差异化影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.economist.com/graphic-detail/2026/08/18/does-ai-stop-children-from-learning">Does AI stop children from learning? - The Economist</a></li>
<li><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6868618">The Generative AI Learning Penalty: Evidence from Chinese ...</a></li>
<li><a href="https://fortune.com/2026/07/21/gen-z-cheating-homework-school-exam-scores-crash-post-literate-society-incentives/">AI is boosting student homework scores, but tanking exam ...</a></li>

</ul>
</details>

**标签**: `#AI in education`, `#learning outcomes`, `#chatbots`, `#China`, `#empirical study`

---

<a id="item-tech-news-12"></a>
### [美国 CFTC 就 AI 算力期货公开征求意见](https://www.reuters.com/business/us-cftc-seeks-comment-compute-derivatives-ai-demand-grows-2026-08-19/) ⭐️ 7.0/10

美国商品期货交易委员会（CFTC）周三宣布，正就“算力衍生品合约”公开征求意见，以应对人工智能蓬勃发展带来的新型市场产品需求。此举是监管机构为算力市场制定规则的早期步骤，旨在帮助企业和投资者管理计算成本与可用性风险，征求意见范围涵盖算力现货市场、市场监管与操纵问题、客户保护以及永续算力期货。CFTC 主席表示，“没有稳健的算力衍生品市场，美国无法赢得 AI 竞赛”，此次征求意见是确立清晰规则的第一步。该消息由路透社报道，反映了 AI 基础设施领域监管框架的初步构建。

telegram · xhqcankao · 8月20日 10:40

**「背景」** 算力衍生品是一种金融合约，其价值与计算能力（如 GPU 算力）的价格或可用性挂钩，类似于大宗商品期货。随着人工智能的快速发展，算力成为关键投入品，其成本和供应波动给企业带来风险。美国商品期货交易委员会（CFTC）是负责监管衍生品市场的联邦机构，此次征求意见是其为算力市场制定规则的第一步。CFTC 主席 Michael Selig 表示，没有稳健的算力衍生品市场，美国无法赢得 AI 竞赛。

**「影响」** 此举可能为企业和投资者提供对冲 AI 算力成本与可用性风险的新工具，从而影响 AI 基础设施的财务规划和投资策略。但具体影响取决于最终规则如何界定合约设计、市场监督和客户保护措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://money.usnews.com/investing/news/articles/2026-08-19/us-cftc-seeks-comment-on-compute-derivatives-as-ai-demand-grows">US CFTC Seeks Comment on Compute Derivatives as AI Demand...</a></li>
<li><a href="https://www.pymnts.com/legal/2026/cftc-prepares-to-draft-rules-for-trading-compute-derivatives-contracts/">CFTC Prepares to Draft Rules for Trading Compute Derivatives</a></li>
<li><a href="https://beincrypto.com/cftc-compute-derivatives-comment-request/">Michael Selig Calls Compute the Most Important Commodity as...</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#compute derivatives`, `#regulation`, `#CFTC`, `#AI economics`

---

