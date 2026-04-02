---
layout: default
title: "Horizon Summary: 2026-04-02 (ZH)"
date: 2026-04-02
lang: zh
---

> From 25 items, 7 important content pieces were selected

---

1. [NASA Artemis II 载人任务成功发射前往月球。](#item-1) ⭐️ 9.0/10
2. [Axios npm 维护者账号遭劫持，恶意版本注入跨平台远程控制木马](#item-2) ⭐️ 9.0/10
3. [脑机接口植入者已能用意念创作音乐并发行专辑曲目](#item-3) ⭐️ 8.0/10
4. [GitHub 出现 Claude Code 非官方还原仓库，从公开 npm 包 source map 文件还原源码](#item-4) ⭐️ 8.0/10
5. [NASA“阿尔忒弥斯 2 号”载人绕月任务进入发射倒计时](#item-5) ⭐️ 8.0/10
6. [DRAM 价格上涨威胁业余爱好者单板计算机市场](#item-6) ⭐️ 7.0/10
7. [Cloudflare 发布 EmDash：一款基于 TypeScript、具备沙盒插件安全性的 CMS](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [NASA Artemis II 载人任务成功发射前往月球。](https://www.nasa.gov/blogs/missions/2026/04/01/live-artemis-ii-launch-day-updates/) ⭐️ 9.0/10

NASA 的 Artemis II 任务于 2026 年 4 月 1 日成功发射，搭载宇航员乘组，这是人类 50 多年来的首次载人月球任务。该任务将执行一次月球飞越，然后于 4 月 10 日返回地球并溅落。 此次发射是 NASA Artemis 计划的一个关键里程碑，为在月球上建立持续的人类存在铺平了道路，并成为未来火星探索的垫脚石。它证明了太空发射系统（SLS）火箭和 Orion 飞船等关键系统对于深空载人任务的操作准备就绪。 该任务将在深空测试 Orion 飞船的生命支持、导航和乘员系统，包括氧气调节和二氧化碳清除等关键功能。在此次任务之后，重点将转向开发推进剂在轨加注（通过 SpaceX 的 Starship）和月球着陆器（如 Blue Origin 的 Blue Moon）等能力，以实现后续的 Artemis III 月球着陆任务。

hackernews · apitman · Apr 1, 17:11

**背景**: Artemis 计划是 NASA 旨在让人类重返月球并在那里建立可持续存在的倡议。其核心架构依赖于太空发射系统（SLS）这一超重型运载火箭来发射载人的 Orion 飞船。Orion 飞船专为深空任务设计，配备了先进的生命支持系统，以保障宇航员在超出地球轨道的长时间飞行中的安全。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Artemis_program">Artemis program - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Space_Launch_System">Space Launch System - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Orion_(spacecraft)">Orion (spacecraft) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区对此次任务的技术成就表示惊叹，例如一位用户提到的惊人发射速度。一个关键的讨论点集中在任务的更广泛价值上，一些人捍卫太空探索是推动进步和激励人类的崇高事业，而另一些人则提到了对隔热罩等技术风险的担忧。此外，还有关于 Artemis 计划下一步的前瞻性讨论，包括 Starship 和月球着陆器的开发。

**标签**: `#space-exploration`, `#nasa`, `#artemis-program`, `#space-technology`, `#human-spaceflight`

---

<a id="item-2"></a>
## [Axios npm 维护者账号遭劫持，恶意版本注入跨平台远程控制木马](https://t.me/zaihuapd/40637) ⭐️ 9.0/10

2026 年 3 月 30 日至 31 日，安全机构 StepSecurity 发现主流 JavaScript 库 axios 的一位主要维护者的 npm 账号遭劫持。攻击者手动发布了两个恶意版本 axios@1.14.1 和 axios@0.30.4，通过注入一个名为 plain-crypto-js 的恶意依赖包来部署跨平台远程访问木马（RAT）。 这是一次针对 axios 的重大软件供应链攻击，axios 是一个基础 HTTP 客户端库，每周下载量约 1 亿次。此次攻击手段复杂，绕过了 CI/CD、针对多种操作系统并使用预先部署的依赖，凸显了对整个 JavaScript/Node.js 生态系统以及依赖它的无数应用程序安全的严重威胁。 攻击者利用一个被盗的、长期有效的 npm 访问令牌，通过 npm CLI 直接发布包，从而绕过了项目的 GitHub Actions CI/CD 流程。恶意依赖 `plain-crypto-js` 在攻击发生前 18 小时就已预先部署，其唯一目的是执行一个 `postinstall` 脚本来投放针对特定操作系统的 RAT 载荷，且所有痕迹都被设计为自毁。

telegram · zaihuapd · Apr 1, 05:25

**背景**: Axios 是一个流行的、基于 Promise 的 JavaScript HTTP 客户端，广泛用于 Node.js 和浏览器环境。npm（Node 包管理器）是 JavaScript 生态系统的默认包注册中心，像 axios 这样的库在此发布并被开发者安装。供应链攻击是指攻击者通过入侵受信任的组件（如库）向其用户分发恶意软件。远程访问木马（RAT）是一种恶意软件，能让攻击者远程控制受感染的系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan">axios Compromised on npm - Malicious Versions Drop Remote Access Trojan - StepSecurity</a></li>
<li><a href="https://snyk.io/blog/axios-npm-package-compromised-supply-chain-attack-delivers-cross-platform/">Axios npm Package Compromised: Supply Chain Attack Delivers Cross-Platform RAT | Snyk</a></li>
<li><a href="https://www.elastic.co/security-labs/axios-one-rat-to-rule-them-all">Inside the Axios supply chain compromise - one RAT to rule them all — Elastic Security Labs</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain`, `#npm`, `#javascript`, `#malware`

---

<a id="item-3"></a>
## [脑机接口植入者已能用意念创作音乐并发行专辑曲目](https://www.wired.com/story/meet-the-man-making-music-with-his-brain-implant/) ⭐️ 8.0/10

69 岁的四肢瘫痪者 Galen Buckwalter 在 2024 年植入了六枚 Blackrock Neurotech 脑机接口芯片后，已能通过神经信号创作音乐。他在实验中生成的音调被用于其乐队 Siggy 于 3 月 15 日发行的专辑中的歌曲《Wirehead》。 这标志着脑机接口（BCI）的应用从恢复基本运动或沟通功能，显著扩展到了创造性表达和个人实现的领域。它强调了神经技术设计应转向关注使用者的个人兴趣和生活质量，这对于技术的长期接受度至关重要。 该系统使用研究团队开发的算法将神经信号转化为音调，使 Buckwalter 能够同时控制两路声音。除了音乐创作，该植入体还使他能操作电脑，并恢复了他部分的手指感觉。

telegram · zaihuapd · Apr 1, 07:34

**背景**: 脑机接口（BCI）是在大脑与外部设备之间建立直接通信通路的系统，通常用于为瘫痪或神经系统疾病患者恢复功能。像 Blackrock Neurotech 这样的公司开发可植入的微电极阵列来记录神经活动，这些数据随后由算法解码以控制计算机或假肢。脑机音乐接口（BCMI）研究探索如何从脑信号中提取控制信息，并设计能响应这些信息的生成式音乐技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blackrockneurotech.com/">Blackrock Neurotech | Empowered by Thought</a></li>
<li><a href="https://www.researchgate.net/publication/321619139_Guide_to_Brain-Computer_Music_Interfacing">Guide to Brain - Computer Music Interfacing | Request PDF</a></li>

</ul>
</details>

**标签**: `#brain-computer-interface`, `#neurotechnology`, `#human-computer-interaction`, `#assistive-technology`, `#neuroscience`

---

<a id="item-4"></a>
## [GitHub 出现 Claude Code 非官方还原仓库，从公开 npm 包 source map 文件还原源码](https://t.me/zaihuapd/40641) ⭐️ 8.0/10

一个名为 'claude-code-sourcemap' 的 GitHub 仓库通过解析公开 npm 包 `@anthropic-ai/claude-code` 中附带的 source map 文件 `cli.js.map` 内的 `sourcesContent` 字段，成功还原了 Anthropic 公司 Claude Code 2.1.88 版本的 TypeScript 源代码。该过程共还原出 4756 个文件，其中包括 1884 个 .ts 与 .tsx 文件。 这一事件凸显了一个关键的软件供应链漏洞，一家主要 AI 公司的专有代码通过一个常见的开发构件被无意中暴露。它强调了知识产权保护的重大风险，并对 AI 工具的安全实践提出了质疑，可能影响对商业 AI 产品及其部署流程的信任。 此次泄露的发生是因为生产环境的 npm 包中包含了一个含有 `sourcesContent` 字段的 source map 文件，该字段内嵌了原始源代码。该仓库创建于 2026 年 3 月 31 日，由安全研究员 Chaofan Shou 发现后，泄露的代码在 GitHub 上被数万名用户迅速分叉。

telegram · zaihuapd · Apr 1, 08:07

**背景**: Source map（源码映射）文件是在 Web 应用程序（例如使用 TypeScript 或压缩后的 JavaScript）构建过程中生成的，用于将转换、压缩后的代码映射回原始源代码，以便于调试。`sourcesContent` 字段是 source map 的一个可选部分，可以包含原始源文件的完整文本，这使得 source map 自包含，但如果被包含在生产环境的软件包中，也会带来安全风险。NPM（Node Package Manager）是 JavaScript 软件包的主要注册中心，发布包含 source map 的软件包是一种常见但常被忽视的做法，可能导致源代码泄露。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://insiderllm.com/guides/claude-code-source-leak-what-we-learned/">Claude Code's Source Just Leaked: What 500K Lines of... | InsiderLLM</a></li>
<li><a href="https://web.dev/articles/source-maps">What are source maps? | Articles | web.dev</a></li>
<li><a href="https://dev.to/alanwest/your-npm-package-is-leaking-source-code-and-you-probably-dont-know-it-4kf5">Your npm Package Is Leaking Source Code... - DEV Community</a></li>

</ul>
</details>

**标签**: `#reverse-engineering`, `#source-maps`, `#anthropic`, `#intellectual-property`, `#npm-security`

---

<a id="item-5"></a>
## [NASA“阿尔忒弥斯 2 号”载人绕月任务进入发射倒计时](https://www.nasa.gov/) ⭐️ 8.0/10

NASA 的“阿尔忒弥斯 2 号”任务，即自 1972 年以来的首次载人月球飞行，已在肯尼迪航天中心发射台就位，最早将于美国东部时间 4 月 1 日 18 时 24 分发射升空。该任务将使用太空发射系统（SLS）火箭，搭载四名宇航员乘坐“猎户座”飞船进行为期 10 天的绕月飞行。 此次任务标志着人类时隔半个多世纪后重返月球空间，是 NASA“阿尔忒弥斯”计划建立可持续月球存在、并为未来火星任务进行技术验证的关键一步。其成功对于恢复美国在深空探索领域的领导地位，以及推动月球科学与探索的国际合作至关重要。 此次发射历经多次技术延误，包括在燃料加注测试中出现的液氢泄漏，以及火箭上面级氦气流中断问题，这些问题导致火箭在 2 月和 3 月被迫撤回装配大楼进行检修。该任务是一次载人绕月飞行，不涉及月球着陆，主要目的是测试“猎户座”飞船在载人深空环境下的系统性能。

telegram · zaihuapd · Apr 1, 22:01

**背景**: NASA 的“阿尔忒弥斯”计划是一系列旨在让人类重返月球并最终将宇航员送往火星的任务。太空发射系统（SLS）是 NASA 为这些深空任务设计的新型超重型运载火箭，而“猎户座”飞船是载人航天器。上一次人类进入月球轨道的任务是 1972 年 12 月的阿波罗 17 号。无人测试任务“阿尔忒弥斯 1 号”已于 2022 年底成功完成绕月飞行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/太空發射系統">太空发射系统 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.voachinese.com/a/artemis-ii-march-launch-window-out-of-consideration-after-helium-pressure-system-fault-20260225/8117595.html">由于 氦 气 压力系统 故 障 ，“阿尔忒弥斯二号”3月发射计划推迟 | 美国之音</a></li>

</ul>
</details>

**标签**: `#space-exploration`, `#nasa`, `#artemis-program`, `#aerospace-engineering`, `#science-news`

---

<a id="item-6"></a>
## [DRAM 价格上涨威胁业余爱好者单板计算机市场](https://www.jeffgeerling.com/blog/2026/dram-pricing-is-killing-the-hobbyist-sbc-market/) ⭐️ 7.0/10

Jeff Geerling 的博客文章指出，DRAM（动态随机存取存储器）价格的大幅上涨正导致树莓派等面向业余爱好者的单板计算机（SBC）变得不再那么经济实惠且供应紧张。TrendForce 的市场分析预测，2026 年第二季度 DRAM 合约价格可能环比上涨 58% 至 63%。 这很重要，因为单板计算机对于教育、原型设计和 DIY 项目至关重要，其成本上升可能会抑制这些领域的创新和学习。此外，DRAM 价格上涨是一个更广泛的供应链问题，预计也将显著影响智能手机市场和其他消费电子领域。 价格压力不仅限于单板计算机；评论指出，由于内存和供应链问题，其他设备的供应商报价也上涨了 50%。一些社区成员还指出，高昂的 DRAM 成本可能会将更简单的计算任务推回到更具成本效益的微控制器上，这代表了一种潜在的设计理念转变。

hackernews · ingve · Apr 1, 21:36

**背景**: DRAM 是一种易失性存储器，用作大多数计算机和电子设备（包括单板计算机）的主工作内存。单板计算机，如树莓派，是在单个电路板上构建的完整计算机，在业余爱好者项目、教育和嵌入式应用中很受欢迎。DRAM 市场高度集中在少数几家主要制造商手中，对供需动态、制造技术进步以及人工智能和数据中心等领域的需求非常敏感。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/dram/dram-and-nand-contract-prices-to-climb-again-in-q2">DRAM prices predicted to jump 63% in Q2, NAND up to 75% ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Raspberry_Pi">Raspberry Pi - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dynamic_random-access_memory">Dynamic random - access memory - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，一些用户指出当前价格仍远低于历史高点，而另一些用户则强调其影响已超出单板计算机范围。主要观点包括：由于内存成本导致智能手机市场萎缩的预测，对氦气供应问题加剧现状的担忧，以及观察到成本压力正迫使人们重新评估哪些任务真正需要单板计算机级别的算力，哪些可以回归微控制器。

**标签**: `#hardware`, `#supply-chain`, `#single-board-computers`, `#dram`, `#market-trends`

---

<a id="item-7"></a>
## [Cloudflare 发布 EmDash：一款基于 TypeScript、具备沙盒插件安全性的 CMS](https://blog.cloudflare.com/emdash-wordpress/) ⭐️ 7.0/10

Cloudflare 宣布推出 EmDash，这是一个完全使用 TypeScript 编写、基于无服务器架构构建的新内容管理系统（CMS）。其核心创新在于采用了基于 Cloudflare Dynamic Workers 的沙盒化插件系统，通过隔离插件来解决 WordPress 插件架构中固有的根本性安全漏洞。 这很重要，因为 WordPress 支撑着超过 40% 的网站，而其插件生态系统由于插件拥有无限制的系统访问权限，是安全漏洞的主要来源。EmDash 的架构方法可能为 CMS 安全性树立新标准，有望减少大规模的网站被攻击事件，并吸引寻求现代、安全、可扩展替代方案的开发者。 EmDash 构建于 Astro（一个用于内容驱动型网站的快速 Web 框架）之上，其插件是标准的 TypeScript 模块。虽然它解决了安全性和现代开发工作流程的问题，但其成功将取决于能否克服 WordPress 庞大的网络效应和已建立的生态系统。

hackernews · elithrar · Apr 1, 16:14

**背景**: WordPress 是一个占主导地位的、基于 PHP 的 CMS，以其庞大的插件生态系统而闻名，但这种架构赋予插件对服务器的完全访问权限，带来了重大的安全风险。沙盒化插件架构将插件代码隔离，限制其对主机系统资源和数据的访问，以防止恶意或有缺陷的代码造成损害。TypeScript 是 JavaScript 的超集，它增加了静态类型，有助于在开发过程中捕获错误，并使大型代码库更易于维护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.codecentric.de/en/knowledge-hub/blog/plug-in-architectures-webassembly">Plug - in architectures with server-side WebAssembly</a></li>
<li><a href="https://en.wikipedia.org/wiki/TypeScript">TypeScript - Wikipedia</a></li>
<li><a href="https://www.unicon.net/insights/articles/contrasting-system-architectures-an-overview-of-serverless-and-traditional-approaches">System Architecture : Traditional and Serverless CMS Approaches</a></li>

</ul>
</details>

**社区讨论**: 社区讨论既包含对技术方案的认可，也包含对采用率的怀疑。开发者赞扬其对 TypeScript 和沙盒化 Workers 的关注，认为这是解决 WordPress 安全性和插件管理痛点的正确方案。然而，也有人认为 WordPress 的主导地位源于其易用性和巨大的网络效应，暗示仅凭技术优势可能不足以推动从现有平台的大规模迁移。

**标签**: `#cms`, `#security`, `#cloudflare`, `#typescript`, `#serverless`

---