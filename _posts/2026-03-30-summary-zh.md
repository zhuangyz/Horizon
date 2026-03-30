---
layout: default
title: "Horizon Summary: 2026-03-30 (ZH)"
date: 2026-03-30
lang: zh
---

> From 18 items, 10 important content pieces were selected

---

1. [谷歌将量子威胁应对期限提前至 2029 年，警告现有加密算法面临破解风险](#item-1) ⭐️ 9.0/10
2. [ChatGPT 在允许用户输入前，使用 Cloudflare 读取 React 状态进行机器人检测](#item-2) ⭐️ 8.0/10
3. [文章警告 AI 吸收公共创新，形成'认知黑暗森林'](#item-3) ⭐️ 8.0/10
4. [旅行者 1 号仅靠 69KB 内存和 8 轨磁带录音机运行，展现 1977 年的工程成就。](#item-4) ⭐️ 8.0/10
5. [GitHub 遭遇大规模机器人攻击，大量仓库 Issues 被黑产广告灌入](#item-5) ⭐️ 8.0/10
6. [Pretext 库实现无需 DOM 交互的文本高度计算，提升网页性能](#item-6) ⭐️ 7.0/10
7. [Firefox 服务条款披露数据共享细节：浏览记录与唯一标识符或传至谷歌](#item-7) ⭐️ 7.0/10
8. [谷歌内部 AI 编码工具 Agent Smith 因使用激增被限制访问，同时推动员工强制采用 AI](#item-8) ⭐️ 7.0/10
9. [北京推出全国首个覆盖 L2 至 L4 级别的智能网联汽车专属商业保险](#item-9) ⭐️ 7.0/10
10. [沃顿商学院研究发现'认知投降'现象：人们更易接受 AI 输出而不加核验](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [谷歌将量子威胁应对期限提前至 2029 年，警告现有加密算法面临破解风险](https://blog.google/innovation-and-ai/technology/safety-security/cryptography-migration-timeline/) ⭐️ 9.0/10

谷歌宣布将应对“量子日（Q Day）”的期限大幅提前至 2029 年，届时量子计算机预计将能破解现有公钥加密算法（如 RSA 和椭圆曲线）。谷歌调整了威胁模型，其研究显示破解 2048 位 RSA 密钥可能仅需约 100 万个“有噪声的量子比特”，远低于此前预估的 10 亿个。 这一声明标志着威胁评估的重大范式转变，为全球安全基础设施带来了直接且深远的紧迫感。它迫使各国政府、行业和标准机构加速向后量子密码学（PQC）迁移，以防范针对敏感数据的“先存储后解密”攻击。 谷歌将优先推进身份验证服务和数字签名的后量子加密（PQC）迁移作为初步防御。修订后的 2029 年时间表比此前的行业预期及美国政府的要求更为激进，其目的是为全球数字化转型提供必要的清晰度与紧迫感。

telegram · zaihuapd · Mar 29, 01:18

**背景**: 公钥密码学，如 RSA 和椭圆曲线密码学（ECC），保障了当今大多数数字通信和交易的安全。一台足够强大的量子计算机可以利用肖尔算法破解这些算法，使当前加密方式失效。后量子密码学（PQC）指的是设计用于抵御经典和量子计算机攻击的密码算法。“先存储后解密”威胁描述的是一种攻击策略，即攻击者现在收集加密数据，待未来量子计算机具备能力时再进行解密。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post - quantum cryptography - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Harvest_now,_decrypt_later">Harvest now, decrypt later - Wikipedia</a></li>

</ul>
</details>

**标签**: `#quantum-computing`, `#cryptography`, `#cybersecurity`, `#post-quantum-cryptography`, `#encryption`

---

<a id="item-2"></a>
## [ChatGPT 在允许用户输入前，使用 Cloudflare 读取 React 状态进行机器人检测](https://www.buchodi.com/chatgpt-wont-let-you-type-until-cloudflare-reads-your-react-state-i-decrypted-the-program-that-does-it/) ⭐️ 8.0/10

一项技术分析揭示，ChatGPT 网页应用在启用用户的文本输入框之前，会将特定的 React 组件状态数据发送给 Cloudflare 进行验证。这项检查发生在页面初始加载期间，是一个复杂的、应用层的机器人检测机制的一部分，旨在区分运行完整 React 应用的真实浏览器和自动化脚本。 这很重要，因为它代表了机器人防护的重大演变，超越了传统的网络或浏览器层检查，转而检查客户端应用框架的实际状态。它直接影响 OpenAI 保护其免费 ChatGPT 服务不被滥用作非官方 API 的能力，确保 GPU 资源分配给真实的人类用户，但也引发了关于合法用户的网络可用性和隐私的疑问。 该检测依赖于仅在 React 应用完全渲染和水合（hydrated）后才存在的特定属性；不执行 JavaScript 包或不运行 React 的无头浏览器或机器人框架将缺少这些属性。这项技术是利用客户端信号的一个例子，Cloudflare 的 Bot Management 系统可以将其与包含机器学习和行为分析的多层检测模型集成。

hackernews · alberto-m · Mar 29, 20:21

**背景**: Cloudflare Bot Management 是一项服务，它使用多层检测，包括全局和特定于应用的机器学习模型、客户端 JavaScript 信号和请求元数据，来识别和管理自动化机器人流量。React 是一个用于构建用户界面的流行 JavaScript 库，其“状态”指的是决定组件在任何时间点的渲染和行为的数据。客户端机器人检测方法通常涉及分析用户代理字符串、设备指纹识别以及监控与人类交互模式不同的行为异常。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.cloudflare.com/bots/additional-configurations/detection-ids/">Detection IDs · Cloudflare bot solutions docs</a></li>
<li><a href="https://assets.ctfassets.net/slt3lc6tev37/1DzWC1w6QLq0pvyYplHRDZ/650902f4caedb5c22bd83bbb8cd7b1c4/Cloudflare_Bot_Management_Datasheet.pdf">Cloudflare Bot Management Datasheet - assets.ctfassets.net</a></li>
<li><a href="https://www.humansecurity.com/learn/topics/what-is-bot-detection/">Bot Detection Guide 2025: How to Identify & Block Bots</a></li>

</ul>
</details>

**社区讨论**: 讨论中包含了 OpenAI 工程师（Nick）的直接回应，他解释这些检查是为了保护资源免遭滥用并维持免费访问的可用性。社区情绪复杂：一些用户批评其对网络可用性的影响，列举了过多的验证码；另一些用户则争论这种应用层检测水平对于复杂平台来说是新颖的还是意料之中的。一个关键的争论点是这究竟是一种合理的安全措施，还是一种损害用户体验的过度行为。

**标签**: `#web-security`, `#react`, `#bot-detection`, `#cloudflare`, `#openai`

---

<a id="item-3"></a>
## [文章警告 AI 吸收公共创新，形成'认知黑暗森林'](https://ryelang.org/blog/posts/cognitive-dark-forest/) ⭐️ 8.0/10

一篇发表在 Rye 编程语言博客上的文章提出了'认知黑暗森林'的概念，认为 AI 系统吸收人类生成的内容，创造了一个新想法会立即被作为训练数据吸收的环境。作者认为，这种动态可能会抑制公共创新，因为控制 AI 模型的一方可以克隆新想法，而无需回报原始创造者。 这个概念之所以重要，是因为它挑战了 AI 时代传统的创新与知识共享经济学。如果公开分享想法成为强大、中心化的 AI 模型的直接输入，却没有公平的补偿或归属，可能会导致创新退回到私有的封闭系统中，从而降低公共信息生态系统的质量。 文章概述了两种可能的路径：创新被完全纳入 AI'森林'，使公共创新者无利可图；或者大规模退出公共分享，导致创新转向私有。社区讨论中的一个关键反驳点是病毒式许可证（如 GPL 或 CC）应用于数据的潜在作用，这可能对 AI 模型如何使用该数据进行训练施加法律限制。

hackernews · kaycebasques · Mar 29, 19:36

**背景**: '黑暗森林'一词借用于一个科幻假说，该假说认为高级文明会隐藏起来以避免被发现和潜在毁灭。大语言模型（LLMs）是在来自公共互联网的海量文本和代码数据集上训练的 AI 系统。'创新公地'指的是公共知识和想法的共享池，经济和技术的进步常常从中产生。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dark_forest_hypothesis">Dark forest hypothesis - Wikipedia</a></li>
<li><a href="https://oxylabs.io/blog/llm-training-data">LLM Training Data: The 8 Main Public Data Sources</a></li>
<li><a href="https://en.wikipedia.org/wiki/Innovation_economics">Innovation economics - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示出不同的反应，一些人认为这个类比很有说服力，另一些人则持怀疑态度。关键观点包括：将其与凯斯勒综合征（太空碎片）进行比较；争论这种动态是全新的还是现有模仿行为的加速；以及探索潜在的解决方案，如对数据应用病毒式许可证以限制 AI 训练使用。一些评论者还指出，当前的大语言模型并非从新的公开帖子中'即时'学习，因为它们有固定的知识截止日期。

**标签**: `#AI Ethics`, `#Information Theory`, `#Innovation Economics`, `#LLM Training`, `#Knowledge Commons`

---

<a id="item-4"></a>
## [旅行者 1 号仅靠 69KB 内存和 8 轨磁带录音机运行，展现 1977 年的工程成就。](https://techfixated.com/a-1977-time-capsule-voyager-1-runs-on-69-kb-of-memory-and-an-8-track-tape-recorder-4/) ⭐️ 8.0/10

近期一篇文章强调，美国宇航局于 1977 年发射的旅行者 1 号探测器，至今仍在星际空间运行，其全部内存仅为 69KB，并使用 8 轨磁带录音机进行数据存储。其卓越的寿命已远超原定任务时限。 这证明了坚固、专用工程的强大力量，并挑战了现代关于复杂任务需要庞大计算资源的假设。它成为航空航天及其他领域可靠性、效率和长期系统设计的持久标杆。 这 69KB 内存由旅行者号上六台定制计算机共享，这些计算机使用 CMOS 和 TTL 集成电路。8 轨磁带录音机采用 20 世纪 60 至 80 年代流行的 Stereo 8 格式，用于在将科学数据传回地球前进行存储。

hackernews · speckx · Mar 29, 16:12

**背景**: 旅行者 1 号和 2 号是 1977 年发射的相同航天器，用于研究外行星。它们的计算机系统设计在严苛的太空环境中，极度注重可靠性和能效。20 世纪 60 年代的阿波罗制导计算机（AGC）拥有 72KB ROM 和 4KB RAM，为有限内存的太空计算提供了先例。在固态存储器普及之前，磁带录音机是标准且可靠的数据存储技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Voyager_1">Voyager 1 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Voyager_program">Voyager program - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apollo_Guidance_Computer">Apollo Guidance Computer - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区对旅行者号的寿命及其涉及的高风险工程（例如一次耗时 46 小时、无法回滚的推进器修复成功）表示惊叹。评论还将旅行者号的效率与现代软件膨胀进行鲜明对比，指出一个内存 69KB 的航天器与使用数 GB 内存的应用程序并存的讽刺性。有人推荐了一部关于日渐老化的任务团队的纪录片。

**标签**: `#space-technology`, `#systems-engineering`, `#hardware`, `#historical-computing`, `#reliability`

---

<a id="item-5"></a>
## [GitHub 遭遇大规模机器人攻击，大量仓库 Issues 被黑产广告灌入](https://github.com/microsoft/WSL/issues) ⭐️ 8.0/10

GitHub 正遭遇一场有组织的大规模机器人攻击，多个机器人并发地在热门仓库的 Issues 板块中大量发布垃圾信息和黑产广告，内容主要为中文赌博引流。受影响的仓库包括 Microsoft/WSL、anomalyco/opencode、msgpack/msgpack-node 和 home-assistant/frontend 等，部分仓库已暂时关闭 Issues 功能以恢复正常。 此次攻击直接干扰了重要开源项目的协作流程，损害了这一全球软件开发核心平台的完整性。它凸显了 GitHub 等平台面临的安全和内容审核挑战，即自动化垃圾信息可以绕过标准的举报和拉黑工具，这可能削弱社区对平台功能的信任。 垃圾帖子的典型模式是前半部分贴广告图片，后半部分模仿技术讨论或 AI 模型论述，这增加了自动过滤的难度。标准的审核操作，如举报和拉黑用户，在此次攻击浪潮中似乎无法生效，表明机器人可能使用了更复杂的规避技术。

telegram · zaihuapd · Mar 29, 13:35

**背景**: GitHub Issues 是软件项目内用于跟踪错误、功能请求和进行一般讨论的核心功能，是社区协作的主要渠道。对此类平台的垃圾信息和机器人攻击，通常旨在利用其可见性进行非法广告宣传，如赌博或诈骗。保持这些空间的信噪比对于高效的开源开发至关重要。

**标签**: `#github`, `#security`, `#spam`, `#open-source`, `#incident`

---

<a id="item-6"></a>
## [Pretext 库实现无需 DOM 交互的文本高度计算，提升网页性能](https://simonwillison.net/2026/Mar/29/pretext/#atom-everything) ⭐️ 7.0/10

前 React 核心开发者程娄发布了 Pretext，这是一个新的浏览器库，能够在无需与 DOM 交互的情况下计算换行文本段落的高度。该库采用 prepare() 和 layout() 函数的两步法，运用巧妙的技巧使计算速度比传统的 DOM 测量方法快得多。 这很重要，因为 DOM 操作是 Web 应用中的主要性能瓶颈，每个 DOM 节点在样式重计算和布局工作时都会消耗内存和 CPU 时间。通过消除文本高度计算中的 DOM 交互，Pretext 使得以前因成本过高而无法在浏览器应用中实现的新文本渲染效果和动态布局成为可能。 该库通过在多个浏览器中渲染《了不起的盖茨比》全文来严格验证测量准确性，并包含一个 corpora 文件夹，其中包含针对泰语、中文、韩语、日语、阿拉伯语等语言的长篇公共领域文档的测试。prepare() 函数将文本分割成片段（单词、软连字符、表情符号等）并使用离屏 canvas 进行测量并缓存结果，而 layout() 则模拟浏览器换行逻辑来确定指定宽度下的行数和总高度。

rss · Simon Willison · Mar 29, 20:08

**背景**: 传统上，在 Web 应用中计算文本尺寸需要将文本渲染到 DOM 中再进行测量，这会触发昂贵的浏览器布局和绘制操作。文档对象模型 (DOM) 表示网页的结构，操作它的计算成本很高，因为每次更改都可能触发样式重计算、布局和重绘操作。程娄以创建 react-motion 动画库而闻名，并曾任职于 React 核心团队，这为该技术方案带来了重要的可信度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://allahabadi.dev/blogs/frontend/dom-size-interactivity-performance/">DOM Size Is Killing Your Interactivity — Here’s How to Fix It</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/CSS/line-height">line-height - CSS - MDN Web Docs</a></li>
<li><a href="https://motion.dev/">Motion — JavaScript & React animation library</a></li>

</ul>
</details>

**标签**: `#web-development`, `#performance`, `#javascript`, `#ui-ux`, `#frontend`

---

<a id="item-7"></a>
## [Firefox 服务条款披露数据共享细节：浏览记录与唯一标识符或传至谷歌](https://www.mozilla.org/zh-CN/privacy/firefox/) ⭐️ 7.0/10

Mozilla 近期更新的 Firefox 服务条款明确显示，浏览数据、搜索记录、地理位置及唯一标识符等信息可能会与包括谷歌云平台在内的合作伙伴共享，用于云端计算、数据分析和营销活动改进。这一披露引发了隐私合规质疑，焦点在于“浏览数据”与“浏览历史”的定义差异，以及通过共享唯一标识符可能导致的跨平台追踪风险。 此事之所以重要，是因为 Firefox 一直以注重隐私的浏览器形象建立其品牌声誉，而此次披露的条款似乎与这一形象相悖，可能侵蚀用户信任。共享唯一标识符尤其关键，因为它使得跨不同网站和服务的持续性用户追踪成为可能，这在数据实践日益受到审查的生态系统中引发了严重的用户隐私担忧。 一个关键细节在于条款中对“浏览数据”（可能包括缓存、Cookie 和其他技术信息）和“浏览历史”（访问过的具体页面列表）的模糊区分，前者被共享，而 Mozilla 声称后者不会与营销合作伙伴共享。此外，条款并未明确说明触发数据上传的具体场景，也未说明默认设置下的收集频率。

telegram · zaihuapd · Mar 29, 06:57

**背景**: 浏览器指纹识别是一种追踪技术，它收集用户浏览器和设备的众多数据点（如屏幕分辨率、已安装字体、时区）来创建唯一标识符，该标识符可以跨网站追踪用户，而无需像 Cookie 那样在本地存储任何信息。Firefox 用于防范网络钓鱼和恶意软件的“安全浏览”功能，就是来自谷歌的专有协议，涉及数据交换。浏览数据是一个比浏览历史更广泛的类别，它包含历史记录以及缓存、Cookie 和保存的密码等。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://whatismylocation.org/blog/browser-fingerprinting-explained">Browser Fingerprinting: What Websites Know About You (And How ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Firefox">Firefox - Wikipedia</a></li>
<li><a href="https://linuxhint.com/clear_cache_vs_browsing_history/">Is clearing cache the same as deleting browsing history? – Linux Hint</a></li>

</ul>
</details>

**社区讨论**: 根据新闻内容的上下文，社区讨论显示用户正在敦促 Mozilla 提高透明度，明确解释在默认配置下数据收集的频率与具体用途。用户对此问题的重要性表示严重关切和认同，并质疑这些数据共享实践如何与 Firefox “隐私优先”的品牌形象保持一致。

**标签**: `#privacy`, `#firefox`, `#data-sharing`, `#browser-security`, `#user-tracking`

---

<a id="item-8"></a>
## [谷歌内部 AI 编码工具 Agent Smith 因使用激增被限制访问，同时推动员工强制采用 AI](https://www.businessinsider.com/google-agent-smith-employees-ai-driven-coding-2026-3) ⭐️ 7.0/10

谷歌因其内部 AI 编码工具'Agent Smith'的员工需求量意外激增而限制了访问权限。与此同时，公司正从鼓励转向强制要求技术和非技术岗位员工使用 AI，并将 AI 采用情况纳入绩效考核。 这凸显了公司在部署强大的内部 AI 工具时面临的实际扩展挑战，即便他们正在推动全组织范围的采用。它揭示了谷歌的一项战略转变：AI 正从一个可选的生产力提升工具，转变为员工绩效中强制性的、可衡量的组成部分。 Agent Smith 建立在谷歌现有的'智能体优先'集成开发环境平台 Antigravity 之上，可以在后台异步运行，并与各种内部工具交互。员工甚至可以通过手机向其下达指令，该工具可以引用内部文档并访问员工资料以完成任务。

telegram · zaihuapd · Mar 29, 10:10

**背景**: Google Antigravity 是谷歌开发的一款 AI 驱动的集成开发环境，被设计为软件开发中 AI 智能体的平台。它具有用于任务编排的'智能体管理器'，并允许自主智能体规划、编写和验证代码。异步 AI 智能体是一种可以在后台执行多个步骤（如推理和工具调用）而不会阻塞用户交互的系统，从而实现可扩展、非阻塞的任务执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_Antigravity">Google Antigravity - Wikipedia</a></li>
<li><a href="https://blog.openreplay.com/google-antigravity-ide-guide/">A Beginner's Guide to Google's Antigravity IDE</a></li>
<li><a href="https://dev.to/programmingcentral/stop-waiting-how-to-build-instant-ai-agents-with-optimistic-ui-3agp">Stop Waiting: How to Build "Instant" AI Agents with... - DEV Community</a></li>

</ul>
</details>

**标签**: `#AI-tools`, `#enterprise-ai`, `#google`, `#coding-assistants`, `#organizational-change`

---

<a id="item-9"></a>
## [北京推出全国首个覆盖 L2 至 L4 级别的智能网联汽车专属商业保险](https://ysxw.cctv.cn/article.html?toc_style_id=feeds_default&amp;t=1774774414992&amp;item_id=12554965963627942738&amp;channelId=1119) ⭐️ 7.0/10

3 月 29 日，北京在全国率先推出智能网联新能源汽车商业保险专属产品，覆盖从 L2（部分驾驶自动化）到 L4（高度驾驶自动化）的全级别车型。该产品在原有新能源车险框架内进行针对性优化，重点保障智能驾驶系统特有的风险。 此举意义重大，因为它解决了传统车险在界定'人机共驾'责任以及覆盖软硬件相关损失方面的关键空白。通过建立一个先例，这一保险框架对于推动更高级别自动驾驶汽车在中国的广泛部署和消费者接受至关重要。 该产品将先从新车入手，分批适配不同车企和车型。对于已在北京取得合法资质的 L3、L4 级别自动驾驶车辆，也将纳入保障范围。初步预计，整体保费水平不会明显高于现有车险。

telegram · zaihuapd · Mar 29, 11:57

**背景**: SAE J3016 标准定义了六个驾驶自动化等级（L0-L5）。L2 级（部分驾驶自动化）系统，如自适应巡航和车道居中，需要人类驾驶员持续监督。L3 级（有条件驾驶自动化）允许驾驶员在特定条件下脱手，但系统请求时必须接管。L4 级（高度驾驶自动化）能在特定运行设计域内完成所有驾驶任务，无需人类干预。传统的保险模式在判定涉及这些系统的事故责任时面临挑战，尤其是在人机控制权交接的过程中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sae.org/news/blog/sae-levels-driving-automation-clarity-refinements">SAE International | Advancing mobility knowledge and solutions</a></li>
<li><a href="https://www.linkedin.com/pulse/legal-challenges-civil-liability-autonomous-vehicles-andre-santana-hqymf">The Legal Challenges of Civil Liability in Autonomous Vehicles</a></li>

</ul>
</details>

**标签**: `#autonomous-vehicles`, `#insurance`, `#regulation`, `#smart-driving`, `#china-tech`

---

<a id="item-10"></a>
## [沃顿商学院研究发现'认知投降'现象：人们更易接受 AI 输出而不加核验](https://t.me/zaihuapd/40591) ⭐️ 7.0/10

宾夕法尼亚大学沃顿商学院的研究人员上月在一篇发布于 SSRN 的预印本中提出，人们在使用生成式 AI 时表现出'认知投降'倾向。研究团队通过三项实验对近 1300 名参与者进行观察，发现他们在超过一半的情况下会选择使用 ChatGPT 解答逻辑推理题，而在求助 AI 的参与者中，约 80%的人会不加审视地接受错误答案。 这项研究为生成式 AI 如何通过鼓励人们不加批判地接受输出结果来重塑人类决策提供了实证证据，对 AI 伦理、教育和职场实践具有重要影响。研究结果突显了一个潜在风险：过度依赖 AI 工具可能导致批判性思维能力下降，并增加受错误信息影响的可能性。 该研究专门观察了人们在逻辑推理任务中使用 ChatGPT 时的行为，发现'认知投降'不仅涉及使用外部辅助工具，更意味着完全放弃认知控制。研究通过实验室和线上实验相结合的方式进行，预印本发布于 SSRN——一个面向社会科学领域早期研究的开放获取知识库。

telegram · zaihuapd · Mar 29, 16:03

**背景**: 生成式 AI 是指能够根据从训练数据中学到的模式，创建文本、图像或代码等新内容的人工智能系统。'认知投降'是一种心理现象，指用户在使用外部工具时，不加批判地放弃自己的推理过程，这超越了单纯的工具辅助，意味着完全放弃认知控制。SSRN（社会科学研究网络）是一个开放获取的在线知识库，研究人员在此分享经过正式同行评审和发表前的预印本和早期研究论文。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Social_Science_Research_Network">Social Science Research Network - Wikipedia</a></li>
<li><a href="https://datachutney.io/cognitive-surrender-explainer/">The Cognitive Lab — Thinking: Fast, Slow, and Artificial</a></li>
<li><a href="https://www.thealgorithmicbridge.com/p/a-new-wharton-study-on-ai-warns-of">A New Wharton Study on AI Warns of a Growing Problem: Cognitive ...</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Human-Computer Interaction`, `#Behavioral Science`, `#Cognitive Psychology`, `#AI Safety`

---