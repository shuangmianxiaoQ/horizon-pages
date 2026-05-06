---
layout: default
title: "Horizon Summary: 2026-05-06 (ZH)"
date: 2026-05-06
lang: zh
---

> From 18 items, 12 important content pieces were selected

---

1. [Micron 开始出货 245TB 6600 ION SSD](#item-1) ⭐️ 8.0/10
2. [DENIC 的 .de 域名 DNSSEC 故障已解决](#item-2) ⭐️ 8.0/10
3. [Gemma 4 用多 token 起草器加速](#item-3) ⭐️ 8.0/10
4. [GUI 电脑操作比 API 贵得多](#item-4) ⭐️ 8.0/10
5. [Cloudflare 允许代理创建账户、购买域名并部署](#item-5) ⭐️ 7.0/10
6. [逆向还原 1998 年《Ultima Online》试玩服务器](#item-6) ⭐️ 7.0/10
7. [AI 垃圾内容进入编织圈](#item-7) ⭐️ 7.0/10
8. [YouTube 的 RSS 订阅失灵了](#item-8) ⭐️ 7.0/10
9. [开源还是收费软件](#item-9) ⭐️ 7.0/10
10. [Willison 称两者正在融合](#item-10) ⭐️ 7.0/10
11. [StarFighter 16 英寸笔记本发布](#item-11) ⭐️ 6.0/10
12. [Andon Labs 在斯德哥尔摩开设 AI 咖啡馆](#item-12) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Micron 开始出货 245TB 6600 ION SSD](https://investors.micron.com/news-releases/news-release-details/industry-leading-245tb-micron-6600-ion-data-center-ssd-now) ⭐️ 8.0/10

Micron 已开始出货 245TB 规格的 6600 ION NVMe SSD，同时该系列还提供 122TB 版本。该公司将这款产品定位于 AI、云、企业和超大规模数据中心负载。 这对数据中心存储密度来说是一个重要里程碑，因为单个 SSD 现在几乎可以容纳四分之一个 PB。对于超大规模运营商来说，这有助于减少机架数量并提升每机架容量，从而改善空间、电力和部署效率。 Micron 表示，6600 ION 是其目前商用容量最高的 SSD，产品页将其列为数据中心 NVMe 硬盘。行业报道指出，它相较传统 HDD 机架方案可实现最高 6.8 倍的每机架容量，但代价是这种超高密度闪存盘的写入性能可能明显低于读取性能。

hackernews · neilfrndes · May 6, 03:37 · [社区讨论](https://news.ycombinator.com/item?id=48031867)

**背景**: NVMe 是一种为闪存和低延迟访问设计的存储接口，因此常见于现代 SSD。超大规模数据中心是为运行和扩展成千上万台服务器而建设的大型云设施，通常更重视密度、效率和可管理性，而不是面向消费级的性能体验。像这类高容量企业 SSD，通常用于替代或补充基于 HDD 的存储层。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.micron.com/products/storage/ssd/data-center-ssd/6600-ion">Micron 6600 ION NVMe SSD | 245TB & 122TB</a></li>
<li><a href="https://www.blocksandfiles.com/flash/2026/05/05/microns-new-ssd-replaces-disk-for-fast-access-storage/5219265">Micron's new SSD replaces disk for fast access storage</a></li>
<li><a href="https://www.cisco.com/site/us/en/learn/topics/computing/what-is-a-hyperscale-data-center.html">What is a hyperscale data center? - Cisco</a></li>

</ul>
</details>

**社区讨论**: 讨论整体上对容量突破感到兴奋，但很多评论把焦点放在企业级与消费级存储趋势的落差上。一些人感叹消费级 SSD 价格上涨，以及缺少价格可接受的 16TB 到 32TB 便携 SSD；另一些人则质疑 6600 ION 的写入速度偏低，并对这种高密度盘的散热问题表示担忧。

**标签**: `#storage`, `#SSD`, `#data centers`, `#enterprise hardware`, `#Micron`

---

<a id="item-2"></a>
## [DENIC 的 .de 域名 DNSSEC 故障已解决](https://status.denic.de/pages/incident/592577eab611ce1e0d00046f/69fa60ef9d12f5057a974f38) ⭐️ 8.0/10

DENIC 报告并已解决一起与 DNSSEC 相关的故障，该故障导致 .de 域名出现验证失败。在故障期间，即使底层区域数据仍然存在，支持验证的递归解析器也可能对 .de 查询返回 SERVFAIL。 由于 DENIC 运营着德国的 .de 国家顶级域，这起事件可能一次性影响大量域名。它也说明，即使权威 DNS 服务器仍在正常响应，DNSSEC 签名或验证问题也会让用户的解析直接失效。 社区排查指向一个畸形的 DNSSEC 签名，可能是覆盖 NSEC3 记录的 RRSIG 出了问题，而不是普通的 nameserver 故障。`dig +cd` 可以正常工作而普通的验证查询失败，这是一个典型信号，说明权威数据可达，但递归解析器无法完成验证。

hackernews · warpspin · May 5, 20:16 · [社区讨论](https://news.ycombinator.com/item?id=48027897)

**背景**: DNSSEC 会给 DNS 数据添加数字签名，让解析器能够验证响应是否真实且未被篡改。如果签名或信任链断裂，支持验证的解析器即使能连到 DNS 服务器，也可能直接以 SERVFAIL 拒绝回答。DENIC 是所有 .de 域名的注册局，因此那里发生的 DNSSEC 问题会影响一个重要的国家顶级域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.cloudflare.com/dns/dnssec/troubleshooting/">Troubleshooting DNSSEC · Cloudflare DNS docs</a></li>
<li><a href="https://www.denic.de/en/">DENIC eG: DENIC – Registry for all .de domains</a></li>

</ul>
</details>

**社区讨论**: 评论者很快一致认为这是 DNSSEC 验证失败，而不是 nameserver 故障，并指出使用 `+cd` 的直接查询仍然可用。还有人提到了解析器侧的临时缓解措施，例如 Cloudflare 曾在 1.1.1.1 上暂时关闭 DNSSEC 验证，讨论里也夹杂了一些轻松的调侃。

**标签**: `#DNSSEC`, `#DNS`, `#incident response`, `#domain names`, `#internet infrastructure`

---

<a id="item-3"></a>
## [Gemma 4 用多 token 起草器加速](https://blog.google/innovation-and-ai/technology/developers-tools/multi-token-prediction-gemma-4/) ⭐️ 8.0/10

Google 宣布，Gemma 4 可以通过多 token 预测（MTP）起草器获得更快的推理速度。其目标是在尽量不影响质量的前提下更快地产生文本。 推理延迟是大模型部署中最重要的成本之一，尤其是在本地和自托管场景里。若 Gemma 4 能在保持大部分质量的同时更快生成 token，就会更适合交互式产品和较小的 GPU 环境。 这项技术与投机解码密切相关：先由起草器提出候选 token，再由主模型进行验证。它的关键权衡在于，速度提升取决于起草 token 的接受率，因此实际收益会随提示词和负载而变化。

hackernews · amrrs · May 5, 16:14 · [社区讨论](https://news.ycombinator.com/item?id=48024540)

**背景**: 大多数 LLM 都是一次生成一个 token，因此即使模型本身很高效，解码过程仍然会成为瓶颈。多 token 预测是一条研究路线，它让模型一次预测多个未来 token，从而提升样本效率并支持更快的推理。投机解码则建立在这一思路之上，先用更便宜的起草模型提出候选，再由更大的模型并行校验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2404.19737">[2404.19737] Better & Faster Large Language Models via Multi-token Prediction</a></li>
<li><a href="https://research.google/blog/looking-back-at-speculative-decoding/">Looking back at speculative decoding</a></li>

</ul>
</details>

**社区讨论**: 评论者整体上对投机解码和 MTP 持积极态度，认为这是在几乎不损失质量的情况下提升生成速度的聪明方法。也有人表示，这类进展对本地和自托管推理尤其令人兴奋，但较大的 Gemma 4 版本在有限显存中的部署仍然有挑战。

**标签**: `#LLM inference`, `#speculative decoding`, `#Gemma`, `#Google AI`, `#open-source models`

---

<a id="item-4"></a>
## [GUI 电脑操作比 API 贵得多](https://reflex.dev/blog/computer-use-is-45x-more-expensive-than-structured-apis/) ⭐️ 8.0/10

一篇新文章认为，依赖计算机视觉和直接图形界面交互的 AI 代理，成本大约是使用结构化 API 的 45 倍。文章的核心观点是：只要软件系统能够提供明确的操作接口，“computer use” 就不应该成为默认方案。 这很重要，因为代理的设计选择会直接影响成本、可靠性和可扩展性，尤其会影响产品团队和自动化工作流。如果这种 45 倍的差距在实践中成立，那么 API、CLI 工具、MCP 式接口和基于可访问性的集成，会明显优于脆弱的界面自动化。 这篇文章的批评与 Anthropic 对 computer use 的描述相符：模型通过截图以及鼠标、键盘控制与计算机交互，这种方式比调用结构化端点更依赖状态。正是这种额外的感知与导航循环，使得图形界面自动化比直接 API 调用更慢、更脆弱，也更昂贵。

hackernews · palashawas · May 5, 16:34 · [社区讨论](https://news.ycombinator.com/item?id=48024859)

**背景**: Anthropic 的 computer use 功能允许 Claude 通过查看截图并发出鼠标和键盘操作来与桌面环境交互。与之相比，结构化 API 会直接暴露命名好的操作和数据，因此代理可以跳过图形界面所需的视觉解析和逐步导航。这个领域的争论在于：当许多工作流都可以通过明确接口以更低成本、更高可靠性实现时，通用的 computer use 是否真的值得。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/3-5-models-and-computer-use">Introducing computer use, a new Claude 3.5 Sonnet, and Claude ...</a></li>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/computer-use-tool">Computer use tool - Claude API Docs</a></li>

</ul>
</details>

**社区讨论**: 评论区整体对把图形界面自动化作为首选方案持怀疑态度，几位评论者认为它应该是“最后手段”，并更倾向于 CLI、MCP、REST 或可访问性 API。还有人指出，很多企业应用本来就会刻意让界面自动化变得困难；另一些讨论则在探讨是否可以先让代理“映射”界面，再把它整理成更像 API 的接口。

**标签**: `#AI agents`, `#APIs`, `#GUI automation`, `#software architecture`, `#accessibility`

---

<a id="item-5"></a>
## [Cloudflare 允许代理创建账户、购买域名并部署](https://blog.cloudflare.com/agents-stripe-projects/) ⭐️ 7.0/10

Cloudflare 宣布，代理现在可以创建 Cloudflare 账户、购买域名并完成部署等端到端流程。这个更新旨在让 AI 代理从规划直接走到上线运行，减少人工介入。 这让 AI 代理更接近“全栈操作员”，不再只是聊天工具，而是能接触真实基础设施和交易流程。它可能加快网站上线和自动化，但也会放大欺诈、滥用和账户安全方面的风险。 Cloudflare Registrar 早已提供按成本价的域名注册和续费，没有额外附加费；Cloudflare Workers 则可以把无服务器应用全球部署到 330 多个数据中心。实际效果是，代理现在可以在同一平台上串联起账户注册、域名购买和应用部署。

hackernews · rolph · May 6, 03:10 · [社区讨论](https://news.ycombinator.com/item?id=48031684)

**背景**: Cloudflare 是一家提供域名、DNS、安全和边缘计算等服务的基础设施公司。域名注册商负责购买和续费域名，而像 Workers 这样的平台可以在不管理服务器的情况下部署代码。AI 代理是可以代表用户执行操作的软件系统，因此让它们接入这些服务会让它们更自主。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cloudflare.com/products/registrar/">Cloudflare Registrar | Domain Registration & Renewal | Cloudflare</a></li>
<li><a href="https://www.cloudflare.com/developer-platform/products/workers/">Cloudflare Workers | Build and deploy code with Easy-to Use Developer Tools | Cloudflare</a></li>

</ul>
</details>

**社区讨论**: 讨论整体偏怀疑：不少评论者认为这个功能像个玩具，缺少清晰的日常应用场景。另一些人警告说，让代理能够买域名和部署站点，可能会被用于欺诈、钓鱼和快速生成一次性网站；还有评论者提到，Cloudflare 过去曾因验证问题停过真人账户，形成了讽刺对比。

**标签**: `#AI agents`, `#Cloudflare`, `#web automation`, `#infrastructure`, `#security`

---

<a id="item-6"></a>
## [逆向还原 1998 年《Ultima Online》试玩服务器](https://draxinar.github.io/articles/2026-05-01-uodemo-reverse-engineering.html) ⭐️ 7.0/10

一篇详细的技术文章和代码仓库重建了 1998 年的《Ultima Online》试玩服务器，作者表示这项工作经历了 10 年的断续推进才最终完成。随附的 OUO 仓库展示了对《Ultima Online: The Second Age》试玩版中服务器的逆向工程，而作者还提到，近期 LLM 的进展帮助他完成了这项反编译工作。 这是一项重要的游戏保存考古工作，因为它有助于还原早期 MMO 服务器的行为方式，从而支持模拟器、历史研究和玩家自发的保存项目。它也反映出逆向工程领域的一个更大趋势：LLM 正开始加速长期的反编译和二进制分析任务。 这个项目聚焦的是随《Ultima Online: The Second Age》试玩版发布的服务器，而不是完整的商业在线服务。之所以重要，是因为精确重建服务器通常依赖原始数据文件和协议细节；社区讨论里甚至提到 dynamic0.mul、regions.txt 和 resbank.mul 这类旧文件仍然是很有价值的材料。

hackernews · notsentient · May 6, 06:31 · [社区讨论](https://news.ycombinator.com/item?id=48032976)

**背景**: 《Ultima Online》是经典的网络角色扮演游戏之一，其服务器端行为一直受到保存者和模拟器作者的关注。在这个语境下，逆向工程指的是分析二进制文件、数据格式和网络行为，以重建兼容的服务器或理解原始实现。这个试玩版本身是一个可离线游玩的游戏片段，粉丝社区多年来一直在研究它。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://draxinar.github.io/articles/2026-05-01-uodemo-reverse-engineering.html">Reverse-engineering the 1998 Ultima Online demo server - Draxinar</a></li>
<li><a href="https://github.com/draxinar/ouo">GitHub - draxinar/ouo: OUO: reverse engineering of Ultima Online: The Second Age server · GitHub</a></li>
<li><a href="http://uodemo.uo98.org/index.php?title=Main_Page">UO Demo - UODemo Wiki</a></li>

</ul>
</details>

**社区讨论**: 评论区整体情绪非常积极且充满怀旧感：有几位网友分享了自己搭建 UO shard 的经历，或者表示正是这款游戏让他们对网络编程和 MMO 模拟产生了兴趣。讨论里也出现了关于 radare2、Ghidra 和 IDA Pro 的工具选择话题，同时大家对作者提到“LLM 终于让一个持续十年的反编译任务变得可完成”表现出明显的兴趣和认同。

**标签**: `#reverse engineering`, `#game preservation`, `#binary analysis`, `#Ultima Online`, `#LLMs`

---

<a id="item-7"></a>
## [AI 垃圾内容进入编织圈](https://katedaviesdesigns.com/2026/04/29/knitting-bullshit/) ⭐️ 7.0/10

Kate Davies 发表了一篇题为《Knitting bullshit》的文章，讨论 AI 生成的低质量内容如何在编织相关的网络空间中扩散。她以编织圈为案例，说明合成媒体和内容农场式运作正在改变小众社区。 这篇文章说明，AI 生成垃圾内容不只是泛网络问题，它同样会侵蚀小众爱好社区中的信任和真实性。讨论还指向更广泛的激励机制，例如 SEO 操纵、广告欺诈和其他变现手段，可能正是这类内容的驱动力。 这篇文章把 AI 生成的“胡扯”描述为一种低质量合成媒体，它可能通过搜索结果、信息流和社区空间大量涌入，内容看似合理却缺乏价值。文章之所以特别，是因为它把编织视为一种严肃、真实的生活社区，而不只是一个无关紧要的爱好，因此真实性的流失显得更有分量。

hackernews · ColinEberhardt · May 6, 05:13 · [社区讨论](https://news.ycombinator.com/item?id=48032461)

**背景**: AI 生成内容是指由模型而不是人类作者生成的文字或媒体。内容农场是指为了获取流量而批量生产材料的网站或运营方式，通常会针对搜索引擎或平台算法进行优化。在网络社区里，真实性很重要，因为成员往往依赖个人经验、专业知识和信任来判断一条帖子是否有用或真实。

**社区讨论**: 评论整体上对 AI 生成内容表现出疲惫和悲观，有人把这种感受形容为“悲伤”或情绪消耗。也有人把重点放在动机上，猜测可能与 SEO 滥用、广告欺诈、洗钱或垄断某个细分市场有关；还有少数评论加入了幽默，或补充了作者为何以编织为主题会特别有个人色彩。

**标签**: `#AI-generated content`, `#content farms`, `#online communities`, `#authenticity`, `#Hacker News discussion`

---

<a id="item-8"></a>
## [YouTube 的 RSS 订阅失灵了](https://openrss.org/blog/youtube-your-feeds-are-broken) ⭐️ 7.0/10

OpenRSS 的一篇文章认为，YouTube 的 RSS 订阅实际上已经失效，因为它的单页应用流程会把订阅链接藏起来，只有在浏览器里从头刷新频道页时才会出现。评论区还给出了一些绕过办法，比如改写订阅地址来过滤 Shorts，或者用脚本识别 Shorts 视频。 对于依赖 RSS 来追踪 YouTube 频道、而不是使用算法推荐的人来说，这会让订阅流程变得更不稳定，也更难发现。它还反映出一个更广泛的问题：单页应用式网站的浏览器导航，可能会把订阅器依赖的页面元数据隐藏起来。 有评论指出，YouTube 其实会暴露一个 feed 的 `<link>` 元素，但只有在刷新频道的视频页之后才会出现，这说明阻碍点在单页应用的导航流程。另一个绕过方法是把频道订阅地址从 `channel_id=UC...` 改成 `playlist_id=UULF...`，这样只会列出普通视频；还有人用脚本访问 `https://www.youtube.com/shorts/VIDEO_ID`，如果返回 200 就把它当作 Shorts。

hackernews · veeti · May 6, 01:15 · [社区讨论](https://news.ycombinator.com/item?id=48030964)

**背景**: RSS 是一种订阅格式，用户可以通过一个 URL 订阅网站或频道的更新，通常以 XML 形式提供。YouTube 长期支持类似 `/feeds/videos.xml?channel_id=...` 这样的频道订阅地址，很多阅读器都能直接读取。单页应用会在浏览器里直接更新内容，而不是整页重新加载，因此原本会出现在页面源码中的链接和元数据，可能更难被发现或暴露出来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/dotnet/architecture/modern-web-apps-azure/choose-between-traditional-web-and-single-page-apps">Choose between traditional web apps and single page apps ... Single Page Application - GeeksforGeeks Single Page Apps (SPA) | Wappler Docs Respecting Browser Navigation in Single Page Applications Your Single-Page Applications Are Vulnerable: Here's How to ...</a></li>
<li><a href="https://danielmiessler.com/blog/rss-feed-youtube-channel">How to Get an RSS Feed for a YouTube Channel | Daniel Miessler</a></li>

</ul>
</details>

**社区讨论**: 评论区整体上以实用和吐槽为主：不少人分享了过滤 Shorts 和发现订阅链接的具体办法，也有人抱怨订阅访问和可见性过于脆弱。还有一些带着黑色幽默的担心，认为如果 계속提醒 YouTube 他们还有 RSS，平台可能会干脆把它删掉。

**标签**: `#RSS`, `#YouTube`, `#web apps`, `#feeds`, `#browser behavior`

---

<a id="item-9"></a>
## [开源还是收费软件](https://nonogra.ph/write-some-software-give-it-away-for-free-05-05-2026) ⭐️ 7.0/10

这篇以讨论为主的文章探讨了软件是否应该免费提供，并权衡了开源社区价值与收费软件可持续性之间的取舍。该帖子在 Hacker News 上获得了广泛关注，拿到了 315 分和 217 条评论。 这篇文章触及了开发者和小型软件业务面临的核心问题：如何在传播范围、社区口碑和收入之间取得平衡。它的热度也说明，变现方式与开源伦理仍然是开发者生态中持续存在的现实议题。 这不是一次技术产品发布，而是一篇围绕免费软件、开源参与和财务可持续性权衡的观点文章。讨论中呈现了明显分歧，包括对开源用户“理所当然”心态的担忧、把社区放在首位的价值观，以及“愿意付费”可以作为一种有效筛选机制的看法。

hackernews · nohell · May 5, 21:26 · [社区讨论](https://news.ycombinator.com/item?id=48028842)

**背景**: 开源软件通常会在特定许可证下公开发布，允许他人使用、修改和再分发；而收费软件则依赖直接收入来支持开发和维护。许多开发者会同时采用这两种方式，因为免费分发有助于扩大使用和建立社区，但并不一定能覆盖持续工作的成本。这类讨论通常归结为：一个项目究竟应被视为社区协作、个人爱好，还是商业业务。

**社区讨论**: 评论整体上呈现出一种分歧但认真讨论的氛围。有人认为收费软件带来的互动更建设性，而“是否愿意付费”本身就是一种有效筛选；也有人把开源看作以社区为先的活动，即使收益不高也很有成就感。还有评论强调，这个问题没有统一答案，因为开发者终究还是需要收入来维持生计。

**标签**: `#open source`, `#software business`, `#developer community`, `#monetization`, `#Hacker News`

---

<a id="item-10"></a>
## [Willison 称两者正在融合](https://simonwillison.net/2026/May/6/vibe-coding-and-agentic-engineering/#atom-everything) ⭐️ 7.0/10

在 Heavybit 的 High Leverage 播客讨论中，Simon Willison 说他自己使用 AI 编程工具时，已经感到“vibe coding”和“agentic engineering”的界限开始模糊。此前他一直把两者看作不同方式，但现在认为它们在实际工作中正在重叠。 这表明 AI 辅助软件开发比表面上的分类更灵活，也更接近真实工作流。它还触及生产软件开发中的核心问题：工程师究竟可以把多少代码交给代理生成，而不会削弱质量、安全性或责任边界？ Willison 在原则上仍然区分两者：vibe coding 更适合随意项目或个人工具，对代码质量和审查要求较低；而 agentic engineering 则面向专业开发，需要考虑安全性、可维护性、运维和性能。他表示像 Claude Code 这样的工具已经能可靠完成简单的生产任务，例如生成带测试和文档的 JSON API 接口，但他自己也越来越不会逐行审查每一段代码。

rss · Simon Willison · May 6, 14:24

**背景**: 通常来说，vibe coding 是指用自然语言向 AI 模型描述任务，并让它自动生成代码，往往不会对结果做太多直接检查。agentic engineering 则是相关但不同的思路：AI 代理作为工具嵌入传统工程流程中，而不是取代工程判断。这种区分之所以重要，是因为前者可能适合一次性或个人用途，而后者的目标是支持专业软件交付。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/vibe-coding">What is Vibe Coding? | IBM</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-engineering">What is agentic engineering? - IBM</a></li>

</ul>
</details>

**标签**: `#AI coding`, `#software engineering`, `#agentic workflows`, `#vibe coding`, `#developer tools`

---

<a id="item-11"></a>
## [StarFighter 16 英寸笔记本发布](https://us.starlabs.systems/pages/starfighter) ⭐️ 6.0/10

StarLabs 发布了 StarFighter 16 英寸，这是一款面向 Linux 的独占笔记本，主打隐私和性能。Tom's Hardware 报道称其起售价为 1,878 美元，配置包括 16 英寸 165Hz QHD 哑光屏、Intel Core Ultra 5 125H 和 32GB LPDDR5x 内存。 这次发布对 Linux 硬件用户很重要，因为 StarLabs 是少数提供高端、以 Linux 为先系统的厂商之一。它又恰逢内存价格上涨，可能同时影响这类小众笔记本的成本和供货。 有评论指出，一张宣传图似乎展示了可插拔内存，但实际机器据称采用的是焊接式 BGA LPDDR5X，这会取消用户自行升级的可能。讨论中还提到，捆绑的 65W 充电器、欧盟对充电器的规定以及默认仅一年保修等问题也引发了争议。

hackernews · signa11 · May 6, 02:03 · [社区讨论](https://news.ycombinator.com/item?id=48031261)

**背景**: StarLabs 是一家英国厂商，主要销售以 Linux 为先的笔记本和迷你主机。Fedora 文档提到，StarLabs 使用 coreboot 和 edk2 等开源固件，禁用 Intel Management Engine，并通过 LVFS 提供固件更新。StarFighter 系列面向那些希望高端硬件从一开始就为 Linux 设计的用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://starlabs.systems/pages/starfighter">StarFighter 16-inch – Star Labs®</a></li>
<li><a href="https://www.tomshardware.com/laptops/new-linux-starfighter-laptop-family-debuts-starting-at-usd1-878-star-labs-systems-laptops-arrive-with-spacious-ram-several-options">New Linux StarFighter laptop family debuts ... - Tom's Hardware</a></li>
<li><a href="https://docs.fedoraproject.org/en-US/marketing/ready/starlabs/">StarLabs :: Fedora Docs</a></li>

</ul>
</details>

**社区讨论**: 讨论整体上既有兴趣也很谨慎，几位评论者表示会等第三方评测出来再决定是否购买。另一些人则关注高内存价格带来的成本压力，以及设计和政策方面的抱怨，比如内存规格疑似不一致、缺少独立鼠标按键、强制捆绑充电器和保修期较短等。

**标签**: `#Linux hardware`, `#laptops`, `#PC hardware`, `#product launch`, `#community discussion`

---

<a id="item-12"></a>
## [Andon Labs 在斯德哥尔摩开设 AI 咖啡馆](https://simonwillison.net/2026/May/5/our-ai-started-a-cafe-in-stockholm/#atom-everything) ⭐️ 6.0/10

Andon Labs 表示，他们在瑞典斯德哥尔摩启动了一个新的 AI 管理咖啡馆实验，此前他们已经在旧金山做过一个 AI 运营零售店项目。这个实验已经暴露出明显的运营失误，包括离谱的库存采购，以及与供应商和当地机构之间充满错误的交互。 这是一个具体案例，展示了当 AI 代理接入真实业务流程而不是演示环境时会如何表现。它既说明了把常规运营交给软件的潜力，也暴露出如果缺少人工监督，让系统对外部世界直接行动会带来风险。 文章提到，AI 经理 Mona 在咖啡馆没有炉灶的情况下订购了 120 个鸡蛋，还试图用 22.5 公斤罐装番茄来解决新鲜番茄腐坏的问题。这个实验还催生了一个可见的“羞耻墙”，上面陈列着诸如 6000 张餐巾纸等奇怪采购；此外，提交许可申请和给供应商发邮件等对外动作，也迫使人类花时间纠正 AI 犯下的错误。

rss · Simon Willison · May 5, 22:14

**背景**: AI 代理是能够规划并执行任务的系统，而不仅仅是生成文本，因此企业正在把它们用于真实运营场景。Andon Labs 此前已经用旧金山的 Andon Market 零售店验证过这一思路，而斯德哥尔摩咖啡馆是他们进一步测试 AI 能否管理日常业务的又一次尝试。文章还提到 AI 伦理问题，尤其是那些会影响他人的未经请求或低质量自动化行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://andonlabs.com/blog/andon-market-launch">We gave an AI a 3 year retail lease in SF and asked it to ...</a></li>
<li><a href="https://www.ibm.com/think/insights/building-evaluating-ai-agents-real-world">Building and evaluating AI agents that work in the real world ...</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#real-world experiment`, `#automation`, `#robotics`, `#case study`

---
