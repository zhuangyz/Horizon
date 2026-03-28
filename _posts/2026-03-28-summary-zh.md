---
layout: default
title: "Horizon Summary: 2026-03-28 (ZH)"
date: 2026-03-28
lang: zh
---

> From 27 items, 9 important content pieces were selected

---

1. [西班牙全部 8,642 部法律被转换为 Git 仓库，每次法律修订都是一个提交记录](#item-1) ⭐️ 8.0/10
2. [关于通过沙箱和权限模型保护文件系统免受 AI 代理侵害的讨论](#item-2) ⭐️ 8.0/10
3. [中科院文献情报中心宣布自 2026 年起停更期刊分区表](#item-3) ⭐️ 8.0/10
4. [因 iPhone 13 启用锁定模式，FBI 无法提取记者手机数据](#item-4) ⭐️ 8.0/10
5. [欧洲议会否决“聊天控制”监控延期，后续或转向强制身份验证](#item-5) ⭐️ 8.0/10
6. [AI 深伪视频渗入美国中期选举，共和党竞选团队率先大规模应用](#item-6) ⭐️ 8.0/10
7. [SGLang v0.5.10rc0 通过默认 CUDA 图、容错 MoE 和稀疏注意力增强推理能力。](#item-7) ⭐️ 7.0/10
8. [欧盟委员会确认 AWS 云环境遭入侵，Europa.eu 平台数百 GB 数据被盗](#item-8) ⭐️ 7.0/10
9. [沃顿商学院研究发现人们易对 AI 输出产生'认知投降'，放弃信息核验](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [西班牙全部 8,642 部法律被转换为 Git 仓库，每次法律修订都是一个提交记录](https://github.com/EnriqueLop/legalize-es) ⭐️ 8.0/10

开发者 Enrique Lop 创建了一个数据处理管道，将西班牙全部国家立法转换为 Git 仓库，其中每部法律存储为 Markdown 文件，每次历史修订都记录为带有实际日期的提交。该仓库包含 8,642 部法律和 27,866 次提交，将法律修订变成了可读的差异对比。 这展示了版本控制系统如何为法律体系带来透明度和可追溯性，使追踪立法随时间的变化变得更加容易。它使得 AI 系统和其他工具能够分析法律的演变过程，并可能成为全球政府文档管理现代化的一个典范。 该管道将立法转换为机器可读的 Markdown 格式，每次修订都会创建一个真实的 git 提交，保留了历史时间线。用户不再需要阅读传统的修订语言如'删除第 3 段'，而是可以直接查看显示版本间具体变化的差异对比。

hackernews · enriquelop · Mar 28, 12:01

**背景**: Git 是一个分布式版本控制系统，最初为跟踪软件代码变化而开发，但其原理同样适用于任何随时间演变的文档。法律文档历史上使用手动版本控制方法，如'合同红线'和'法律黑线'，这些都是修订控制的早期形式。将现代版本控制应用于立法的概念此前已有探索，例如用于美国法典的美国立法标记语言（USLM）标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Version_control">Version control - Wikipedia</a></li>
<li><a href="https://datafoundation.org/news/blogs/335/335-Version-Control-for-Law-Tracking-Changes-in-the-US-Congress">Version Control for Law: Tracking Changes in the U.S. Congress | ANALYSIS | Data Foundation</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞该项目是迈向透明法律数据库的一步，并表示希望看到其他国家也有类似的实现。几位评论者提到了法国和加利福尼亚州现有的版本化法律系统，而其他人则强调这种方法如何解决了传统法律工作流程中的低效问题。讨论强调这项技术应成为立法跟踪的标准实践。

**标签**: `#legal-tech`, `#git`, `#open-government`, `#data-transformation`, `#version-control`

---

<a id="item-2"></a>
## [关于通过沙箱和权限模型保护文件系统免受 AI 代理侵害的讨论](https://jai.scs.stanford.edu/) ⭐️ 8.0/10

一场高评分社区讨论（476 分，272 条评论）围绕实施文件系统沙箱和权限模型展开，旨在保护系统免受可能损坏或窃取数据的 AI 代理侵害。讨论探讨了包括 Claude Code 沙箱功能、Unix 权限系统和基于容器的隔离技术在内的多种实用方法。 这很重要，因为随着 AI 代理获得更多自主权和系统访问权限，它们引入了传统安全模型未曾设计应对的数据损坏和窃取新攻击途径。讨论突显了当前 AI 部署实践中的一个关键缺口：强大的代理以过度权限运行，可能危及个人和企业系统中的敏感数据。 讨论揭示，简单的 Unix 权限模型（为用户和 AI 设置独立账户并共享组文件夹）可以提供基本保护，而像 Claude Code 沙箱化 bash 工具这类更复杂的方法则提供文件系统和网络隔离。社区成员指出，容器能提供隔离但可能有性能开销，一些人质疑现有权限系统是否足以应对 AI 不可预测的行为模式。

hackernews · mazieres · Mar 28, 00:39

**背景**: 文件系统沙箱是一种安全技术，限制应用程序对文件系统特定部分的访问，防止其读取或写入未经授权的位置。AI 代理权限模型定义了 AI 可以访问的资源及其可执行的操作，类似于传统系统中的用户权限。数据窃取防护涉及阻止受保护环境外未经授权数据传输的技术，这对于可能无意或恶意通过其输出或操作泄露信息的 AI 代理来说尤其具有挑战性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/sandboxing">Sandboxing - Claude Code Docs</a></li>
<li><a href="https://dl.acm.org/doi/10.1145/3265723.3265734">A Lightweight and Fine-grained File System Sandboxing Framework</a></li>
<li><a href="https://www.osohq.com/learn/ai-agent-permissions-delegated-access">Setting Permissions for AI Agents - Oso</a></li>

</ul>
</details>

**社区讨论**: 社区情绪显示对以广泛系统权限运行 AI 代理的安全风险表示担忧，一些人对用户如此轻易地向不可预测软件授予权限感到惊讶。技术讨论包括 Claude 配置设置、Unix 权限设置等实际实施细节，以及不同沙箱方法之间的比较。几位评论者寻求更多关于不同隔离方法（沙箱、容器、虚拟机）之间安全权衡的资源。

**标签**: `#AI Security`, `#Filesystem Sandboxing`, `#Agent Safety`, `#Unix Permissions`, `#System Security`

---

<a id="item-3"></a>
## [中科院文献情报中心宣布自 2026 年起停更期刊分区表](https://mp.weixin.qq.com/s/_vf0g6qlG9mFbyyARa0IPQ) ⭐️ 8.0/10

3 月 27 日，中国科学院文献情报中心发布声明，宣布自 2026 年起将不再更新与发布期刊分区表。声明表示，后续将继续开展学术资源评价方法研究，服务国内外学术交流与出版生态建设。 此举标志着中国学术评价体系的一次重大政策转向，因为中科院期刊分区表长期以来是国内科研评价、论文投稿和机构评估中影响广泛的参考工具。它的停更预示着相关体系可能正在摆脱对简单期刊分级指标的依赖，转向更精细的评价方法，这或将重塑全国范围内研究者、高校和出版机构的科研激励导向。 文献中心特别强调，2026 年后任何其他机构发布的期刊分区表均与其无关。同时，针对 2026 年度已订购用户的相关合同事宜，中心将尽快启动后续处理。

telegram · zaihuapd · Mar 28, 02:45

**背景**: 《中国科学院文献情报中心期刊分区表》是该中心的科研成果，其设计思路始于 2000 年左右，旨在纠正当时国内科研界对不同学科期刊影响因子数值差异的忽视。该表基于引文指标，将自然科学、工程技术、医学、管理科学、社会科学及人文艺术等领域的重要国际学术期刊划分为不同分区（如 Q1-Q4 或 1-4 区），长期以来被国内高校和科研机构广泛用于绩效评价、资源分配和职称晋升等决策。分区数据可通过官方在线平台或微信公众号进行查询。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.jiemian.com/article/14177382.html">中国科学院文献情报中心：将不再更新与发布期刊分区表</a></li>
<li><a href="https://www.las.ac.cn/front/knowledgeServices/serviceDetail?entityId=26&entityType=ApplicationMart">期刊分区表 - las</a></li>

</ul>
</details>

**标签**: `#academic-publishing`, `#research-evaluation`, `#china-science-policy`, `#scholarly-communication`

---

<a id="item-4"></a>
## [因 iPhone 13 启用锁定模式，FBI 无法提取记者手机数据](https://t.me/zaihuapd/40569) ⭐️ 8.0/10

美国联邦调查局（FBI）近日披露，其计算机分析响应小组（CART）无法从《华盛顿邮报》记者 Hannah Natanson 的 iPhone 13 中提取数据，原因是该设备启用了苹果的“锁定模式”（Lockdown Mode）。此次数据提取尝试发生在针对一名政府承包商涉嫌泄露机密信息的调查过程中。 这一事件为苹果“锁定模式”抵御高级执法机构取证尝试的有效性提供了重要的现实世界例证。它突显了消费级设备安全功能保护敏感信息（如新闻线人）免受国家级行为体侵害的能力正在不断增强。 尽管 FBI 通过指纹解锁了记者的 MacBook Pro 并从中获取了部分 Signal 通讯记录，但由于 iPhone 13 启用了锁定模式，手机本身的数据无法被提取。此案的相关情况记录在针对政府承包商 Aurelio Perez-Lugones 的调查法庭文件中。

telegram · zaihuapd · Mar 28, 08:57

**背景**: 苹果的“锁定模式”是 iPhone 上一项可选的极端保护功能，旨在防御由国家资助的攻击者发起的极其复杂的网络攻击。启用后，它会通过限制某些应用程序、网络技术和连接类型来严重限制设备功能，从而减少受攻击面。FBI 的计算机分析响应小组（CART）是其主要的数字取证部门，专门从事从电子设备中提取和分析数据以用于调查。Signal 是一款以其强大的端到端加密而闻名的通讯应用，这种加密会对信息进行加扰，使得只有发送方和接收方才能阅读。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/en-us/105120">About Lockdown Mode - Apple Support</a></li>
<li><a href="https://www.ojp.gov/ncjrs/virtual-library/abstracts/computer-analysis-and-response-team-cart-microcomputer-evidence">Computer Analysis and Response Team (CART): The Microcomputer ...</a></li>
<li><a href="https://signal.org/">Signal >> Home</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#digital-privacy`, `#apple-security`, `#law-enforcement`, `#journalism`

---

<a id="item-5"></a>
## [欧洲议会否决“聊天控制”监控延期，后续或转向强制身份验证](https://www.patrick-breyer.de/en/end-of-chat-control-eu-parliament-stops-mass-surveillance-in-voting-thriller-paving-the-way-for-genuine-child-protection/) ⭐️ 8.0/10

欧洲议会近日以一票之差的微弱优势，正式否决了延长“聊天控制 1.0”临时法规的提案。自 2026 年 4 月 4 日起，该条例将失效，Meta、谷歌和微软等美国科技公司必须停止对欧洲公民私人聊天记录、图片和文字内容的自动扫描。 这是欧盟数字隐私权的一次重大胜利，阻止了一种被批评者认为会破坏端到端加密的大规模监控形式。它迫使欧盟的在线儿童保护策略发生重大转变，将辩论焦点从批量扫描转向可能引发争议的强制身份或年龄验证等措施。 否决的主要依据是该系统高达 13%至 20%的误报率，这导致警方收到的举报中约 48%与犯罪无关，且未能有效提升实际定罪率。尽管此次大规模扫描被叫停，但欧盟关于永久性儿童保护法的谈判仍在进行，其中仍在考虑的“聊天控制 2.0”提案可能强制要求扫描社交平台上的所有通信。

telegram · zaihuapd · Mar 28, 13:06

**背景**: 自 2021 年 7 月起，一项通常被称为“聊天控制 1.0”的欧盟临时条例，对《电子隐私指令》的部分内容提供了临时豁免。这项豁免允许通信服务提供商使用“哈希值扫描”等技术扫描私人信息，以查找已知的儿童性虐待材料。该条例原定到期，但此前一直存在被延期的可能，由此引发了关于隐私保护与儿童保护之间长期存在的争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gigazine.net/gsc_news/en/20260327-end-eu-chat-control/">The EU has decided to repeal 'Chat Control 1.0,' which ...</a></li>
<li><a href="https://edri.org/our-work/a-beginners-guide-to-eu-rules-on-scanning-private-communications-part-1/">A beginner’s guide to EU rules on scanning private communications: Part 1 - European Digital Rights (EDRi)</a></li>
<li><a href="https://www.computerweekly.com/news/366640781/EU-Parliament-rejects-Chat-Control-message-scanning">EU Parliament rejects Chat Control message scanning | Computer Weekly</a></li>

</ul>
</details>

**标签**: `#privacy`, `#eu-regulation`, `#surveillance`, `#tech-policy`, `#digital-rights`

---

<a id="item-6"></a>
## [AI 深伪视频渗入美国中期选举，共和党竞选团队率先大规模应用](https://www.reuters.com/business/media-telecom/ai-deepfakes-blur-reality-2026-us-midterm-campaigns-2026-03-28/) ⭐️ 8.0/10

随着 2026 年美国中期选举临近，共和党阵营，包括其全国参议院委员会（NRSC），正在大规模部署 AI 生成的深伪政治广告，捏造竞争对手的言论。例如，一则深伪广告虚假地描绘了德克萨斯州参议员候选人 James Talarico 宣称“激进白人是最大的恐怖威胁”。 这标志着 AI 被武器化用于政治虚假信息的严重升级，使欺骗性内容正常化并直接威胁选举公正性。在监管零散的背景下，一个主要政党的广泛使用，有侵蚀公众对民主机构信任的风险，并可能为全球未来的选举树立一个危险的先例。 尽管许多此类广告带有微小的 AI 标识，但由于其高度逼真性以及披露法律约束力有限，它们在误导选民方面仍然非常有效。虽然已有 28 个州通过了要求在政治广告中披露 AI 使用的法律，但执法力度薄弱，尤其是对于在社交媒体平台传播的内容。

telegram · zaihuapd · Mar 28, 15:42

**背景**: 深伪（Deepfake）是一种利用人工智能将一个人的形象替换为另一个人形象的合成媒体，能创造出高度逼真但虚假的视频或音频。全国共和党参议院委员会（NRSC）是一个致力于选举共和党人进入美国参议院的主要政治委员会。在美国，对政治广告中 AI 的监管主要由州一级负责，导致法律零散不一，对披露要求或某些欺骗性用途的禁令各不相同。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/National_Republican_Senatorial_Committee">National Republican Senatorial Committee - Wikipedia</a></li>
<li><a href="https://www.adexchanger.com/data-driven-thinking/ai-disclosure-requirements-navigating-state-laws-and-platform-rules/">AI Disclosure Requirements: Navigating State Laws And Platform Rules | AdExchanger</a></li>
<li><a href="https://www.broadcastlawblog.com/2026/03/articles/ai-in-political-attack-ads-watch-state-laws-on-deep-fakes-and-synthetic-media-in-political-content/">AI in Political Attack Ads – Watch State Laws on Deep Fakes and Synthetic Media in Political Content | Broadcast Law Blog</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Disinformation`, `#Political Technology`, `#Deepfakes`, `#Election Integrity`

---

<a id="item-7"></a>
## [SGLang v0.5.10rc0 通过默认 CUDA 图、容错 MoE 和稀疏注意力增强推理能力。](https://github.com/sgl-project/sglang/releases/tag/v0.5.10rc0) ⭐️ 7.0/10

SGLang v0.5.10rc0 已发布，将分段式 CUDA 图捕获设为默认执行模式以提升吞吐量。该版本还引入了用于 MoE 模型部分故障容错的 Elastic EP，集成了用于长上下文推理的 HiSparse 稀疏注意力后端，并更新了 SGLang-Diffusion，增加了新模型支持和性能提升。 此版本显著提升了大型语言模型服务系统的可靠性和效率。默认的分段式 CUDA 图降低了内存开销，Elastic EP 确保了 MoE 部署中 GPU 故障时的服务连续性，而 HiSparse 则实现了对长序列的更高效处理，共同推动了可用于生产环境的推理能力。 分段式 CUDA 图功能会预捕获一组 token 数量的图，并在运行时选择最接近的匹配项，这对于可变长度的预填充/扩展操作尤其有益。Elastic EP 专门使 DeepSeek MoE 部署能够在 GPU 故障时重新分配专家权重并继续服务，而无需完全重启。

github · Kangyan-Zhou · Mar 28, 05:58

**背景**: SGLang 是一个旨在优化推理的高性能语言模型服务框架。分段式 CUDA 图是一种优化技术，它将模型的前向传播过程捕获为针对不同输入大小的多个较小图，相比单一图在处理可变长度输入时性能更优。混合专家模型使用多个专门的子网络来处理输入的不同部分，这些子网络可以分布在多个 GPU 上。稀疏注意力机制通过让 token 仅关注其他 token 的一个子集来降低计算成本，这对于处理长上下文至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.sglang.io/advanced_features/piecewise_cuda_graph.html">Piecewise CUDA Graph — SGLang</a></li>
<li><a href="https://deepwiki.com/kvcache-ai/Mooncake/7.6-elastic-expert-parallelism">Elastic Expert Parallelism | kvcache-ai/Mooncake | DeepWiki</a></li>
<li><a href="https://arxiv.org/abs/2602.03560">[2602.03560] HySparse: A Hybrid Sparse Attention Architecture ...</a></li>

</ul>
</details>

**标签**: `#inference-optimization`, `#gpu-computing`, `#llm-serving`, `#sparse-attention`, `#model-serving`

---

<a id="item-8"></a>
## [欧盟委员会确认 AWS 云环境遭入侵，Europa.eu 平台数百 GB 数据被盗](http://europa.eu/) ⭐️ 7.0/10

欧盟委员会确认其云基础设施遭网络攻击，具体目标是承载 Europa.eu 平台内容的 AWS 环境，导致数百 GB 数据被盗。委员会表示已立即采取处置和风险缓解措施，攻击已被控制，内部系统未受影响，调查仍在进行。 此次入侵事件影响重大，因为它针对的是一个主要政府机构的对外数字平台，可能泄露敏感信息并损害对欧盟数字服务的信任。它突显了公共部门实体在将关键基础设施迁移到 AWS 等云平台时，即使使用成熟的供应商，也依然面临持续的安全挑战。 据 Bleeping Computer 报道，黑客从欧盟委员会的 AWS 账户中窃取了包括多个数据库在内的数据，并提供了访问截图作为证据。委员会尚未披露被窃取数据的具体类型，因此入侵的完整范围和数据的敏感性尚不明确。

telegram · zaihuapd · Mar 28, 01:16

**背景**: Amazon Web Services (AWS) 是全球政府和企业广泛使用的领先按需云计算平台。Europa.eu 平台是欧盟的官方网站，是一个关键的公共信息和服务门户。数据窃取（Data exfiltration）是指攻击者用于从网络中窃取数据的技术，通常涉及对敏感信息的未授权访问和转移。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Amazon_Web_Services">Amazon Web Services - Wikipedia</a></li>
<li><a href="https://attack.mitre.org/tactics/TA0010/">Exfiltration , Tactic TA0010 - Enterprise | MITRE ATT&CK</a></li>

</ul>
</details>

**标签**: `#Cybersecurity`, `#Data Breach`, `#AWS`, `#European Commission`, `#Cloud Security`

---

<a id="item-9"></a>
## [沃顿商学院研究发现人们易对 AI 输出产生'认知投降'，放弃信息核验](https://www.forbes.com/sites/lesliekatz/2026/03/27/cognitive-surrender-we-trust-ai-over-our-own-brains-research-finds/) ⭐️ 7.0/10

宾夕法尼亚大学沃顿商学院的研究人员上月于 SSRN 发布预印本，报告称在对近 1300 名参与者进行的实验中，人们在超过一半的逻辑推理任务中会选择使用 ChatGPT。在大约 80%寻求 AI 帮助的情况下，参与者会不加审视地接受错误答案，研究人员将这种行为称为'采纳而不核验'。 这种'认知投降'现象表明，生成式 AI 正在从根本上重塑人类的决策过程，可能带来系统性风险，即人们将批判性思维和认知能动性让渡给自动化系统。这凸显了重新审视传统决策模型、并设计能鼓励而非绕过人类认知参与的 AI 界面的必要性。 研究发现，使用 ChatGPT 的参与者对自己答案的信心高出 10%，尽管答案可能存在错误。研究人员主张，应在决策框架中将 AI 作为一种新的外部认知系统纳入，超越传统的'双过程'模型。

telegram · zaihuapd · Mar 28, 14:23

**背景**: 决策的'双过程理论'描述了两个相互作用的系统：系统 1（快速、直觉、自动）和系统 2（缓慢、审慎、分析）。SSRN（社会科学研究网络）是一个用于分享早期研究和预印本的开放获取知识库，预印本是指尚未经过正式同行评审的论文。'认知投降'这一概念超越了简单的工具依赖，它描述了一种认知控制的让渡，即用户不加批判地用 AI 输出替代自己的推理过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Social_Science_Research_Network">Social Science Research Network - Wikipedia</a></li>
<li><a href="https://www.globalcognition.org/dual-process-theory/">Dual Process Theory: Two Ways to Think and Decide</a></li>
<li><a href="https://medkharbach.com/cognitive-surrender-how-ai-is-quietly-reshaping-the-way-we-think/">Cognitive Surrender: How AI Is Quietly Reshaping the Way We ...</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Human-Computer Interaction`, `#Behavioral Science`, `#Decision Making`, `#Generative AI`

---