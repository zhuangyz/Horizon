---
layout: default
title: "Horizon Summary: 2026-03-01 (ZH)"
date: 2026-03-01
lang: zh
---

> From 24 items, 12 important content pieces were selected

---

1. [OpenAI 为 Anthropic 辩护，反对五角大楼将其列为供应链风险](#item-1) ⭐️ 8.0/10
2. [Google 对 Gemini CLI 的不透明封禁政策引发开发者担忧](#item-2) ⭐️ 8.0/10
3. [青龙面板遭.fullgc 挖矿木马植入，导致 CPU 占用率达 800%](#item-3) ⭐️ 8.0/10
4. [Meta 放弃高端 AI 芯片研发，1350 亿美元资本转向硬件投资](#item-4) ⭐️ 8.0/10
5. [美国国防部接受 OpenAI 安全准则，将在机密网络部署 AI](#item-5) ⭐️ 8.0/10
6. [五角大楼禁止军官就读常春藤盟校及卡内基梅隆等关键 AI 合作院校，2026 年起生效](#item-6) ⭐️ 8.0/10
7. [研究显示大模型在多轮对话中性能大幅下降，GPT-5 等前沿模型准确率损失达 33%](#item-7) ⭐️ 8.0/10
8. [Obsidian Sync 推出无头客户端，支持对知识库进行程序化访问和自动化。](#item-8) ⭐️ 7.0/10
9. [提出交互式解释作为对抗 AI 生成代码认知债的模式](#item-9) ⭐️ 7.0/10
10. [Google Chrome 默认下载约 4GB 本地 AI 模型 Gemini Nano](#item-10) ⭐️ 7.0/10
11. [韩国国税厅误曝硬件钱包助记词，导致 480 万美元代币被转走](#item-11) ⭐️ 7.0/10
12. [摩托罗拉内部文件泄露暗示与 GrapheneOS 合作，首款非 Pixel 设备或于 2027 年推出](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI 为 Anthropic 辩护，反对五角大楼将其列为供应链风险](https://twitter.com/OpenAI/status/2027846016423321831) ⭐️ 8.0/10

OpenAI 公开表示，美国国防部不应将 Anthropic 指定为供应链风险，这凸显了两家 AI 公司在处理涉及军事 AI 使用的政府合同时采取的不同方法。此前，五角大楼在 Anthropic 坚持在其协议中保留道德护栏后，最近决定将该公司标记为“供应链风险”。 一家主要 AI 公司公开反对政府指定，这标志着硅谷的 AI 伦理原则与军事采购需求之间的裂痕正在加深，并可能为科技公司与政府谈判的方式开创先例。其结果可能影响未来的政府-AI 合作伙伴关系、监管方法，以及国家安全利益与企业道德政策之间的平衡。 核心分歧在于执行方式：Anthropic 寻求将其道德红线（反对自主武器和大规模监控）嵌入技术本身，而据报道，OpenAI 的合同依赖于法律语言，并相信政府不会违反商定的条款。五角大楼的“供应链风险”指定是一种正式机制，可以限制或排除供应商参与国防合同。

hackernews · golfer · Feb 28, 21:24

**背景**: Claude AI 的创造者 Anthropic 划定了“硬线”或道德红线，禁止在军事合同中使用其 AI 用于自主武器或大规模监控。美国国防部在部长 Pete Hegseth 的领导下，一直在推动减少对 AI 使用的限制。“供应链风险”指定是五角大楼使用的一种工具，用于标记那些其产品、服务或商业行为被认为对国家安全构成潜在威胁的供应商，从而允许实施合同限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wired.com/story/anthropic-supply-chain-risk-shockwaves-silicon-valley/">Anthropic Hits Back After US Military Labels It a 'Supply Chain Risk'</a></li>
<li><a href="https://decod.tech/en/news/anthropic-ai-ethics-military-use-stance">Anthropic 's Ethical Red Line : Resisting Unrestricted Military AI ...</a></li>
<li><a href="https://www.politico.com/news/2026/02/26/incoherent-hegseths-anthropic-ultimatum-confounds-ai-policymakers-00800135">‘Incoherent’: Hegseth’s Anthropic ultimatum confounds AI ... - POLITICO</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示了对 OpenAI 合同方法的怀疑，用户批评其依赖法律语言的做法与 Anthropic 的技术执行相比可能具有欺骗性且效果不佳。还有人担心五角大楼的“任何合法用途”条款赋予了过度且可自我解释的权力，并有一种观点认为政府正在惩罚采取更强有力道德措施的公司（Anthropic）。

**标签**: `#AI Ethics`, `#Government Contracts`, `#Military AI`, `#Corporate Responsibility`, `#Regulation`

---

<a id="item-2"></a>
## [Google 对 Gemini CLI 的不透明封禁政策引发开发者担忧](https://github.com/google-gemini/gemini-cli/discussions/20632) ⭐️ 8.0/10

Gemini CLI 的 GitHub 仓库中一场高参与度的讨论揭示，Google 一直在以涉嫌违反政策为由封禁用户账户，且通常不提供明确解释或有效的申诉流程。这些封禁似乎与使用第三方工具（例如 'antigravity'）与 Gemini CLI 的 OAuth 认证进行交互有关。 此事之所以重要，是因为不透明且自动化的执行措施为开发者带来了巨大的平台风险，可能导致其失去与主账户绑定的关键 Google 服务（如 Gmail）的访问权限。这反映了一个更广泛的行业趋势，即 AI 服务提供商在平衡安全、政策执行和用户信任方面面临挑战，这可能会抑制围绕其工具进行的创新和实验。 据报道，封禁遵循一种模式：初次封禁可能在提交表格后自动解除，但随后的自动标记可能导致永久封禁，且支持机器人只会引用服务条款（TOS）而不说明具体违规行为。社区指出，即使在执行开始数月后，Google 关于何为认证'搭便车'行为的政策措辞仍然模糊不清。

hackernews · RyanShook · Feb 28, 13:50

**背景**: Gemini CLI 是 Google 提供的一个命令行界面工具，允许开发者从终端与 Gemini 系列大语言模型（LLM）进行交互。它提供查询代码库、自动化工作流等功能。此处的'平台风险'指的是服务提供商的行为（如账户封禁）可能对开发者的项目或对其他集成服务的访问产生负面影响的潜在可能性。OAuth 是一种标准的授权协议，第三方工具可能会利用它与官方 CLI 进行交互。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(language_model)">Gemini (language model)</a></li>
<li><a href="https://geminicli.com/">Build, debug & deploy with AI | Gemini CLI</a></li>
<li><a href="https://www.softwareseni.com/identifying-and-assessing-risks-in-web-and-app-development/">Identifying and Assessing Risks in Web and App Development</a></li>

</ul>
</details>

**社区讨论**: 社区情绪普遍是担忧和批评的。主要观点包括：担心'连带损害'，即与 Gemini 相关的封禁可能导致用户无法访问其主要的 Google 账户（如 Gmail）；对不透明、自动化的执行以及缺乏人工申诉渠道感到沮丧；并怀疑该政策的真实目的是迫使用户为官方应用中未使用的配额付费，而非解决真正的滥用问题。讨论中还直接对比了 Anthropic 的 CLI 存在的类似问题。

**标签**: `#google-gemini`, `#platform-risk`, `#account-suspension`, `#developer-tools`, `#ai-ethics`

---

<a id="item-3"></a>
## [青龙面板遭.fullgc 挖矿木马植入，导致 CPU 占用率达 800%](https://t.me/zaihuapd/39934) ⭐️ 8.0/10

2026 年 2 月 7 日，多名用户发现青龙面板被植入名为.fullgc 的挖矿木马，导致服务器 CPU 占用率异常升至 800%。该木马通过篡改 config.sh 配置文件实现持久化，并能根据系统架构自动下载恶意程序。 此事影响重大，因为青龙面板是一款广泛使用的开源自动化工具，一旦被成功入侵，可能导致服务器上大规模、未经授权的加密劫持，给受害者带来高昂的云资源费用和性能下降等经济损失。这凸显了暴露在公网的服务所面临的安全风险，以及针对 DevOps 工具的恶意软件战术的演变。 安全分析判定该程序属于 SusMiner 家族，主要通过连接 XMR（门罗币）矿池进行非法挖矿。暴露于公网 IPv4 环境的服务器是其主要攻击目标，建议用户检查`/ql/data/db/`路径下的隐藏文件以进行排查。

telegram · zaihuapd · Feb 28, 13:16

**背景**: 青龙面板是一个支持 Python3、JavaScript、Shell 和 TypeScript 脚本的开源定时任务管理平台，常被开发者和管理员用于自动化任务。加密劫持是一种网络攻击，恶意软件秘密使用受害者的计算资源来挖掘加密货币，通常在后台静默运行而不被用户察觉。SusMiner 家族是一个已知的加密劫持恶意软件家族。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/whyour/qinglong">GitHub - whyour/qinglong: 支持 Python3、JavaScript、Shell、Typescript ...</a></li>
<li><a href="https://cybernews.com/hosting-hub/cryptojacking-how-to-detect-crypto-mining-malware/">Cryptojacking: how to detect crypto mining malware - Cybernews</a></li>

</ul>
</details>

**社区讨论**: GitHub 上已出现多例受害者报告和案例讨论，表明社区积极参与并确认了此次攻击的影响范围。社区情绪普遍担忧，用户们根据提供的路径（`/ql/data/db/`）分享检测方法和清理步骤。

**标签**: `#security`, `#malware`, `#cryptojacking`, `#server-security`, `#incident-report`

---

<a id="item-4"></a>
## [Meta 放弃高端 AI 芯片研发，1350 亿美元资本转向硬件投资](https://www.theinformation.com/articles/metas-internal-chip-design-efforts-hit-roadblocks) ⭐️ 8.0/10

Meta 因技术复杂性和制造风险，已放弃代号为 Olympus 的最先进自研 AI 芯片研发，转而开发简化版本。该公司已与 AMD 达成 600 亿美元采购协议，并与英伟达及谷歌签署供应或租用合同，同时计划到 2026 年资本支出最高达 1350 亿美元，其中大部分资金将用于芯片和服务器投资。 这对 Meta 而言是一次重大的战略转向，揭示了即使是科技巨头在开发定制 AI 芯片时也面临巨大挑战，并突显了它们对成熟半导体供应商的持续依赖。高达 1350 亿美元的资本重新分配投向硬件，表明尽管在自研芯片雄心上受挫，Meta 仍对 AI 基础设施做出了积极承诺，这将影响 AI 硬件供应链的竞争格局。 这一决定是由于 MTIA（Meta 训练与推理加速器）项目在软件稳定性和性能方面遇到了挑战。在缩减其最雄心勃勃的芯片计划的同时，Meta 仍致力于推进其芯片组合，并计划在今年分享更多进展。

telegram · zaihuapd · Feb 28, 23:11

**背景**: Meta 的 MTIA（Meta 训练与推理加速器）是一系列自研 AI 芯片，旨在更高效地处理公司独特的 AI 工作负载，并减少对英伟达等外部 GPU 供应商的依赖。开发定制 AI 芯片是一项复杂且资本密集的工作，不仅涉及硬件设计，还需要创建强大的软件栈并确保大规模制造的可靠性。谷歌（凭借 TPU）和亚马逊（凭借 Trainium/Inferentia）等大型科技公司也采取了类似策略，以掌控其 AI 基础设施并优化成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.meta.com/blog/next-generation-meta-training-inference-accelerator-AI-MTIA/">Our next generation Meta Training and Inference Accelerator</a></li>
<li><a href="https://dl.acm.org/doi/full/10.1145/3695053.3731409">Meta's Second Generation AI Chip: Model-Chip Co-Design and ...</a></li>

</ul>
</details>

**标签**: `#AI Hardware`, `#Semiconductor Industry`, `#Meta`, `#Capital Investment`, `#Supply Chain`

---

<a id="item-5"></a>
## [美国国防部接受 OpenAI 安全准则，将在机密网络部署 AI](https://t.me/zaihuapd/39939) ⭐️ 8.0/10

美国国防部已初步同意 OpenAI 提出的安全条件，包括禁止将其 AI 用于国内大规模监控和自主武器系统，以便在军方机密网络中部署其技术。此前，五角大楼公开批评竞争对手 Anthropic 提出的类似准则具有“意识形态”倾向，据报道这已导致政府停止使用 Anthropic 的 AI。 这标志着五角大楼在与领先 AI 公司合作进行敏感军事应用方面的重大转变，为国家安全领域 AI 部署所需的安全和伦理护栏设立了先例。它凸显了先进 AI 对国防日益增长的战略重要性，并表明企业关于伦理使用的政策如何影响政府采购决策并塑造竞争格局。 尽管尚未签署正式合同，但该协议授予了 OpenAI 保留云端部署及安全监控权的权利。OpenAI 声称其协议包含了比以往任何机密 AI 部署协议都更多的护栏，但具体的技术和监督机制尚未完全披露。

telegram · zaihuapd · Mar 1, 00:28

**背景**: OpenAI 和 Anthropic 开发的大型语言模型（LLM）是先进的 AI 系统，经过海量数据训练，能够生成类人文本、回答问题并执行任务。在政府或军方机密网络中部署此类模型需要严格的安全协议，以防止数据泄露并确保 AI 在定义的伦理和操作边界内运行。像 Anthropic 这样的公司制定了包含“红线”的使用政策，例如禁止大规模监控和自主武器，这已成为政府合同中的争议点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehill.com/policy/technology/5760495-pentagon-deal-openai-trump-hegseth-anthropic/">Pentagon reaches deal with OpenAI amid Anthropic beef - The Hill</a></li>
<li><a href="https://www.theguardian.com/technology/2026/feb/28/openai-us-military-anthropic">OpenAI to work with Pentagon after Anthropic dropped by Trump over ...</a></li>
<li><a href="https://www.databreachtoday.co.uk/openai-will-deploy-ai-in-us-military-classified-networks-a-30888">OpenAI Will Deploy AI in US Military Classified Networks</a></li>

</ul>
</details>

**标签**: `#AI Governance`, `#National Security`, `#OpenAI`, `#Defense Technology`, `#AI Ethics`

---

<a id="item-6"></a>
## [五角大楼禁止军官就读常春藤盟校及卡内基梅隆等关键 AI 合作院校，2026 年起生效](https://fortune.com/2026/02/28/pentagon-officer-education-ivy-league-schools-universities-partners-ai-space/) ⭐️ 8.0/10

美国国防部长皮特·赫格塞斯签署备忘录，宣布从 2026-2027 学年起，禁止军官前往哈佛、耶鲁、麻省理工学院等常春藤盟校及其他顶尖大学进修，卡内基梅隆大学等关键 AI 合作院校也受波及。国防部批评这些机构已成为反美情绪的工厂，并表示将停止投资于未能强化领导者作战能力或破坏美国价值观的院校，转而寻求与自由大学、乔治梅森大学等新伙伴合作。 这一政策转变可能严重破坏在人工智能和太空等关键技术领域长期存在的军事-学术合作，其中像卡内基梅隆大学这样的机构一直是关键合作伙伴。它可能重塑国防研发的人才输送渠道，并影响未来军事领导人接受高等教育的地点，进而对国家安全创新产生影响。 此次调整涉及多项高级军官奖学金与专业军事教育项目。虽然指令明确提出了意识形态原因，但它也影响了实际的合作伙伴关系，例如卡内基梅隆大学与美国陆军价值数千万美元的人工智能研究协议，不过对现有合同的具体影响尚不明确，因为陆军 AI 中心和太空军尚未就此发表评论。

telegram · zaihuapd · Mar 1, 01:03

**背景**: 专业军事教育项目是为军官提供的高级培训课程，通常包括在地方大学进行研究生学习，以培养战略思维和技术专长。像卡内基梅隆大学这样的机构，通过与美国陆军研究实验室签署的 7200 万美元合作研究协议等项目，已与美国军方建立了深厚的合作伙伴关系，尤其是在人工智能研究领域。常春藤盟校和其他精英大学传统上是高级军官寻求奖学金和高级学位的目的地。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fortune.com/2026/02/28/pentagon-officer-education-ivy-league-schools-universities-partners-ai-space/">Pentagon chief blocks officers from attending Ivy League schools and ...</a></li>
<li><a href="https://militaryembedded.com/ai/deep-learning/advancing-ai-solutions-is-part-of-carnegie-mellon-arl-72-million-research-agreement">Advancing AI solutions is part of Carnegie Mellon, ARL $72 ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Air_University_(United_States_Air_Force)">Air University (United States Air Force) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#military-policy`, `#ai-research`, `#academic-partnerships`, `#national-security`, `#education`

---

<a id="item-7"></a>
## [研究显示大模型在多轮对话中性能大幅下降，GPT-5 等前沿模型准确率损失达 33%](https://arxiv.org/abs/2505.06120) ⭐️ 8.0/10

最新研究表明，大型语言模型（LLMs）在多轮对话中的表现远逊于单次指令设置，平均性能降幅达 39%。即便以 GPT-5 为代表的前沿模型，在处理跨多轮消息的任务时，准确率损失仍高达 33%。研究发现模型往往在对话早期做出错误假设且难以自我修复，导致其在复杂交互中“迷失”。 这一发现至关重要，因为多轮对话是 AI 助手、客户支持和教学系统等实际应用的基础。显著的性能下降突显了一个主要的可靠性瓶颈，这可能削弱用户信任，并限制即使是最高级大语言模型在现实世界中的部署。 研究表明，在 Python 编码等特定任务上表现略好，但降低采样温度等技术手段并不能有效解决该核心问题。研究人员建议，当对话偏离预期时，用户应通过总结此前需求并开启新对话的方式来重置模型状态。

telegram · zaihuapd · Mar 1, 02:19

**背景**: 多轮对话评估是衡量大语言模型现实世界交互能力的关键领域。MultiChallenge 和 MT-Bench 等基准测试旨在评估模型在多次交流中保持上下文和连贯性的能力。采样温度是一个控制大语言模型输出随机性的参数，较低的值会使响应更加确定。管理对话状态，即模型对对话历史的内部表示，是对话式 AI 中一个已知的挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2501.17399">MultiChallenge: A Realistic Multi-Turn Conversation Evaluation ... - arXiv</a></li>
<li><a href="https://arxiv.org/abs/2402.05201">The Effect of Sampling Temperature on Problem Solving in ...</a></li>
<li><a href="https://martinb-ai.github.io/Agentic-Prototyping/1_6_conversational_state.html">Conversation state — Agentic Prototyping - martinb-ai.github.io</a></li>

</ul>
</details>

**标签**: `#LLM`, `#AI Research`, `#Conversational AI`, `#Model Evaluation`, `#GPT-5`

---

<a id="item-8"></a>
## [Obsidian Sync 推出无头客户端，支持对知识库进行程序化访问和自动化。](https://help.obsidian.md/sync/headless) ⭐️ 7.0/10

热门笔记应用 Obsidian 的付费同步服务 Obsidian Sync 发布了一个新的“无头客户端”。该客户端允许开发者和高级用户通过编程方式访问和操作他们的 Obsidian 知识库（笔记集合），而无需使用图形用户界面。 此举意义重大，因为它开启了服务器端自动化、与其他工具的集成以及高级工作流，例如将 Obsidian 知识库用作检索增强生成（RAG）AI 系统的数据源或用于自动化博客发布。它将 Obsidian 从一个纯粹面向用户的应用转变为一个可编程的知识管理平台。 该无头客户端是付费订阅服务 Obsidian Sync 的一部分，这意味着程序化访问需要订阅 Sync 服务。与此同时，Obsidian 还发布了一个独立的命令行界面（CLI）工具，进一步扩展了其对开发者的自动化能力。

hackernews · adilmoujahid · Feb 28, 16:31

**背景**: Obsidian 是一款流行的、本地存储的笔记应用，使用 Markdown 文件。用户在一个称为“知识库”的文件夹内组织笔记。Obsidian Sync 是一项独立的可选服务，用于跨设备同步这些知识库。“无头”架构在内容管理系统中很常见，指的是将后端（数据和逻辑）与前端（用户界面）分离，允许通过 API 访问后端，以便在不同的上下文中使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techtarget.com/searchapparchitecture/tip/An-overview-of-headless-architecture-design">An overview of headless architecture design - TechTarget What is a Headless Architecture? Definition, Examples, & More What is a headless architecture? Pros & cons | Hygraph Headless Architecture: Benefits, Best Practices, Challenges ... What is Headless Architecture? (with Examples ... - ButterCMS What is Headless Arhitecture and How Does it Work? - Embeddable An overview of headless architecture design - TechTarget What is Headless Arhitecture and How Does it Work? - Embeddable What is Headless Architecture ? (with Examples & Comparisons ... - B… What is Headless Arhitecture and How Does it Work? - Embeddable What Is Headless Architecture? Benefits and Risks - Naturaily</a></li>
<li><a href="https://sesamedisk.com/obsidian-sync-headless-client-automation/">Obsidian Sync Headless Client: Automation Unlocked</a></li>

</ul>
</details>

**社区讨论**: 社区反应非常积极，用户对解锁自动化功能感到兴奋。提到的关键用例包括服务器端自动化、将知识库用于 RAG 系统以及自动化博客发布。一位项目团队成员也参与了讨论，表示愿意回答问题。一些用户还同时提到了 CLI 工具的发布，并表达了希望无需完整知识库设置即可编辑单个文件的愿望。

**标签**: `#obsidian`, `#automation`, `#markdown`, `#developer-tools`, `#sync`

---

<a id="item-9"></a>
## [提出交互式解释作为对抗 AI 生成代码认知债的模式](https://simonwillison.net/guides/agentic-engineering-patterns/interactive-explanations/#atom-everything) ⭐️ 7.0/10

Simon Willison 引入了'认知债'这一概念，指当开发者对 AI 智能体生成的代码失去理解时所积累的债务，并提出'交互式解释'作为一种具体的工程模式来缓解此问题。他通过创建一个动画可视化来解释 AI 生成的 Rust 词云应用中使用的'阿基米德螺旋放置'算法，演示了这种模式。 这很重要，因为随着 AI 智能体编写更多生产代码，认知债有可能创造出开发者无法自信推理的黑盒系统，从而像技术债一样拖慢开发进度。交互式解释模式通过提供直观的理解机制来帮助保持开发者的专业知识和系统理解力，解决了 AI 辅助开发中的一个关键缺口。 交互式解释被实现为一个带有动画控制功能的 HTML 页面，可逐步可视化词云生成算法，包括用于暂停、速度调整和逐帧步进的滑块。这种方法将'带有每词随机角度偏移的阿基米德螺旋放置'等抽象算法描述转化为直观的可视化演示，从而建立真正的理解。

rss · Simon Willison · Feb 28, 23:09

**背景**: 认知债是一个新兴概念，描述了当问题解决从人类转移到 AI 算法时所积累的专业知识损失，特别是在软件开发领域。智能体工程指的是与 AI 编码智能体有效协作的编码实践和模式，强调将其作为工具而非端到端的代码生成器。该术语由 OpenAI 联合创始人 Andrej Karpathy 推广，代表了从'氛围编码'向更有意识、基于模式的 AI 辅助开发方法的转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://margaretstorey.com/blog/2026/02/09/cognitive-debt/">How Generative and Agentic AI Shift Concern from Technical Debt to Cognitive Debt</a></li>
<li><a href="https://simonwillison.net/2026/Feb/23/agentic-engineering-patterns/">Writing about Agentic Engineering Patterns - simonwillison.net</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-engineering">What is agentic engineering? - IBM</a></li>

</ul>
</details>

**标签**: `#agentic-ai`, `#software-engineering`, `#cognitive-debt`, `#ai-assisted-development`, `#explainability`

---

<a id="item-10"></a>
## [Google Chrome 默认下载约 4GB 本地 AI 模型 Gemini Nano](https://winaero.com/google-chrome-secretly-downloads-huge-local-ai-models/) ⭐️ 7.0/10

Google Chrome 浏览器被发现在默认配置下自动下载一个名为 'weights.bin' 的大型本地 AI 模型文件（约 4GB）。该文件包含 Gemini Nano 模型，用于支持浏览器内置的 Prompt API、翻译和摘要等功能。 这标志着浏览器架构的重大转变，将 AI 处理从云端转移到本地设备，这可以提高响应速度并保护用户隐私。然而，未经用户明确同意就自动进行大规模下载，立即引发了数亿 Chrome 用户对存储占用、数据透明度和控制权的担忧。 该模型在网站首次使用 Prompt API 时被单独下载，并存储在本地以实现离线 AI 功能。用户可以通过浏览器的实验性标志禁用此行为，并手动删除文件以释放空间，但这会导致相关的 AI 功能失效。

telegram · zaihuapd · Feb 28, 05:02

**背景**: Gemini Nano 是 Google Gemini 大语言模型（LLM）家族中的一个轻量级、高效版本，专门设计用于在设备上本地运行。Prompt API 是 Chrome 内置 AI 团队提出的一种新的标准化浏览器 API，允许 Web 应用程序访问设备的本地 AI 模型，以执行摘要和翻译等任务。.bin 文件（如 weights.bin）是一种常见的文件格式，用于存储训练好的 AI 模型的数值参数，即'权重'。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/ai/prompt-api">The Prompt API | AI on Chrome | Chrome for Developers</a></li>
<li><a href="https://developer.android.com/ai/gemini-nano">Gemini Nano | AI | Android Developers</a></li>
<li><a href="https://medium.com/@ch.mittendorf/navigating-model-weight-file-formats-safetensors-bin-pt-hdf5-and-beyond-97266a621bdf">Navigating Model Weight File Formats: .safetensors, .bin, .pt, HDF5 ...</a></li>

</ul>
</details>

**标签**: `#Google Chrome`, `#AI Models`, `#Privacy`, `#Browser`, `#Gemini`

---

<a id="item-11"></a>
## [韩国国税厅误曝硬件钱包助记词，导致 480 万美元代币被转走](https://www.mk.co.kr/cn/stock/11974731) ⭐️ 7.0/10

韩国国税厅近日在公布现场搜查成果的新闻资料中，未加遮挡地完整公开了一台被查封的 Ledger 硬件钱包的助记词。这导致该钱包内价值约 480 万美元的 400 万个 PRTG 代币被转走，但约 20 小时后，代币被全部退回原钱包。 这一事件暴露了政府机构在处理查封的数字资产时，在基础安全协议上存在严重失误，损害了公众信任。它尖锐地提醒人们助记词（加密货币钱包的主密钥）安全的重要性，并展示了即使流动性极低的代币也可能成为目标。 受影响的至少 3 个钱包自 2023 年 1 月以来就不活跃，它们合计持有 PRTG 代币总供应量的 40%。PRTG 代币流动性极低，仅在 MEXC 交易所上线，日成交额约 332 美元，卖出价值 59 美元的代币就可能导致价格下跌 2%。

telegram · zaihuapd · Feb 28, 11:27

**背景**: 助记词（或种子短语）是一个由 12-24 个单词组成的序列，用于生成加密货币钱包的所有私钥和地址，是钱包的终极备份。像 Ledger 这样的硬件钱包是物理设备，旨在将私钥离线存储以增强安全性，但助记词本身必须绝对保密，绝不能以数字形式暴露。一旦助记词泄露，无论硬件设备在谁手中，任何人都可以完全控制相关资产。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theblock.co/post/391578/south-korea-tax-service-reveals-crypto-wallet-recovery-phrase-report">South Korea tax service reveals crypto wallet recovery phrase in press release, seized tokens moved in suspected breach: report | The Block</a></li>
<li><a href="https://learnmeabitcoin.com/technical/keys/hd-wallets/mnemonic-seed/">Mnemonic Seed | Source of Keys in an HD Wallet - Learn Me A Bitcoin</a></li>
<li><a href="https://guarda.com/academy/tutorials/mnemonic-wallet-phrases-what-are-they-for/">Mnemonic Wallet Phrases: What Are They and How to Import? - Guarda</a></li>

</ul>
</details>

**标签**: `#cryptocurrency`, `#security`, `#government`, `#blockchain`, `#hardware-wallet`

---

<a id="item-12"></a>
## [摩托罗拉内部文件泄露暗示与 GrapheneOS 合作，首款非 Pixel 设备或于 2027 年推出](https://grapheneos.social/@GrapheneOS/116115497756691311) ⭐️ 7.0/10

一张最初发布在 Reddit 上的摩托罗拉内部演示文稿截图泄露，其中将 GrapheneOS 列入了该公司的安全功能板块，强烈暗示双方已达成合作。随后，GrapheneOS 官方账号在 Mastodon 上确认，关于 OEM 合作伙伴的公告定于 2026 年 3 月发布，相关设备计划在 2027 年推出。 这标志着 GrapheneOS 突破了长期以来仅支持 Google Pixel 设备的限制，是一次关键的扩张，可能使其高安全性、注重隐私的操作系统惠及更广泛的用户群。与摩托罗拉这样隶属于联想集团、且专注于企业安全业务的主要 OEM 厂商合作，可能会在注重安全性和企业市场中，对标准 Android 的主导地位构成重大挑战。 泄露的截图很快被 r/GrapheneOS 版块的版主删除，但已广泛传播。截至目前，GrapheneOS 和摩托罗拉双方均未就泄露内容发表官方声明，不过官方 Mastodon 帖子中透露的时间线增加了合作传闻的可信度。

telegram · zaihuapd · Feb 28, 12:38

**背景**: GrapheneOS 是一个基于 Android 开源项目 (AOSP)、专注于隐私和安全性的开源操作系统。它以其强化的安全功能而闻名，例如用于硬件验证的 Auditor 应用以及许多尚未包含在原生 Android 中的内核补丁。由于 Google Pixel 手机强大的硬件安全能力，GrapheneOS 历史上仅官方支持该系列设备。隶属于联想集团的摩托罗拉近年来一直在加强其企业移动性和安全解决方案，提供如 moto-safe 等商业设备管理产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.webpronews.com/grapheneos-expands-to-snapdragon-devices-via-oem-partnership-by-2026/">GrapheneOS Expands to Snapdragon Devices via OEM Partnership ...</a></li>
<li><a href="https://reclaimthenet.org/grapheneos-expands-beyond-pixel-phones-with-new-android-partner">GrapheneOS Plans Partnership with Major Android OEM to Expand ...</a></li>
<li><a href="https://www.allthingssecured.com/identity-protection/android-vs-grapheneos-compared/">Android vs GrapheneOS: Privacy, Security & Features Compared</a></li>

</ul>
</details>

**标签**: `#Mobile Security`, `#Privacy`, `#GrapheneOS`, `#Android`, `#Motorola`

---