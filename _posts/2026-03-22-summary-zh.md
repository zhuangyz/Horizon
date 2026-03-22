---
layout: default
title: "Horizon Summary: 2026-03-22 (ZH)"
date: 2026-03-22
lang: zh
---

> From 14 items, 3 important content pieces were selected

---

1. [马斯克计划在 30 至 36 个月内将 AI 计算中心部署至太空。](#item-1) ⭐️ 8.0/10
2. [Simon Willison 演示利用 Hacker News 评论历史进行 AI 用户画像分析](#item-2) ⭐️ 7.0/10
3. [宇树科技计划 2026 年出货 2 万台人形机器人，进军家用市场挑战特斯拉 Optimus](#item-3) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [马斯克计划在 30 至 36 个月内将 AI 计算中心部署至太空。](https://t.me/zaihuapd/40437) ⭐️ 8.0/10

埃隆·马斯克披露，计划在 30 至 36 个月内将 AI 计算中心部署至太空，他指出太空的太阳能效率是地面的 5 倍且无需电池储备，是解决地球能源瓶颈的方案。此外，他还宣布了通过 Tesla 和 SpaceX 实现年产 100 GW 太阳能电池的目标，筹建大规模芯片工厂 TeraFab，并预计人形机器人 Optimus 的第三代版本年产量可达 100 万台。 这一计划意义重大，因为它为解决 AI 指数级增长所面临的能源供应瓶颈提出了一个根本性的解决方案，可能使计算能力摆脱对地面电网的依赖。如果实现，它将重塑高性能计算的经济性和地理布局，而其集成的太阳能、芯片制造和机器人愿景，旨在为自动化和 AI 构建一个垂直整合的生态系统。 马斯克声称太空的太阳能效率是地球的 5 倍，且无需电池储备。TeraFab 芯片工厂是 Tesla 和 SpaceX 的联合项目，旨在每年生产超过 1 太瓦（万亿瓦）的 AI 算力。Optimus Gen 3 机器人手部具有 22 个自由度，这是一次旨在实现通用任务的重大升级。

telegram · zaihuapd · Mar 22, 02:24

**背景**: 天基太阳能是指在大空收集太阳能并传输回地球的概念，与受昼夜循环和天气影响的地面太阳能板相比，其优势在于能获得近乎持续的日照（地球同步轨道上可达 99.9%的时间）。TeraFab 是 Tesla 和 SpaceX 提出的一个大规模半导体制造项目，旨在生产海量的 AI 计算芯片。Tesla 的 Optimus 是一个旨在执行危险、重复或枯燥任务的人形机器人项目，其开发历经数代，灵巧性不断提升，例如 Gen 3 版本的手部具有 22 个自由度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Space-based_solar_power">Space-based solar power - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Terafab">Terafab - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Optimus_(robot)">Optimus (robot) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Space Technology`, `#Renewable Energy`, `#High-Performance Computing`, `#Strategic Vision`

---

<a id="item-2"></a>
## [Simon Willison 演示利用 Hacker News 评论历史进行 AI 用户画像分析](https://simonwillison.net/2026/Mar/21/profiling-hacker-news-users/#atom-everything) ⭐️ 7.0/10

Simon Willison 开发并描述了一种为 Hacker News 用户创建画像的方法：通过 Algolia API 程序化地获取用户最近的 1000 条评论，然后使用 Claude Opus 等大型语言模型对聚合的文本进行分析。他创建了一个简单的网页工具，利用该 API 开放的 CORS 标头来获取任何用户名的评论数据，并为 LLM 分析步骤提供了方便的复制到剪贴板功能。 这项技术展示了如何将公开可访问的社交数据与现代 AI 结合，用于推断详细的个人及职业画像，这为在线社区带来了重大的隐私和伦理问题。它也展示了 LLM 在社会数据分析中的一个实用、低代码的应用，可能会影响研究人员、营销人员或社区管理者处理公共论坛数据的方式。 该方法依赖于 Algolia Hacker News API 的 `search_by_date` 端点，该端点允许通过 `author_username` 标签过滤评论，并支持每次请求获取多达 1000 条结果。一个关键的技术推动因素是，该 API 配置了开放的 CORS 标头，使得抓取工具可以在任何网页上运行客户端 JavaScript，而无需服务器端代理。

rss · Simon Willison · Mar 21, 23:59

**背景**: Hacker News 是一个专注于科技和创业的流行社交新闻网站，由创业孵化器 Y Combinator 运营。Algolia Hacker News API 是一个免费的公共 API，无需认证即可对 Hacker News 的内容（包括故事和评论）提供全文搜索。CORS（跨源资源共享）标头是 HTTP 标头，它告诉浏览器允许运行在一个源上的 Web 应用程序访问来自不同源的资源，这就是为什么 Simon 的工具可以直接从用户浏览器获取数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@otabekjon0302/how-to-use-a-hacker-news-data-from-algolia-api-d7dd32341436">How to Use a Hacker News data from Algolia API | by Otabekjon | Medium</a></li>
<li><a href="https://stackoverflow.com/questions/50261027/access-algolia-rest-api-via-javascript-cors-errors">Access Algolia REST API via JavaScript: CORS errors - Stack Overflow</a></li>

</ul>
</details>

**标签**: `#data-analysis`, `#hacker-news`, `#api`, `#llm`, `#profiling`

---

<a id="item-3"></a>
## [宇树科技计划 2026 年出货 2 万台人形机器人，进军家用市场挑战特斯拉 Optimus](https://www.eweek.com/news/unitree-20000-humanoid-robots-2026-china/) ⭐️ 7.0/10

中国机器人公司宇树科技计划在 2026 年将其人形机器人出货量提升至 2 万台，相比 2025 年约 5500 台的目标大幅增长。该公司正筹备在上海证券交易所进行首次公开募股，拟募资 42 亿元人民币用于研发人形机器人平台，并计划在三年内进军家用机器人市场，直接挑战特斯拉的 Optimus。 这一声明标志着人形机器人商业化进程的重大加速，宇树科技旨在抢占一个中国制造商已占据全球近 80%出货量的市场的重要份额。在消费级市场与特斯拉的直接竞争，可能会推动更快的创新、降低成本，并促进人形机器人技术的更广泛应用。 根据摩根士丹利的数据，2025 年全球人形机器人出货量预计约为 1.3 万台，其中宇树科技和另一家中国公司智元机器人是中国占据主导市场份额的主要贡献者。宇树科技的 H2 人形机器人拥有 31 个自由度并集成了语音交互功能，专为实际部署和研究应用而设计。

telegram · zaihuapd · Mar 22, 04:15

**背景**: 宇树科技是一家知名的中国领先机器人公司，最初以其高性能的四足（仿狗）机器人闻名，其产品曾亮相于央视春晚和冬奥会开幕式等重大场合。人形机器人，如特斯拉的 Optimus 和宇树的 H2，是设计用于在人类环境中执行任务的双足机器，代表了专注于通用自动化的机器人技术前沿。该领域的竞争涉及运动控制、操作和 AI 集成方面的重大技术挑战，各公司正致力于将研究原型转化为大规模生产、具有商业可行性的产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unitree.com/">Unitree Robotics | Robot Dog_Quadruped_Humanoid Robotics Company</a></li>
<li><a href="https://www.reuters.com/world/asia-pacific/unitree-plans-shanghai-ipo-testing-interest-humanoid-robots-2026-03-20/">Unitree plans Shanghai IPO, testing interest in humanoid robots</a></li>
<li><a href="https://en.wikipedia.org/wiki/Optimus_(robot)">Optimus (robot) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#robotics`, `#humanoid-robots`, `#industrial-news`, `#china-tech`, `#tesla-competition`

---