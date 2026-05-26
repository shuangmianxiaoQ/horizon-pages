---
layout: default
title: "Horizon Summary: 2026-05-26 (ZH)"
date: 2026-05-26
lang: zh
---

> From 36 items, 16 important content pieces were selected

---

1. [GitHub Actions 再次宕机](#item-1) ⭐️ 8.0/10
2. [荷兰阻止关键数字供应商被收购](#item-2) ⭐️ 8.0/10
3. [离体人脑用于药物测试](#item-3) ⭐️ 8.0/10
4. [欧盟初步认定谷歌或违反 DMA](#item-4) ⭐️ 8.0/10
5. [更慢但更好的 AI 编程](#item-5) ⭐️ 7.0/10
6. [法拉利首款纯电车型](#item-6) ⭐️ 7.0/10
7. [日本完成 Mach-5 冲压发动机试验](#item-7) ⭐️ 7.0/10
8. [中国审查 Meta 收购 Manus](#item-8) ⭐️ 7.0/10
9. [支付宝发布 Token Pay 和 AI 钱包](#item-9) ⭐️ 7.0/10
10. [DynIP 带来 RFC 2136、IPv6 和 DNSSEC 动态 DNS](#item-10) ⭐️ 6.0/10
11. [How Shamir's Secret Sharing Works](#item-11) ⭐️ 6.0/10
12. [MiniCPM5-1B](#item-12) ⭐️ 6.0/10
13. [📱 X 打击内容搬运，收益将划归原创者](#item-13) ⭐️ 6.0/10
14. [🤖 马斯克称 xAI 将于年底前开源 0.5T 参数模型，外界推测或为 Grok 4.2](#item-14) ⭐️ 6.0/10
15. [伊朗计划永久断开全球互联网，仅允许通过政府审查的人员上网  据伊朗数字权利活动人士透露，伊朗正计划永久断开与全球互联网的连接，仅允许通过政府审查的人员上网。](#item-15) ⭐️ 6.0/10
16. [🦘 美团发布跑腿 Skill，用户可用任意 AI 助手一句话下单](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [GitHub Actions 再次宕机](https://www.githubstatus.com/?today) ⭐️ 8.0/10

根据 GitHub 状态页，GitHub Actions 今天再次发生故障。此次事件再次引发了大家对部署风险、CI/CD 依赖以及核心自动化平台宕机时备用方案的讨论。 GitHub Actions 被广泛用于自动化构建、测试和部署，因此一次故障就可能同时阻塞许多项目的发布。此次讨论也凸显了更广泛的 DevOps 问题：即使团队自托管 runner，仍可能暴露在平台级可用性风险之下。 评论主要聚焦于运维影响，而不是技术根因，原始内容中也没有提供具体修复细节。几位评论者提到可以把更多流程留在 git 中，或者构建更简单的内部 CI/CD 自动化，以降低对 GitHub 的依赖。

hackernews · cebert · May 26, 11:42 · [社区讨论](https://news.ycombinator.com/item?id=48278374)

**背景**: GitHub Actions 是 GitHub 的工作流自动化系统，可以直接在仓库中运行任务。它通常用于 CI/CD，也就是持续集成代码变更、进行测试，并将其部署到生产环境。团队既可以使用 GitHub 托管的 runner，也可以使用自己管理的自托管 runner，但这两种方式都仍然依赖更广泛的 GitHub Actions 平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/actions">GitHub Actions documentation - GitHub Docs</a></li>
<li><a href="https://docs.github.com/en/actions/reference/runners/self-hosted-runners">Self-hosted runners reference - GitHub Docs</a></li>

</ul>
</details>

**社区讨论**: 整体语气既有抱怨也很务实：有人调侃任务失败，但核心担忧是 GitHub 不可用时部署会变得有风险。部分评论者建议通过 GitSocial 之类的工具或轻量级自建自动化来降低对 GitHub 的依赖，另一些人则指出，即使付费使用该服务，团队仍然需要准备应急方案。

**标签**: `#GitHub Actions`, `#CI/CD`, `#outage`, `#DevOps`, `#infrastructure reliability`

---

<a id="item-2"></a>
## [荷兰阻止关键数字供应商被收购](https://www.politico.eu/article/netherlands-blocks-us-takeover-vital-digital-supplier/) ⭐️ 8.0/10

荷兰已阻止一家美国公司收购一家被描述为对本国数字基础设施至关重要的数字供应商。此举源于外界对关键服务被外国控制、从而影响主权的担忧。 这表明欧洲政府在认为某家私营供应商过于关键、不能由境外控制时，可能会直接出手干预。此事关系到数字主权、网络安全，以及依赖少数基础设施供应商的公共服务韧性。 这一决定似乎与该供应商支撑关键国家数字系统的角色有关，而不是单纯的反并购立场。社区评论提到相关公司可能是 Solvinity，并称其托管荷兰电子身份系统 DigiD，这也解释了为什么这笔交易会引发政治关注。

hackernews · vrganj · May 26, 11:46 · [社区讨论](https://news.ycombinator.com/item?id=48278406)

**背景**: 数字主权指一个国家对支撑核心公共和私人服务的系统与供应商保持控制的能力。当某家供应商负责身份认证、托管或其他关键功能时，所有权问题就不只是商业问题，也会变成政策问题。这里的担忧是，关键数字提供商的控制权可能会影响国家服务的安全性和独立运行能力。

**社区讨论**: 评论者总体上欢迎这一阻止行动，认为它早就应该发生，并批评政府此前过于沉默。也有人质疑为什么如此关键的基础设施仍由私人持有，还有人把这件事看作欧洲逐步摆脱美国技术栈的一部分。

**标签**: `#digital sovereignty`, `#cybersecurity`, `#European tech policy`, `#critical infrastructure`, `#Hacker News`

---

<a id="item-3"></a>
## [离体人脑用于药物测试](https://www.science.org/content/article/not-alive-not-dead-disembodied-human-brains-used-drug-testing) ⭐️ 8.0/10

《Science》报道了一项研究：捐献的人脑在死亡数小时后通过灌流被恢复出部分代谢和细胞活动，并被用于药物测试。该研究借助 Bexorg 的 BrainEx 灌流系统，尝试评估阿尔茨海默病和帕金森病等疾病的候选药物。 如果这种方法被证明可靠，它可能为神经药物研发提供比动物模型更接近真实的人类组织，从而提高找到有效疗法的概率。与此同时，它也把医学推向关于意识、死亡以及何种组织使用需要新伦理规则的未定边界。 研究团队强调，这些大脑没有恢复意识，也没有恢复完整神经活动，但在灌流后确实出现了有限的功能迹象。其主要技术限制和伦理争议在于，这类组织既不能被简单视为完全死亡，也不能被视为整体意义上的“活着”。

telegram · zaihuapd · May 25, 14:57

**背景**: “离体”是指在人体之外对组织进行操作，而“灌流”则是让液体在器官中循环，以提供氧气和营养。神经科学之所以探索这类系统，是因为活体人脑组织通常无法直接用于测试，而动物模型又常常难以真实反映人类疾病的复杂性。这个新闻还涉及脑死亡、器官捐献知情同意，以及局部组织活动是否会改变研究对象道德地位的讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tno-pharma.com/Ex_vivo.html">Ex vivo Organ</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC10409188/">Hemiparkinsonism-Hemiatrophy Syndrome with Hypoperfusion in Basal...</a></li>

</ul>
</details>

**标签**: `#神经科学`, `#生物技术`, `#药物研发`, `#医学伦理`, `#脑灌流`

---

<a id="item-4"></a>
## [欧盟初步认定谷歌或违反 DMA](https://t.me/zaihuapd/41566) ⭐️ 8.0/10

欧盟委员会表示，Alphabet 可能因在搜索中优先展示谷歌自家服务，以及限制开发者将用户引导至其他购买渠道，而违反《数字市场法》（DMA）。谷歌虽然已经做出一些调整以求合规，但欧盟委员会认为这些措施仍然不够。 如果这一认定最终成立，谷歌可能被迫改变搜索中购物、航班和酒店结果的呈现方式，以及 Play 商店对外部支付和应用分发的规则。这也是欧盟检验 DMA 是否能够真正约束看门人平台的重要案例。 此案主要涉及两个 DMA 关注点：搜索中的自我偏好，以及 Play 商店对开发者引导用户的限制。欧盟委员会的表态说明，谷歌的整改措施尚未达到欧盟预期，但这仍然只是初步结论，不是最终裁决。

telegram · zaihuapd · May 26, 00:27

**背景**: 《数字市场法》（DMA）是欧盟用来让数字市场更公平、竞争性更强的一部法律。它主要约束那些被视为“看门人”的大型平台，因为这些平台规模巨大、控制力很强，可能让竞争对手更难进入市场。搜索中的“自我偏好”是指平台可能把自家服务放在比竞争服务更显眼的位置。应用商店中的“开发者引导”则是指允许开发者把用户带到其他购买方式，例如自家网站或其他应用商店。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://digital-markets-act.ec.europa.eu/index_en">Digital Markets Act</a></li>
<li><a href="https://appleinsider.com/articles/24/01/16/apples-app-store-anti-steering-rules-are-gone-but-the-replacement-isnt-much-better">Apple App Store replaces anti-steering rules</a></li>

</ul>
</details>

**标签**: `#EU regulation`, `#Google`, `#Digital Markets Act`, `#antitrust`, `#app stores`

---

<a id="item-5"></a>
## [更慢但更好的 AI 编程](https://nolanlawson.com/2026/05/25/using-ai-to-write-better-code-more-slowly/) ⭐️ 7.0/10

这篇文章主张，AI 辅助编程在更刻意、更迭代的流程里效果最好：先设计实现方案，再生成代码，然后审查并反复修改。它反对“AI 编程就一定要追求极致速度”或“完全交给智能体一次跑完”的思路。 这很重要，因为很多开发者都在用 AI 工具追求更快交付，但文章指出，速度可能会牺牲对边界情况、架构匹配度和最终质量的把握。若流程设计得当，LLM 也可能在放慢节奏的同时提升代码质量和可维护性。 核心观点是让人始终参与其中，并在多个阶段使用 AI，而不是只把它当作补全工具或完全自治的编码者。评论区也体现了这种取舍：有些读者把 AI 用在方案设计、实现和审查的多轮循环里，另一些人则认为这种来回调整往往比手写代码更耗时。

hackernews · signa11 · May 25, 23:16 · [社区讨论](https://news.ycombinator.com/item?id=48272984)

**背景**: 在软件工程中，代码审查是指在合并之前检查变更中的漏洞、边界情况、风格问题和设计问题。智能体式软件开发则是让 AI 智能体承担更多端到端责任，从理解需求说明到生成并检查结果。LLM 辅助审查是一种新兴模式，它把模型放在实现之后作为第二遍检查，而不是完全替代开发者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcommunity.microsoft.com/blog/appsonazureblog/an-ai-led-sdlc-building-an-end-to-end-agentic-software-development-lifecycle-wit/4491896">An AI led SDLC: Building an End-to-End Agentic Software ...</a></li>
<li><a href="https://arxiv.org/html/2505.16339v1">Rethinking Code Review Workflows with LLM Assistance: An Empirical Study</a></li>
<li><a href="https://medium.com/quantumblack/agentic-workflows-for-software-development-dc8e64f4a79d">Agentic workflows for software development - Medium</a></li>

</ul>
</details>

**社区讨论**: 评论区整体偏务实，但观点分化明显。几位评论者表示，他们现在会把 AI 放进设计、实现和审查的长迭代流程里；也有人认为智能体式编程会掩盖关键的微架构决策，并降低对边界情况的信心。还有少数人反驳文章的表述，认为只要经过仔细审查，LLM 也能产出高质量代码。

**标签**: `#AI coding`, `#code review`, `#developer productivity`, `#LLMs`, `#software engineering`

---

<a id="item-6"></a>
## [法拉利首款纯电车型](https://www.ferrari.com/en-EN/auto/ferrari-luce) ⭐️ 7.0/10

法拉利发布了 Luce，这被描述为该公司首款纯电动汽车。此次发布引发了 Hacker News 上的大量讨论，焦点集中在车型设计、潜在买家以及电动车对法拉利品牌意味着什么。 这对法拉利来说是一个重要转向，因为它表明即使是超豪华性能品牌也在迈向全面电动化。它不仅影响汽车消费者，也影响更广泛的电动车行业，因为品牌形象、定价和设计预期如今和续航、加速一样，都是竞争的一部分。 现有材料没有提供具体技术参数，因此目前能确认的核心信息只有一点：Luce 是法拉利的首款纯电车型。围绕它的讨论也显示，这次发布被评判的不只是动力系统技术，还有外观设计和市场定位是否匹配。

hackernews · jumploops · May 25, 21:00 · [社区讨论](https://news.ycombinator.com/item?id=48271629)

**背景**: 电动车（EV）使用电动机和电池，而不是传统内燃机。对于法拉利这样的品牌来说，推出纯电车型会引出一个问题：如何在电动化的同时保留消费者对这个名字所联想到的视觉风格和情感认同。它也让法拉利进入一个豪华电动车市场，在这个市场里，性能和身份象征同样重要。

**社区讨论**: 讨论整体上非常热烈，但态度偏向分裂和怀疑。一些评论者认为外观过于普通，几乎失去了法拉利的品牌辨识度；也有人认为目标买家并不是传统法拉利车主，这款车仍然可能作为身份象征获得成功。

**标签**: `#electric-vehicles`, `#automotive`, `#Ferrari`, `#product-launch`, `#industry-discussion`

---

<a id="item-7"></a>
## [日本完成 Mach-5 冲压发动机试验](https://www.bgr.com/2178211/japan-hypersonic-engine-ramjet-2-hour-flights-to-us/) ⭐️ 7.0/10

据报道，日本完成了一次面向 Mach-5 飞行器的冲压发动机成功试验。报道将这次测试描述为高超音速推进的一步进展，而不是整机飞行演示。 冲压发动机试验成功很重要，因为这表明人们在高超音速空气吸气推进方面仍在持续推进。即使只是渐进式进展，也会影响需要在极高马赫数下高效工作的航空航天和防务项目。 冲压发动机是一种结构较简单的吸气式发动机，没有主要运动部件，它依靠飞行器的前进速度来压缩进气并进行燃烧。网页资料指出，冲压发动机在大约 Mach 3 的超音速区间效率最高，且可工作到大约 Mach 6，这也解释了为什么 Mach-5 应用在技术上可行，但已经接近其工作边界。

hackernews · rmason · May 25, 19:43 · [社区讨论](https://news.ycombinator.com/item?id=48270812)

**背景**: 马赫数表示相对于音速的速度，因此 Mach 5 大约就是音速的 5 倍。冲压发动机与传统喷气发动机不同，因为它不需要同样形式的压气机转子，但它要求飞行器先达到足够高的速度，才能让进气压缩正常工作。正因为如此，它常被用于高速飞行、导弹以及其他高超音速概念。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ramjet">Ramjet - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hypersonic_flight">Hypersonic flight - Wikipedia</a></li>
<li><a href="https://www.grc.nasa.gov/WWW/k-12/airplane/ramth.html">Ramjet / Scramjet Thrust - NASA</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为这项结果在技术上有意思，但算不上革命性，并指出冲压发动机概念已经有几十年历史，类似性能也早已存在于军事系统中。讨论还集中在实际用途上，有人认为它更可能用于导弹和威慑场景，而不是客机；也有人质疑 Mach-5 飞行器是否真的是最终目标。

**标签**: `#hypersonics`, `#ramjet`, `#aerospace`, `#defense`, `#propulsion`

---

<a id="item-8"></a>
## [中国审查 Meta 收购 Manus](https://t.me/zaihuapd/41577) ⭐️ 7.0/10

中国监管部门正在审查 Meta 收购 AI 初创公司 Manus 是否违反投资规定。英国《金融时报》援引知情人士称，Manus 首席执行官 Xiao Hong 和首席科学家 Ji Yichao 在北京与国家发展和改革委员会会面后，被告知不得离境，但仍可在中国境内出行。 这一事件显示，跨境 AI 并购可能引发中国的投资与合规审查，尤其是在涉及外国买家的情况下。若审查进一步升级为执法或限制措施，可能影响全球科技公司未来与中国 AI 初创企业的交易设计。 据称 Meta 在去年 12 月宣布收购 Manus，但交易金额未公开。Manus 被描述为开发通用型 AI 智能体的公司，而 AI 智能体通常指能够感知环境、进行推理、调用工具并自主执行任务的软件。

telegram · zaihuapd · May 26, 09:56

**背景**: AI 智能体不同于普通聊天机器人，它的目标不仅是回答问题，还包括围绕目标自动执行动作。中国的跨境并购和外商投资可能受到监管审查，尤其是在需要核查是否符合投资规定以及是否涉及国家利益时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/2031061805380920973">AI智能体（AI Agent）完整指南：概念、类型与应用</a></li>
<li><a href="https://press.anu.edu.au/downloads/press/p184401/pdf/ch064.pdf">press.anu.edu.au/downloads/press/p184401/pdf/ch064.pdf</a></li>

</ul>
</details>

**标签**: `#AI政策`, `#跨境并购`, `#中国监管`, `#Meta`, `#创业公司`

---

<a id="item-9"></a>
## [支付宝发布 Token Pay 和 AI 钱包](https://finance.sina.com.cn/jjxw/2026-05-26/doc-inhzffss1524895.shtml) ⭐️ 7.0/10

支付宝在 5 月 26 日发布了 Token Pay 和 AI 钱包。用户现在可以在支付宝内搜索“AI 钱包”体验，用于管理智能体任务的支付流程，并在支付后查看账单。 这次发布表明，主流金融科技平台开始为 AI 智能体而不仅是人类用户构建支付基础设施。如果被广泛采用，它可能会影响 AI 应用的订阅变现方式，以及用户对自动化支出的授权流程。 Token Pay 面向大模型公司，支持全球用户订阅、应用内充值 Token 等场景。支付宝表示，MiniMax 和阶跃星辰已经与其合作，多个 AI 原生产品将采用这一支付方案。

telegram · zaihuapd · May 26, 12:31

**背景**: AI 钱包正在成为一种让用户把支付动作交给软件智能体处理，同时仍保留控制权和账单可见性的方式。Token 计费在 AI 服务里也很常见，因为它把费用和实际使用量绑定起来，而不是采用固定月费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unite.ai/stripe-hands-ai-agents-a-wallet-ushering-in-agentic-purchasing/">Stripe Hands AI Agents a Wallet, Ushering In Agentic ...</a></li>
<li><a href="https://www.kinde.com/learn/billing/billing-for-ai/payment-acceptance-for-ai-companies/">Kinde Payment Acceptance for AI Companies: Usage-Based and Tokenized Billing Models</a></li>
<li><a href="https://www.coinbase.com/developer-platform/discover/launches/agentic-wallets">Introducing Agentic Wallets: Give Your Agents the Power of ...</a></li>

</ul>
</details>

**标签**: `#AI payments`, `#fintech`, `#Alipay`, `#tokenization`, `#agentic AI`

---

<a id="item-10"></a>
## [DynIP 带来 RFC 2136、IPv6 和 DNSSEC 动态 DNS](https://dynip.dev/) ⭐️ 6.0/10

DynIP 推出了一个围绕 RFC 2136/TSIG 更新构建的动态 DNS 服务，并支持端到端 IPv6 和 DNSSEC。对于不原生支持 DNS UPDATE 的设备，它还提供 HTTP API，适用于常见路由器和自托管环境。 这之所以重要，是因为许多动态 DNS 服务仍沿用较旧的、仅支持 HTTP 的工作方式，且对 IPv6 支持不足，这限制了它们在现代网络中的实用性。DynIP 可能会让网络工程师、自托管用户以及运行 BIND、FortiGate、MikroTik 或 Kubernetes 相关 DNS 工具的管理员更容易实现自动化域名更新。 DynIP 将 RFC 2136 更新作为一等路径，这意味着 FortiGate 的 generic DDNS 和 MikroTik 的 `/tool dns-update` 等设备可以无需自定义客户端直接使用。社区评论还提到它与 `external-dns` 兼容性很好，同时也有人指出，对于偏好自托管的用户，BIND 本身已经支持 RFC 2136 和 DNSSEC。

hackernews · dynip · May 26, 07:35 · [社区讨论](https://news.ycombinator.com/item?id=48276363)

**背景**: RFC 2136 定义了一种通过向允许更新的区域发送 DNS UPDATE 消息来动态修改 DNS 记录的方法。TSIG 通过事务签名为这些更新增加认证能力，使用共享密钥来验证请求。DNSSEC 则通过给 DNS 记录添加加密签名来保护数据，帮助客户端验证返回结果没有在传输过程中被篡改。实际上，当 IP 地址经常变化但域名又需要保持最新时，这些功能会非常有用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datatracker.ietf.org/doc/html/rfc2136">RFC 2136 - Dynamic Updates in the Domain Name System (DNS UPDATE)</a></li>
<li><a href="https://www.rfc-editor.org/rfc/rfc8945">RFC 8945: Secret Key Transaction Authentication for DNS ( TSIG )</a></li>
<li><a href="https://www.cloudflare.com/learning/dns/dnssec/how-dnssec-works/">How does DNSSEC work?</a></li>

</ul>
</details>

**社区讨论**: 讨论整体上偏正面，不少评论者欢迎这一领域出现更多竞争，并认可其对 RFC 2136 的重视。主要话题集中在与 `external-dns` 等工具的互操作性、自托管用户的积极反馈，以及一个现实问题：并不是每台路由器都能直接支持 DNS UPDATE，因此有些用户仍需要 HTTP 到 DNS UPDATE 的转换方案。

**标签**: `#dynamic DNS`, `#DNSSEC`, `#IPv6`, `#RFC 2136`, `#networking`

---

<a id="item-11"></a>
## [How Shamir's Secret Sharing Works](https://ente.com/blog/how-shamirs-secret-sharing-works/) ⭐️ 6.0/10

This article explains how Shamir's Secret Sharing works and why it provides both secrecy and redundancy for distributing sensitive data.

hackernews · subract · May 25, 22:37 · [社区讨论](https://news.ycombinator.com/item?id=48272715)

**标签**: `#cryptography`, `#secret-sharing`, `#security`, `#data-protection`, `#Shamir's Secret Sharing`

---

<a id="item-12"></a>
## [MiniCPM5-1B](https://www.producthunt.com/products/minicpm-4-0) ⭐️ 6.0/10

MiniCPM5-1B is presented as a new state-of-the-art compact open model designed for edge use.

rss · Product Hunt · May 26, 03:07

**标签**: `#llm`, `#edge-ai`, `#open-models`, `#small-models`, `#product-launch`

---

<a id="item-13"></a>
## [📱 X 打击内容搬运，收益将划归原创者](https://www.businessinsider.com/x-cracks-down-on-stolen-content-nikita-bier-2026-5) ⭐️ 6.0/10

X is cracking down on accounts that repost stolen content to game creator earnings, and says revenue will now be directed to the original creators.

telegram · zaihuapd · May 26, 01:22

**标签**: `#X`, `#content moderation`, `#creator monetization`, `#platform policy`, `#copyright`

---

<a id="item-14"></a>
## [🤖 马斯克称 xAI 将于年底前开源 0.5T 参数模型，外界推测或为 Grok 4.2](https://x.com/i/status/2058796067592736866) ⭐️ 6.0/10

Musk reportedly said xAI will open-source a 0.5T-parameter model by the end of the year, with outside speculation that it may be Grok 4.2.

telegram · zaihuapd · May 26, 02:46

**标签**: `#xAI`, `#Grok`, `#open-source models`, `#large language models`, `#AI news`

---

<a id="item-15"></a>
## [伊朗计划永久断开全球互联网，仅允许通过政府审查的人员上网  据伊朗数字权利活动人士透露，伊朗正计划永久断开与全球互联网的连接，仅允许通过政府审查的人员上网。](https://t.me/zaihuapd/41574) ⭐️ 6.0/10

The report says Iran is planning to permanently sever global internet access for most users and restrict connectivity to government-approved individuals through a filtered domestic network.

telegram · zaihuapd · May 26, 06:36

**标签**: `#internet censorship`, `#digital rights`, `#Iran`, `#network isolation`, `#government surveillance`

---

<a id="item-16"></a>
## [🦘 美团发布跑腿 Skill，用户可用任意 AI 助手一句话下单](http://client.sina.com.cn/news/2026-05-26/doc-inhzffss1481138.shtml) ⭐️ 6.0/10

Meituan has launched a "跑腿 Skill" that lets users place delivery/errand orders through any AI assistant using natural language, with core ordering capabilities exposed via a standard interface.

telegram · zaihuapd · May 26, 08:29

**标签**: `#AI assistants`, `#agentic workflows`, `#local services`, `#platform integration`, `#e-commerce`

---
