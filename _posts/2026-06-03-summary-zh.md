---
layout: default
title: "Horizon Summary: 2026-06-03 (ZH)"
date: 2026-06-03
lang: zh
---

> From 49 items, 15 important content pieces were selected

---

1. [SpaceX 拟固定价 IPO 筹资 750 亿美元](#item-1) ⭐️ 9.0/10
2. [USB 扬声器固件攻击可无线入侵电脑](#item-2) ⭐️ 8.0/10
3. [VS Code Web 漏洞可窃取 GitHub 令牌](#item-3) ⭐️ 8.0/10
4. [微软发布 MAI-Code-1-Flash](#item-4) ⭐️ 8.0/10
5. [谷歌允许网站退出 AI 搜索](#item-5) ⭐️ 8.0/10
6. [把 Nvidia 显存当作 Linux 交换空间](#item-6) ⭐️ 7.0/10
7. [自然为何重复利用蛋白折叠](#item-7) ⭐️ 7.0/10
8. [AI 在斯坦福研究中胜过法学教授](#item-8) ⭐️ 7.0/10
9. [法院叫停特朗普 10%全球关税](#item-9) ⭐️ 7.0/10
10. [内存布局细节为何会影响性能](#item-10) ⭐️ 6.0/10
11. [Edsger 将手写 Clojure 带到 reMarkable 2](#item-11) ⭐️ 6.0/10
12. [Quick Share 扩展更多安卓旗舰的 AirDrop 兼容](#item-12) ⭐️ 6.0/10
13. [代理服务大规模被封禁](#item-13) ⭐️ 6.0/10
14. [千问开放第三方 Agent 与 Skill](#item-14) ⭐️ 6.0/10
15. [64GB 是创作工作站的甜点配置。](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [SpaceX 拟固定价 IPO 筹资 750 亿美元](https://www.reuters.com/business/media-telecom/spacex-plans-raise-75-billion-ipo-135-per-share-source-says-2026-06-03/) ⭐️ 9.0/10

据称，SpaceX 计划以每股 135 美元的固定价格发行 5.556 亿股，筹资 750 亿美元。按这一方案，公司估值约为 1.75 万亿美元，计划最早于 6 月 12 日在纳斯达克挂牌交易，股票代码为 SPCX，但路演期间细节仍可能调整。 如果最终落地，这将成为史上规模最大的 IPO 之一，并可能重塑市场对超大规模上市的预期。募资用途指向 AI 算力和星链网络扩张，把 SpaceX 的航天业务进一步连接到 AI 基础设施热潮和全球卫星宽带增长。 在路演前就锁定发行价的做法极为罕见，这也是该交易最引人注目的结构性细节之一。公司去年营收 187 亿美元、净亏损 49 亿美元，且据称只有星链实现盈利。

telegram · zaihuapd · Jun 3, 09:01

**背景**: 星链是 SpaceX 的近地轨道卫星互联网网络，目标是从太空提供宽带服务。由于运行在近地轨道，它相比传统卫星系统通常具有更低时延，因此可以支持流媒体、在线游戏和视频通话。AI 算力通常指用于大规模训练和运行模型的 GPU 基础设施，扩展这类能力一般意味着增加更多集群和配套硬件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://starlink.com/technology">Starlink | Technology</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#IPO`, `#Starlink`, `#AI计算`, `#资本市场`

---

<a id="item-2"></a>
## [USB 扬声器固件攻击可无线入侵电脑](https://blog.nns.ee/2026/06/03/katana-badusb/) ⭐️ 8.0/10

一名安全研究人员演示了，连接到电脑的 USB 扬声器可以被变成攻击入口，从而在无需直接接触的情况下通过无线方式入侵电脑。这个发现表明，问题出在普通外设的 BadUSB 式固件弱点，而不是电脑本身。 这扩大了日常 USB 外设的攻击面，也说明原本可信的设备可以变成主机上的隐蔽落点。对于企业和普通用户来说，这尤其重要，因为很多人默认插上扬声器几乎没有风险。 核心问题在于固件：恶意行为存在于设备控制器代码中，因此传统杀毒软件未必能发现，简单擦除存储内容也未必能清除。这个案例符合更广义的 BadUSB 模型，即 USB 设备可以被重新编程，从而以非预期方式工作。

hackernews · xx_ns · Jun 3, 10:53 · [社区讨论](https://news.ycombinator.com/item?id=48382310)

**背景**: BadUSB 指的是修改 USB 设备内部固件的攻击，这样设备就可以冒充受信任的外设，或者表现出异常行为。与 U 盘里存放的文件不同，固件是控制设备基本功能的代码，因此更难检查，也更难替换。供应链安全在这里很重要，因为固件问题可能在制造、分发或厂商支持阶段就被引入，而且事后往往很难修补。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/BadUSB">BadUSB - Wikipedia</a></li>
<li><a href="https://hub.ivanti.com/s/article/USB-Device-Firmware-Attacks-BadUSB?language=en_US">USB Device Firmware Attacks (BadUSB) - hub.ivanti.com</a></li>
<li><a href="https://eclypsium.com/blog/endpoint-firmware-attack-timeline-introduction/">Firmware Attacks: An Endpoint Timeline - Eclypsium | Supply Chain Security for the Modern Enterprise</a></li>

</ul>
</details>

**社区讨论**: 评论整体上以不满和质疑为主，不少人批评厂商把这个问题轻描淡写地当成“不是漏洞”。还有人指出更普遍的行业问题：硬件厂商常常把软件和补丁支持当成事后补充，这会让固件漏洞和生命周期结束后的维护问题反复成为安全风险。

**标签**: `#security`, `#hardware-hacking`, `#USB`, `#firmware`, `#supply-chain-security`

---

<a id="item-3"></a>
## [VS Code Web 漏洞可窃取 GitHub 令牌](https://blog.ammaraskar.com/github-token-stealing/) ⭐️ 8.0/10

一份安全报告详细披露了一个 VS Code 网页版漏洞：攻击者可诱导用户打开 github.dev 链接，并利用 Webview 的键盘事件处理问题安装扩展，从而窃取 GitHub 令牌。报告还指出，微软随后很快发布了一个临时修复。 GitHub 令牌和个人访问令牌可以授予对仓库及其他账户资源的访问权，因此一旦被窃取，就可能以受害者的权限暴露代码和密钥，包括私有仓库。由于 VS Code 网页版与 GitHub 工作流深度集成，这一问题也说明云端开发工具本身已经成为高价值攻击面。 这篇分析指出，网页版 VS Code 比桌面版更容易被利用，不过桌面版也存在该问题。根据后续讨论，微软的临时补丁是在 web VS Code 中打开笔记本时增加确认步骤，并阻止命令跳过受信任发布者检查。

hackernews · ammar2 · Jun 2, 15:29 · [社区讨论](https://news.ycombinator.com/item?id=48371562)

**背景**: VS Code 是一款广泛使用的代码编辑器，其网页版通过 github.dev 等托管工作流在浏览器中运行。GitHub 个人访问令牌是用于代表用户进行 API 和命令行认证的凭据，因此属于必须严格保护的敏感密钥。安全研究一再表明，编辑器和扩展会扩大攻击面，因为开发工具通常能深度访问文件、账户以及云服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens">Managing your personal access tokens - GitHub Docs</a></li>
<li><a href="https://www.sonarsource.com/blog/visual-studio-code-security-deep-dive-into-your-favorite-editor/">Visual Studio Code Security: Deep Dive into Your Favorite ...</a></li>

</ul>
</details>

**社区讨论**: 讨论整体上对这篇报告和研究工作给予了高度评价。一些评论者认为让网页版编辑器直接登录 GitHub 本身就带来了不必要的风险面，另一些人则称赞微软响应很快，同时也提到 MSRC 的安全漏洞报告流程过去常常让研究人员感到沮丧。

**标签**: `#security`, `#vscode`, `#github`, `#vulnerability`, `#cloud-developer-tools`

---

<a id="item-4"></a>
## [微软发布 MAI-Code-1-Flash](https://microsoft.ai/news/introducingmai-code-1-flash/) ⭐️ 8.0/10

微软推出了 MAI-Code-1-Flash，这是一款面向代码任务的大型模型，并表示它属于一次发布的七个新 MAI 模型之一。公司还为这次发布提供了模型页面和 PDF 版模型卡。 这次发布让微软进一步进入代码模型竞争，开发者和工具厂商都很看重基准表现与 API 成本。若微软能在价格和性能上保持竞争力，可能会影响代码助手、企业工作流以及更广泛的开发者 AI 市场。 有评论者指出，模型卡里把 MAI-Code-1-Flash 描述为 137B 总参数模型，并提到它在 SWE-bench Pro 上得分为 51%。讨论中的主要保留意见是，它相对更小的竞争对手优势并不大，因此实际编码效果和价格对比仍是核心问题。

hackernews · EvanZhouDev · Jun 2, 18:47 · [社区讨论](https://news.ycombinator.com/item?id=48374466)

**背景**: 模型卡是随 AI 模型附带的一种文档，通常会说明预期用途、评测指标、训练数据和限制。面向代码的大语言模型会针对代码生成、修改和调试等编程任务进行优化，而不只是用于通用对话。对于这类模型来说，基准测试有参考价值，但还不够，因为真实编程效果和成本往往才决定是否被采用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techtarget.com/whatis/definition/model-card-in-machine-learning">What is a model card in machine learning and ... - TechTarget Model card - AI Wiki What Are Model Cards? - Dataconomy Model Cards and Data Sheets: Documentation Standards for ML Model Card Hub -- ML Model Documentation and Evaluation 2025.09.16 Ki Tutorial FAIR4ML - Model Cards - Zenodo Model Cards, Datasheets & Governance Frameworks - Medium</a></li>
<li><a href="https://blog.runpod.io/runpod-roundup-5-visual-language-comprehension-code-focused-llms-and-bias-detection/">Visual/ Language Comprehension, Code - Focused LLMs, and Bias...</a></li>
<li><a href="https://aiwiki.ai/wiki/model_card">Model card - AI Wiki</a></li>

</ul>
</details>

**社区讨论**: 整体讨论偏谨慎但有兴趣。几位评论者认为，相比模型规模，这点基准提升并不算大，而且把 Claude Haiku 作为对比对象说服力有限；也有人认为公布的价格看起来有竞争力，并在 GitHub Copilot 最近调整计费后欢迎更多竞争。

**标签**: `#AI models`, `#code generation`, `#Microsoft`, `#benchmarks`, `#developer tools`

---

<a id="item-5"></a>
## [谷歌允许网站退出 AI 搜索](https://9to5google.com/2026/06/02/google-ai-mode-overviews-opt-out/) ⭐️ 8.0/10

谷歌将在 Search Console 中新增一个设置，让网站所有者决定其内容是否可以出现在 AI Mode 和 AI Overviews 中。与此同时，谷歌还将推出新的生成式 AI 搜索统计数据，供站长查看展示量、页面级表现和地域分布等指标。 这让内容发布者和 SEO 团队对内容如何被用于谷歌的 AI 搜索体验拥有了更多控制权，同时又不会影响其在常规搜索和 Discover 中的曝光。新增的数据统计也可能影响内容策略，因为 AI 生成答案正在成为搜索流量中越来越重要的一部分。 报道指出，退出 AI 生成内容展示不会影响网站在常规搜索结果和 Discover 中的排名与展示。该控制项目前已在英国部分网站测试，之后计划向全球推广。

telegram · zaihuapd · Jun 3, 12:00

**背景**: Search Console 是谷歌提供的网站管理工具，用来查看网站在搜索中的表现。AI Mode 和 AI Overviews 是谷歌的 AI 搜索体验，它们会在搜索界面中生成总结性答案，而不只是展示链接。由于这些功能会改变用户看到和点击网页内容的方式，发布者才会特别关注是否纳入以及如何查看相关数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://smart-link.com.tw/reports/google-ai-mode">Google AI Mode 是 什 麼？ 搜尋從取回變成推論的關鍵轉變</a></li>
<li><a href="https://www.seozzr.com/blog/ai-overviews-ai-mode-impact/">Google AI Overviews / AI Mode ... | 西品东来</a></li>

</ul>
</details>

**标签**: `#Google`, `#AI搜索`, `#SEO`, `#Search Console`, `#网站管理`

---

<a id="item-6"></a>
## [把 Nvidia 显存当作 Linux 交换空间](https://github.com/c0dejedi/nbd-vram) ⭐️ 7.0/10

开源项目 nbd-vram 让 Linux 系统可以把一部分 NVIDIA GPU 显存当作普通交换设备来使用。它通过 CUDA 驱动 API 分配显存，再经由 NBD 提供为 /dev/nbdX，最后作为交换空间接入系统。 这是一种把原本闲置的显存利用起来的方法，尤其适合内存紧张、内存焊死的笔记本或已有大显存独显的台式机。它有机会减少系统对 SSD 交换空间的依赖，对内存受限用户有实际价值，尽管适用场景仍然比较小众。 这个项目依赖一个小型守护进程和内核自带的 NBD 驱动，而不是直接把显存页固定到 BAR1 中。GitHub 说明提到，直接页固定的方案在消费级 GeForce GPU 上会被 NVIDIA 驱动返回 EINVAL，因此才改用基于 NBD 的设计。

hackernews · tanelpoder · Jun 2, 22:55 · [社区讨论](https://news.ycombinator.com/item?id=48377404)

**背景**: 交换空间是 Linux 在内存压力较大时使用的辅助存储。VRAM 是 GPU 上的显存，而 NBD 是 Linux 的一种机制，可以让用户态服务把存储以块设备的形式提供给内核。这个项目把 CUDA 和 NBD 结合起来，让操作系统把 GPU 显存看作普通交换设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/c0dejedi/nbd-vram">GitHub - c0deJedi/nbd- vram : Use your NVIDIA GPU's VRAM as swap...</a></li>
<li><a href="https://www.phoronix.com/news/NVIDIA-NBD-VRAM">NBD- VRAM Provides Swap Space On Your NVIDIA GeForce GPUs</a></li>

</ul>
</details>

**社区讨论**: 评论区总体认为这是一个小众但实用的技巧，特别适合笔记本和显存长期闲置的机器，至少能替代一部分 SSD 交换空间。主要担忧集中在性能上：有人提到 RTX 3070 Laptop 的顺序吞吐量约为 1.3 GB/s，并认为 NVMe 交换在顺序速度上可能更快，只是延迟更高。

**标签**: `#Linux`, `#GPU VRAM`, `#swap memory`, `#Nvidia`, `#systems programming`

---

<a id="item-7"></a>
## [自然为何重复利用蛋白折叠](https://research.ligo.bio/posts/unreasonable-redundancy-of-natural-protein-folds/) ⭐️ 7.0/10

这篇文章认为，自然蛋白折叠空间高度冗余，因为进化反复复用那些在能量上有利、且对突变具有鲁棒性的结构模式。文章将此解释为许多看似无关的序列最终会采用相似折叠的原因。 如果蛋白结构的复用程度比直觉中更高，这会改变我们对进化、折叠多样性以及蛋白设计搜索空间的理解。它也有助于解释为什么突变常常仍能保留功能，以及为什么工程蛋白可能更适合借用已有折叠。 文章强调，折叠空间并不是被均匀采样的：进化更容易在那些多功能、易折叠、且能容忍突变的模式中积累。讨论还把这一点与这样一个现象联系起来：即便相距很远的蛋白折叠，也可能共享片段或结构母题。

hackernews · ray__ · Jun 3, 03:47 · [社区讨论](https://news.ycombinator.com/item?id=48379669)

**背景**: 蛋白折叠是指一条线性的氨基酸链形成稳定三维结构的过程。在这里，蛋白“折叠”指的是一种重复出现的结构排列，而“折叠空间”则是蛋白可能占据的所有折叠构型所构成的整体景观。过去的研究常把折叠空间看作某种离散结构，而较新的讨论则开始考虑不同折叠之间可能存在的切换、重叠或共同的进化路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Protein_folding">Protein folding - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC10529699/">Fluid protein fold space and its implications - PMC</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0959440X14000724">The robustness and innovability of protein folds - ScienceDirect</a></li>

</ul>
</details>

**社区讨论**: 评论整体上比较认可，但也有人认为对于有生物化学基础的读者来说并不意外，尤其是考虑到活性位点保守性和突变耐受性这些早已熟悉的观点。也有评论补充了相关视角，包括不同折叠之间共享片段、蛋白设计中的类似例子，以及进化反复复用成功结构模式的现象。

**标签**: `#protein folding`, `#biochemistry`, `#evolution`, `#protein design`, `#structural biology`

---

<a id="item-8"></a>
## [AI 在斯坦福研究中胜过法学教授](https://law.stanford.edu/press/ai-outperforms-law-professors-in-stanford-law-study/) ⭐️ 7.0/10

斯坦福法学院发布了一项研究，声称 AI 在某些法律辅导任务上优于法学教授。这个结果很快引发了关于研究方法以及它对法律教育和法律工作的意义的争论。 如果这一结果成立，说明 LLM 可能可以处理一些文本密集型法律任务，并有望降低法律辅导或文书支持的成本。它也引发了更广泛的问题：AI 会以多快的速度改变法律训练以及法律服务市场的部分环节。 围绕这篇论文的讨论强调，这个结论比“AI 取代律师”要窄得多；评论者表示，研究的框架更接近把 LLM 当作法学生的辅导工具。批评者还指出，教授样本很小，而且对比结果方差很高，这可能限制结论的推广性。

hackernews · berlianta · Jun 2, 23:43 · [社区讨论](https://news.ycombinator.com/item?id=48377761)

**背景**: 大型语言模型，简称 LLM，是通过大量文本训练出来、用于生成和分析语言的 AI 系统。在法律 AI 研究中，像 LegalBench 这样的领域专用基准会被用来测试模型是否能完成法律推理任务，因为通用聊天能力并不一定能直接迁移到法律场景。这个背景很重要，因为这条新闻中的结论取决于法律任务是如何设计和衡量的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/large-language-models">What are large language models (LLMs)? - IBM</a></li>
<li><a href="https://hazyresearch.stanford.edu/legalbench/">A collaborative benchmark for evaluating legal reasoning in large...</a></li>

</ul>
</details>

**社区讨论**: 评论者总体上对这项研究的严谨性持怀疑态度，其中几位指出实验设计可能存在统计弱点和偏差。与此同时，也有人认为，即使研究本身有缺陷，它仍然反映出一个真实趋势：LLM 非常适合处理文本密集型法律工作，尤其是阅读、归纳和写作类任务。

**标签**: `#AI`, `#law`, `#LLMs`, `#legal-tech`, `#research`

---

<a id="item-9"></a>
## [法院叫停特朗普 10%全球关税](https://t.me/zaihuapd/41737) ⭐️ 7.0/10

美国纽约国际贸易法院裁定，特朗普新推出的 10%临时全球关税无效，且缺乏《1974 年贸易法》第 122 条所要求的法律授权。该裁决目前阻止政府向原告华盛顿州和两家企业继续征收相关关税，政府预计将提起上诉。 这一裁决限制了总统以贸易权力实施广泛关税的空间，可能影响进口商、出口商以及全球供应链。它也表明，特朗普时期的关税政策争议可能继续进入联邦上诉程序，并最终再次到达最高法院。 法院认为，这项 10%关税超出了国会在《1974 年贸易法》第 122 条中赋予总统的权限，而且该措施具有临时性和全球性。至于其他企业是否仍需继续缴纳，目前仍不明确，下一步很可能会进入美国联邦巡回上诉法院。

telegram · zaihuapd · Jun 3, 10:02

**背景**: 美国国际贸易法院是负责处理海关和贸易法律争议的联邦法院。《1974 年贸易法》第 122 条是美国贸易争端中有时会被援引的关税工具之一。联邦巡回上诉法院位于华盛顿，通常会审理贸易案件，因此如果政府上诉，它很可能成为下一站。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://info.51.ca/articles/1516676">台湾，马 年 的两大关卡_无忧资讯</a></li>
<li><a href="https://www.wikiwand.com/zh-tw/articles/美国联邦巡回区上诉法院">美国 联 邦 巡 回 区 上 诉 法 院 - Wikiwand</a></li>

</ul>
</details>

**标签**: `#贸易政策`, `#美国法院`, `#关税`, `#特朗普`, `#国际经济`

---

<a id="item-10"></a>
## [内存布局细节为何会影响性能](https://fzakaria.com/2026/06/01/every-byte-matters) ⭐️ 6.0/10

文章《Every Byte Matters》认为，看似很小的内存布局选择也可能带来可测量的性能影响，尤其是在数组结构体和结构体数组两种设计之间的比较上。讨论的重点集中在 Java/JVM 的内存开销、字段排列，以及在真实程序里做字节级优化是否值得。 这很重要，因为对性能敏感的软件往往不是只输赢在算法，而是输赢在缓存行为、分配开销和数据访问模式。Java 团队、游戏引擎以及运行在 JVM 上的系统代码，都可能需要权衡数据是按面向对象的方式组织，还是按更快的访问方式布局。 这篇文章的核心矛盾，是面向对象友好的设计与更有利于局部性、减少空间浪费的布局之间的取舍，例如 SoA 和 AoS。在 JVM 场景中，对象头和填充会带来额外开销，因此这些选择会更显眼，但它们是否真正有价值，仍然取决于代码是否位于热点路径上。

hackernews · ingve · Jun 3, 11:04 · [社区讨论](https://news.ycombinator.com/item?id=48382382)

**背景**: 数组结构体（AoS）把每条记录连续存放，而结构体数组（SoA）则把每个字段拆成独立数组。SoA 往往更有利于缓存局部性和 SIMD 风格处理，因为 CPU 可以连续读取同类型的许多值。在 JVM 上，对象通常带有对象头和对齐开销，所以每个字段或对象的成本可能比很多开发者预期的更高。缓存局部性指的是把数据安排得更有利于 CPU 高效复用相邻内存，而不是频繁跳转到主存。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AOS_and_SOA">AoS and SoA - Wikipedia</a></li>
<li><a href="https://www.baeldung.com/java-memory-layout">Memory Layout of Objects in Java - Baeldung Java Object Memory Footprint Determination and Overhead … Java HotSpot JVM Object Layout. As Java developers, we’re ... What is the actually memory overhead in Java? - Stack Overflow Java Memory Management - GeeksforGeeks JVM Memory Fundamentals: Stack, Heap, and Object Headers JVM Memory Model — OOMKilled by Non-Heap Overhead</a></li>
<li><a href="https://www.geeksforgeeks.org/computer-organization-architecture/locality-of-reference-and-cache-operation-in-cache-memory/">Locality of Reference - GeeksforGeeks</a></li>

</ul>
</details>

**社区讨论**: 评论区观点不一但讨论很活跃。有人批评文章把“每个字节都很重要”说得过头了，真正的问题往往是针对数百万元素的 AoS 与 SoA 取舍，而不是单个字节本身；也有人认同在热点路径上微优化确实有意义。另有评论指出，JVM 对象头今天仍然不便宜，但即将到来的紧凑对象头和 Project Valhalla 可能会显著降低这类开销。

**标签**: `#performance-optimization`, `#memory-layout`, `#jvm`, `#data-structures`, `#software-engineering`

---

<a id="item-11"></a>
## [Edsger 将手写 Clojure 带到 reMarkable 2](https://handwritten.danieljanus.pl/2026-06-01-edsger.html) ⭐️ 6.0/10

Show HN 介绍了 Edsger，这是一个把 reMarkable 2 变成手写 Clojure REPL 的项目。演示展示了在平板上手写代码并交互式求值，形成了一种少见的“用笔编程”流程。 这是一个具体而有趣的例子，展示了 REPL 驱动开发被推进到全新的输入媒介中，也说明交互式编程还能被扩展到什么程度。对于 Clojure 和开发者工具爱好者来说，它凸显了在一台原本为记笔记设计的设备上进行手写计算的吸引力与阻力。 reMarkable 2 是一款纸感很强的记笔记平板，因此这个项目必须先完成手写采集与转换，才能对 Clojure 代码进行求值。社区评论指出延迟比较明显，并讨论了多种实现思路，例如直接访问帧缓冲、通过 SSH 动手改造，以及使用本地 OCR 替代方案。

hackernews · nathell · Jun 2, 18:52 · [社区讨论](https://news.ycombinator.com/item?id=48374552)

**背景**: REPL 是“读-求值-打印循环”的缩写：用户输入一个表达式，系统立即计算并显示结果。在 Clojure 中，REPL 是开发方式的核心，尤其适合渐进式探索和测试。reMarkable 2 是一款数字纸张平板，主要面向手写、阅读和记笔记，而不是通用应用。OCR，也就是光学字符识别，是把手写内容转换成机器可读文本的过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.remarkable.com/s/article/About-reMarkable-2">About reMarkable 2</a></li>
<li><a href="https://clojure.org/guides/repl/introduction">Programming at the REPL: Introduction - Clojure</a></li>

</ul>
</details>

**社区讨论**: 评论区整体上偏正面，很多人觉得这个项目巧妙而有趣。主要担忧是延迟，尤其是有人提到的多秒级等待；评论者也提出了通过直接访问帧缓冲、利用 SSH 折腾设备，以及使用更快的本地 OCR 来降低延迟的思路。

**标签**: `#Clojure`, `#reMarkable`, `#Hacker News`, `#OCR`, `#developer tools`

---

<a id="item-12"></a>
## [Quick Share 扩展更多安卓旗舰的 AirDrop 兼容](https://weibo.com/2022252207/5305648180890368) ⭐️ 6.0/10

谷歌表示，Quick Share 对 AirDrop 的兼容性正在扩展到更多安卓机型，包括一加 15、小米 17T Pro、vivo X300 系列、OPPO Find X9 系列、荣耀 Magic V6 和三星 S26 系列。此次扩展是在此前 Pixel 10 系列率先支持之后进行的。 这让安卓和苹果用户可以更轻松地互传文件，而不必依赖第三方应用或繁琐的替代方案。如果这一能力覆盖更多旗舰机型，就有望缓解两大移动生态之间最明显的使用摩擦之一。 Quick Share 是谷歌的近距离无线分享系统，而与 AirDrop 的联通意味着它可以和苹果的文件分享功能互通。此次公告只列出了部分旗舰机型，没有给出更详细的推送时间表或更广泛的设备名单。

telegram · zaihuapd · Jun 3, 08:47

**背景**: Quick Share 是谷歌为 Android、ChromeOS 和 Windows 提供的无线点对点文件传输功能。AirDrop 是苹果内置的分享工具，服务于 iPhone、iPad 和 Mac，而这两套系统过去通常彼此独立。两者实现互通很重要，因为它让用户可以更直接地在不同生态之间传输照片、视频和文档。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/security/android-quick-share-support-for-airdrop-security/">Android Quick Share Support for AirDrop: A Secure Approach to ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Quick_Share">Quick Share - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Android`, `#Quick Share`, `#AirDrop`, `#Cross-platform`, `#Mobile OS`

---

<a id="item-13"></a>
## [代理服务大规模被封禁](https://t.me/zaihuapd/41740) ⭐️ 6.0/10

一则帖子称，从 3 月 4 日中午开始，多个热门代理服务商的 IP 段被 GFW 针对性封禁，导致无法正常使用。帖子还表示，VLESS 受到的影响较深，而较新的 AnyTLS 似乎也被大量阻断。 如果属实，这说明被针对的可能不只是单个服务器，而是整类代理基础设施，这会影响依赖加密传输进行连接的用户和运维者。它也暗示审查系统可能正在适应并识别新的代理协议，而不只是封锁老旧或更显眼的方案。 这则信息属于转述，并且帖子明确提到目前缺乏事实性的统计数据，因此实际影响范围仍不清楚。帖子还称，非 TLS 类型的加密似乎没有被大量阻断；这点值得注意，因为 VLESS 通常使用标准 TLS 1.3，而 AnyTLS 的设计目标之一就是应对与 TLS 指纹相关的问题。

telegram · zaihuapd · Jun 3, 11:15

**背景**: VLESS 是 Xray 生态中的一种代理协议，常被视为 VMess 的轻量化后继方案。根据相关文档，它依赖标准 TLS 1.3，而不是再额外叠加自己的加密层。AnyTLS 也是一种代理协议，目标之一是减少嵌套 TLS 握手带来的指纹特征，因此它同样属于用于让流量更难被识别的加密传输技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://horizon-vpn.app/en/docs/protocol-vless-reality.html">VLESS + Reality — Horizon VPN documentation</a></li>
<li><a href="https://github.com/anytls/anytls-go/blob/main/docs/protocol.md">anytls-go/docs/protocol.md at main · anytls/anytls-go · GitHub</a></li>

</ul>
</details>

**标签**: `#networking`, `#censorship`, `#proxy`, `#encryption`, `#internet-blocking`

---

<a id="item-14"></a>
## [千问开放第三方 Agent 与 Skill](https://www.stcn.com/article/detail/3941333.html) ⭐️ 6.0/10

千问 APP 宣布将全面开放第三方 Agent 和 Skill 接入。企业可以在千问内运营自己的品牌 Agent，瑞幸、肯德基、蜜雪冰城、东方航空等首批企业已经开始进行 Agent 服务测试，并将陆续上线。 这意味着千问正在从聊天型应用向品牌自有 AI 服务平台扩展，可能为企业带来新的用户触达入口和运营场景。它也反映出行业正在向开放式助手生态演进，Agent 和 Skill 正成为服务交付的重要方式。 这次公告属于高层级发布，没有披露技术文档、API 细节，也没有说明第三方 Agent 和 Skill 的具体接入方式。当前只确认首批企业服务已经在测试中，并会逐步上线。

telegram · zaihuapd · Jun 3, 12:15

**背景**: AI Agent 通常指能够理解任务、规划步骤并执行动作的系统，而不只是回答问题。Skill 一般是可调用的能力或执行单元，用来让系统完成某个具体操作。放到这次千问的公告里，开放 Agent 和 Skill 意味着品牌可能把面向任务的服务直接放进千问 APP 中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1895877953453265781">什么是AI Agent？AI Agent综述，看这一篇就够了！ - 知乎</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/2000612266601641650">什么是 Skill？深入理解 AI 系统中的 Skill 概念 - 知乎</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#Platform Open Ecosystem`, `#Product Announcement`, `#Enterprise AI`, `#Chatbot`

---

<a id="item-15"></a>
## [64GB 是创作工作站的甜点配置。](https://www.pugetsystems.com/labs/articles/when-does-ram-capacity-impact-performance/) ⭐️ 6.0/10

Puget Systems 针对 Adobe 全家桶和 DaVinci Resolve 的测试发现，16GB 内存在很多创作软件中会成为明显瓶颈。比如在 After Effects 的 2D 合成和 Lightroom 导出等场景中，性能跌幅可达 40% 以上，而 64GB 则成为更均衡的专业创作配置。 这组结果为创作者选择或升级工作站内存提供了实用参考，尤其适用于 After Effects、Lightroom 和 DaVinci Resolve 这类吃内存的软件。对专业用户来说，从 16GB 升到更高容量，往往意味着更顺畅的时间线、更少卡顿，以及在复杂项目中更快的导出速度。 Puget Systems 指出，32GB 足以应对轻度修图或短视频剪辑，但在 AI 特效、复杂合成和 Fusion 节点式工作流中仍不如 64GB 流畅。核心结论并不是所有任务都必须上 64GB，而是当项目复杂度提升后，64GB 目前更像是最舒适的选择。

telegram · zaihuapd · Jun 3, 12:30

**背景**: DaVinci Resolve 是一款视频剪辑和调色软件，而它的 Fusion 页面可以在同一软件内完成视觉特效、动态图形和合成。所谓基于节点的工作流，就是把不同处理步骤连接起来生成效果，项目越复杂，越容易消耗大量内存。Adobe After Effects 常用于 2D 合成和动态图形，Lightroom 常用于照片编辑和导出，因此在处理较重任务时，它们都可能对内存容量比较敏感。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.blackmagicdesign.com/products/davinciresolve">DaVinci Resolve | Blackmagic Design</a></li>

</ul>
</details>

**标签**: `#内存容量`, `#工作站配置`, `#创意软件`, `#性能测试`, `#DaVinci Resolve`

---
