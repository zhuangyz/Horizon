---
layout: default
title: "Horizon Summary: 2026-03-23 (ZH)"
date: 2026-03-23
lang: zh
---

> From 28 items, 6 important content pieces were selected

---

1. [Starlette 1.0 发布，为支撑 FastAPI 的 ASGI 框架带来稳定性](#item-1) ⭐️ 8.0/10
2. [OpenAI 建议英国将 AI 聊天机器人纳入 Google 搜索选择页](#item-2) ⭐️ 8.0/10
3. [为数据主权将数字服务从美国迁移至欧盟提供商的指南](#item-3) ⭐️ 7.0/10
4. [GitHub 可靠性据称降至“三个九”可用性，同时面临服务中断与安全担忧。](#item-4) ⭐️ 7.0/10
5. [研究对比 isolated-vm、vm2、QuickJS、ShadowRealm 和 Deno Workers 等 JavaScript 沙箱技术](#item-5) ⭐️ 7.0/10
6. [交互式可视化工具发布，用于演示 Bram Cohen 基于 CRDT 的版本控制概念](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Starlette 1.0 发布，为支撑 FastAPI 的 ASGI 框架带来稳定性](https://simonwillison.net/2026/Mar/22/starlette/#atom-everything) ⭐️ 8.0/10

基础 Python ASGI 框架 Starlette 于 2026 年 3 月发布了 1.0 版本，这是其首个主要的稳定版本。此次更新引入了破坏性变更，最显著的是用新的 `lifespan` 异步上下文管理器系统取代了原有的 `on_startup` 和 `on_shutdown` 参数。 此次发布意义重大，因为 Starlette 是广受欢迎的 FastAPI 框架的底层引擎，其稳定性直接影响着庞大的现代 Python Web 应用生态系统。1.0 里程碑为开发者和项目（如 Datasette）提供了一个稳定的 API 基础，这些项目此前曾因其版本不稳定而犹豫是否基于其构建。 该项目于 2025 年 9 月移交给了 Marcelo Trylesinski 管理，以便于获得赞助。一个关键的技术转变是采用了 `lifespan` 模式，它利用 Python 的 `contextlib.asynccontextmanager` 来管理启动和关闭逻辑，相比旧的回调参数方式更为清晰。

rss · Simon Willison · Mar 22, 23:57

**背景**: Starlette 是一个为 ASGI（异步服务器网关接口）规范构建的轻量级异步 Web 框架，ASGI 是 Python 中 WSGI 的现代继任者。它提供了 FastAPI 所构建的核心请求/响应处理和路由功能，而 FastAPI 在此基础上增加了自动数据验证和 OpenAPI 文档生成。ASGI 使 Python 框架能够异步处理 HTTP、WebSocket 和其他协议，从而提高了 I/O 密集型操作的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asynchronous_Server_Gateway_Interface">Asynchronous Server Gateway Interface - Wikipedia</a></li>
<li><a href="https://dev.to/ceb10n/understanding-fastapi-how-starlette-works-43i1">Understanding FastAPI: How Starlette works - DEV Community</a></li>
<li><a href="https://leapcell.medium.com/fastapi-is-overkill-starlette-and-pydantic-are-all-you-really-need-2b2d55c53de0">FastAPI is Overkill: Starlette and Pydantic Are All You Really Need | by Leapcell | Medium</a></li>

</ul>
</details>

**标签**: `#python`, `#web-frameworks`, `#asgi`, `#backend-development`, `#fastapi`

---

<a id="item-2"></a>
## [OpenAI 建议英国将 AI 聊天机器人纳入 Google 搜索选择页](https://assets.publishing.service.gov.uk/media/69b970dcc06ba9576435ab5a/OpenAI.pdf) ⭐️ 8.0/10

3 月 6 日，OpenAI 在提交给英国竞争与市场管理局（CMA）的公开咨询意见中正式建议，Google 搜索选择页的资格标准应明确纳入具备搜索功能的 AI 聊天机器人。这将使得像 ChatGPT 这样的服务能够在 Android 设备和 Chrome 浏览器上被用户选为默认搜索服务。 此举意义重大，因为它代表了一家领先的 AI 公司为争取自身利益而塑造竞争政策的战略努力，可能挑战 Google 在搜索领域的主导地位。如果建议被采纳，将加速对话式 AI 融入主流搜索生态系统，并为用户提供传统搜索引擎之外的更多选择。 OpenAI 认为，像 ChatGPT 这样通过对话式或多模态方式完成广泛信息发现的服务，在功能上与 Google 自家的 AI Overviews 和 AI Mode 功能相近。它还建议采用透明、动态的流行度标准来决定入选服务，并将选择页的覆盖范围扩展到语音、视觉和 AI 辅助搜索等入口。

telegram · zaihuapd · Mar 23, 14:50

**背景**: 英国竞争与市场管理局（CMA）是一个负责促进竞争、防止反竞争行为的监管机构。Google 的搜索选择页是一种机制，在欧盟和英国等地区由监管机构强制要求，出现在 Android 设备和 Chrome 浏览器上，让用户可以从一个选项列表中选择默认搜索引擎，旨在减少 Google 的默认优势。AI Overviews 和 AI Mode 是 Google 自家的 AI 驱动搜索功能，前者提供摘要式答案，后者提供对话式交互，均超越了传统的链接列表形式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_Overviews">AI Overviews - Wikipedia</a></li>
<li><a href="https://frankknow.com/google-ai-mode/">AI Mode 是什麼？Google 搜尋進化！教你提升被 AI 引用的機會</a></li>

</ul>
</details>

**标签**: `#AI Regulation`, `#Search Competition`, `#OpenAI`, `#UK CMA`, `#ChatGPT`

---

<a id="item-3"></a>
## [为数据主权将数字服务从美国迁移至欧盟提供商的指南](https://rz01.org/eu-migration/) ⭐️ 7.0/10

一份全面的指南和讨论已经发布，详细阐述了将数字服务和基础设施从美国公司迁移到欧盟替代方案的实际策略。讨论内容包括具体的技术实施细节、不同司法管辖区的法律考量以及对服务提供商的比较分析。 这很重要，因为它回应了人们对隐私、数据主权以及减少对美国科技巨头依赖的日益增长的担忧，尤其是在欧盟 GDPR 等法规的背景下。成功的迁移可以帮助个人和组织更好地控制其数据、遵守区域法律，并可能降低与外国监控或数据访问法律相关的风险。 讨论承认迁移过程是复杂的，通常只能完成约 90%，并会残留一些小的依赖项，而且一些基于欧盟的服务可能仍与美国公司有间接联系。讨论还强调了实际挑战，例如在某些提供商处配置从自定义域名发送电子邮件。

hackernews · exitnode · Mar 23, 10:17

**背景**: 数据主权指的是数据受其所在国家的法律和治理结构管辖的概念。欧盟已为数据保护建立了强大的法律框架，尤其是《通用数据保护条例》(GDPR)，旨在让个人控制其个人数据。云迁移策略是在不同环境（例如从本地或一个云提供商迁移到另一个）之间移动数字资产和基础设施的系统方法。基于欧盟的云替代方案，如 OVHcloud 和 STACKIT，常因其符合欧盟数据保护法规而被推广。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://incountry.com/blog/the-eus-data-sovereignty-framework/">The EU’s data sovereignty framework - InCountry</a></li>
<li><a href="https://www.digitalocean.com/resources/articles/cloud-migration-strategy">Complete Cloud Migration Strategy Guide: Planning and ...</a></li>
<li><a href="https://www.softwareseni.com/comparing-european-cloud-providers-and-open-source-alternatives-to-us-platforms/">Comparing European Cloud Providers and Open Source ...</a></li>

</ul>
</details>

**社区讨论**: 社区情绪投入且务实，用户分享了个人迁移经验和具体的提供商推荐（例如 mailbox.org）。然而，讨论中也包含批判性观点，质疑欧盟司法管辖区是否能提供实质更好的隐私保护，并提及了对当地执法权力和跨境证据令的担忧。部分评论推广了针对特定美国服务的欧盟替代方案。

**标签**: `#privacy`, `#data-sovereignty`, `#digital-migration`, `#EU-regulation`, `#service-providers`

---

<a id="item-4"></a>
## [GitHub 可靠性据称降至“三个九”可用性，同时面临服务中断与安全担忧。](https://www.theregister.com/2026/02/10/github_outages/) ⭐️ 7.0/10

据报道，GitHub 正经历严重的可用性问题，其整体平台可靠性可能已降至约 99.9%（三个九），这意味着每年可能超过 8 小时的服务中断。与此同时，近期还出现了安全漏洞，例如 GitHub Actions 中可变引用的滥用导致了 Aqua Security 被入侵，并可能感染了数千次 CI/CD 运行。 GitHub 是全球软件开发生态的基础设施，其可靠性的下降直接影响着数百万依赖其进行代码托管、协作和 CI/CD 的开发者与企业。这种情况引发了关于在快速功能扩张（如 AI 工具）与维护核心平台稳定性及安全性之间如何权衡的关键问题，尤其是在向 Azure 进行重大基础设施迁移期间。 “三个九”（99.9%）的可用性指标，与关键服务通常期望的“五个九”（99.999%）标准相比显著下降，这意味着每年允许超过 8 小时的中断时间。批评者指出，GitHub 正在进行的向 Microsoft Azure 的基础设施迁移（于 2025 年宣布并承诺提高可靠性）可能是当前不稳定的根本原因。

hackernews · richtr · Mar 23, 10:39

**背景**: 在系统可靠性工程中，可用性通常以“九”来衡量。“三个九”意味着 99.9% 的正常运行时间，相当于每年允许大约 8.76 小时的中断。作为对比，“五个九”（99.999%）每年仅允许大约 5.26 分钟的中断。GitHub Actions 是 GitHub 的 CI/CD 平台，用于自动化软件工作流，其中的“可变引用”如果未得到妥善保护则会构成安全风险，因为它们允许在创建后更改构件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_availability">High availability - Wikipedia</a></li>
<li><a href="https://docs.github.com/en/actions/concepts/metrics">About GitHub Actions metrics</a></li>

</ul>
</details>

**社区讨论**: 社区表达了强烈的不满，认为 GitHub 过于关注 Copilot 等 AI 功能，而牺牲了核心平台的稳定性和安全性。许多人将可靠性问题直接归因于强制性的 Azure 迁移，并引用了 GitHub 管理层过去关于此举将提高可用性的保证。此外，社区对 GitHub Actions 中长期存在且未解决的安全漏洞在真实攻击中被利用表示严重担忧。

**标签**: `#infrastructure`, `#reliability`, `#devops`, `#cloud-services`, `#security`

---

<a id="item-5"></a>
## [研究对比 isolated-vm、vm2、QuickJS、ShadowRealm 和 Deno Workers 等 JavaScript 沙箱技术](https://simonwillison.net/2026/Mar/22/javascript-sandboxing-research/#atom-everything) ⭐️ 7.0/10

Simon Willison 在受到 Aaron Harper 关于 Node.js worker threads 的文章启发后，开展了一项对比多种 JavaScript 沙箱技术的研究。这项在 Claude Code 协助下完成的研究，系统性地评估了 isolated-vm、vm2、quickjs-emscripten、QuickJS-NG、ShadowRealm 和 Deno Workers 在安全代码执行方面的表现。 这项研究很重要，因为安全的 JavaScript 沙箱对于需要执行不可信代码的应用程序（如在线代码编辑器、插件系统和无服务器平台）至关重要。该对比为开发者在 Node.js 和 JavaScript 运行时环境中选择隔离解决方案提供了实用指导。 该研究具体考察了 isolated-vm（它提供了对 V8 Isolate 功能的访问）、ShadowRealm（一个处于 Stage 2.7 阶段的 ECMAScript 提案，用于创建隔离的执行环境）以及包括原版和 NG 分支在内的 QuickJS 实现。这项对比的起因是探索 Node.js worker threads 是否能增强沙箱安全性。

rss · Simon Willison · Mar 22, 19:53

**背景**: JavaScript 沙箱化指的是在受控环境中隔离并执行不可信代码，以防止其访问敏感系统资源的技术。isolated-vm 是一个 Node.js 库，它利用 V8 的 Isolate API 来创建安全的执行上下文。ShadowRealm 是 TC39 的一项提案，旨在在 JavaScript 语言本身内提供标准化的同步隔离环境。QuickJS 是一个小型、可嵌入的 JavaScript 引擎，可以通过 quickjs-emscripten 编译为 WebAssembly，以便在浏览器或 Node.js 中使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/laverdet/isolated-vm">GitHub - laverdet/isolated-vm: Secure & isolated JS environments for nodejs · GitHub</a></li>
<li><a href="https://github.com/tc39/proposal-shadowrealm">GitHub - tc39/proposal-shadowrealm: ECMAScript Proposal ...</a></li>
<li><a href="https://deepwiki.com/tc39/proposal-shadowrealm">tc39/proposal-shadowrealm | DeepWiki</a></li>

</ul>
</details>

**标签**: `#javascript`, `#sandboxing`, `#security`, `#runtime-environments`, `#nodejs`

---

<a id="item-6"></a>
## [交互式可视化工具发布，用于演示 Bram Cohen 基于 CRDT 的版本控制概念](https://simonwillison.net/2026/Mar/22/manyana/#atom-everything) ⭐️ 7.0/10

Simon Willison 利用 Claude AI 和 Pyodide 创建了一个名为 Merge State Visualizer 的交互式网页工具，用于演示 Bram Cohen 的 Manyana 项目——一个 470 行 Python 代码的、基于 CRDT 的版本控制概念验证。该工具提供了一个可视化界面，帮助理解无冲突合并算法在实际中如何工作。 这很重要，因为它使分布式系统的高级概念对开发者变得易于理解，可能加速基于 CRDT 的方法在版本控制领域的理解和采用。随着 AI 辅助开发的发展，能够可视化复杂算法的工具对于教育和原型设计变得越来越有价值。 该可视化工具是通过将 Cohen 的 Python 代码（不含注释）输入 Claude AI 生成解释，然后使用 Pyodide 创建基于浏览器的交互界面而构建的。Manyana 本身被描述为一个演示而非完整的版本控制系统，像 cherry-picking 和本地撤销等功能尚未实现。

rss · Simon Willison · Mar 22, 18:57

**背景**: CRDT（无冲突复制数据类型）是一种数据结构，使分布式系统能够在多个副本之间保持一致性，而无需解决冲突。BitTorrent 协议的创建者 Bram Cohen 最近提出了 Manyana，作为将 CRDT 原理应用于版本控制系统的愿景。Pyodide 是一项通过 WebAssembly 允许 Python 直接在 Web 浏览器中运行的技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bramcohen.com/p/manyana">Manyana - by Bram Cohen - Bram’s Thoughts</a></li>
<li><a href="https://crdt.tech/">About CRDTs • Conflict-free Replicated Data Types</a></li>
<li><a href="https://scribbler.live/2024/07/08/Python-in-Browser.html">Python in the Browser with Pyodide</a></li>

</ul>
</details>

**标签**: `#version-control`, `#crdt`, `#visualization`, `#python`, `#ai-tools`

---