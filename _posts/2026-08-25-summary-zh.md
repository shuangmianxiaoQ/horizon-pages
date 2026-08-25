---
layout: default
title: "Horizon Summary: 2026-08-25 (ZH)"
date: 2026-08-25
lang: zh
---


> 从 49 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [苹果发布搭载 M5 Max 与 M5 Ultra 的新款 Mac Studio](#item-tech-news-1) ⭐️ 8.0/10
2. [Qwen 3.8-Flash-Next 明日发布：125B MoE 模型](#item-tech-news-2) ⭐️ 8.0/10
3. [苹果发布 M6 与 M5 Ultra：性能与 AI 算力大幅跃升](#item-tech-news-3) ⭐️ 8.0/10
4. [Meta 开源 MetaRoCE：为 AI 以太网打造的全新 RDMA 传输协议](#item-tech-news-4) ⭐️ 8.0/10
5. [英伟达 Vera Rubin NVL72 宣称能效提升 30 倍](#item-tech-news-5) ⭐️ 8.0/10
6. [苹果发布 M6/M5 Pro Mac mini 与 M5 Max/Ultra Mac Studio](#item-tech-news-6) ⭐️ 8.0/10
7. [苹果保留 iCloud+ 隐藏邮件地址于 icloud.com 域名](#item-tech-news-7) ⭐️ 7.0/10
8. [道交法修订草案新增自动驾驶专章并调整电动自行车限速](#item-tech-news-8) ⭐️ 7.0/10
9. [SpaceX 计划 2027 年将英伟达 Vera Rubin NVL72 送入轨道](#item-tech-news-9) ⭐️ 7.0/10
10. [台湾起诉英伟达等员工非法出口 AI 服务器](#item-tech-news-10) ⭐️ 7.0/10
11. [中国黑客利用开源模型提升攻击能力](#item-tech-news-11) ⭐️ 7.0/10
12. [OpenAI 封禁俄秘密散布虚假信息的 ChatGPT 账户](#item-tech-news-12) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [苹果发布搭载 M5 Max 与 M5 Ultra 的新款 Mac Studio](https://www.apple.com/newsroom/2026/08/apple-introduces-new-mac-studio-with-m5-max-and-m5-ultra/) ⭐️ 8.0/10

苹果于 2026 年 8 月发布新款 Mac Studio，搭载 M5 Max 与全新 M5 Ultra 芯片，采用 PCIe Gen 6 存储架构，存储速度提升至上一代的两倍。M5 Ultra 版本支持最高 512GB 统一内存和 1.2TB/s 内存带宽，可完全在设备端运行大型语言模型；四台集群可带来最高 3 倍的分布式 AI 推理速度提升。AI 性能最高提升 4.3 倍，图形性能提升 1.8 倍，并配备 Thunderbolt 5 接口，提供 120Gb/s 的外部 I/O 带宽。新品今日起接受预购，9 月 22 日开售。

hackernews · interpol\_p · 8月25日 13:03 · [社区讨论](https://news.ycombinator.com/item?id=49433316)

**「背景」** Apple 的 M 系列芯片自 2020 年推出以来，一直是 Mac 产品线的核心，其中 M5 系列于 2025 年发布，采用台积电第三代 3 纳米工艺，M5 Pro 和 M5 Max 使用 Fusion Architecture 将两个芯片封装在一起。M5 Ultra 是 M5 系列的最强版本，通过组合两个 M5 Max 芯片实现更高性能，配备最多 36 核 CPU、80 核 GPU 和 32 核神经引擎，支持最高 512GB 统一内存和 1.2TB/s 内存带宽，旨在满足高端 AI 和创意工作负载的需求。

**「影响」** 对于需要本地运行大型 AI 模型或处理高负载创意工作流的专业用户，M5 Ultra 版本提供了前所未有的内存容量和带宽，但 256GB 内存版本售价约 1 万美元，512GB 版本预计价格翻倍且要到 10 月才能交付，可能限制其普及。

**「社区讨论」** 社区对 PCIe Gen 6 存储首次出现在个人电脑上表示兴奋，但担心其散热和热节流问题；同时，有用户因价格过高而考虑用 Mac Studio 替代常驻扩展坞的 MacBook Pro，也有用户对苹果新闻稿中频繁使用“最高达”一词表示不满。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_M5">Apple M5 - Wikipedia</a></li>
<li><a href="https://www.macrumors.com/2026/08/25/apple-debuts-m5-ultra/">Apple Debuts M5 Ultra as Most Powerful Chip Ever - MacRumors</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Mac Studio`, `#M5 chip`, `#PCIe Gen 6`, `#AI hardware`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8-Flash-Next 明日发布：125B MoE 模型](https://modelscope.cn/models/Qwen/Qwen3.8-Flash-Next) ⭐️ 8.0/10

Qwen 团队宣布将于明日（2026 年 8 月 26 日）在魔搭社区发布多模态 MoE 模型 Qwen3.8-Flash-Next，提供标准版与 FP8 两个版本。该模型总参数量为 125B，但仅有 6B 活跃参数，旨在降低推理时的内存带宽需求，使高质量本地 AI 推理在消费级硬件上成为可能。官方表示，此次发布包含架构改进，为即将到来的完整 Qwen4 模型家族做准备。该模型有望在 128GB 内存的 Strix Halo 或 Mac Studio 等设备上以接近可用的速度运行。

hackernews · garo-pro · 8月25日 11:49 · [社区讨论](https://news.ycombinator.com/item?id=49432317)

**「背景」** Qwen 系列是阿里巴巴通义实验室开发的开源大语言模型家族，此前已发布多代版本，包括 Qwen2.5 和 Qwen3 等，广泛应用于本地部署和云端推理。MoE（混合专家）架构是一种通过仅激活部分参数来降低计算成本的技术，例如总参数 125B 但每次仅激活 6B 参数，能在保持模型能力的同时减少推理时的内存带宽需求。此次预告的 Qwen3.8-Flash-Next 基于新一代 Qwen4 架构，是多模态 MoE 模型，预计于 2026 年 8 月 26 日开放下载，将提供标准版与 FP8 两个版本。

**「影响」** 对于拥有 128GB 统一内存设备（如 Strix Halo、Mac Studio）或高内存带宽 GPU 的用户，该模型可能首次提供优于现有 27B 级模型的本地推理体验，并可能推动本地 AI 应用生态发展。

**「社区讨论」** 社区用户普遍期待该模型，认为它终于为 128GB 设备提供了值得使用的本地模型，并可能通过 FreeToken 等推理引擎在 CPU/RAM 与 GPU/VRAM 间优化 MoE 工作负载，从而降低硬件门槛。部分用户对 Qwen 模型在 OpenRouter 上的稳定性表示不满，同时有用户希望 Qwen4 完整系列包含 4B 等更小尺寸的模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://forums.developer.nvidia.com/t/qwen3-8-flash-next/381228">Qwen3.8-Flash-Next - DGX Spark / GB10 - NVIDIA Developer Forums</a></li>
<li><a href="https://x.com/ItsmeAjayKV/status/2092212601459818570">AJ on X: &quot;Model scope has a new countdown started! We will be getting Qwen3.8-flash-next tomorrow 😍!! &quot;Qwen3.8-Flash-Next is a multimodal MoE model built on the next-generation Qwen4 architecture.&quot; I think it&#x27;s the MoE one, prob going to be 70 - 122B range Really stoked now. LFGGGG&quot; / X</a></li>

</ul>
</details>

**标签**: `#Qwen`, `#MoE`, `#Local AI`, `#Model Release`, `#Inference`

---

<a id="item-tech-news-3"></a>
### [苹果发布 M6 与 M5 Ultra：性能与 AI 算力大幅跃升](https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/) ⭐️ 8.0/10

苹果于 2026 年 8 月正式发布 M6 与 M5 Ultra 芯片，主打性能与 AI 算力的显著提升。M6 为苹果首款采用 2 纳米制程的芯片，首发于新款 Mac mini，配备 12 核 CPU、12 核 GPU、双 16 核神经网络引擎，统一内存带宽最高 170GB/s。M5 Ultra 则采用 M 系列首次的四芯片架构，最高可选 36 核 CPU、80 核 GPU 与 512GB 内存，统一内存带宽达 1.2TB/s，较 M3 Ultra 提升 50%，成为苹果迄今最强芯片。定价方面，Mac mini M6 版起售价 6999 元，M5 Pro 版起售价 12999 元；Mac Studio M5 Max 版起售价 19999 元，M5 Ultra 版价格更高。另有传闻称，苹果可能跳过 M6 Pro、M6 Max 与 M6 Ultra，集中资源开发面向 AI 的 M7 芯片。

hackernews · interpol\_p · 8月25日 13:01 · [社区讨论](https://news.ycombinator.com/item?id=49433292)

**「背景」** 苹果的 M 系列芯片自 2020 年推出以来，一直是其 Mac 产品线的核心，每一代都通过制程升级和架构改进来提升性能与能效。M6 是苹果首款采用 2 纳米制程的芯片，配备 12 核 CPU、12 核 GPU 和双 16 核神经网络引擎，统一内存带宽最高 170GB/s；M5 Ultra 则采用 M 系列首次的四芯片架构，最高 36 核 CPU、80 核 GPU，支持最高 512GB 内存，统一内存带宽达 1.2TB/s，比 M3 Ultra 高 50%。这两款芯片分别首发于新款 Mac mini 和 Mac Studio，其中 Mac mini M6 版起售价 6999 元，M5 Pro 版起售价 12999 元，Mac Studio M5 Max 版起售价 19999 元。

**「影响」** 此次发布将直接推动本地 AI 推理和高端计算场景的硬件升级：M5 Ultra 最高支持 512GB 内存和 1.2TB/s 统一内存带宽，使 Mac Studio 成为运行大规模本地模型和 AI 工作负载的更强大平台，但价格也显著提升——M5 Ultra 版 Mac Studio 起售价 5,499 美元，较 M3 Ultra 版贵 200 美元，而顶配（512GB 内存、16TB 存储）预计售价高达 24,699 美元，可能让部分潜在用户转向性价比更高的 M4 Mac mini（16GB 版仅 450 美元）。

**「社区讨论」** 社区对定价反应热烈，有用户计算称，顶配 M5 Ultra Mac Studio（256GB 内存、16TB 存储）售价 18299 美元，若 512GB 内存版本按每 GB 25 美元推算，全配价格可能达 24699 美元，引发对性价比的讨论。也有用户认为，即便价格高企，按通胀调整后仍相当于当年 Mac SE/30 的价位，却换来能轻松通过图灵测试的性能，实属惊人；还有用户称赞 450 美元的 M4 Mac mini 是长期最佳性价比之选。另有评论以“小米宣称追平苹果 CPU 性能，苹果随即发布新芯片”的比喻，调侃苹果的迭代速度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://9to5mac.com/2026/08/25/apple-launches-next-gen-apple-silicon-chips-m6-and-m5-ultra/">Apple launches next-gen Apple Silicon chips: M6 and M5 Ultra</a></li>
<li><a href="https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/">Apple introduces M6 and M5 Ultra for a big leap in ...</a></li>
<li><a href="https://www.forbes.com/sites/davidphelan/2026/08/25/apple-surprise-launches-new-mac-mini-mac-studio-m6-and-m5-ultra-chips-unexpectedly/">Apple Launches New Mac mini, Mac Studio, M6 And M5 Ultra ...</a></li>
<li><a href="https://www.forbes.com/sites/davidphelan/2026/08/25/apple-surprise-launches-new-mac-mini-mac-studio-m6-and-m5-ultra-chips-unexpectedly/">Apple Launches New Mac mini, Mac Studio, M6 And M5 Ultra Chips Unexpectedly</a></li>
<li><a href="https://www.engadget.com/2243379/apple-mac-mini-m6-mac-studio-m5-max/">Apple refreshes Mac mini and Mac Studio with new M6 and M5 Ultra chips - Engadget</a></li>
<li><a href="https://appleinsider.com/articles/26/08/25/mac-studio-gets-update-to-m5-max-and-m5-ultra">Mac Studio gets update to M5 Max and M5 Ultra</a></li>

</ul>
</details>

**标签**: `#apple-silicon`, `#ai-compute`, `#hardware`, `#performance`, `#mac-studio`

---

<a id="item-tech-news-4"></a>
### [Meta 开源 MetaRoCE：为 AI 以太网打造的全新 RDMA 传输协议](https://aihot.virxact.com/items/cmt7nq1d02bs1ro7373u88po4) ⭐️ 8.0/10

Meta 设计并开源了 MetaRoCE，一个专为 AI 工作负载在通用以太网上打造的 RDMA 传输协议，已通过 Open Compute Project（OCP）发布规范、参考软件实现和合规测试套件。该协议将智能移至端点，原生支持乱序交付、多路径、无损容忍和双向拥塞控制，无需 PFC，可在百万 GPU 规模下提供高吞吐、低尾延迟。现有 RDMA Verbs API 和软件栈无需修改即可运行。

rss · AI HOT 精选 · 8月24日 18:02

**「背景」** RDMA（远程直接内存访问）是一种允许网卡直接读写远端内存的技术，常用于高性能计算和 AI 集群以降低延迟。传统 RoCE（基于以太网的 RDMA）依赖 PFC（优先级流控）来避免丢包，并要求数据包按序到达，这在大规模 AI 网络中会导致拥塞扩散和性能瓶颈。MetaRoCE 是 Meta 设计的一种全新 RDMA 传输协议，专为 AI 工作负载在通用以太网上运行而优化，通过将智能移至端点，支持乱序交付、多路径和双向拥塞控制，从而无需 PFC 即可实现高吞吐和低尾延迟。

**「影响」** 对于依赖 RoCE 进行 AI 网络通信的开发者与运维者，MetaRoCE 消除了对 PFC 的依赖并支持乱序交付，有望降低大规模集群的配置复杂度和性能瓶颈，同时保持现有 RDMA 软件栈的兼容性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://engineering.fb.com/2026/08/24/networking-traffic/metaroce-rdma-transport-ai-ethernet/">MetaRoCE : A New RDMA Transport Built for AI-Scale Ethernet</a></li>
<li><a href="https://www.opensourceforu.com/2026/08/metaroce-opens-rdma-transport-for-ai-ethernet/">MetaRoCE Opens RDMA Transport for AI Ethernet - Open Source...</a></li>

</ul>
</details>

**标签**: `#RDMA`, `#AI networking`, `#Ethernet`, `#Meta`, `#Open Compute Project`

---

<a id="item-tech-news-5"></a>
### [英伟达 Vera Rubin NVL72 宣称能效提升 30 倍](https://aihot.virxact.com/items/cmt7e0g7y232wro738qg82x67) ⭐️ 8.0/10

英伟达首次公布下一代机柜 Vera Rubin NVL72 的实测数据，宣称在 AI 智能体工作负载下，其每兆瓦吞吐量较上一代 GB300 NVL72 最高提升 30 倍，每百万 token 成本最高降低 35 倍。测试使用 DeepSeek-V4-Pro 模型执行智能体编码任务，并同期发布了智能体专用 Vera CPU 及量产推理加速芯片 Groq 3 LPX（运行 Gemma 4 31B 时输出速度达 3400 token/秒）。这些数据来自英伟达官方博客，尚未经独立验证。马斯克的 SpaceXAI 已宣布部署 Vera CPU，并计划于 2028 年将优化版机柜送入太空。

rss · AI HOT 精选 · 8月24日 15:00

**「背景」** Vera Rubin 是英伟达下一代 AI 加速器平台，采用 Vera CPU 与 Rubin GPU 的协同设计，NVL72 指单机柜集成 72 颗 GPU 的高密度配置。其前代 GB300 NVL72 基于 Blackwell 架构，是当前数据中心 AI 推理与训练的主流机柜方案。英伟达此次公布的“每兆瓦吞吐量”和“每百万 token 成本”是衡量 AI 基础设施能效与经济性的关键指标，直接反映大规模部署时的运营成本与算力产出。

**「影响」** 若英伟达的实测数据属实，Vera Rubin NVL72 将显著降低 AI 智能体推理的能耗和成本，可能推动数据中心加速采用该平台，并加剧与 AMD、英特尔等竞争对手在 AI 基础设施领域的竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/nvidia-vera-rubin-and-blackwell-set-a-new-standard-for-agentic-ai-performance-per-watt/">NVIDIA Vera Rubin and Blackwell Set a New Standard for ...</a></li>
<li><a href="https://blogs.nvidia.com/blog/vera-rubin-nvl72-efficiency-ai-agents/">NVIDIA Vera Rubin NVL72 Sets a New Efficiency Standard for AI ...</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#AI hardware`, `#data center`, `#AI agents`, `#performance`

---

<a id="item-tech-news-6"></a>
### [苹果发布 M6/M5 Pro Mac mini 与 M5 Max/Ultra Mac Studio](https://api3.cls.cn/share/article/2463992?&amp;amp;sv=8.5.9&amp;amp;) ⭐️ 8.0/10

苹果公司发布了新款 Mac mini，搭载 M6 和 M5 Pro 芯片，并宣称这是全球首款采用 2 纳米制程的电脑，AI 算力大幅提升。其中，搭载 M6 芯片的 Mac mini 在美国起售价为 899 美元，教育优惠价为 799 美元。同时，苹果还推出了搭载 M5 Max 和 M5 Ultra 芯片的新款 Mac Studio，并称这两款芯片是“苹果迄今最强大的芯片”。新款 Mac Studio 即日起接受预购，将于 9 月 22 日在门店正式开售。此次发布标志着苹果在 2 纳米芯片技术上取得领先，对 AI 计算和整个科技行业具有重要影响。

telegram · xhqcankao · 8月25日 13:16

**「背景」** 苹果公司于 2026 年 8 月 25 日发布了新款 Mac mini，搭载 M6 和 M5 Pro 芯片，其中 M6 芯片采用 2 纳米制程，是苹果首款 2 纳米芯片，也是全球首款 2 纳米电脑。同时推出的还有搭载 M5 Max 和 M5 Ultra 芯片的新款 Mac Studio，苹果称这两款芯片是“迄今最强大的芯片”。新款 Mac Studio 即日起接受预购，将于 9 月 22 日在门店开售。

**「影响」** 对于专业用户、开发者和 AI 研究人员，新款 Mac mini 和 Mac Studio 将提供更强的本地 AI 计算能力，可能加速端侧 AI 应用开发；同时，2 纳米制程的率先商用可能推动整个 PC 行业向更先进制程过渡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/08/apple-unveils-a-more-powerful-mac-mini-featuring-the-all-new-m6-and-m5-pro/">Apple’s new Mac mini, featuring M6 and M5 Pro, delivers a ...</a></li>
<li><a href="https://www.forbes.com/sites/davidphelan/2026/08/25/apple-surprise-launches-new-mac-mini-mac-studio-m6-and-m5-ultra-chips-unexpectedly/">Apple Launches New Mac mini, Mac Studio, M6 And M5 Ultra ...</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Mac mini`, `#M6 chip`, `#2nm process`, `#AI hardware`

---

<a id="item-tech-news-7"></a>
### [苹果保留 iCloud+ 隐藏邮件地址于 icloud.com 域名](https://developer.apple.com/news/?id=1ptvdtcm) ⭐️ 7.0/10

苹果宣布 iCloud+ 的“隐藏邮件地址”功能将继续使用 icloud.com 域名，确保现有用户的地址保持可用，避免服务中断。这一决定回应了用户对隐私邮件中继服务可能被屏蔽的担忧，并维持了与普通 iCloud 邮件地址一致的格式。苹果未改变该功能的运作方式，但明确排除了迁移到其他域名的可能性。此举对依赖该功能保护隐私的现有用户是积极信号，但并未引入新功能或改变定价。

hackernews · K7PJP · 8月24日 22:13 · [社区讨论](https://news.ycombinator.com/item?id=49426564)

**「背景」** iCloud+ 的“隐藏邮件地址”是苹果提供的隐私保护功能，允许用户生成随机地址以转发邮件到真实收件箱，避免暴露个人邮箱。此前有猜测认为苹果可能将此类地址迁移到其他域名，但此次公告确认其继续使用 icloud.com。该功能与“通过 Apple 登录”等隐私工具相关，是苹果生态内保护用户身份的重要机制。

**「影响」** 现有 iCloud+ 用户无需更改任何设置或地址，其隐藏邮件地址将继续正常工作，避免了因域名变更可能导致的邮件丢失或服务中断。这一决定也降低了第三方服务因识别中继域名而屏蔽邮件的风险，但用户仍可能面临与苹果生态绑定的长期限制。

**「社区讨论」** 社区普遍认为这是正确决策，因为私有邮件中继常被屏蔽，而使用 icloud.com 域名有助于提高送达率，但部分评论指出这加剧了用户对苹果的锁定。有用户提到，如果拥有自定义域名，可以自行创建任意地址，但自动检测仍可能暴露身份。

**标签**: `#Apple`, `#iCloud+`, `#privacy`, `#email`, `#product-update`

---

<a id="item-tech-news-8"></a>
### [道交法修订草案新增自动驾驶专章并调整电动自行车限速](https://m.weibo.cn/status/ReZGreh0P?jumpfrom=weibocom) ⭐️ 7.0/10

十四届全国人大常委会会议今日初次审议道路交通安全法修订草案。草案新增自动驾驶汽车专章，明确自动驾驶汽车在功能激活状态下发生交通违法时，由生产企业或进口企业接受处理；未激活或仅具备辅助驾驶功能的车辆按非自动驾驶汽车管理。草案还针对“盲驾”等妨碍安全驾驶行为，规定造成事故或严重后果的处 200 元以上 500 元以下罚款，可并处暂扣三个月驾驶证；未经许可不得占用道路从事非交通活动，以治理“暴走团”等问题。电动自行车在非机动车道内行驶的最高时速限制从 15 公里调整为 20 公里，并明确禁止逆向行驶、超速、违反交通信号及手持电话、观看视频等行为。此次修订聚焦醉驾、盲驾、僵尸车、超标车及电动自行车管理等突出问题，旨在完善道路交通安全制度。

telegram · zaihuapd · 8月25日 03:03

**「背景」** 中国现行《道路交通安全法》自 2004 年施行，此前多次修订均未系统涉及自动驾驶汽车。随着智能网联汽车试点上路（2023 年 11 月启动）及国家计划于 2025 年实现智能驾驶汽车规模化生产，事故责任认定与承担问题亟待法律明确。此次修订草案在既有试点要求（如 L3/L4 级车辆投保不低于 500 万元责任险、建立 EDR 数据锁存机制）基础上，首次以专章形式对自动驾驶汽车的上路条件、违章处理原则和保险制度作出规定。

**「影响」** 对自动驾驶汽车生产企业和进口企业而言，草案明确了其在自动驾驶模式下的违法处理责任，将直接影响产品责任划分与合规设计；对电动自行车使用者，限速上调至 20 公里/小时，但新增的禁止行为可能增加违规处罚风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.mydrivers.com/newsview/1146268.html">m.mydrivers.com/newsview/1146268.html</a></li>
<li><a href="https://huluic.cn/article/g1i7c0c9g8i204366.html">两会提 案 ，“ 自 动 驾 驶 ”又有新方向了？ | Hulu AI平台</a></li>
<li><a href="https://m.dzplus.dzng.com/share/general/0/NEWS2995064FWVVZSQKVXYYK">m.dzplus.dzng.com/share/general/0/NEWS2995064FWVVZSQKVXYYK</a></li>

</ul>
</details>

**标签**: `#autonomous vehicles`, `#regulation`, `#China`, `#road safety`, `#AI policy`

---

<a id="item-tech-news-9"></a>
### [SpaceX 计划 2027 年将英伟达 Vera Rubin NVL72 送入轨道](https://www.theregister.com/off-prem/2026/08/25/spacex-claims-it-will-put-a-vera-rubin-nvl72-rack-scale-system-into-orbit-next-year/5292067) ⭐️ 7.0/10

SpaceX 计划在 2027 年将一套英伟达 Vera Rubin NVL72 机架级 AI 系统送入轨道，以验证太空数据中心相关技术。NVL72 由 72 颗 Rubin GPU 和 36 颗 Vera CPU 组成，整套系统功耗超过 100 千瓦，通常需要复杂的液冷和供电设施。将这类设备部署到太空，还需解决供电、散热、辐射防护和通信等问题。SpaceX 尚未公布具体发射时间、轨道高度及系统在太空中的供电和冷却方案。此外，SpaceX CEO 埃隆·马斯克在 X 平台表示，首批搭载英伟达芯片的 AI 卫星将于明年第四季度发射，并计划在 2028 年达到“可观规模”。

telegram · zaihuapd · 8月25日 08:03

**「背景」** Vera Rubin NVL72 是英伟达计划推出的机架级 AI 系统，由 72 颗 Rubin GPU 和 36 颗 Vera CPU 组成，整机功耗超过 100 千瓦，通常依赖液冷和专用供电设施。SpaceX 此前已提出太空数据中心构想，计划通过由 AI 卫星组成的网络在轨道上直接进行计算，作为地面数据中心的替代方案。此次宣布的发射计划是这一构想的具体推进，但相关技术细节尚未披露。

**「影响」** 若计划成功，这将为太空数据中心和轨道 AI 计算奠定技术基础，可能为地面数据中心提供成本更低、更环保的替代方案，并推动太空计算基础设施的发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://enterpriseai.economictimes.indiatimes.com/news/industry/spacex-nvidia-develop-space-optimised-ai-system-for-orbital-launch-next-year/133501818">SpaceX, Nvidia develop space-optimised AI system for orbital launch next year, ETEnterpriseai</a></li>
<li><a href="https://aninews.in/news/business/spacex-nvidia-develop-space-optimized-ai-system-for-orbital-launch-next-year-elon-musk20260825081524/">SpaceX, Nvidia develop space-optimized AI system for orbital launch next year: Elon Musk</a></li>
<li><a href="https://www.thehindubusinessline.com/news/science/spacex-nvidia-develop-space-optimised-ai-system-for-orbital-launch-next-year-elon-musk/article71387191.ece">SpaceX, Nvidia develop space-optimised AI system for orbital launch next year: Elon Musk - The HinduBusinessLine</a></li>

</ul>
</details>

**标签**: `#space computing`, `#AI infrastructure`, `#Nvidia`, `#SpaceX`, `#data centers`

---

<a id="item-tech-news-10"></a>
### [台湾起诉英伟达等员工非法出口 AI 服务器](http://cn.nikkei.com/politicsaeconomy/politicsasociety/63748-2026-08-25-08-56-53.html) ⭐️ 7.0/10

台湾基隆地方检察署于 8 月 24 日宣布，对九名涉嫌向中国大陆非法出口 AI 服务器的人员提起公诉，其中包括美国英伟达和超微电脑的在台员工。涉案服务器搭载英伟达 B300 芯片，属于高性能 AI 硬件，被禁止转售至中国大陆。检方指控被告通过伪造用户信息、谎称服务器由台湾企业在台安装等方式规避出口管制，并发现部分货物经由日本中转。九人因涉嫌渎职、伪造文件等罪名被起诉，除两家公司员工外，还包括台湾销售代理商和数据中心运营商相关人员。此案凸显了台湾地区对 AI 芯片出口限制的执行力度，可能对 AI 硬件供应链和跨国科技企业的合规操作产生广泛影响。

telegram · xhqcankao · 8月25日 02:03

**「背景」** 美国对华出口管制政策限制向中国大陆出口先进 AI 芯片及搭载此类芯片的服务器，英伟达 B300 芯片属于受管制的高性能 GPU。台湾基隆地方检察署此次起诉九人，包括英伟达和超微电脑的在台员工，指控他们通过伪造用户信息、谎称服务器由台湾企业安装于台湾域内等手段，将搭载 B300 芯片的服务器非法出口至中国大陆，其中部分货物经由日本中转。

**「影响」** 该案对英伟达和超微电脑的在台业务及员工合规行为构成直接法律风险，可能促使相关企业加强出口管制审查，并影响中国大陆获取高端 AI 芯片的渠道。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techtimes.com/articles/325419/20260825/nvidia-manager-unlocked-b300-server-diversion-china-taiwan-indictment-says.htm">Nvidia Manager Unlocked B300 Server Diversion To China ...</a></li>
<li><a href="https://www.yahoo.com/news/world/articles/nine-indicted-taiwan-over-illegal-150955022.html?fr=sycsrp_catchall">Nine indicted by Taiwan over illegal export of Nvidia B300 ...</a></li>
<li><a href="https://www.sofx.com/taiwan-charges-nvidia-manager-in-first-criminal-ai-chip-smuggling-case/">Taiwan Charges Nvidia Manager in First Criminal AI Chip ...</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#export controls`, `#NVIDIA`, `#supply chain`, `#geopolitics`

---

<a id="item-tech-news-11"></a>
### [中国黑客利用开源模型提升攻击能力](https://www.bloomberg.com/news/articles/2026-08-24/chinese-hackers-use-deepseek-to-boost-attacks-researchers-say-mt7o4205) ⭐️ 7.0/10

彭博社报道称，中国黑客在将 DeepSeek 等开源 AI 模型整合到其行动中后，攻击能力显著增强。据台湾研究机构 TeamT5 称，与国家相关的网络组织自开始将日常任务委托给 AI 并利用其开发高级恶意软件以来，发起的攻击数量增加了一倍以上。研究人员表示，虽然并非总能确定黑客使用的是哪种 AI 模型，但 DeepSeek 的产品因其高性能和可定制能力而颇受欢迎。黑客被 DeepSeek 相对宽松的网络安全防护壁垒和较低的运行成本所吸引，尽管中国生产的其他模型可能更为强大。这一趋势凸显了攻击者利用基础 AI 工具打击海外目标的能力。

telegram · xhqcankao · 8月25日 04:03

**「背景」** DeepSeek 是中国人工智能公司深度求索开发的开源大语言模型，因其高性能和低成本而受到全球开发者关注。开源模型允许用户自由下载、修改和部署，但也意味着安全防护措施可能不如商业闭源模型严格。TeamT5 是一家总部位于台湾的网络安全研究机构，长期追踪与中国相关的网络攻击活动。

**「影响」** 对于依赖开源 AI 模型的组织和网络安全团队而言，这一趋势意味着攻击者可能以更低成本和更高效率发起攻击，从而加剧对海外目标的威胁，并促使相关方重新评估开源模型的安全防护机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/teamt5-ties-doubled-chinese-state-hacker-attacks-to-deepseek">TeamT5 ties doubled Chinese state hacker attacks to DeepSeek</a></li>

</ul>
</details>

**标签**: `#AI安全`, `#开源模型`, `#网络攻击`, `#DeepSeek`, `#威胁情报`

---

<a id="item-tech-news-12"></a>
### [OpenAI 封禁俄秘密散布虚假信息的 ChatGPT 账户](https://www.cnbc.com/2026/08/25/openai-russia-chatgpt-influence-campaign.html) ⭐️ 7.0/10

OpenAI 在周二发布的一篇博客文章中宣布，已封禁一批源自俄罗斯的 ChatGPT 账户，这些账户被用于支持一项秘密的网络影响力活动，以传播虚假信息。该公司在调查人工智能生成的社交媒体帖子时发现了这一问题，并追踪到一个更广泛的行动，该行动围绕一个网站展开，该网站包含抄袭和错误归属的学术作品、一个将俄罗斯描绘成有利形象的“主权”指数，以及掩盖运营者俄罗斯背景的种种努力。尽管 OpenAI 不允许在俄罗斯访问其模型，但该公司表示，相关行为者使用 VPN 来伪装位置，从而规避了访问限制。这是亲俄罗斯行为者利用人工智能传播虚假信息的最新事件，凸显了 AI 技术被滥用于影响力行动的风险。

telegram · xhqcankao · 8月25日 11:49

**「背景」** OpenAI 长期禁止俄罗斯用户访问其模型，但攻击者常通过 VPN 伪装位置以绕过限制。此次封禁的账户被用于推广一个伪装成以色列智库的虚假网站，该网站包含抄袭的学术文章和一个将俄罗斯描绘为正面形象的“主权”指数，旨在掩盖运营者的俄罗斯背景。

**「影响」** 这一行动表明，OpenAI 正在积极监控和打击其平台上的 AI 滥用行为，但 VPN 等规避手段的存在意味着此类活动可能难以完全根除，对平台治理和 AI 安全提出了持续挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/disrupting-malicious-uses-of-ai-influence-campaign-russia/">Disrupting a new covert influence campaign from Russia | OpenAI</a></li>
<li><a href="https://qz.com/openai-banned-russian-chatgpt-accounts-influence-campaign-082526">OpenAI bans Russian ChatGPT accounts in influence campaign</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#disinformation`, `#OpenAI`, `#cybersecurity`, `#platform governance`

---

