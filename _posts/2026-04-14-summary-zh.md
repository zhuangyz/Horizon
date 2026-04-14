---
layout: default
title: "Horizon Summary: 2026-04-14 (ZH)"
date: 2026-04-14
lang: zh
---

> From 23 items, 7 important content pieces were selected

---

1. [Backblaze 悄然修改备份策略，未通知用户便排除了云存储文件夹。](#item-1) ⭐️ 8.0/10
2. [Steve Yegge 称谷歌的 AI 采用模式与传统行业（如 John Deere）相似](#item-2) ⭐️ 8.0/10
3. [多家主流媒体屏蔽互联网档案馆爬虫，记者联名支持数字保存](#item-3) ⭐️ 8.0/10
4. [斯坦福 2026 年 AI 指数报告：中美 AI 性能差距几近消失，AI 加速普及](#item-4) ⭐️ 8.0/10
5. [Jujutsu (jj) CLI 工具引入自动提交和版本控制新思维模型](#item-5) ⭐️ 7.0/10
6. [Blackmagic Design 发布 DaVinci Resolve Photo，将视频调色工具引入静态摄影](#item-6) ⭐️ 7.0/10
7. [谷歌宣布针对“后退按钮劫持”的新垃圾政策](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Backblaze 悄然修改备份策略，未通知用户便排除了云存储文件夹。](https://rareese.com/posts/backblaze/) ⭐️ 8.0/10

Backblaze 更新了其备份客户端，自动将 OneDrive、Google Drive 和 Dropbox 等流行云存储提供商的文件夹从其备份集中排除。这一策略变更在未直接通知用户的情况下实施，可能导致依赖 Backblaze 备份这些同步目录中文件的用户面临数据丢失风险。 这一变更削弱了用户对一家主要备份服务的信任，并凸显了依赖政策不透明的“无限”消费级 SaaS 产品的风险。它迫使用户重新评估备份策略，特别是对于那些将云同步文件夹视为本地数据生态系统一部分并默认其受到保护的用户。 排除范围包括 Box、iDrive 等服务的挂载点和缓存目录，官方理由是为防止性能问题和数据使用量过大。然而，这一变更并未被显著告知用户，且标准的 Backblaze Personal 备份计划默认有 30 天的版本历史限制，如果在排除生效后云文件夹中的文件被删除或覆盖，可能会加剧数据丢失。

hackernews · rrreese · Apr 14, 08:30

**背景**: Backblaze 是一种流行的云备份服务，以其针对个人电脑的“无限”备份计划而闻名。许多用户使用 Dropbox 或 OneDrive 等服务在设备间同步文件，从而创建了显示为常规目录的本地文件夹。传统上，像 Backblaze 这样的备份软件会将这些本地同步文件夹包含在其备份集中，为云存储数据提供第二个副本。3-2-1 备份规则建议至少拥有数据的三个副本，存储在两种不同的介质上，且有一个副本存放在异地。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rareese.com/posts/backblaze/">Backblaze has quietly stopped backing up your data | Robert Reese's Website</a></li>
<li><a href="https://www.backblaze.com/computer-backup/docs/backup-client-release-notes-windows">Backup Client Release Notes (Windows)</a></li>
<li><a href="https://www.backblaze.com/computer-backup/docs/supported-backup-data">Supported Backup Data</a></li>

</ul>
</details>

**社区讨论**: 社区对缺乏通知和感知到的信任破坏表达了强烈不满，并有用户报告了实际的数据丢失。讨论凸显了围绕 Backblaze 个人版“无限”商业模式的矛盾、其作为消费级工具与专业工具的定位之争，以及备份具有“按需文件”功能的云存储（可能耗尽本地磁盘空间）等技术挑战。

**标签**: `#backup`, `#cloud-storage`, `#data-loss`, `#policy-change`, `#saas`

---

<a id="item-2"></a>
## [Steve Yegge 称谷歌的 AI 采用模式与传统行业（如 John Deere）相似](https://simonwillison.net/2026/Apr/13/steve-yegge/#atom-everything) ⭐️ 8.0/10

前谷歌工程师 Steve Yegge 根据与一位资深谷歌技术总监的对话透露，谷歌内部的 AI 采用曲线与传统公司（如拖拉机制造商 John Deere）惊人地相似，只有约 20% 的员工是“智能体式重度用户”。这一观察立即遭到谷歌高管 Addy Osmani 和 Demis Hassabis 的反驳，他们称这些说法是错误的，并列举了公司内部对 AI 工具的广泛使用。 这场公开分歧突显了关于 AI 在顶尖科技公司内部真实整合速度的关键辩论。如果像谷歌这样的领导者也面临与非科技行业相似的采用挑战，则表明 AI 采用的组织和文化障碍可能是普遍存在的，这可能会减缓整个行业的创新步伐。 Yegge 描述了一种常见的行业采用模式：20% 的智能体式重度用户、20% 的完全拒绝者，以及 60% 仍在使用 Cursor 等基础聊天工具的人。他还将感知到的组织停滞与长达 18 个月的行业招聘冻结联系起来，称这限制了外部新鲜观点的流入。与此相反，Addy Osmani 表示，每周有超过 4 万名谷歌软件工程师使用智能体式编码，并能访问一系列定制的 AI 工具和系统。

rss · Simon Willison · Apr 13, 20:59

**背景**: Steve Yegge 是一位知名的软件工程师和博主，以其对科技巨头的批判性分析而闻名，曾在亚马逊和谷歌工作。“智能体式 AI”指的是能够自主执行任务并做出决策以实现目标的 AI 系统，而不仅仅是提供建议。Cursor 是一个 AI 驱动的集成开发环境，许多开发者通过其聊天界面获得编码辅助。自 2024 年底以来，科技行业经历了显著的招聘冻结，旨在削减成本，但常被批评影响了创新和知识流动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.grammarly.com/agentic-ai">What is Agentic AI ? | Agentic AI 101</a></li>
<li><a href="https://cursor.com/">Cursor : The best way to code with AI</a></li>
<li><a href="https://suchwork.org/hiring-freeze/">Hiring Freeze: Navigating the Impact on Workforce Strategy – SuchWork</a></li>

</ul>
</details>

**社区讨论**: 正如引用的高管回应所示，相关讨论两极分化严重。Yegge 的内部批评描绘了一幅令人惊讶的趋同和潜在平庸的图景。而谷歌官方的反驳，来自 Osmani 和 Hassabis 等人，强烈否认这种描述，坚称内部 AI 采用情况良好，并将原帖称为“无稽之谈”和“点击诱饵”。这就在谷歌 AI 的真实状况上形成了一种鲜明的“各执一词”的局面。

**标签**: `#AI Adoption`, `#Google`, `#Organizational Culture`, `#Software Engineering`, `#Industry Trends`

---

<a id="item-3"></a>
## [多家主流媒体屏蔽互联网档案馆爬虫，记者联名支持数字保存](https://www.wired.com/story/the-internets-most-powerful-archiving-tool-is-in-mortal-peril/) ⭐️ 8.0/10

包括《纽约时报》、USA Today 母公司 Gannett 及 Reddit 在内的至少 23 家主流新闻网站和平台，已开始屏蔽互联网档案馆的 'ia_archiverbot' 爬虫，主要担忧其存档内容被用于训练 AI 模型。作为回应，由电子前哨基金会组织的公开信已获得 100 多名记者联署，他们支持档案馆在事实核查和保存历史记录方面的关键作用。 这场冲突标志着一个关键时刻，AI 发展、版权执行和数字保存的需求在此直接碰撞。其结果可能严重削弱公众对网络历史记录的访问，影响新闻、研究和问责，并为如何处理对公共档案至关重要的网络爬虫树立先例。 屏蔽是通过 robots.txt 协议实现的，针对的是特定的用户代理 'ia_archiver'。一些媒体如《卫报》采取了更细致的方法，限制 API 访问而非完全屏蔽。互联网档案馆警告称，这种对公共网络的封锁将严重削弱社会了解历史和现实的能力。

telegram · zaihuapd · Apr 14, 00:12

**背景**: 互联网档案馆是一个非营利性数字图书馆，以其 Wayback Machine（网站时光机）而闻名，该工具会随时间推移存档可公开访问的网页快照。其自动网络爬虫以用户代理 'ia_archiver' 标识，通过一个称为网络存档的过程系统地收集这些快照。电子前哨基金会是一个领先的非营利性数字权利组织，倡导数字世界中的公民自由。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datadome.co/bots/internet-archive/">What is Internet Archive crawler bot</a></li>
<li><a href="https://en.wikipedia.org/wiki/Web_archiving">Web archiving - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Electronic_Frontier_Foundation">Electronic Frontier Foundation - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Digital Preservation`, `#Copyright`, `#Web Archiving`, `#Media`

---

<a id="item-4"></a>
## [斯坦福 2026 年 AI 指数报告：中美 AI 性能差距几近消失，AI 加速普及](https://hai.stanford.edu/ai-index/2026-ai-index-report) ⭐️ 8.0/10

斯坦福大学发布的《2026 年 AI 指数报告》指出，中美 AI 模型性能差距已基本消失，美国 Anthropic 的领先优势仅剩 2.7%。报告显示，中国在 AI 论文发表、专利产出、工业机器人装机量及公共 AI 超算数量上均位居全球第一，同时全球 AI 普及加速，对就业已产生显著影响。 这份报告为中国在 AI 能力上的快速追赶提供了关键证据，可能重塑全球技术力量平衡并加剧中美竞争。全球 AI 加速普及及其对软件开发岗位的已证实影响，凸显了全球范围内制定劳动力适应策略和政策回应的紧迫性。 报告指出，尽管超过 90%的顶尖 AI 模型在多项人类基准测试中表现出色，但它们呈现出'锯齿前沿'现象，即在不同任务上的能力表现不均。此外，全球 AI 算力在三年内增长了 30 倍，企业投资翻倍至 5817 亿美元，而进入美国的 AI 研究人员数量在过去一年骤降了 80%。

telegram · zaihuapd · Apr 14, 05:09

**背景**: AI 指数报告是斯坦福大学以人为本人工智能研究所（HAI）的年度出版物，负责追踪、整理和可视化全球人工智能发展的数据。Anthropic 是一家美国 AI 安全与研究公司，以开发 Claude 等大型语言模型而闻名。'锯齿前沿'指的是 AI 模型在某些任务上表现异常出色，却在其他对人类来说难度看似相似的任务上表现挣扎的现象，这突显了当前 AI 能力的不均衡性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-index/2025-ai-index-report">The 2025 AI Index Report | Stanford HAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Research`, `#Global AI Trends`, `#Technology Policy`, `#AI Workforce`, `#Industry Analysis`

---

<a id="item-5"></a>
## [Jujutsu (jj) CLI 工具引入自动提交和版本控制新思维模型](https://steveklabnik.github.io/jujutsu-tutorial/introduction/what-is-jj-and-why-should-i-care.html) ⭐️ 7.0/10

新的命令行版本控制工具 Jujutsu (jj) 已发布，它采用了与 Git 根本不同的工作流程，特点是自动提交所有更改并取消了传统的暂存区。它完全兼容现有的 Git 仓库，允许开发者透明地使用它，而队友可以继续使用 Git。 这很重要，因为它通过减少认知负担并使版本控制操作更流畅、更不易出错，挑战了主流的 Git 范式。如果被广泛采用，它可能会显著改变开发者的工作流程，特别是对于那些处理复杂分支、频繁上下文切换或合并冲突的开发者，有可能提高生产力。 一个关键的技术细节是，jj 会自动为工作副本的每一次更改创建一个提交，这从根本上改变了编辑-提交的工作流程。虽然这实现了强大的撤销操作和冲突处理能力，但也要求用户在需要检查旧状态而不改变历史时，采取创建空提交的防御性做法。

hackernews · tigerlily · Apr 14, 10:33

**背景**: Git 是主流的分布式版本控制系统 (DVCS)，其模型要求开发者在将更改提交到本地历史之前，需要显式地将更改暂存。暂存区（或索引）是 Git 的核心概念，它将已修改的文件与已提交的快照分开。Jujutsu (jj) 是一个较新的 DVCS，它使用 Git 作为后端存储层，但向用户呈现了一个不同的、以变更为中心的界面，旨在简化常见操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.jj-vcs.dev/latest/">Jujutsu—a version control system - docs.jj-vcs.dev</a></li>
<li><a href="https://docs.jj-vcs.dev/latest/git-comparison/">Git comparison - Jujutsu docs</a></li>
<li><a href="https://github.com/jj-vcs/jj/blob/main/docs/git-comparison.md">jj/docs/git-comparison.md at main · jj-vcs/jj · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示出复杂但深思熟虑的反应。一些用户正在积极地将 jj 与 GitButler 等其他现代工具进行比较，并探索其范式转变。主要的担忧包括需要适应自动提交模型，一位用户指出这需要创建空提交来安全地检查旧代码。另一位用户对采用前景表示怀疑，认为在没有像 GitHub 这样的平台推动的情况下，很难取代 Git 这样的行业标准。

**标签**: `#version-control`, `#developer-tools`, `#git`, `#cli`, `#workflow`

---

<a id="item-6"></a>
## [Blackmagic Design 发布 DaVinci Resolve Photo，将视频调色工具引入静态摄影](https://www.blackmagicdesign.com/products/davinciresolve/photo) ⭐️ 7.0/10

Blackmagic Design 发布了 DaVinci Resolve Photo，这是一款新的独立照片编辑应用程序，它将专业的视频调色工具以及对佳能、富士、尼康、索尼和 iPhone ProRAW 文件的原生 RAW 支持引入了静态摄影工作流程。 此次发布意义重大，因为它弥合了专业视频和照片编辑之间的鸿沟，让摄影师能够使用 DaVinci Resolve 业界领先的色彩科学和调色工具，这些工具以前是视频后期制作的专属。它为专业照片编辑市场引入了新的竞争，可能对 Adobe 等现有厂商构成挑战。 该应用程序包含对主流相机品牌和 iPhone ProRAW 的原生 RAW 支持，并继承了 DaVinci Resolve 的高级功能，如 HDR 调色、面部修饰和降噪。然而，一些用户报告其 Linux 版本可能难以设置，且产品页面上没有突出列出详细的技术规格。

hackernews · thebiblelover7 · Apr 14, 02:25

**背景**: DaVinci Resolve 是 Blackmagic Design 开发的专业视频编辑、调色和音频后期制作软件套件，因其强大的调色功能而广泛应用于电影和电视行业。RAW 文件是相机传感器捕获的未经处理的图像数据，与 JPEG 等压缩格式相比，在编辑方面提供了更大的灵活性。照片编辑软件市场一直由 Adobe Lightroom 和 Photoshop 等工具主导，而 Darktable 等开源替代品则在推动技术创新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.blackmagicdesign.com/products/davinciresolve/color">DaVinci Resolve – Color | Blackmagic Design</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blackmagic_Design">Blackmagic Design - Wikipedia</a></li>
<li><a href="https://petapixel.com/best-free-raw-editing-programs/">The Best Free RAW Photo Editing Programs in 2026 - PetaPixel</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体上是积极和兴奋的，期待专业的视频调色工具应用于摄影的潜力。关键的讨论点包括：对功能集的热情、对 Linux 安装困难和缺乏清晰技术规格的沮丧，以及与 Darktable 等现有工具的比较。一些用户表示，这次发布实现了他们长久以来对基于 DaVinci Resolve 的照片编辑器的愿望。

**标签**: `#photo-editing`, `#davinci-resolve`, `#raw-processing`, `#creative-tools`, `#software-release`

---

<a id="item-7"></a>
## [谷歌宣布针对“后退按钮劫持”的新垃圾政策](https://developers.google.com/search/blog/2026/04/back-button-hijacking) ⭐️ 7.0/10

谷歌宣布了一项专门针对“后退按钮劫持”的新垃圾政策，该技术指网站通过操纵浏览器历史记录来阻止用户轻松离开。该政策旨在将此类操纵性行为归类为垃圾信息，并可能对违规网站在搜索排名中进行处罚。 这很重要，因为后退按钮劫持严重降低了用户体验，并可能被用于欺骗或恶意目的，例如将用户困在充满广告的页面上或协助网络钓鱼攻击。通过采取行动，谷歌正在解决一个普遍存在的网络困扰，并将其搜索质量工作与核心用户体验原则保持一致。 该政策的执行将依赖谷歌的检测系统来识别那些使用如 `history.replaceState` 或 `location.replace` 等技术、在未经用户同意的情况下操纵浏览器历史记录堆栈的网站。值得注意的是，社区讨论强调，像 LinkedIn 和 Microsoft 这样的大型平台已被引为此类行为的现实案例。

hackernews · zdw · Apr 14, 03:06

**背景**: 后退按钮劫持是一种操纵性的网络行为，指使用 JavaScript 或其他技术干扰浏览器后退按钮的正常功能。通常，点击“后退”应将用户返回到其浏览历史记录中的上一个页面。然而，劫持行为可能将用户重定向到不需要的页面、将他们留在同一网站，甚至通过利用引荐来源信息来协助攻击。谷歌的网络垃圾政策旨在打击各种操纵搜索结果或为不公平收益而降低用户体验的策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wolf-of-seo.de/en/what-is/back-button-hijack/">What is Back Button Hijack ? A glossary entry about online risks</a></li>
<li><a href="https://chromium.googlesource.com/chromium/src/+/main/docs/history_manipulation_intervention.md">Chromium Docs - History manipulation intervention in Chromium</a></li>

</ul>
</details>

**社区讨论**: 社区反应大体上是积极的，但对执行效果持怀疑态度，用户希望谷歌能使其有效运作。评论者提供了 LinkedIn 和 Microsoft 等主要平台从事此类行为的具体例子，证实了该问题的重要性。一些用户表达了希望获得更广泛保护的愿望，反对任何形式的后退按钮干扰，而不仅仅是与垃圾信息相关的劫持。

**标签**: `#web-development`, `#user-experience`, `#search-engines`, `#browser-security`, `#spam-policy`

---