---
layout: default
title: "Horizon Summary: 2026-04-23 (ZH)"
date: 2026-04-23
lang: zh
---

> From 26 items, 20 important content pieces were selected

---

1. [Qwen3.6-27B：27B 密集模型在编码上超越 397B MoE](#item-1) ⭐️ 9.0/10
2. [Anthropic 的 Mythos AI 模型发布当天即遭入侵](#item-2) ⭐️ 9.0/10
3. [Bitwarden CLI npm 包遭 Checkmarx 供应链攻击](#item-3) ⭐️ 9.0/10
4. [Tailscale 联合创始人提议从第一性原理构建更简单的云](#item-4) ⭐️ 8.0/10
5. [阿尔伯塔初创公司半价销售无科技拖拉机](#item-5) ⭐️ 8.0/10
6. [苹果修复警方用于提取 iPhone 已删除聊天记录的漏洞](#item-6) ⭐️ 8.0/10
7. [公民实验室揭露两起电信监控活动](#item-7) ⭐️ 8.0/10
8. [法国 ANTS 确认数据泄露，1900 万公民信息或遭窃](#item-8) ⭐️ 8.0/10
9. [吹风机操控巴黎天气传感器，Polymarket 获利超 3.4 万美元](#item-9) ⭐️ 8.0/10
10. [Google Cloud 默认安全缺陷导致用户产生巨额账单](#item-10) ⭐️ 8.0/10
11. [字节跳动发布 Seed3D 2.0，3D 生成达到生产可用水平](#item-11) ⭐️ 8.0/10
12. [DeepSeek 开源 TileKernels 算子库，支持 Blackwell](#item-12) ⭐️ 8.0/10
13. [腾讯开源混元 Hy3 preview：295B MoE 模型](#item-13) ⭐️ 8.0/10
14. [香港证监会与普华永道就恒大造假达成 10 亿港元和解](#item-14) ⭐️ 8.0/10
15. [中国三大运营商报告国际网络故障](#item-15) ⭐️ 8.0/10
16. [苹果 CEO 蒂姆·库克将卸任，约翰·特努斯 2026 年接任](#item-16) ⭐️ 8.0/10
17. [英国 NCSC 正式将通行密钥列为首选身份验证方式](#item-17) ⭐️ 8.0/10
18. [欧盟施压谷歌开放安卓 AI 助手权限](#item-18) ⭐️ 8.0/10
19. [OpenAI macOS 版 Chronicle 功能引发隐私与安全争议](#item-19) ⭐️ 7.0/10
20. [台积电因成本过高推迟导入 ASML 高数值孔径 EUV 至 2029 年](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Qwen3.6-27B：27B 密集模型在编码上超越 397B MoE](https://simonwillison.net/2026/Apr/22/qwen36-27b/#atom-everything) ⭐️ 9.0/10

阿里巴巴 Qwen 团队发布了 Qwen3.6-27B，这是一个 270 亿参数的密集开源权重模型，在所有主要编码基准测试上超越了前代旗舰模型 Qwen3.5-397B-A17B（总参数 397B/激活参数 17B 的 MoE 模型）。该模型仅 55.6GB，而前代模型为 807GB，量化后的 16.8GB 版本可在消费级硬件上本地运行。 这代表了巨大的效率飞跃，表明一个训练有素的密集模型可以匹配甚至超越大得多的混合专家模型的编码性能，大幅降低最先进智能编码的硬件需求。它使开发者能够在单个 GPU 甚至高端笔记本电脑上本地运行旗舰级编码助手，使高级 AI 编码工具的获取更加民主化。 在 QwenWebBench 等内部基准测试中，Qwen3.6-27B 得分 1487，较前代模型的 1068 有显著提升。该模型已在 Hugging Face 上发布，16.8GB 的 GGUF 量化版本（Q4_K_M）可使用 llama.cpp 在本地运行，在典型消费级机器上达到约每秒 25 个 token 的生成速度。

rss · Simon Willison · Apr 22, 16:45

**背景**: 密集模型每次推理使用所有参数，而混合专家（MoE）模型每个 token 仅激活部分参数，从而在相似计算成本下实现更大的总参数量。GGUF 量化通过压缩权重来减小模型大小和内存需求，同时保持最小质量损失，使大型模型能在消费级硬件上运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/04/22/alibaba-qwen-team-releases-qwen3-6-27b-a-dense-open-weight-model-outperforming-397b-moe-on-agentic-coding-benchmarks/">Alibaba Qwen Team Releases Qwen3.6-27B: A Dense Open-Weight Model Outperforming 397B MoE on Agentic Coding Benchmarks - MarkTechPost</a></li>
<li><a href="https://simonwillison.net/2026/Apr/22/qwen36-27b/">Qwen3.6-27B: Flagship-Level Coding in a 27B Dense Model</a></li>
<li><a href="https://www.buildfastwithai.com/blogs/qwen3-6-27b-review-2026">Qwen3.6-27B: 27B Model Beats 397B on Coding (2026)</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论（文章中提及）参与度很高，用户分享了本地运行该模型的实操测试结果和配方。总体情绪积极，许多人对模型在如此小尺寸下展现的编码性能印象深刻，但有人指出其数学推理能力可能落后于 Gemma 4 等其他模型。

**标签**: `#AI/ML`, `#open-source`, `#coding`, `#model efficiency`, `#Qwen`

---

<a id="item-2"></a>
## [Anthropic 的 Mythos AI 模型发布当天即遭入侵](https://www.bloomberg.com/news/articles/2026-04-21/anthropic-s-mythos-model-is-being-accessed-by-unauthorized-users) ⭐️ 9.0/10

Anthropic 高度受限的网络安全 AI 模型 Mythos（专为零日漏洞发现而设计）在发布当天即被一个小型 Discord 社群绕过限制获取访问权限，并在未触发告警的情况下持续使用近两周，直至彭博社报道后才被外界知晓。 这一事件凸显了强大 AI 模型的严重安全风险：能够发现关键基础设施软件漏洞的 Mythos 被未授权用户利用，可能助长恶意网络攻击，并削弱对 AI 治理的信任。 Mythos 最初仅通过名为 Project Glasswing 的封闭测试向 Apple、Amazon、Cisco 等特定企业开放，Anthropic 已就未授权访问的指控展开调查。

telegram · zaihuapd · Apr 23, 01:49

**背景**: Mythos 是 Anthropic 开发的高级 AI 模型，能够自动发现零日漏洞（即此前未知的软件缺陷），涉及银行、电网和政府等系统。Anthropic 称其过于危险而不向公众发布，仅与少数可信合作伙伴及英国政府共享。该模型的能力已引起全球领导人和网络安全专家的警惕，因为它既可用于防御也可用于攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/cy41zejp9pko">Anthropic investigating claim of unauthorised access to Mythos AI tool</a></li>
<li><a href="https://www.theguardian.com/technology/2026/apr/22/what-is-anthropic-mythos-ai-threat-global-cybersecurity">What is Mythos AI and why could it be a threat to global cybersecurity? | AI (artificial intelligence) | The Guardian</a></li>
<li><a href="https://www.nytimes.com/2026/04/22/technology/anthropics-mythos-ai.html">Anthropic’s New Mythos A.I. Model Sets Off Global Alarms - The New York Times</a></li>

</ul>
</details>

**标签**: `#AI security`, `#cybersecurity`, `#Anthropic`, `#Mythos`, `#data breach`

---

<a id="item-3"></a>
## [Bitwarden CLI npm 包遭 Checkmarx 供应链攻击](https://socket.dev/blog/bitwarden-cli-compromised) ⭐️ 9.0/10

Socket 研究人员发现 Bitwarden CLI 的 npm 包 @bitwarden/cli@2026.4.0 遭遇供应链攻击，攻击者通过篡改 Bitwarden CI/CD 管道中的 GitHub Action 在 bw1.js 文件中植入了恶意代码。 此次攻击针对广泛使用的密码管理器 CLI 工具，可能导致数千用户的凭证、加密货币钱包密钥和开发者机密泄露，凸显了针对流行开源包的供应链攻击威胁日益严重。 该恶意程序会窃取 GitHub 令牌、云服务凭证、SSH 密钥、npm 配置和加密货币钱包数据，并通过创建带有特定主题的公开 GitHub 仓库来泄露数据；它还包含针对俄语系统的自毁机制。

telegram · zaihuapd · Apr 23, 16:02

**背景**: 供应链攻击是指攻击者破坏软件开发管道中的可信组件（如 CI/CD 工具或第三方包），从而向下游用户分发恶意软件。Bitwarden 是一款流行的开源密码管理器，其 CLI 被开发者广泛用于自动化和凭证管理。Checkmarx 攻击活动此前已针对 Trivy 和 LiteLLM 等其他工具，表明这是一场更广泛的持续威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/04/bitwarden-cli-compromised-in-ongoing.html">Bitwarden CLI Compromised in Ongoing Checkmarx Supply Chain Campaign</a></li>
<li><a href="https://thehackernews.com/2026/04/malicious-kics-docker-images-and-vs.html">Malicious KICS Docker Images and VS Code Extensions Hit Checkmarx Supply Chain</a></li>
<li><a href="https://tech.yahoo.com/cybersecurity/articles/bitwarden-cli-supply-chain-attack-142710104.html">Bitwarden CLI Supply Chain Attack Puts Crypto Wallet Keys at Risk</a></li>

</ul>
</details>

**标签**: `#supply chain attack`, `#security`, `#Bitwarden`, `#npm`, `#credential theft`

---

<a id="item-4"></a>
## [Tailscale 联合创始人提议从第一性原理构建更简单的云](https://crawshaw.io/blog/building-a-cloud) ⭐️ 8.0/10

Tailscale 联合创始人 David Crawshaw 发表博文，指出现代云基础设施过于复杂和昂贵，并提出从第一性原理出发，构建更简单、更以用户为中心的云。 来自业界知名人士的批评挑战了云计算现状，尤其是 Kubernetes 的主导地位，可能影响初创公司和工程师重新思考基础设施设计与成本效益。 Crawshaw 认为虚拟机形态错误，因为其成本与 CPU 和内存挂钩而非实际完成的工作，并且让 Kubernetes 变得好用本质上是不可能的。该博文引发了社区强烈反响，获得 755 分和 393 条评论。

hackernews · bumbledraven · Apr 23, 04:44

**背景**: Tailscale 由前 Google 工程师创立，提供以简洁易用著称的网状 VPN 服务。该博文反映了开发者对现代云栈（尤其是 Kubernetes）复杂性和成本日益增长的不满，许多人认为 Kubernetes 为中小规模部署增加了不必要的负担。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tailscale">Tailscale - Wikipedia</a></li>
<li><a href="https://councils.forbes.com/profile/Avery-Pennarun-CEO-Founder-Tailscale/0031c5ae-0eef-4a54-8298-cacfd34ee08d">Avery Pennarun | CEO/Founder - Tailscale | Forbes Technology Council</a></li>

</ul>
</details>

**社区讨论**: 评论者大多认同 Crawshaw 的批评，分享了个人经历中的 Kubernetes 事故以及虚拟机定价与实际工作不匹配的问题。一些人怀疑更简单的云能否在规模化后保持盈利，另一些人则指出像 Firecracker 这样的自托管替代方案是有前途的方向。

**标签**: `#cloud computing`, `#kubernetes`, `#infrastructure`, `#devops`, `#startup`

---

<a id="item-5"></a>
## [阿尔伯塔初创公司半价销售无科技拖拉机](https://wheelfront.com/this-alberta-startup-sells-no-tech-tractors-for-half-price/) ⭐️ 8.0/10

一家位于阿尔伯塔省的初创公司以传统高科技型号一半的价格，提供简单、低技术的拖拉机，目标客户是对锁定且昂贵的农业机械感到沮丧的农民。 这反映了农业领域对过度工程化、软件锁定设备日益增长的抵制情绪，契合了维修权运动以及科技行业关于简洁性和开放生态系统的更广泛讨论。 这些拖拉机没有 GPS 跟踪、触摸屏和软件锁定等现代数字功能，因此独立机械师或农民自己维修起来更简单、更便宜。

hackernews · Kaibeezy · Apr 22, 16:29

**背景**: 像约翰迪尔这样的主要拖拉机制造商越来越多地为其机器配备专有软件和数字锁，限制农民自行维修设备，迫使他们使用授权经销商。这引发了长期的维修权斗争，美国联邦贸易委员会于 2025 年就这些做法起诉了约翰迪尔。这家初创公司的方法直接对抗了这一趋势，提供了一种更简单、更易维修的替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/news/business-64206913">US farmers win right to repair John Deere equipment</a></li>
<li><a href="https://www.npr.org/2025/01/15/nx-s1-5260895/john-deere-ftc-lawsuit-right-to-repair-tractors">FTC sues John Deere over farmers' right to repair tractors : NPR</a></li>
<li><a href="https://thecounter.org/right-to-repair-elizabeth-warren-john-deere/">As farmers fight for the right to repair their tractors , an antitrust...</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍积极，许多人表达了对更简单、可维修机器的怀旧之情，以及对锁定生态系统的沮丧。一些评论者希望在汽车和电动汽车中也有类似选择，而另一些人则指出，由于监管障碍，这类产品在美国历史上难以销售。

**标签**: `#agriculture`, `#startups`, `#technology backlash`, `#open ecosystems`, `#simplicity`

---

<a id="item-6"></a>
## [苹果修复警方用于提取 iPhone 已删除聊天记录的漏洞](https://techcrunch.com/2026/04/22/apple-fixes-bug-that-cops-used-to-extract-deleted-chat-messages-from-iphones/) ⭐️ 8.0/10

苹果发布了紧急更新（iOS 26.4.2 和 iPadOS 26.4.2），修复了编号为 CVE-2026-28950 的 Notification Services 漏洞。该漏洞导致已删除的通知仍保留在设备上，使执法机构能够恢复来自 Signal 等应用的已删除聊天消息。 该漏洞暴露了依赖阅后即焚消息应用的用户面临的重大隐私风险——已删除的消息仍可被取证工具恢复。此次修复解决了特定的缓存问题，但通知内容在设备上存储的广泛问题仍然是跨平台的安全隐患。 该漏洞编号为 CVE-2026-28950，已在 iOS 26.4.2 和 iPadOS 26.4.2 中修复，同时为旧版支持系统发布了补丁。问题在于操作系统在本地数据库中缓存了通知内容，即使源应用已被删除，该漏洞也未能在删除应用时清除这些缓存通知。

hackernews · cdrnsf · Apr 22, 20:27

**背景**: 现代消息应用（如 Signal）对消息内容进行端到端加密，但推送通知通常包含消息预览，这些预览由操作系统解密并显示。这些通知预览存储在设备的本地数据库中，即使用户删除了原始消息或应用本身，数字取证工具仍可访问。苹果和谷歌的推送通知服务充当中间人，意味着通知内容会经过它们的服务器，并可能受到法律请求的约束。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/apple-fixes-ios-bug-that-retained-deleted-notification-data/">Apple fixes iOS bug that retained deleted notification data</a></li>
<li><a href="https://www.macobserver.com/news/fbi-finds-deleted-signal-messages-on-iphone-via-notification-storage-heres-how-to-protect-your-privacy/">FBI Finds Deleted Signal Messages on iPhone via Notification ...</a></li>
<li><a href="https://www.infosecurity-magazine.com/news/apple-ios-notification-bug-deleted/">Apple Fixes iOS Notification Bug Exposing Deleted Messages</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，该漏洞只是问题的一部分；主要问题在于通知文本存储在应用控制之外的系统数据库中。用户建议在 Signal 设置中启用通用通知（例如“您收到了一条消息”），以防止消息内容被缓存，并指出这通常是一种良好的隐私保护做法。

**标签**: `#security`, `#privacy`, `#iOS`, `#digital forensics`, `#notifications`

---

<a id="item-7"></a>
## [公民实验室揭露两起电信监控活动](https://techcrunch.com/2026/04/23/surveillance-vendors-caught-abusing-access-to-telcos-to-track-peoples-phone-locations-researchers-say/) ⭐️ 8.0/10

公民实验室的研究人员揭露了两起复杂的监控活动，其中供应商滥用其对电信网络的访问权限，追踪全球受害者的手机位置。 这一发现凸显了电信基础设施中可被利用进行大规模监控的系统性漏洞，对全球个人和组织的隐私与安全构成严重威胁。 这些活动涉及两家独立的监控供应商，线索指向一家以色列的商业地理情报提供商，但具体供应商未被点名。滥用行为利用了 SS7 等核心电信协议的弱点，实现实时位置追踪。

hackernews · mentalgear · Apr 23, 12:12

**背景**: 电信网络依赖 SS7（七号信令系统）等协议在运营商之间路由呼叫和共享位置数据。这些协议设计于数十年前，基于信任假设，缺乏现代安全防护，因此容易被拥有网络访问权限的行为者滥用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/04/23/surveillance-vendors-caught-abusing-access-to-telcos-to-track-peoples-phone-locations-researchers-say/">Surveillance vendors caught abusing access to telcos to... | TechCrunch</a></li>
<li><a href="https://securityaffairs.com/46473/hacking/ss7-protocol-surveillance.html">Hackers spy on Congressman abusing the SS 7 protocol</a></li>
<li><a href="https://arstechnica.com/information-technology/2019/09/hackers-are-exploiting-a-platform-agnostic-flaw-to-track-mobile-phone-locations/">Hackers are exploiting a platform-agnostic flaw to track mobile phone ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了深深的担忧和沮丧，用户分享了跟踪者利用电信访问权限的个人经历，并指出监控工具常被滥用于个人利益，例如 LOVEINT 事件。一些评论者还指出，在俄罗斯等国家，这种追踪是常态，数据最终会流入黑市。

**标签**: `#surveillance`, `#telecom security`, `#privacy`, `#citizen lab`, `#security research`

---

<a id="item-8"></a>
## [法国 ANTS 确认数据泄露，1900 万公民信息或遭窃](https://techcrunch.com/2026/04/22/france-confirms-data-breach-at-government-agency-that-manages-citizens-ids/) ⭐️ 8.0/10

法国国家安全证件署（ANTS）确认于 2026 年 4 月 15 日监测到数据泄露，黑客声称持有包含 1900 万条公民个人信息的数据库。 此次泄露涉及数百万法国公民的高度敏感个人信息，大幅增加了身份盗窃、欺诈和隐私侵犯的风险，也暴露了政府数字基础设施的脆弱性。 被盗数据包括姓名、出生日期、出生地、地址和电话号码；ANTS 正在调查攻击原因并已开始通知受影响公民，但具体受害人数尚未官方确认。

telegram · zaihuapd · Apr 23, 00:08

**背景**: ANTS（法国国家安全证件署）是负责签发身份证、护照及其他安全证件的政府机构。其在线门户 ants.gouv.fr 允许公民申请和更新这些证件，因此成为网络攻击的重点目标。此次泄露于 2026 年 4 月 15 日首次被发现，随后黑客在论坛上声称持有被盗数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.xinouzhou.com/wenzhang/145213-tu-fa-fa-guo-ants-ping-tai-zao-wang-luo-gong-ji-bu-fen-zheng-jian-shen-qing-ren-xin-xi-xie-lu">突发：法国ANTS平台遭网络攻击，部分证件申请人信息泄露</a></li>
<li><a href="https://www.investgo.cn/article/gb/gbdt/202604/843239.html">法国国家权证中心网站遭骇 大量个人数据泄露-“走出去”导航网</a></li>

</ul>
</details>

**标签**: `#data breach`, `#cybersecurity`, `#privacy`, `#government`, `#France`

---

<a id="item-9"></a>
## [吹风机操控巴黎天气传感器，Polymarket 获利超 3.4 万美元](https://fibo-crypto.fr/en/blog/polymarket-weather-sensor-manipulation-paris-meteo-france-2026/) ⭐️ 8.0/10

2026 年 4 月 6 日和 15 日，有人涉嫌使用吹风机加热巴黎戴高乐机场的法国气象局温度传感器，导致读数异常，从而在 Polymarket 的巴黎天气预测市场上触发超过 3.4 万美元的赔付。 这一事件揭示了一种新型攻击方式：通过物理操控物联网传感器来从预测市场中获利，引发了对去中心化预测平台数据完整性和安全性的严重担忧。 4 月 6 日，传感器读数在数分钟内从接近 18°C 跃升至超过 21°C；4 月 15 日，22°C 区间的概率在 30 分钟内从 0.1% 飙升至 95%。法国气象局已向航空运输宪兵队提起刑事控告，并在现场检查中发现篡改痕迹。

telegram · zaihuapd · Apr 23, 04:36

**背景**: Polymarket 是一个去中心化预测市场平台，用户根据真实世界事件的结果进行交易，赔付由经过验证的数据源决定。物联网传感器（如气象站）远程收集和传输数据，如果安全措施不足，可能成为物理操控的目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nftenex.com/paris-weather-sensor-polymarket-bet-hair-dryer-manipulation/">Paris Weather Sensor in $34K Polymarket Bet Manipulated by Hair ...</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pZZ3VYN0VCRndRREhCc0U1VjBDZ0FQAQ?hl=en-KE&gl=KE&ceid=KE:en">Report: Hair dryer used to manipulate Paris weather sensor - Overview</a></li>

</ul>
</details>

**标签**: `#prediction markets`, `#IoT security`, `#sensor manipulation`, `#Polymarket`, `#cybersecurity`

---

<a id="item-10"></a>
## [Google Cloud 默认安全缺陷导致用户产生巨额账单](https://www.tomshardware.com/tech-industry/artificial-intelligence/google-cloud-customer-wakes-up-to-usd18-000-bill-despite-usd7-budget-thanks-to-forgotten-public-api-key-attacker-put-in-60-000-requests-and-blasted-through-usd1-400-spending-cap) ⭐️ 8.0/10

澳大利亚 AI 顾问 Jesse Davies 尽管设置了 7 美元的预算上限，却因攻击者利用历史项目泄露的 API 密钥发起 6 万次请求，收到了 Google Cloud 高达 18,000 美元的账单。Google Cloud 在未通知的情况下自动上调信用额度，加剧了财务损失，不过 Google 最终免除了相关费用。 此事件揭示了 Google Cloud 默认配置中的系统性安全风险——原本作为公开标识符的 API 密钥，现在可能静默地授予对 Gemini 等付费 AI 服务的访问权限。它凸显了云服务提供商亟需采用安全默认设置和透明的账单控制机制，以保护客户免受意外财务灾难。 Truffle Security 指出，Gemini API 密钥格式单一且安全设置默认关闭，导致遗留的公开密钥容易遭受权限提升攻击。攻击者通过公开 URL 调用容器环境变量中的明文密钥，绕过了多项安全防护措施。

telegram · zaihuapd · Apr 23, 05:21

**背景**: Google Cloud API 密钥最初被设计为用于跟踪使用情况的公开标识符，而非秘密凭证。但随着 Gemini AI 的推出，这些相同的密钥现在可以访问付费的 AI 端点，实际上变成了秘密，却没有警告开发者。这种不安全的默认状态（CWE-1188）和错误的权限分配（CWE-269）意味着，泄露在代码仓库或公开 URL 中的密钥可能被利用进行未经授权的 AI 使用，从而导致巨额账单。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://trufflesecurity.com/blog/google-api-keys-werent-secrets-but-then-gemini-changed-the-rules">Google API Keys Weren't Secrets. But then Gemini Changed the ...</a></li>
<li><a href="https://cybersecuritynews.com/google-api-keys-gemini/">Google API Keys Expose Private Data Silently Through Gemini</a></li>
<li><a href="https://www.techradar.com/pro/security/usd15k-bill-destroyed-a-solo-developers-startup-how-hackers-are-using-leaked-google-api-keys-to-go-wild-with-gemini-ai-for-free">Google API keys give attackers unauthorized Gemini AI access</a></li>

</ul>
</details>

**标签**: `#Google Cloud`, `#security`, `#cloud computing`, `#API keys`, `#financial risk`

---

<a id="item-11"></a>
## [字节跳动发布 Seed3D 2.0，3D 生成达到生产可用水平](https://paipancon.com/fc2daily/detail/FC2-PPV-1700423) ⭐️ 8.0/10

字节跳动发布了新一代 3D 生成大模型 Seed3D 2.0，在几何精度和材质质量两项核心指标上取得 SOTA 结果，纹理生成的人类评测中相对主流模型的偏好率超过 69%。 这一进展将 3D 内容生成从演示级推进到生产可用，大幅降低了为游戏、仿真和机器人领域创建高质量 3D 资产的门槛，并且扩展到了部件级生成和物理仿真兼容性。 Seed3D 2.0 支持部件级生成和场景组合，可先拆分 3D 内容部件再补全形状，并输出带完整关节信息的 URDF 等标准格式内容，适配 NVIDIA Isaac Sim 等物理仿真引擎。

telegram · zaihuapd · Apr 23, 08:15

**背景**: 传统的 3D 模型生成往往在演示中看起来不错，但由于几何精度不足或材质不真实而难以用于生产。URDF（统一机器人描述格式）是一种基于 XML 的标准，用于在机器人领域描述带有连杆和关节的机器人结构；Isaac Sim 是 NVIDIA 的 GPU 加速物理仿真平台，用于训练和验证基于 AI 的机器人。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wiki.ros.org/urdf/XML/model">XML Robot Description Format (URDF) - ROS Wiki</a></li>
<li><a href="https://docs.isaacsim.omniverse.nvidia.com/4.5.0/physics/simulation_fundamentals.html">Physics Simulation Fundamentals — Isaac Sim Documentation</a></li>
<li><a href="https://github.com/isaac-sim">NVIDIA Isaac Sim - GitHub</a></li>

</ul>
</details>

**标签**: `#3D generation`, `#ByteDance`, `#AI`, `#computer graphics`, `#physics simulation`

---

<a id="item-12"></a>
## [DeepSeek 开源 TileKernels 算子库，支持 Blackwell](https://github.com/deepseek-ai/TileKernels) ⭐️ 8.0/10

DeepSeek 开源了基于 TileLang 的高性能 GPU 算子库 TileKernels，该库针对大语言模型（LLM）的训练与推理进行了深度优化。它支持 NVIDIA SM90 及最新的 SM100（Blackwell）架构，运行环境要求 CUDA 13.1 及以上版本。 此次开源为 AI 社区提供了在最新 Blackwell GPU 上运行 LLM 工作负载的、接近硬件极限的生产级算子，有望加速训练和推理性能。这也体现了 DeepSeek 对开源 AI 基础设施的承诺，惠及构建大规模模型的开发者和研究人员。 TileKernels 涵盖了 MoE 路由、FP8/FP4 量化及多种融合算子，并已在 DeepSeek 内部环境投入使用。该库基于 TileLang 构建，TileLang 是一种使用张量分块抽象的 GPU 内核开发领域特定语言。

telegram · zaihuapd · Apr 23, 09:36

**背景**: 像 TileKernels 这样的 GPU 算子库为常见的深度学习操作（如矩阵乘法和注意力机制）提供了底层优化的内核。TileLang 是一种领域特定语言，通过使用张量分块抽象来简化高性能 GPU 内核的编写，从而降低代码复杂度。NVIDIA 的 Blackwell 架构（SM100）引入了新的张量核心指令，其速度是上一代 Hopper 架构的 2 到 4 倍，因此优化的算子对于充分发挥其潜力至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tilelang.com/">TileLang 0.1.8 documentation</a></li>
<li><a href="https://docs.nvidia.com/cutlass/4.3.3/media/docs/cpp/blackwell_functionality.html">Blackwell SM 100 GEMMs — NVIDIA CUTLASS Documentation</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#GPU算子库`, `#LLM`, `#NVIDIA Blackwell`, `#开源`

---

<a id="item-13"></a>
## [腾讯开源混元 Hy3 preview：295B MoE 模型](https://mp.weixin.qq.com/s/5_nUI2mDchlwoedinFUMeA) ⭐️ 8.0/10

腾讯正式发布并开源了混元 Hy3 preview，这是一个总参数量达 295B、激活参数为 21B 的混合专家模型（MoE），支持 256K 上下文长度，专为复杂推理与智能体（Agent）应用优化。 此次发布标志着中国科技巨头在开源领域的重要贡献，提供了一个具备强大推理能力的大规模 MoE 模型，可与其它领先开源模型竞争；同时，该模型已集成到元宝、QQ 等腾讯内部产品中，展示了实际的企业级部署能力。 得益于模型架构与推理框架的深度协同优化，CodeBuddy 等产品的首 token 延迟降低了 54%；该模型已在 GitHub、HuggingFace 等平台开源，并通过腾讯云 API 提供服务，个人版定价最低 28 元/月。

telegram · zaihuapd · Apr 23, 10:07

**背景**: 混合专家模型（MoE）是一种将模型拆分为多个专门子模型（专家）的架构，每次推理仅激活其中一部分专家，从而在保持总参数量庞大的同时实现高效推理。总参数 295B、激活参数 21B 意味着该模型虽然规模巨大，但推理速度可与小得多的稠密模型媲美，便于实际部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/nlp/what-is-mixture-of-experts-moe/">What is Mixture of Experts (MoE)? - GeeksforGeeks</a></li>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts (MoE) Images Mixture of Experts Explained - Hugging Face Understanding Mixture of Experts (MoE): The Architecture ... What is mixture of experts? - IBM What Is Mixture of Experts (MoE)? How It Works (2026) MoE LLM Architecture: How It Works, Benefits And Key Models ...</a></li>
<li><a href="https://medium.com/@sharanharsoor/understanding-mixture-of-experts-moe-the-architecture-powering-next-generation-language-models-49c1d1d467c9">Understanding Mixture of Experts (MoE): The Architecture ...</a></li>

</ul>
</details>

**标签**: `#large language model`, `#open source`, `#MoE`, `#Tencent`, `#AI`

---

<a id="item-14"></a>
## [香港证监会与普华永道就恒大造假达成 10 亿港元和解](https://apps.sfc.hk/edistributionWeb/gateway/TC/news-and-announcements/news/doc?refNo=26PR62) ⭐️ 8.0/10

2026 年 4 月 23 日，香港证券及期货事务监察委员会（证监会）宣布与普华永道香港达成和解协议，普华永道将预留 10 亿港元，用于赔偿中国恒大集团合资格独立少数股东，因其在恒大 2019 及 2020 财年虚增收入 5641 亿元人民币的财务造假中扮演了角色。 这是香港首次有已倒闭公司的核数师直接向股东作出赔偿，为核数师责任和市场廉洁树立了里程碑式的先例。这凸显了审计独立性的关键作用，并可能重塑主要金融市场对核数师的监管预期。 香港证监会认定，普华永道严重违反专业责任，包括丧失审计独立性、缺乏专业怀疑态度及默许管理层操纵审计样本。根据协议，普华永道在不承认法律责任的前提下解决此事，证监会将不再采取进一步行动。

telegram · zaihuapd · Apr 23, 12:07

**背景**: 中国恒大集团曾是中国最大的房地产开发商之一，在多年财务不当行为后因巨额债务崩溃。2024 年，中国监管机构因恒大在 2019 年和 2020 年虚增收入 5641 亿元人民币（将报告盈利转为巨额亏损）对其处以 417.5 亿元人民币罚款。普华永道在此期间担任恒大的核数师，被指控未能发现该欺诈行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://xueqiu.com/3338215700/385417746">突发！香港证监会与普华永道就恒大财务造假达成赔偿协议，10亿港元赔...</a></li>
<li><a href="https://www.thepaper.cn/newsDetail_forward_33037031">香港证监会、会财局同日出手 普华永道同意预留10亿港元赔偿恒大股东_...</a></li>

</ul>
</details>

**标签**: `#financial regulation`, `#audit failure`, `#corporate fraud`, `#market integrity`, `#regulatory tech`

---

<a id="item-15"></a>
## [中国三大运营商报告国际网络故障](https://t.me/zaihuapd/41029) ⭐️ 8.0/10

未经证实的消息称，中国电信、中国联通和中国移动的国际路由出现大范围网络故障，通往香港、日本和美国方向的连接出现严重丢包和中断。 此次事件影响依赖跨境连接进行工作、教育和通信的广泛用户群体，如果中断是人为所致，可能具有地缘政治影响。三大运营商同时出现故障，表明问题具有系统性而非孤立故障。 故障影响包括中国电信 CN2 和中国联通 9929 在内的高级路由，以及 163 和 4837 等标准路由。报告主要集中在北京移动用户，前往美国方向的路由样本较少。

telegram · zaihuapd · Apr 23, 12:45

**背景**: 中国电信运营商运营多级国际路由：高级路由如中国电信 CN2 和中国联通 9929 提供更高优先级和更低延迟，标准路由如 163 和 4837 处理普通流量。这些路由对跨境数据传输至关重要，中断可能源于海底光缆断裂、路由配置错误或人为策略调整。此次事件的原因尚不清楚。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/yeahwu404/status/2047301068175065487">风闻消息，部分地区受影响，受影响的可以底下留言，也别说谣言不谣言...</a></li>
<li><a href="https://www.deepflood.com/post-37587-1">风闻消息：中国联通、移动、电信运营商对海外方向均报告网络故障</a></li>
<li><a href="https://tbbbk.com/vps-route-guide-tcping-as9929-cn2-explained/">VPS 路由完全指南（2026）：Tcping 测速、AS9929、CN2 线路怎么看？</a></li>

</ul>
</details>

**社区讨论**: 社交媒体和论坛上的社区评论大多证实了中断情况，用户分享本地化体验和路由追踪结果。部分用户猜测中断是技术故障还是人为策略调整，但尚未达成共识。

**标签**: `#network outage`, `#China telecom`, `#internet infrastructure`, `#routing`, `#geopolitics`

---

<a id="item-16"></a>
## [苹果 CEO 蒂姆·库克将卸任，约翰·特努斯 2026 年接任](https://t.me/zaihuapd/41030) ⭐️ 8.0/10

苹果公司宣布，现任 CEO 蒂姆·库克将于 2026 年 9 月 1 日卸任，由硬件工程高级副总裁约翰·特努斯接任 CEO。库克将转任董事会执行董事长。 此次领导层变动是苹果自 2011 年库克接任以来的首次 CEO 交接，标志着公司产品战略和企业方向进入新时代。硬件工程资深人士约翰·特努斯将领导这家全球最具价值的科技公司之一。 特努斯于 2001 年加入苹果，2013 年升任硬件工程副总裁，负责 iPhone、iPad、Mac、Apple Watch、AirPods 和 Apple Vision Pro 等产品的工程工作。现任董事长 Arthur Levinson 将于 2026 年 9 月 1 日转任首席独立董事，特努斯同日加入董事会。

telegram · zaihuapd · Apr 23, 13:46

**背景**: 蒂姆·库克自 2011 年接替史蒂夫·乔布斯担任苹果 CEO 以来，带领公司在收入、服务和产品线方面实现了巨大增长。约翰·特努斯在苹果硬件工程领域工作了二十多年，领导了公司许多最具标志性产品的开发。执行董事长一职使库克能够继续参与长期战略和公共事务，同时将日常运营交给特努斯。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/John_Ternus">John Ternus - Wikipedia</a></li>
<li><a href="https://www.apple.com/leadership/john-ternus/">Apple Leadership - John Ternus - Apple</a></li>
<li><a href="https://www.apple.com/newsroom/2026/04/tim-cook-to-become-apple-executive-chairman-john-ternus-to-become-apple-ceo/">Tim Cook to become Apple Executive Chairman John Ternus to ...</a></li>

</ul>
</details>

**标签**: `#Apple`, `#leadership change`, `#CEO transition`, `#tech industry`

---

<a id="item-17"></a>
## [英国 NCSC 正式将通行密钥列为首选身份验证方式](https://www.techradar.com/pro/security/uk-security-agency-officially-declares-passkeys-superior-to-passwords-passkeys-should-be-the-first-choice-for-authentication) ⭐️ 8.0/10

英国国家网络安全中心（NCSC）正式宣布，通行密钥（Passkeys）优于传统密码和两步验证，并建议将其作为数字服务的首选登录方式。这标志着 NCSC 此前因实施挑战而持有的观望态度发生了转变。 作为英国国家网络安全技术权威机构，NCSC 的背书为通行密钥提供了重要的行业认可，可能加速其在公共和私营部门的普及。此举有望重塑全球身份验证标准，减少对易受攻击密码的依赖，并提升整体网络韧性。 在英国，超过 50%的 Google 活跃用户已注册通行密钥，eBay 和 PayPal 等主流平台也已完全适配。NCSC 指出，过去 12 个月内的技术进步解决了核心实施难题，使通行密钥比基于密码的系统更安全且更易用。

telegram · zaihuapd · Apr 23, 14:47

**背景**: NCSC 是英国网络安全技术权威机构，隶属于 GCHQ，于 2016 年成立，旨在提供统一的国家级网络威胁应对方案。通行密钥是一种无密码身份验证方法，使用设备存储的加密密钥和生物识别验证（如指纹或面部识别）替代传统密码，旨在消除网络钓鱼和凭证窃取等常见安全风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/National_Cyber_Security_Centre_(United_Kingdom)">National Cyber Security Centre (United Kingdom) - Wikipedia</a></li>
<li><a href="https://ico.org.uk/for-organisations/the-guide-to-nis/the-role-of-the-national-cyber-security-centre-ncsc/">The role of the National Cyber Security Centre (NCSC) | ICO</a></li>
<li><a href="https://www.gov.uk/government/organisations/national-cyber-security-centre">National Cyber Security Centre - GOV.UK Top Stories Cyber Security - GCHQ Understanding the Role of the NCSC - ukcybersecurity.co.uk National Cyber Security Centre (United Kingdom) - Wikipedia UK Faces a Cyber ‘Perfect Storm’ - Infosecurity Magazine The role of the National Cyber Security Centre ( NCSC ) | ICO Cyber Security | GCHQ - GCHQ.GOV. UK Understanding the Role of the NCSC - ukcybersecurity.co. uk The role of the National Cyber Security Centre ( NCSC ) | ICO</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#authentication`, `#passkeys`, `#NCSC`, `#identity`

---

<a id="item-18"></a>
## [欧盟施压谷歌开放安卓 AI 助手权限](https://www.bloomberg.com/news/articles/2026-04-23/google-faces-eu-pressure-to-open-up-android-to-gemini-rivals) ⭐️ 8.0/10

欧盟正在起草要求，迫使谷歌在安卓系统上给予 ChatGPT、Claude 等竞争对手的 AI 助手与其自家 Gemini 相同的系统级权限。 这可能通过降低竞争对手在主导安卓平台上的门槛来重塑 AI 助手市场的竞争格局，但谷歌警告称这可能损害用户安全和隐私。 这些要求仍处于草案阶段，发布时间可能推迟；谷歌担心这种开放可能对用户安全和隐私产生负面影响。

telegram · zaihuapd · Apr 23, 15:31

**背景**: 欧盟的《数字市场法案》（DMA）将谷歌等大型平台指定为“守门人”，并制定规则确保公平竞争。安卓是全球使用最广泛的移动操作系统，谷歌的 Gemini 是许多安卓设备上的默认 AI 助手，这使其相对于第三方助手拥有显著优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://digital-markets-act.ec.europa.eu/index_en">Digital Markets Act</a></li>
<li><a href="https://www.android.com/intl/en_us/ai/gemini/">Try Gemini, your personal AI assistant | Android</a></li>

</ul>
</details>

**标签**: `#EU regulation`, `#Android`, `#AI assistants`, `#Google`, `#antitrust`

---

<a id="item-19"></a>
## [OpenAI macOS 版 Chronicle 功能引发隐私与安全争议](https://www.theregister.com/2026/04/22/openai_chronicle_no_privacy_screenshot/) ⭐️ 7.0/10

OpenAI 为其 macOS 版 Codex 应用推出了一项名为 Chronicle 的选择性加入研究预览功能，该功能通过截取屏幕图像为 AI 代理提供上下文信息。安全研究人员批评该功能是微软 Recall 功能的翻版，指出其存在 OCR 文本未加密本地存储以及易受提示注入攻击等风险。 该功能引发了重大的隐私和安全担忧，可能削弱用户对 AI 工具的信任并减缓其采用，尤其是在安全敏感的环境中。此次争议与微软 Recall 此前遭遇的抵制如出一辙，凸显了 AI 便利性与数据保护之间的持续紧张关系。 截屏数据仅在本地存储 6 小时，但通过 OCR 提取的文本“记忆”会以未加密形式长期保存在本地，并可被设备上其他程序访问。此外，这些记忆可能在后续对话中被重新发送至 OpenAI 服务器，且该功能会加速消耗 Codex 的速率限制，降低了其在安全环境下的实用性。

telegram · zaihuapd · Apr 23, 03:06

**背景**: 提示注入是一种通过恶意提示攻击机器学习模型的网络安全攻击方式，可能导致 AI 忽略其预期指令。微软的 Recall 功能同样通过截取屏幕为 AI 提供上下文，在 2024 年遭遇了类似的隐私抵制。OpenAI 的 Chronicle 以类似方式运行，将 OCR 文本存储在本地，使其容易受到此类攻击和未授权访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#privacy`, `#security`, `#AI`, `#macOS`

---

<a id="item-20"></a>
## [台积电因成本过高推迟导入 ASML 高数值孔径 EUV 至 2029 年](https://money.udn.com/money/story/5599/9458925?from=edn_newestlist_rank) ⭐️ 7.0/10

台积电在北美技术论坛上宣布，至少到 2029 年底前不会将 ASML 的高数值孔径 EUV 光刻机用于晶圆量产，原因是单台售价已超过 3.5 亿欧元。 这一决定标志着半导体制造路线图的重大转变——全球领先的代工厂台积电选择优化现有 EUV 设备而非采用下一代光刻技术，可能放缓摩尔定律的推进速度，并影响 ASML 的营收预期。 台积电还披露，A13 制程计划于 2029 年投产，并计划在同年于亚利桑那州建立 CoWoS 和 3D-IC 封装产能，当地首座晶圆厂良率已接近台湾工厂。

telegram · zaihuapd · Apr 23, 11:22

**背景**: 高数值孔径 EUV 光刻是 ASML 最新的极紫外光刻机，用于制造更小晶体管的先进芯片。CoWoS（Chip-on-Wafer-on-Substrate）是台积电的先进封装技术，通过垂直堆叠芯片来提升性能并降低功耗，对 AI 和高性能计算应用至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1890075894934132607">半导体芯片封装“CoWoS工艺技术”的详解； - 知乎</a></li>
<li><a href="https://blog.csdn.net/u013669912/article/details/143434272">CoWoS 封装 | CoWoS-S / CoWoS-R / CoWoS-L-CSDN博客</a></li>
<li><a href="https://finance.sina.com.cn/cj/2026-02-27/doc-inhpfxrh6696864.shtml">台积电先进封装科普：CoWoS、CoPoS、CoWoP 到底是个啥？谁才是下一代...</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#TSMC`, `#ASML`, `#EUV`, `#manufacturing`

---