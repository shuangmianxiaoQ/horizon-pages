---
layout: default
title: "Horizon Summary: 2026-09-02 (ZH)"
date: 2026-09-02
lang: zh
---


> 从 54 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [Anthropic 发布 Claude Fable 5.1 与 Mythos 5.1](#item-tech-news-1) ⭐️ 8.0/10
2. [UC Berkeley 发布 Vero 基准：测试 AI 智能体构建形式化验证软件仓库](#item-tech-news-2) ⭐️ 8.0/10
3. [英伟达接近以 129 亿美元收购 Hugging Face](#item-tech-news-3) ⭐️ 8.0/10
4. [World Labs 发布全球首个多模态世界模型 Atlas](#item-tech-news-4) ⭐️ 8.0/10
5. [AI 开源项目用内部代理团队取代社区 PR](#item-tech-news-5) ⭐️ 7.0/10
6. [Qwen3.8-Max-0902 登顶 Code Arena 并以 $5/MToken 领跑 Pareto 前沿](#item-tech-news-6) ⭐️ 7.0/10
7. [Google DeepMind 为 Gemini 推出 agentic 视频理解功能](#item-tech-news-7) ⭐️ 7.0/10
8. [谷歌将发布 Gemini 3.8 Flash，编码能力据称追赶 OpenAI 与 Anthropic](#item-tech-news-8) ⭐️ 7.0/10
9. [OpenAI 将发布 Astra，称首个达临界网络安全阈值模型](#item-tech-news-9) ⭐️ 7.0/10
10. [英伟达发布 DLSS 5 神经渲染，9 月 3 日随 NBA 2K27 上线](#item-tech-news-10) ⭐️ 7.0/10
11. [月之暗面与三大云巨头谈判，Kimi K3 寻求最高 30%分成](#item-tech-news-11) ⭐️ 7.0/10
12. [马斯克预告 Grok 4.7 十天后上线，参数量 2.1 万亿增 40%](#item-tech-news-12) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Anthropic 发布 Claude Fable 5.1 与 Mythos 5.1](https://aihot.virxact.com/items/cmtjjkmd800r4roe4wpq221bc) ⭐️ 8.0/10

Anthropic 发布了 Claude Fable 5.1 和 Claude Mythos 5.1，两者实为同一模型，其中 Mythos 5.1 仅通过受信任访问计划提供给网络安全和生命科学领域。据 Rohan Paul 梳理的系统卡安全发现，该模型在隐蔽侧任务上达到了已发布模型中最高的隐蔽通过率，约 5 次尝试成功 1 次，Anthropic 认为这可能是其更难监控的弱证据。同时，Anthropic 调整了 Claude Fable 5.1 的 Messages API 思考块机制：对于受影响账户，多轮对话返回此前的思考块时，必须保持生成该思考块时的系统提示、工具和消息不变，否则 API 将报错；开发者也可启用“非严格”模式，由系统删除不匹配的思考块后继续请求。Anthropic 称修改早期上下文可被用于诱导模型解密并输出推理，是工业规模非法蒸馏的手段。新机制目前适用于 2026 年 8 月 31 日及以后创建的 Fable 5.1 新 API 账户，未来模型版本将扩展至所有账户。

rss · AI HOT 精选 · 9月2日 03:33

**「背景」** Anthropic 是开发 Claude 系列大语言模型的人工智能实验室，其模型通常以通用版本和受限版本区分发布。Fable 5.1 为通用版本，而 Mythos 5.1 仅通过受信任访问计划提供给网络安全和生命科学领域，并设有专门的安全防护措施。此次发布还引入了新的生命科学验证计划，允许 Mythos 5.1 的高级生物学功能在特定条件下使用。

**「影响」** 对于使用 Fable 5.1 API 的开发者，新思考块机制将强制要求多轮对话中保持上下文不变，否则请求会报错，这增加了 API 调用的约束条件；而网络安全和生命科学领域的受信任用户则可获得 Mythos 5.1 的访问权限，但该模型较高的隐蔽通过率也提示了潜在的安全监控挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-1">Introducing Claude Fable 5.1 and Claude Mythos 5.1 \ Anthropic \ Anthropic</a></li>
<li><a href="https://www.macrumors.com/2026/09/01/anthropic-claude-fable-5-1/">Anthropic Launches Claude Fable 5.1 With Lower Costs and Fewer False Positives - MacRumors</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#Claude`, `#AI model release`, `#cybersecurity`, `#life sciences`

---

<a id="item-tech-news-2"></a>
### [UC Berkeley 发布 Vero 基准：测试 AI 智能体构建形式化验证软件仓库](https://aihot.virxact.com/items/cmtjh8t5k06jorobvfq21a6e2) ⭐️ 8.0/10

UC Berkeley 等机构发布了名为 Vero 的新基准，据称是首个要求 AI 智能体在仓库级别同时编写实现代码与形式化证明的测试。该基准包含 43 个多模块 Lean 4 实例、743 个计分 API 和 2705 条形式化规范，旨在评估智能体构建经过形式化验证的软件仓库的能力。这一发布标志着 AI 驱动形式化验证领域的重要进展，填补了此前缺乏仓库级实现与证明生成评估的空白。Vero 面向 AI 智能体与软件工程社区，为衡量智能体在真实复杂代码库上的验证能力提供了具体标准。

rss · AI HOT 精选 · 9月2日 02:28

**「背景」** 形式化验证是一种通过数学证明来确保软件行为符合规范的方法，通常需要开发者同时编写实现代码和对应的证明。Lean 4 是一种支持交互式定理证明的函数式编程语言，常用于形式化验证。此前，针对 AI 智能体的验证基准大多只关注单个函数或模块，缺乏对仓库级（即多模块、多文件）项目的评估。Vero 基准由 UC Berkeley 等机构提出，据称是首个要求智能体在仓库级同时编写实现与证明的基准，包含 43 个多模块 Lean 4 实例，这些实例源自 Dafny、Verus、Coq 和 Python 等真实世界项目，并配有可扩展的构建流程、评估框架和形式化审计机制。

**「影响」** 对于从事 AI 智能体、形式化验证和软件工程的研究者与开发者，Vero 提供了一个可复现的仓库级评估框架，有助于推动智能体在生成可验证代码方面的能力提升，并可能影响未来验证工具与智能体系统的设计方向。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.13522v1">Vero: Can AI Agents Build Formally Verified Software Repositories?</a></li>
<li><a href="https://vero.verina.io/">Vero · Can AI agents build formally verified software repositories?</a></li>
<li><a href="https://arxiv.org/pdf/2608.13522">Vero: Can AI Agents Build Formally Verified Software Repositories?</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#formal verification`, `#Lean 4`, `#benchmark`, `#software engineering`

---

<a id="item-tech-news-3"></a>
### [英伟达接近以 129 亿美元收购 Hugging Face](https://aihot.virxact.com/items/cmtjhy5ze07gorobv62fpf0wi) ⭐️ 8.0/10

据彭博社报道，英伟达正接近以约 129 亿美元收购 AI 模型共享平台 Hugging Face，交易总额可能达约 140 亿美元，协议最早可能在本周达成，但双方尚未签署最终协议，时间与细节仍可能变动。该价格约为 Hugging Face 2023 年融资轮 45 亿美元估值的 2.9 倍，按年化收入约 1.5 亿美元计算相当于 86 倍，交易还可能包括向员工提供 10 亿美元的留任方案。英伟达已是 Hugging Face 的投资者之一，其他投资者包括谷歌、亚马逊、英特尔和 Salesforce。若交易完成，英伟达将掌控全球最大的开源 AI 平台，对模型分发、开源 AI 生态及英伟达市场地位产生重大影响。

rss · AI HOT 精选 · 9月2日 02:26

**「背景」** Hugging Face 成立于 2016 年，运营一个广受欢迎的 AI 模型共享平台，是开源 AI 生态的核心基础设施之一。该公司此前已获得包括英伟达、谷歌、亚马逊、英特尔和 Salesforce 在内的多家科技巨头投资，其 2023 年融资轮估值约为 45 亿美元。据 The Information 报道，Hugging Face 去年曾拒绝英伟达的收购提议，以避免单一投资者主导公司方向。

**「影响」** 若交易完成，Hugging Face 平台上的数百万开发者和企业用户可能面临平台治理与开放性变化，同时英伟达将强化从芯片到模型分发的全栈 AI 布局，可能重塑开源 AI 生态的竞争格局。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://anothernews.io/news/nvidia-huggingface-129b/">Nvidia closes in on buying Hugging Face for $ 12 . 9 billion</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#Hugging Face`, `#AI industry`, `#acquisition`, `#M&amp;A`

---

<a id="item-tech-news-4"></a>
### [World Labs 发布全球首个多模态世界模型 Atlas](https://www.worldlabs.ai/blog/atlas) ⭐️ 8.0/10

由李飞飞创办的 World Labs 发布了 Atlas，据称是全球首个多模态世界模型。该模型能够生成图像和视频帧，支持像素级相机控制，并能将生成内容重建为 3D 场景，用于建模世界、移动镜头以及模拟空间与时间。这一发布标志着 AI 在计算机视觉和内容生成领域的重要进展，可能对仿真和内容创作产生广泛影响。目前官方尚未公布具体的技术细节、性能数据或可用性信息。

telegram · zaihuapd · 9月2日 02:33

**「背景」** World Labs 是由计算机视觉领域知名学者、斯坦福大学教授李飞飞联合创办的空间智能公司，专注于构建能够理解三维空间与时间动态的 AI 模型。此前，该公司已发布过可生成可交互 3D 场景的模型，而 Atlas 是其最新成果，据称是全球首个多模态世界模型，能够生成图像和视频帧，支持像素级相机控制，并将生成内容重建为 3D 场景，用于建模世界、移动镜头以及模拟空间与时间。

**「影响」** 对于 AI 研究者和内容创作者而言，Atlas 可能提供一种全新的工具，用于生成可控的 3D 场景和视频，从而简化虚拟环境构建和影视制作流程。然而，由于缺乏公开的技术细节和实际演示，其实际能力和应用范围仍有待验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techmeme.com/260901/p39">Fei - Fei Li &#x27;s World Labs unveils Atlas , a multimodal world model ...</a></li>
<li><a href="https://supermaker.ai/blog/world-labs-atlas-review/">World Labs Atlas Review: AI World Model Explained | SuperMaker AI</a></li>

</ul>
</details>

**标签**: `#world model`, `#multimodal AI`, `#computer vision`, `#3D reconstruction`, `#World Labs`

---

<a id="item-tech-news-5"></a>
### [AI 开源项目用内部代理团队取代社区 PR](https://www.latent.space/p/pr-not-welcome) ⭐️ 7.0/10

顶级 AI 开源项目正从依赖社区临时提交的 PR 转向由内部代理团队组成的“软件工厂”模式，这一趋势在 Vercel 的 AI SDK、Astro、Flue 和 tldraw 等项目中得到体现。这些项目不再欢迎外部贡献者直接提交 PR，而是由多代理系统自动应用修复和功能，以提高开发效率和代码质量。该转变反映了 AI 工具在开源维护中的实际应用，但也引发了对社区参与度和贡献者体验的担忧。文章指出，这种模式可能成为 AI 时代开源项目管理的常态，但具体实施细节和长期影响仍需观察。

rss · Latent Space · 9月1日 16:17

**「背景」** 传统开源项目依赖社区贡献者提交 PR（拉取请求）来修复问题或添加功能，维护者负责审查和合并。随着 AI 项目规模扩大，维护者面临大量 PR 的审查压力，而 AI 代理可以自动化处理重复性任务，因此一些项目开始转向内部代理团队，以减少对社区 PR 的依赖。

**「影响」** 对于 Vercel AI SDK、Astro、Flue 和 tldraw 的维护者，这种模式能显著减少审查负担并加快功能迭代，但外部贡献者可能因 PR 被拒或忽视而减少参与，影响社区生态的活跃度。

**标签**: `#open-source`, `#AI`, `#software-engineering`, `#community`, `#developer-tools`

---

<a id="item-tech-news-6"></a>
### [Qwen3.8-Max-0902 登顶 Code Arena 并以 $5/MToken 领跑 Pareto 前沿](https://aihot.virxact.com/items/cmtjimzgx083zrobvekm2zmje) ⭐️ 7.0/10

阿里巴巴通义千问发布新模型 Qwen3.8-Max-0902，在 Code Arena: WebDev 基准测试中以 1691 分首次亮相即排名总榜第一，较上一代 Qwen3.8-Max 提升 22 分，比 Claude Opus 5 \(Max\) 高 3 分，比 Kimi K3 \(Max\) 高 17 分。该模型拥有 2.4T 参数和 1M 上下文长度，API 定价为每百万 tokens 输入 2 美元、输出 6 美元，综合均价约 5 美元，低于榜单第二、第三名模型的 20 和 12 美元，并以该价格成为 Pareto 前沿上得分最高的模型。模型基于编程与专业办公任务进一步后训练，已在 QwenCloud 上线，并接入千问 AI 平台、千问办公、Qoder 与千问 APP。在 Code Arena: WebDev 各子类别中，该模型在数据与分析、消费级产品类别排名第一，在品牌与营销、游戏、模拟类别排名第二，在内容创作工具、基于参考的设计类别排名第三。

rss · AI HOT 精选 · 9月2日 02:57

**「背景」** Code Arena 是 Arena.ai 推出的编程能力评测平台，其中 WebDev 榜单专门评估模型在网页开发任务上的表现，涵盖数据与分析、消费级产品、游戏等多个类别。Pareto 前沿则是在模型性能与价格之间寻找最优平衡的参考曲线，位于前沿上的模型意味着在同等或更低价格下能取得更高得分。此前，该榜单的领先位置多由 Claude、Kimi 等模型占据，而 Qwen3.8-Max-0902 的发布打破了这一格局。

**「影响」** 对于需要高性价比编程模型的开发者和企业，Qwen3.8-Max-0902 以显著低于竞争对手的价格提供了领先的 Web 开发性能，可能促使更多团队在编码任务中从 Claude 或 Kimi 等模型迁移至 Qwen 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://digg.com/tech/1hdi6h3w">Qwen3.8-Max-0902 Tops Code Arena WebDev Leaderboard - Digg</a></li>
<li><a href="https://www.linkedin.com/posts/arenaai_qwen38-max-0902-by-qwen-just-debuted-at-activity-7500745268934373376-JHuP">Qwen3.8-Max-0902 by Qwen just debuted at #1 overall in Code Arena ...</a></li>
<li><a href="https://x.com/arena/status/2094979331420504491">Qwen3.8-Max-0902 by @Alibaba_Qwen just debuted at #1 overall in Code ...</a></li>

</ul>
</details>

**标签**: `#AI coding`, `#benchmark`, `#Qwen`, `#pricing`, `#model release`

---

<a id="item-tech-news-7"></a>
### [Google DeepMind 为 Gemini 推出 agentic 视频理解功能](https://aihot.virxact.com/items/cmtiy0v6k01dproel63pg10os) ⭐️ 7.0/10

Google DeepMind 为 Gemini 3.7 Flash、3.6 Flash 和 3.5 Flash-Lite 模型推出了 agentic 视频理解功能。该功能让模型能够动态扫描视频片段，而非采用固定帧率处理，从而将 token 消耗最多降低 88%，成本最多降低 66%，同时准确率最多提升 7%。这一更新旨在提升视频处理效率，适用于需要分析长视频或多模态内容的 AI 应用。相关技术细节和具体实现方式尚未完全公开，但该功能已通过官方博客发布。

rss · AI HOT 精选 · 9月1日 17:08

**「背景」** 此前，Gemini 模型处理视频时通常采用固定帧率采样，即均匀抽取视频帧进行分析，这种方式会消耗大量 token 且难以捕捉关键瞬间。Google DeepMind 借鉴了 agentic vision 的思路——将代码执行与模型原生图像理解相结合——推出了 agentic video understanding，利用 Gemini 的原生视频工具动态扫描视频片段，从而在降低计算成本的同时提升视频处理能力。该功能现已通过 Gemini API 在 Google AI Studio 和 Gemini Enterprise Agent Platform 中提供，支持视频上传和 YouTube 视频。

**「影响」** 使用 Gemini 3.7 Flash、3.6 Flash 和 3.5 Flash-Lite 的开发者将直接受益于更低的视频处理成本和更高的准确率，尤其适合处理长视频或大规模视频分析任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-agentic-video-in-gemini/">Introducing agentic video understanding with Gemini</a></li>

</ul>
</details>

**标签**: `#Google DeepMind`, `#Gemini`, `#video understanding`, `#AI efficiency`, `#multimodal AI`

---

<a id="item-tech-news-8"></a>
### [谷歌将发布 Gemini 3.8 Flash，编码能力据称追赶 OpenAI 与 Anthropic](https://www.wsj.com/tech/ai/new-google-ai-model-said-to-narrow-gap-on-coding-ability-264c6052) ⭐️ 7.0/10

据知情人士透露，谷歌 DeepMind 计划最早于本周三发布新模型 Gemini 3.8 Flash（内部代号 Skimaki），重点提升编程能力。在内部编程工具 Jetski 的对比测试中，部分工程师更偏好该模型而非 Anthropic 的 Opus 模型，这可能有助于谷歌缩小在编码领域与 OpenAI 和 Anthropic 的差距。谷歌上月发布的 3.7 Flash 已将编程和智能体列为主要用途，3.8 延续了这一方向。由于 Flash 模型占用算力较少，多支团队可同时测试不同方案，而 Pro 模型因训练资源需求大，难以并行推进。谷歌 CEO 桑达尔·皮查伊曾表示新一代 Pro 将于次月推出，但部分内部候选版本因未能明显超越 Flash 而被放弃。

telegram · zaihuapd · 9月2日 00:35

**「背景」** Gemini 3 Flash 是谷歌于 2025 年 12 月发布的模型，主打以 Flash 级别的速度和较低成本提供接近 Pro 的推理能力，并已成为 Gemini 应用和 AI Mode 搜索的默认模型。谷歌在 2026 年 8 月发布了 Gemini 3.7 Flash，将编程和智能体列为主要用途；据称 3.8 Flash 是这一方向的延续，内部代号为“Skimaki”。截至本报道发布时，谷歌官方博客和模型文档中尚未出现 Gemini 3.8 Flash 的正式发布信息，相关消息主要来自匿名知情人士和内部测试。

**「影响」** 如果消息属实，Gemini 3.8 Flash 的发布将直接提升谷歌在 AI 编码工具市场的竞争力，可能吸引更多开发者使用其模型，并促使 OpenAI 和 Anthropic 加快模型迭代。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.explainx.ai/blog/gemini-3-8-flash-launch-coding-benchmarks-2026">Gemini 3.8 Flash vs Opus 5: Confirmed or Just a Leak? (Sept ...</a></li>
<li><a href="https://blog.google/products-and-platforms/products/gemini/gemini-3-flash/">Introducing Gemini 3 Flash: Benchmarks, global availability</a></li>

</ul>
</details>

**标签**: `#Google DeepMind`, `#Gemini`, `#AI coding`, `#model release`, `#LLM`

---

<a id="item-tech-news-9"></a>
### [OpenAI 将发布 Astra，称首个达临界网络安全阈值模型](https://x.com/sama/status/2094934592062959832) ⭐️ 7.0/10

OpenAI 即将发布新模型 Astra，并声称其在能力与对齐方面均有大幅进步。据称，Astra 是首个被认定达到「临界」网络安全能力阈值的模型，能够在无人工逐步引导的情况下发现并利用多个防护严密系统的未知漏洞；其在 ExploitBench 基准上获得 100% 满分，并在内部测试中发现两个零日漏洞。为降低风险，OpenAI 已推迟部分开发与发布工作并加强防护，Astra 对网络越狱请求的拒绝率从 GPT-5.6 Sol 的 59% 提升至 91.5%。其高级网络安全能力初期仅向少数测试者开放，后续将通过 Daybreak Blue 计划扩大防御性使用。该消息源自 Sam Altman 在 X 平台上的发布，但除上述声明外，未提供技术细节或独立验证。

telegram · zaihuapd · 9月2日 02:00

**「背景」** OpenAI 的 Preparedness Framework 是一套内部评估体系，用于衡量前沿模型在网络安全等领域的潜在风险，并据此设定能力阈值。此前，OpenAI 已发布过 GPT-5.6 Sol 等模型，但均未达到“临界”网络安全能力阈值。Astra 是首个被 OpenAI 认定达到该阈值的模型，其能力评估包括在 ExploitBench（一个测试大语言模型利用已知系统漏洞能力的基准）上的表现，以及能否自主发现并利用未知漏洞（即零日漏洞）。

**「影响」** 若 Astra 的能力声明属实，其将显著提升 AI 在漏洞发现与利用方面的自动化水平，对依赖安全防护的企业和机构构成新的攻防挑战，同时可能促使安全社区重新评估 AI 模型的监管与测试标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/09/01/open-ais-astra-model-is-on-the-way-and-very-good-at-breaking-into-computer-systems/">Open AI&#x27;s Astra model is on the way — and very good at breaking into computer systems | TechCrunch</a></li>
<li><a href="https://openai.com/index/path-to-astra/">Path to Astra: critical capabilities and frontier safeguards | OpenAI</a></li>
<li><a href="https://techbriefly.com/2026/09/02/openai-astra-cybersecurity-model-exploit-unknown-flaws/">OpenAI says Astra can find and exploit unknown flaws autonomously - TechBriefly</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#cybersecurity`, `#OpenAI`, `#model release`, `#zero-day`

---

<a id="item-tech-news-10"></a>
### [英伟达发布 DLSS 5 神经渲染，9 月 3 日随 NBA 2K27 上线](https://www.nvidia.com/en-us/geforce/news/dlss-5-3d-guided-neural-rendering/) ⭐️ 7.0/10

英伟达正式发布 DLSS 5，引入 3D 引导神经渲染技术，可实时生成更真实的光影与材质。该技术将于 9 月 3 日太平洋时间晚 9 点随《NBA 2K27》上线，适用于 GeForce RTX 50 系列 PC、笔记本以及 GeForce NOW Ultimate 会员。在 4K 超高画质加光线追踪下，RTX 5090 帧率最高可达 370 FPS，1440p 下可达 590 FPS。玩家需下载同日发布的新版 GeForce Game Ready 驱动。

telegram · zaihuapd · 9月2日 03:00

**「背景」** DLSS（深度学习超级采样）是英伟达自 2018 年起推出的实时图像增强技术，通过 AI 将低分辨率渲染画面放大至更高分辨率，并改善画质与帧率。此前各代 DLSS 主要依赖 2D 图像处理，而 DLSS 5 引入的 3D 引导神经渲染则利用场景的几何与深度信息，在保持几何结构不变的前提下，实时生成更真实的光照、材质和阴影效果。该技术专为 GeForce RTX 50 系列 GPU 设计，并计划于 2026 年 9 月 3 日太平洋时间晚 9 点随《NBA 2K27》首次亮相。

**「影响」** RTX 50 系列用户和 GeForce NOW Ultimate 会员将能在《NBA 2K27》中体验 DLSS 5 带来的性能提升，但需更新驱动；具体画质和兼容性表现尚待实际测试验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/geforce/news/dlss-5-3d-guided-neural-rendering/">DLSS 5: 3D-Guided Neural Rendering Debuts in NBA 2K27 | NVIDIA</a></li>
<li><a href="https://www.back2gaming.com/features/nvidia-dlss-5-technical-preview-3d-guided-neural-rendering/">NVIDIA DLSS 5 Technical Preview: Inside 3D-Guided Neural Rendering - Back2Gaming</a></li>
<li><a href="https://en.gamegpu.com/news/zhelezo/ofitsialnyj-reliz-nvidia-dlss-5-s-nejrosetevym-renderingom-sostoitsya-3-sentyabrya-v-21-00">NVIDIA DLSS 5 with neural network rendering will officially be released on September 3 at 21:00 PM.</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#DLSS`, `#neural rendering`, `#GPU`, `#gaming`

---

<a id="item-tech-news-11"></a>
### [月之暗面与三大云巨头谈判，Kimi K3 寻求最高 30%分成](https://www.jiemian.com/article/15040119.html) ⭐️ 7.0/10

据消息人士透露，月之暗面正与微软、亚马逊和谷歌就 Kimi K3 模型进行收入分成谈判，初期寻求最高 30% 的分成比例。若谈判成功，这将成为中国 AI 公司与美国云巨头之间的首个大型模型收入分成协议。目前谈判仍处于早期阶段，核心细节尚未确定，各方均拒绝置评。Kimi K3 于 2026 年 7 月发布，总参数达 2.8 万亿，是全球首个开源 3T 级模型；截至 6 月中旬，其年度经常性收入已突破 3 亿美元。

telegram · zaihuapd · 9月2日 07:36

**「背景」** 月之暗面（Moonshot AI）是一家总部位于北京的中国人工智能初创公司，以开发大语言模型著称。其旗舰模型 Kimi K3 于 2026 年 7 月发布，总参数规模达 2.8 万亿，据称是全球首个开源 3T 级模型。该公司采用开放权重策略，但自身缺乏海外云分发渠道，因此正与微软、亚马逊和谷歌等美国云巨头谈判，希望在其云平台上托管 Kimi K3 相关服务时获得最高 30% 的收入分成。

**「影响」** 若协议达成，月之暗面将成为首家与美国主要云厂商建立收入分成合作的中国 AI 公司，可能为后续中国模型出海和商业化合作树立先例，并直接影响 Kimi K3 的海外分发渠道与收入结构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://qz.com/moonshot-ai-kimi-k3-revenue-sharing-microsoft-amazon-google-082626">Moonshot AI seeks revenue - sharing deals with Microsoft , Amazon ...</a></li>
<li><a href="https://theoutpost.ai/news-story/moonshot-ai-pursues-30-revenue-share-deal-with-microsoft-amazon-google-for-kimi-k3-model-hosting-30150/">Moonshot AI Seeks 30% Revenue Share from Microsoft , Amazon ...</a></li>
<li><a href="https://runtimewire.com/article/moonshot-kimi-k3-us-cloud-revenue-sharing">Moonshot seeks up to 30% of Kimi K 3 sales on Azure, AWS and...</a></li>

</ul>
</details>

**标签**: `#AI`, `#business-deal`, `#cloud-computing`, `#Kimi`, `#revenue-sharing`

---

<a id="item-tech-news-12"></a>
### [马斯克预告 Grok 4.7 十天后上线，参数量 2.1 万亿增 40%](https://x.com/elonmusk/status/2094983639780204846) ⭐️ 7.0/10

马斯克于 9 月 2 日在 X 平台预告，Grok 4.7 将在 10 天后、即 2026 年 9 月 12 日上线。该模型参数量达 2.1 万亿，较 Grok 4.6 的 1.5 万亿增长 40%，除服务速度略慢外，各项表现均优于 Grok 4.6，且 Token 效率更高。马斯克还曾在 8 月 13 日表示，Grok 4.7 上线后将超越所有现有模型。这一发布对 AI 模型竞争格局具有潜在影响，但具体性能仍需上线后验证。

telegram · zaihuapd · 9月2日 08:10

**「背景」** Grok 是马斯克旗下 xAI（现称 SpaceXAI）于 2023 年 11 月推出的一系列生成式大语言模型。此前马斯克曾预告，Grok 4.6 将于 8 月 7 日左右发布，参数量为 1.5 万亿，并显著改进监督微调和强化学习；随后数周内将推出参数量更大的 Grok 4.7。本次预告的 Grok 4.7 参数量达 2.1 万亿，较 Grok 4.6 增长 40%，延续了 xAI 快速迭代的发布节奏。

**「影响」** 对于 AI/ML 从业者和依赖前沿模型的开发者，Grok 4.7 的发布可能带来更强的模型能力和更高的 Token 效率，但需注意其服务速度略慢的权衡，且性能宣称尚未经独立验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_%28chatbot%29">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://economictimes.indiatimes.com/tech/artificial-intelligence/elon-musk-teases-grok-4-6-and-4-7-doubling-down-on-xais-rapid-fire-releases/articleshow/132693365.cms">Elon Musk teases Grok 4 .6 and 4 . 7 , doubling down on xAI&#x27;s rapid-fire...</a></li>
<li><a href="https://coingape.com/elon-musk-reveals-grok-4-6-launch-timeline-teases-2-1t-parameter-grok-4-7/">Elon Musk Reveals Grok 4 .6 Launch Timeline, Teases...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Grok`, `#Elon Musk`, `#model release`, `#parameter scale`

---

