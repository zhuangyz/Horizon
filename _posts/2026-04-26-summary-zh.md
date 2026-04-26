---
layout: default
title: "Horizon Summary: 2026-04-26 (ZH)"
date: 2026-04-26
lang: zh
---

> From 19 items, 10 important content pieces were selected

---

1. [DeepSeek-V4 预览版发布并开源](#item-1) ⭐️ 9.0/10
2. [Asahi Linux 进度报告 7.0：M3 硬件支持取得进展](#item-2) ⭐️ 8.0/10
3. [业余数学家借助 ChatGPT 解决 60 年历史的 Erdős 问题](#item-3) ⭐️ 8.0/10
4. [阿尔茨海默病研究为何停滞：淀粉样蛋白陷阱](#item-4) ⭐️ 8.0/10
5. [西方编程技能流失，重蹈制造业覆辙](#item-5) ⭐️ 8.0/10
6. [OpenAI 推出 GPT-5.5 生物安全漏洞赏金计划](#item-6) ⭐️ 8.0/10
7. [1900 名美国院士呼吁特朗普停止攻击科学](#item-7) ⭐️ 8.0/10
8. [顶级大学网站因 DNS 管理疏忽被劫持发布色情内容](#item-8) ⭐️ 8.0/10
9. [Headspace 应用每日静默安装到 iPhone](#item-9) ⭐️ 7.0/10
10. [砺算科技 7G100 显卡获微软 WHQL 认证](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [DeepSeek-V4 预览版发布并开源](https://t.me/zaihuapd/41074) ⭐️ 9.0/10

DeepSeek 发布了 DeepSeek-V4 的预览版本，包括 V4-Pro 和 V4-Flash 两个变体，并同步开源了模型权重。V4-Pro 在数学、STEM 和竞赛编程基准测试中超越当前所有开源模型，性能接近三大闭源模型。 此次发布是开源大语言模型的一个重要里程碑，通过以更低成本提供顶尖性能，可能重塑竞争格局。大幅增强的 Agent 能力使其非常适合实际自动化与工具使用任务，惠及开发者与企业。 DeepSeek-V4-Pro 是一个混合专家（MoE）模型，总参数量达 1.6 万亿，激活参数量为 490 亿，支持 100 万 token 的上下文窗口。V4-Flash 变体通过更小的参数激活提供更快、更经济的 API 服务，同时仍保持强大的推理与 Agent 能力。

telegram · zaihuapd · Apr 26, 07:17

**背景**: DeepSeek 是一家以开发高性能开源语言模型闻名的中国人工智能公司。术语“Agent”指模型自主使用工具、调用函数和执行多步任务的能力，这对编码助手和自动化工作流等实际应用至关重要。“御三家”指 GPT-4o 和 Claude Opus 等领先的闭源模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.knightli.com/en/2026/04/24/deepseek-v4-preview-release/">DeepSeek-V4 Preview Released: 1M Context, Two Models, and API ...</a></li>
<li><a href="https://stable-learn.com/en/deepseek-v4-release/">DeepSeek-V4: 1M Context, Best Open-Source Agent, Beats Claude ...</a></li>
<li><a href="https://deepinfra.com/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/ DeepSeek - V 4 -Pro - Demo - DeepInfra</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#LLM`, `#open-source`, `#AI`, `#Agent`

---

<a id="item-2"></a>
## [Asahi Linux 进度报告 7.0：M3 硬件支持取得进展](https://asahilinux.org/2026/04/progress-report-7-0/) ⭐️ 8.0/10

Asahi Linux 的进度报告 7.0 宣布，针对 M3 Mac 的补丁已加入 Asahi 内核树，支持 PCIe、NVMe、键盘/触控板、基于 SMC 的实时时钟和重启控制器，使 M3 的支持水平大致达到首个 M1 alpha 版本的水平。 这一里程碑显著扩展了 Linux 对苹果最新 M3 硬件的兼容性，为用户在高性能 Apple Silicon Mac 上提供了 macOS 之外的可行替代方案，并展示了该项目在逆向工程方面的持续成功。 该支持工作由 Michael Reeves 和 Alyssa Milburn 贡献，目前 CS42L84 编解码器的音频驱动仅支持 48 kHz 和 96 kHz 采样率，因为 macOS 仅编程了这两个速率。

hackernews · elisaado · Apr 26, 10:50

**背景**: Asahi Linux 是一个社区驱动的项目，通过逆向工程将 Linux 移植到 Apple Silicon Mac 上。苹果的 M1、M2、M3 及更新芯片采用定制的 ARM 架构，缺乏官方公开文档，使得驱动开发异常困难。该项目于 2022 年 3 月发布了首个 M1 alpha 版本，目前 M3 的进展已接近这一早期里程碑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asahi_linux_project">Asahi linux project</a></li>
<li><a href="https://en.wikipedia.org/wiki/Asahi_Linux">Asahi Linux - Wikipedia</a></li>
<li><a href="https://asahilinux.org/">Asahi Linux</a></li>

</ul>
</details>

**社区讨论**: 社区对 M3 的进展表示热情，一些用户称赞技术文章并希望项目获得动力。然而，也有人对长期可持续性持怀疑态度，因为这项工作仍独立于主线内核和主流发行版，部分用户质疑苹果为何不提供官方文档来帮助该项目。

**标签**: `#Asahi Linux`, `#Apple Silicon`, `#Linux kernel`, `#reverse engineering`, `#M3`

---

<a id="item-3"></a>
## [业余数学家借助 ChatGPT 解决 60 年历史的 Erdős 问题](https://www.scientificamerican.com/article/amateur-armed-with-chatgpt-vibe-maths-a-60-year-old-problem/) ⭐️ 8.0/10

一位业余数学家利用 ChatGPT 提出了一种新颖的方法，帮助解决了一个存在 60 年之久的 Erdős 问题，随后由数学家 Jared Lichtman 和陶哲轩等专家对原始输出进行了精炼。 这表明大型语言模型能够为长期未解决的数学问题提供创造性见解，通过打破人类的思维定势，可能加速数学研究的进展。 ChatGPT 的原始证明质量较差，需要专家筛选，但其中包含了一个关键见解，最终促成了一个更简洁、严谨的证明。该问题可能比之前认为的更简单，表明人工智能可以帮助清理这类问题。

hackernews · pr337h4m · Apr 25, 17:40

**背景**: Paul Erdős 是一位多产的匈牙利数学家，以提出许多未解决问题而闻名，并常为这些问题提供奖金。Erdős 问题的难度跨度很大，数十年来一直挑战着数学家。这个特定问题已悬而未决约 60 年。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Erdős_problem">Erdős problem</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_conjectures_by_Paul_Erdős">List of conjectures by Paul Erdős - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出，ChatGPT 的原始输出质量较差，但其关键见解很有价值；该问题可能比预期更简单，人工智能帮助克服了思维定势。一些人指出，标题过度简化了所需的协作努力。

**标签**: `#AI`, `#mathematics`, `#LLM`, `#research`, `#Erdős problem`

---

<a id="item-4"></a>
## [阿尔茨海默病研究为何停滞：淀粉样蛋白陷阱](https://freakonomics.com/podcast/why-has-there-been-so-little-progress-on-alzheimers-disease/) ⭐️ 8.0/10

一档《怪诞经济学》播客探讨了为何数十年的阿尔茨海默病研究进展甚微，重点分析了淀粉样蛋白假说的失败以及科学界对替代方法的抵制。 这之所以重要，是因为阿尔茨海默病影响着全球数百万人，而研究的停滞浪费了数十亿美元资金，并延误了潜在疗法的开发，暴露了医学科学在主导范式下存在的系统性问题。 该播客和社区评论指出，淀粉样蛋白级联假说——即认为β-淀粉样蛋白斑块导致阿尔茨海默病——是一个占主导地位但有缺陷的模型，数十年来锁定了资金和研究方向，而 tau 蛋白病理、炎症和衰老等替代理论则被边缘化。

hackernews · chiefalchemist · Apr 26, 00:12

**背景**: 淀粉样蛋白级联假说于 20 世纪 90 年代提出，认为β-淀粉样蛋白在大脑中的积累会引发一系列反应，最终导致阿尔茨海默病。该假说指导了二十多年来的大部分药物研发工作，但针对淀粉样蛋白的临床试验屡屡未能显示出对患者有意义的认知改善。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://academic.oup.com/brain/article/146/10/3969/7162122">The amyloid cascade hypothesis: an updated critical review</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9662281/">Amyloid Cascade Hypothesis for the Treatment of Alzheimer’s ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Paradigm_shift">Paradigm shift - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为淀粉样蛋白假说是一个代价高昂的错误，有人将其归因于科学惯性和资金锁定，而非恶意。一位用户推荐了 Karl Herrup 的著作《如何不研究一种疾病》作为关键批评，另一位则认为阿尔茨海默病是衰老的产物，而医疗系统回避了这一根本原因。

**标签**: `#Alzheimer's`, `#medical research`, `#scientific paradigm`, `#pharmaceutical industry`, `#public health`

---

<a id="item-5"></a>
## [西方编程技能流失，重蹈制造业覆辙](https://techtrenches.dev/p/the-west-forgot-how-to-make-things) ⭐️ 8.0/10

一篇文章指出，西方过去失去制造业专长的现象正在软件工程领域重演，对人工智能的依赖和短期成本削减正在侵蚀深层编程知识与师徒传承。 这一趋势削弱了隐性知识的传递——这对创新和解决问题至关重要——从而威胁软件行业的长期健康，并可能导致一代开发者过度依赖 AI 工具。 文章强调，短期成本削减减少了初级员工的招聘，并消除了资深工程师教学所需的组织缓冲，导致隐性知识停止传递，只剩下文档和自动化。

hackernews · milkglass · Apr 26, 06:24

**背景**: 隐性知识是通过实践经验和师徒传承获得的、难以写入文档或代码的直觉性理解。西方制造业技能的早期衰退常被归因于外包和短期利润导向，文章认为这一模式如今正在软件开发中重演。

**社区讨论**: 社区评论普遍认同文章的观点，一位用户指责管理层优先考虑短期成本削减而非知识传递，另一位则指出依赖 AI 处理琐碎任务“令人恐惧”，因为这会导致大脑技能萎缩。还有评论者批评文章本身是 AI 生成的，指出写作能力同样是一种会退化的技能。

**标签**: `#software engineering`, `#AI`, `#knowledge transfer`, `#management`, `#skill atrophy`

---

<a id="item-6"></a>
## [OpenAI 推出 GPT-5.5 生物安全漏洞赏金计划](https://openai.com/zh-Hans-CN/index/gpt-5-5-bio-bug-bounty/) ⭐️ 8.0/10

OpenAI 为 GPT-5.5 启动了一项生物安全漏洞赏金计划，首个能绕过全部五道生物安全挑战题且不触发内容审核的通用越狱提示词将获得 25,000 美元奖励。该计划采取申请邀请制，申请通道于 2026 年 4 月 23 日至 6 月 22 日开放，测试阶段为 2026 年 4 月 28 日至 7 月 27 日。 该计划代表了对主动式 AI 安全研究的重大投入，专门针对 AI 被滥用于生成危险生物信息的风险。通过激励外部红队成员寻找通用越狱方法，OpenAI 旨在更广泛部署前加强 GPT-5.5 的安全护栏，为高风险领域的负责任 AI 开发树立先例。 测试范围仅限于 Codex Desktop 中的 GPT-5.5 模型，参与者需签署保密协议。挑战要求提供一个通用越狱提示词，能在干净聊天中成功回答全部五道生物安全题，且不触发模型的审核系统。

telegram · zaihuapd · Apr 25, 16:36

**背景**: 通用越狱是指一个能绕过 AI 模型在多项任务中安全护栏的单一提示词，而非利用特定漏洞。AI 生物安全指的是先进语言模型可能提供创建生物威胁（如病原体或毒素）的详细指令的风险。OpenAI 一直在迭代 GPT-5.x 系列模型，GPT-5.4 于 2026 年 3 月发布，GPT-5.5 现已在 Codex Desktop 中面向 ChatGPT 用户提供。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-5-bio-bug-bounty/">GPT‑5.5 Bio Bug Bounty - OpenAI</a></li>
<li><a href="https://openai.smapply.org/prog/gpt-5-5-safety-bio-bounty-program">GPT-5.5 Bio Bounty Program - OpenAI</a></li>
<li><a href="https://gbhackers.com/gpt-5-5-bio-bug-bounty-program/">GPT-5.5 Bio Bug Bounty Program Aims to Improve AI Safety and ...</a></li>

</ul>
</details>

**标签**: `#AI Safety`, `#Bug Bounty`, `#GPT-5.5`, `#Biosafety`, `#OpenAI`

---

<a id="item-7"></a>
## [1900 名美国院士呼吁特朗普停止攻击科学](https://t.me/zaihuapd/41070) ⭐️ 8.0/10

3 月 31 日，1900 名美国国家科学院、工程院和医学院成员（包括十多位诺贝尔奖得主）发表公开信，呼吁特朗普政府停止其所谓的对美国科学的全面攻击。 这一前所未有的顶尖科学家动员标志着重大政策冲突，可能扰乱科研经费、削弱公众对科学的信任，并损害美国在创新和健康领域的全球领导地位。 这封信由来自医学、流行病学、心理学、气候科学、社会学和经济学等领域的 13 位科学家起草，签名者包括 Harvey J. Alter、Francoise Barre-Sinoussi、Reinhard Genzel、Edvard I. Moser 和 May-Britt Moser 等诺贝尔奖得主。

telegram · zaihuapd · Apr 26, 00:40

**背景**: 美国国家科学院是享有盛誉的荣誉性学术机构，为政府提供科技咨询。特朗普政府曾提议大幅削减 NIH 和 NSF 等机构的预算，并采取了一些科学家认为破坏基于证据的政策的行动，例如退出《巴黎协定》和淡化气候变化。

**标签**: `#science policy`, `#research funding`, `#Trump administration`, `#open letter`, `#US academia`

---

<a id="item-8"></a>
## [顶级大学网站因 DNS 管理疏忽被劫持发布色情内容](https://arstechnica.com/security/2026/04/why-are-top-university-websites-serving-porn-it-comes-down-to-shoddy-housekeeping/) ⭐️ 8.0/10

包括加州大学伯克利分校和哥伦比亚大学在内的至少 34 所顶尖大学的子域名被 Hazy Hawk 攻击团伙劫持，用于发布色情内容和诈骗信息，攻击者利用了子域名停用后未清理的 CNAME 记录漏洞。 这一事件凸显了一个普遍且严重的域名管理漏洞，即使是最负盛名的机构也未能幸免；攻击者利用大学的高信誉域名在搜索结果中获得高排名并欺骗用户，可能损害机构信誉和用户信任。 Hazy Hawk 团伙自 2023 年 12 月以来一直利用废弃的云资源进行攻击，曾针对德勤、松下等大型组织，目前已攻陷数百个大学子域名，导致搜索引擎中出现了数千个恶意页面。

telegram · zaihuapd · Apr 26, 09:02

**背景**: DNS 中的 CNAME 记录将一个域名映射到另一个域名，常用于将子域名指向外部服务（如云平台）。当子域名被停用但 CNAME 记录未被移除时，该记录就成为“悬空”或孤立的 DNS 条目。攻击者随后可以注册该悬空记录所引用的外部服务端点，从而有效控制该子域名并托管恶意内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.spamhaus.org/resource-hub/dns/dangling-dns-and-the-dangers-of-subdomain-hijacking/">Blog | Dangling DNS and the dangers of subdomain hijacking | Resources</a></li>
<li><a href="https://quorumcyber.com/threat-intelligence/hazy-hawk-exploits-dns-vulnerabilities-to-target-major-organisations/">Hazy Hawk Exploits DNS Vulnerabilities | Quorum Cyber</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/security/fundamentals/subdomain-takeover">Prevent dangling DNS entries and avoid subdomain takeover</a></li>

</ul>
</details>

**标签**: `#security`, `#domain hijacking`, `#DNS`, `#cyber attack`, `#university`

---

<a id="item-9"></a>
## [Headspace 应用每日静默安装到 iPhone](https://news.ycombinator.com/item?id=47906253) ⭐️ 7.0/10

用户报告称，Headspace 冥想应用每天大约美国东部时间下午 1 点静默安装到他们的 iPhone 上，尽管自动下载已关闭且 iOS 已更新至最新版本。 这种无法解释的行为引发了隐私和安全担忧，因为它表明可能存在 iOS 漏洞或未经授权的应用安装机制，可能影响除 Headspace 之外的许多用户。 该问题已在 iPhone 12、13 Pro 甚至 iPhone 17 Pro 机型上被报告，涉及不同 iOS 版本且没有 MDM 配置文件，表明它不是特定于设备或与 MDM 相关。

hackernews · _-x-_ · Apr 26, 00:50

**背景**: MDM（移动设备管理）配置文件允许组织远程安装和管理设备上的应用，但在此案例中用户报告未安装此类配置文件。2017 年曾有一个类似的 iOS 漏洞，导致具有本地时间通知的应用触发无限崩溃循环，一些社区成员将当前问题与之类比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=47906253">Tell HN: An app is silently installing itself on my iPhone every day</a></li>

</ul>
</details>

**社区讨论**: 社区成员推测，通知触发的应用启动与 iOS 的卸载功能结合可能导致应用重新出现。其他人回忆起 2017 年涉及冥想应用和本地通知的 iOS 漏洞，暗示可能存在重复出现的模式。

**标签**: `#iOS`, `#bug`, `#privacy`, `#app installation`, `#security`

---

<a id="item-10"></a>
## [砺算科技 7G100 显卡获微软 WHQL 认证](http://www.cnbeta.com.tw/articles/tech/1559976.htm) ⭐️ 7.0/10

砺算科技的 7G100 系列 GPU 已获得微软 WHQL 认证，成为国内首家、全球第四家获此认证的 GPU 公司。在实测中，Lisuan eXtreme 系列在 3DMark Steel Nomad 测试中跑分为 2268，性能接近 NVIDIA RTX 4060。 这一认证表明砺算科技的 GPU 驱动通过了微软严格的质量标准，实现了广泛的 Windows 兼容性，增强了市场对国产 GPU 的信心。同时，它也证明国产 GPU 在真实游戏和 AI 负载中能够与 RTX 4060 等主流产品竞争。 7G100 系列基于 6nm 工艺及自研“天图”架构，实现了计算核心、指令集与软件栈的完全自主设计。在 1080P 高画质下运行《黑神话：悟空》平均帧率超 70 帧，并支持 AIPC 主流大模型。

telegram · zaihuapd · Apr 26, 02:59

**背景**: WHQL（Windows 硬件质量实验室）认证是微软对第三方设备驱动程序的测试流程，旨在确保驱动在 Windows 上的稳定性和兼容性。此前仅有 NVIDIA、AMD 和 Intel 三家 GPU 公司获得该认证。砺算科技的 7G100 系列面向中端显卡市场，与 RTX 4060 等产品竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WHQL_Testing">WHQL Testing - Wikipedia</a></li>
<li><a href="https://store.steampowered.com/app/2695340/3DMark_Steel_Nomad/">3DMark Steel Nomad on Steam</a></li>

</ul>
</details>

**标签**: `#GPU`, `#WHQL`, `#Chinese semiconductor`, `#hardware`, `#graphics`

---