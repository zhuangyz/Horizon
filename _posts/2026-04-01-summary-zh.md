---
layout: default
title: "Horizon Summary: 2026-04-01 (ZH)"
date: 2026-04-01
lang: zh
---

> From 28 items, 7 important content pieces were selected

---

1. [Axios npm 包遭供应链攻击，通过恶意依赖项植入](#item-1) ⭐️ 9.0/10
2. [axios npm 包因维护者账号遭劫持被植入跨平台远程访问木马](#item-2) ⭐️ 9.0/10
3. [特朗普称正强烈考虑让美国退出北约，抨击其为“纸老虎”](#item-3) ⭐️ 9.0/10
4. [可视化指南分析泄露的 Claude Code 源代码，揭示 AI 智能体架构](#item-4) ⭐️ 8.0/10
5. [GitHub 出现 Claude Code 非官方还原仓库，从公开 npm 包还原 4756 个文件](#item-5) ⭐️ 8.0/10
6. [脑机接口植入者已能用意念创作音乐](#item-6) ⭐️ 8.0/10
7. [百度萝卜快跑夜间故障，多车高架趴窝致乘客被困数小时](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Axios npm 包遭供应链攻击，通过恶意依赖项植入](https://simonwillison.net/2026/Mar/31/supply-chain-attack-on-axios/#atom-everything) ⭐️ 9.0/10

2026 年 3 月 31 日，一个供应链攻击入侵了广泛使用的 Axios HTTP 客户端 npm 包，该包每周下载量超过 1.01 亿次。恶意版本 1.14.1 和 0.30.4 包含了一个名为 `plain-crypto-js` 的新发布依赖项，该依赖项旨在窃取凭证并安装远程访问木马（RAT）。 这次攻击展示了供应链攻击对基础开源软件包构成的严重风险，可能影响下游数百万个应用程序和开发者。它凸显了改进发布安全措施（如可信发布）的迫切需求，以防止因凭证泄露导致的未授权发布。 攻击媒介是一个泄露的、长期有效的 npm 令牌，而非直接修改 Axios 源代码。恶意包 `plain-crypto-js` 以版本 4.2.1 发布，在此前 18 小时发布了一个看似干净的版本 4.2.0，以在注册表中建立短暂的历史记录。

rss · Simon Willison · Mar 31, 23:28

**背景**: 软件供应链攻击是指攻击者入侵被其他软件使用的第三方组件（如库或依赖项），从而将恶意代码注入依赖该组件的更大生态系统中。npm 是 JavaScript 运行时 Node.js 的默认包管理器，托管着数百万个可重用代码包。可信发布是一项安全功能，它允许包发布者配置 npm，使其仅接受来自特定授权工作流（如 GitHub Actions）的发布，从而降低传统身份验证令牌泄露带来的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack - Wikipedia</a></li>
<li><a href="https://docs.npmjs.com/trusted-publishers/">Trusted publishing for npm packages | npm Docs</a></li>
<li><a href="https://snyk.io/blog/axios-npm-package-compromised-supply-chain-attack-delivers-cross-platform/">Axios npm Package Compromised: Supply Chain Attack Delivers Cross-Platform RAT | Snyk</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain`, `#npm`, `#axios`, `#malware`

---

<a id="item-2"></a>
## [axios npm 包因维护者账号遭劫持被植入跨平台远程访问木马](https://t.me/zaihuapd/40637) ⭐️ 9.0/10

2026 年 3 月 31 日，安全机构 StepSecurity 发现主流 JavaScript 库 axios 的 npm 维护者账号遭劫持。攻击者绕过了项目正常的 GitHub Actions CI/CD 流程，手动发布了两个恶意版本（axios@1.14.1 和 axios@0.30.4），通过注入一个依赖项来部署针对 Windows、macOS 和 Linux 系统的远程访问木马（RAT）。 这是一次影响重大的供应链攻击，波及每周下载量约 6000 万次的 axios 库，对无数网络应用和开发流水线构成巨大潜在威胁。该事件表明，复杂的攻击者可以通过劫持长期有效的凭证并手动发布恶意包来绕过自动化安全检查，这削弱了人们对 npm 生态系统的信任。 攻击手段是添加了一个从未被导入的依赖项 `plain-crypto-js@^4.2.1`，该恶意包由另一个攻击者账号在大约 18 小时前预先部署。该依赖包含一个 `postinstall` 钩子脚本，用于执行针对特定操作系统的恶意载荷，且所有痕迹在执行后都设计为自毁。

telegram · zaihuapd · Apr 1, 05:25

**背景**: Axios 是一个广泛使用的、基于 Promise 的 JavaScript HTTP 客户端，常用于浏览器和 Node.js 环境。npm（Node 包管理器）是 JavaScript 包的主要注册中心，供应链攻击通常通过入侵合法软件包来分发恶意软件。像 GitHub Actions 这样的 CI/CD（持续集成/持续部署）流水线是用于自动构建、测试和部署代码的工作流，但如果攻击者获得了直接发布权限，就可以绕过这些安全检查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/axios-npm-compromised-maintainer-hijacked-rat">axios compromised on npm: maintainer account hijacked, RAT deployed</a></li>
<li><a href="https://anonhaven.com/en/news/axios-npm-supply-chain-attack-rat/">Axios npm package compromised after maintainer account hijack delivers cross-platform RAT</a></li>
<li><a href="https://snyk.io/blog/axios-npm-package-compromised-supply-chain-attack-delivers-cross-platform/">Axios npm Package Compromised: Supply Chain Attack Delivers Cross-Platform RAT | Snyk</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain`, `#npm`, `#javascript`, `#malware`

---

<a id="item-3"></a>
## [特朗普称正强烈考虑让美国退出北约，抨击其为“纸老虎”](https://www.telegraph.co.uk/world-news/2026/04/01/donald-trump-strongly-considering-pulling-us-out-of-nato/) ⭐️ 9.0/10

美国总统特朗普在接受《每日电讯报》专访时表示，他正“强烈考虑”让美国退出北约，并将该联盟形容为“纸老虎”。这一考虑源于北约盟国拒绝参与针对伊朗的军事行动，并拒绝了美国要求派遣军舰重新开放霍尔木兹海峡的请求。 美国若退出北约，将是自该联盟 1949 年成立以来对跨大西洋安全架构最重大的冲击，将从根本上削弱欧洲的集体防御和全球力量格局。这标志着美国数十年外交政策的戏剧性转变，可能助长对手的气焰，并在剩余成员国中引发严重的信任危机。 直接的导火索是北约拒绝支持美国主导的在霍尔木兹海峡的军事行动，该海峡已被伊朗实际关闭数周，影响了全球约 20%的石油运输。特朗普声称俄罗斯总统普京也深知该组织的虚弱，并将这一考虑定性为对欧洲盟友“不再是可靠的防御伙伴”的回应。

telegram · zaihuapd · Apr 1, 14:15

**背景**: 北大西洋公约组织（北约）是一个成立于 1949 年的军事联盟，其核心原则是《北大西洋公约》第五条规定的集体防御，即对任一成员国的攻击被视为对所有成员国的攻击。自成立以来，美国一直是该联盟最强大的成员国和主要的安全保障者。霍尔木兹海峡是波斯湾和阿曼湾之间的关键海上咽喉要道，全球很大一部分的海运石油出口需经过此地。

**标签**: `#geopolitics`, `#international-relations`, `#defense-policy`, `#nato`, `#us-foreign-policy`

---

<a id="item-4"></a>
## [可视化指南分析泄露的 Claude Code 源代码，揭示 AI 智能体架构](https://ccunpacked.dev/) ⭐️ 8.0/10

一位开发者创建了一个可视化指南（ccunpacked.dev），用于分析 Anthropic 旗下 AI 编程智能体 Claude Code 泄露的 50 万行源代码。该指南梳理了其复杂的架构，并揭示了用于管理大语言模型行为的特定防御性编程模式，例如“沮丧正则表达式”。 这项分析罕见地详细揭示了在智能体系统中让概率性大语言模型可靠运行所面临的工程挑战。它凸显了在生产级 AI 智能体中，用于状态管理、错误处理和安全性所需的巨大代码开销，为更广泛的 AI 智能体开发社区提供了宝贵的经验。 该代码库包含诸如“沮丧正则表达式”（旨在从用户提示中检测沮丧情绪的正则表达式）等模式，以及用于工具调用的广泛数据清理和重试逻辑。这份可视化指南由一位独立开发者快速创建，旨在帮助理解庞大复杂的代码库，用于个人学习和项目借鉴。

hackernews · autocracy101 · Apr 1, 05:15

**背景**: Claude Code 是 Anthropic 开发的一款 AI 驱动的编程助手，能够根据自然语言指令自主调用工具（如 shell 命令或代码编辑器）来执行任务。LLM 智能体是一种系统，其中大语言模型充当“大脑”，决定何时以及如何使用外部工具来完成多步骤任务。一个关键挑战是确保本质上具有概率性的大语言模型表现出确定且可靠的行为，这通常需要大量的“防御性编程”来处理边界情况和错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://alex000kim.com/posts/2026-03-31-claude-code-source-leak/">The Claude Code Source Leak: fake tools, frustration regexes, undercover mode, and more | Alex Kim's blog</a></li>
<li><a href="https://www.datacamp.com/blog/llm-agents">LLM Agents Explained: Architecture, Frameworks, and Use Cases | DataCamp</a></li>

</ul>
</details>

**社区讨论**: 社区讨论呈现出不同的反应。一些评论者对一个 CLI 智能体拥有 50 万行代码库的规模感到惊讶，认为这证明了让大语言模型具有确定性所涉及的“状态管理噩梦”。另一些人则认为真正的价值在于 Anthropic 的专有模型，而非智能体框架，他们认为后者只是一个可解决的工程问题。该指南的作者表示，他们创建此指南是为了将其中的思路借鉴到自己的项目中。

**标签**: `#ai-agents`, `#reverse-engineering`, `#llm-engineering`, `#software-architecture`, `#anthropic`

---

<a id="item-5"></a>
## [GitHub 出现 Claude Code 非官方还原仓库，从公开 npm 包还原 4756 个文件](https://t.me/zaihuapd/40632) ⭐️ 8.0/10

一个名为 'claude-code-sourcemap' 的非官方 GitHub 仓库，通过提取公开 npm 包 @anthropic-ai/claude-code 中包含的 `cli.js.map` 源映射文件中 `sourcesContent` 字段的数据，还原出了 Claude Code 2.1.88 版本的 TypeScript 源代码。此次还原共得到 4756 个文件，其中包括 1884 个 .ts 和 .tsx 文件。 这一事件凸显了软件发布者面临重大的安全和知识产权风险，展示了公开分发的软件包中的源映射如何可能无意间暴露专有源代码。它提供了对一款专有 AI 编程助手内部结构的罕见详细观察，并强调了所有软件（尤其是在竞争激烈的 AI 领域）采取安全构建和部署实践的重要性。 此次还原特别利用了源映射中可选的 `sourcesContent` 字段，该字段可以直接嵌入原始源代码，从而无需单独的源文件。暴露的代码涉及 Claude Code 的 2.1.88 版本，该仓库的存在展示了专为处理源映射而设计的逆向工程工具的实际应用。

telegram · zaihuapd · Apr 1, 02:36

**背景**: 源映射是用于在压缩/转译后的代码（如 JavaScript）和原始源代码（如 TypeScript）之间建立映射关系的文件，有助于调试。源映射中可选的 `sourcesContent` 字段可以包含原始源代码的完整文本，将其直接嵌入到映射文件中。当此类源映射被包含在公开分发的 npm 包中时，如果未经过妥善处理，它们可能会暴露完整的原始源代码，这是开发者安全社区中已知的一个问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/alanwest/your-npm-package-is-leaking-source-code-and-you-probably-dont-know-it-4kf5">Your npm Package Is Leaking Source Code (And You Probably Don't Know It) - DEV Community</a></li>
<li><a href="https://blog.openreplay.com/source-maps-work/">What Are Source Maps and How Do They Work - blog.openreplay.com</a></li>
<li><a href="https://stackoverflow.com/questions/19802462/do-source-maps-include-the-source-text">Do source maps include the source text? - Stack Overflow</a></li>

</ul>
</details>

**标签**: `#reverse-engineering`, `#ai-systems`, `#source-code-analysis`, `#npm-security`, `#anthropic`

---

<a id="item-6"></a>
## [脑机接口植入者已能用意念创作音乐](https://www.wired.com/story/meet-the-man-making-music-with-his-brain-implant/) ⭐️ 8.0/10

一位 69 岁的四肢瘫痪者 Galen Buckwalter 参与了加州理工学院的研究，于 2024 年接受了 6 枚 Blackrock Neurotech 芯片的开颅植入。在研究团队开发的算法帮助下，他现在能够直接用神经信号生成音调，并将实验中创作的音轨用于自己乐队 Siggy 于 3 月 15 日发行的歌曲《Wirehead》中。 这标志着脑机接口（BCI）的应用从基础的医疗功能恢复，扩展到了提升生活质量和实现创造性表达的新领域。它强调了神经技术应以人为本的发展方向，关注使用者的个人能动性和长期使用意愿，这对于该技术的广泛接受至关重要。 该系统允许 Buckwalter 用意念同时控制两路声音。除了创作音乐，该植入体还使他能够操作电脑，并恢复了他部分手指的感觉，展示了该技术的多功能潜力。

telegram · zaihuapd · Apr 1, 07:34

**背景**: 脑机接口（BCI）是一种解码神经信号，实现大脑与外部设备直接通信的系统，常用于为瘫痪患者恢复功能。Blackrock Neurotech 是植入式 BCI 技术的领先公司，其设备已被全球 1000 多个研究实验室使用。将神经信号转化为音乐涉及复杂的算法，这些算法通过解读大脑活动模式来生成或控制音乐参数，这一领域有时被称为脑机音乐接口（BCMI）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blackrockneurotech.com/">Blackrock Neurotech | Empowered by Thought</a></li>
<li><a href="https://link.springer.com/article/10.1007/s12559-024-10280-6">NeuralPMG: A Neural Polyphonic Music Generation System Based on Machine Learning Algorithms | Cognitive Computation | Springer Nature Link</a></li>

</ul>
</details>

**标签**: `#Brain-Computer Interface`, `#Neurotechnology`, `#Human-Computer Interaction`, `#Assistive Technology`, `#Creative AI`

---

<a id="item-7"></a>
## [百度萝卜快跑夜间故障，多车高架趴窝致乘客被困数小时](https://www.sznews.com/news/content/2026-03/31/content_32000110.htm) ⭐️ 7.0/10

3 月 31 日晚，百度旗下自动驾驶出行服务平台“萝卜快跑”在武汉发生大面积系统故障，导致多辆自动驾驶车辆在高架桥或主干道上突然停车，将乘客困在车内。车内系统提示“驾驶系统异常”，乘客反映紧急联系方式和 App 客服长时间难以接通，有人等待近 2 小时后才在交警和工作人员协助下离开高架。 此次事件是商业化 Robotaxi 服务一次重大的现实世界故障，暴露了其在安全协议、应急响应和系统韧性方面的关键缺陷。它直接影响了公众对自动驾驶技术的信任，并对大规模部署（尤其是在高架路等复杂城市环境）所需的操作准备和故障安全机制提出了紧迫质疑。 服务方客服最初将故障归因于“网络原因”，但后续记者致电官方客服时，对方却表示不了解武汉故障情况，并要求提供车号才能查询。值得注意的是，截至发稿时，萝卜快跑官方平台未就此次故障及应对措施发布任何信息。

telegram · zaihuapd · Apr 1, 01:06

**背景**: 百度“萝卜快跑”是在中国多个城市运营的商用 Robotaxi（自动驾驶出行）服务，基于百度的 Apollo 自动驾驶平台。这些车辆依赖人工智能、传感器（激光雷达、雷达、摄像头）和 GPS 的组合进行导航，通常需要稳定的网络连接来实现某些云端功能和远程监控。“Robotaxi”特指用于共享出行的自动驾驶汽车，其设计目标是在车内没有人类驾驶员的情况下运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apollo_Go">Apollo Go - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Self-driving_car">Self-driving car - Wikipedia</a></li>

</ul>
</details>

**标签**: `#autonomous-vehicles`, `#safety`, `#reliability`, `#robotaxi`, `#incident-report`

---