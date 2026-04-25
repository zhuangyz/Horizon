---
layout: default
title: "Horizon Summary: 2026-04-25 (EN)"
date: 2026-04-25
lang: en
---

> From 24 items, 17 important content pieces were selected

---

1. [Google Plans Up to $40B Investment in Anthropic](#item-1) ⭐️ 9.0/10
2. [DeepSeek V4 Preview: Largest Open Weights Model, Low Cost](#item-2) ⭐️ 9.0/10
3. [DeepSeek-V4 Preview Released and Open-Sourced with Agent Optimization](#item-3) ⭐️ 9.0/10
4. [Nilay Patel: 'Software Brain' Explains AI's Unpopularity](#item-4) ⭐️ 8.0/10
5. [Anthropic Postmortem Reveals Three Claude Code Bugs](#item-5) ⭐️ 8.0/10
6. [Bluesky 'For You' Feed Runs on a Gaming PC with SQLite](#item-6) ⭐️ 8.0/10
7. [Huawei unveils ADS 4, targeting L3 commercial use by 2025](#item-7) ⭐️ 8.0/10
8. [Reverse Engineering Reveals Lifetime Subscription Flaw](#item-8) ⭐️ 8.0/10
9. [OpenAI Open-Sources Model Monitoring Evaluation Suite](#item-9) ⭐️ 8.0/10
10. [AI Table Tennis Robot Defeats Elite Human Players](#item-10) ⭐️ 8.0/10
11. [Samsung union strike vote threatens chip supply](#item-11) ⭐️ 8.0/10
12. [Overthinking and scope creep sabotage projects](#item-12) ⭐️ 7.0/10
13. [Honker Brings Postgres NOTIFY/LISTEN to SQLite](#item-13) ⭐️ 7.0/10
14. [Apple Requires USCI from App Store Developers in China](#item-14) ⭐️ 7.0/10
15. [US AI tool users show income stratification: Claude high, Meta AI low](#item-15) ⭐️ 7.0/10
16. [Tesla Cybercab enters production in North America](#item-16) ⭐️ 7.0/10
17. [Android Verified Email Registration Eliminates OTPs](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Google Plans Up to $40B Investment in Anthropic](https://www.bloomberg.com/news/articles/2026-04-24/google-plans-to-invest-up-to-40-billion-in-anthropic) ⭐️ 9.0/10

Google plans to invest up to $40 billion in AI company Anthropic, with an initial $10 billion at a $350 billion valuation and an additional $30 billion contingent on performance targets. This massive investment signals a strategic bet on AI infrastructure and capacity, deepening Google's ties to Anthropic amid an accelerating AI arms race and highlighting the commodification of foundation models. Anthropic's annual run-rate revenue surpassed $30 billion this month, up from about $9 billion at the end of 2025, and its Claude Code tool has gained strong traction among developers.

hackernews · elffjs · Apr 24, 16:04

**Background**: Anthropic is an AI safety and research company that develops large language models (LLMs) named Claude. Google has previously provided Anthropic with TPU capacity through deals with Broadcom, and the new investment is seen as a form of vendor financing at a very large scale.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/business/google-plans-invest-up-40-billion-anthropic-bloomberg-news-reports-2026-04-24/">Google to invest up to $40 billion in AI rival Anthropic | Reuters</a></li>
<li><a href="https://www.quiverquant.com/news/Google+Invests+$10+Billion+in+Anthropic+as+AI+Infrastructure+Race+Accelerates">Google Invests $10 Billion in Anthropic as AI Infrastructure Race Accelerates | Quiver Quantitative</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments highlight that Anthropic was becoming severely capacity constrained, leading to adverse contracts with both Amazon and Google. Some see the investment as a hedge against commodification of foundation models, while others note the astounding revenue potential from Claude models for developers.

**Tags**: `#AI`, `#investment`, `#Anthropic`, `#Google`, `#cloud computing`

---

<a id="item-2"></a>
## [DeepSeek V4 Preview: Largest Open Weights Model, Low Cost](https://simonwillison.net/2026/Apr/24/deepseek-v4/#atom-everything) ⭐️ 9.0/10

Chinese AI lab DeepSeek released two preview models, DeepSeek-V4-Pro and DeepSeek-V4-Flash, on April 24, 2026. V4-Pro is the largest open weights model to date with 1.6 trillion total parameters and 1 million token context, while V4-Flash offers a lighter 284B total parameters at a fraction of the cost of frontier models. This release significantly advances open-source AI by making a frontier-competitive model available at dramatically lower prices—V4-Flash costs just $0.14 per million input tokens, far below competitors like GPT-5.4 Nano ($0.20) and Claude Haiku 4.5 ($1.00). It challenges the dominance of proprietary models and could accelerate adoption of open-weight AI in production systems. Both models use a Mixture of Experts (MoE) architecture: V4-Pro has 1.6T total parameters with 49B active per token, while V4-Flash has 284B total with 13B active. They are released under the standard MIT license, and V4-Pro is 865GB on Hugging Face, while V4-Flash is 160GB.

rss · Simon Willison · Apr 24, 06:01

**Background**: Mixture of Experts (MoE) is a neural network architecture that splits computation into multiple expert subnetworks, enabling models to be pretrained with far less compute than dense models of similar capacity. Open weights models, unlike fully open-source AI, release only the trained model parameters under permissive licenses, allowing broad use while keeping training data and code proprietary. DeepSeek's V4 series builds on its V3 lineage, with V3.2 released in December 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://www.neowin.net/news/deepseek-v4-goes-live-with-massive-16t-parameters-and-1m-context-support/">DeepSeek V4 goes live with massive 1.6T parameters and 1M ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#DeepSeek`, `#open-source`, `#large language models`, `#machine learning`

---

<a id="item-3"></a>
## [DeepSeek-V4 Preview Released and Open-Sourced with Agent Optimization](https://mp.weixin.qq.com/s/8bxXqS2R8Fx5-1TLDBiEDg?scene=1) ⭐️ 9.0/10

DeepSeek has released the preview version of DeepSeek-V4, including V4-Pro and V4-Flash, and open-sourced the models. The V4-Pro variant surpasses all previously benchmarked open-source models in math, STEM, and competitive coding, matching the capabilities of top-tier proprietary models. This release significantly advances open-source AI by providing a highly capable, cost-efficient model optimized for agent workflows. It lowers the barrier for developers and researchers to build sophisticated AI agents, potentially accelerating innovation in autonomous systems and tool-use applications. Both V4-Pro and V4-Flash support a maximum context length of 1 million tokens and offer both non-thinking and thinking modes. V4-Flash uses fewer parameters and activations, providing faster and more economical API services while maintaining strong reasoning and agent capabilities.

telegram · zaihuapd · Apr 24, 02:50

**Background**: DeepSeek-V4 is a Mixture-of-Experts (MoE) language model with 1.6 trillion total parameters and 49 billion activated parameters. It features a hybrid attention architecture combining Compressed Sparse Attention (CSA) and Heavily Compressed Attention (HCA), achieving high efficiency for long-context tasks. The model is specifically optimized for popular agent frameworks such as Claude Code, OpenClaw, OpenCode, and CodeBuddy.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.sglang.io/cookbook/autoregressive/DeepSeek/DeepSeek-V4">DeepSeek-V4 - SGLang Documentation</a></li>
<li><a href="https://build.nvidia.com/deepseek-ai/deepseek-v4-pro/modelcard">deepseek-v4-pro Model by Deepseek-ai | NVIDIA NIM</a></li>
<li><a href="https://deepseekmodel1.org/deepseek-v4">DeepSeek V4 — Next-Generation AI Model Architecture</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-source`, `#large language model`, `#DeepSeek`, `#agent`

---

<a id="item-4"></a>
## [Nilay Patel: 'Software Brain' Explains AI's Unpopularity](https://simonwillison.net/2026/Apr/24/the-people-do-not-yearn-for-automation/#atom-everything) ⭐️ 8.0/10

Nilay Patel, editor-in-chief of The Verge, published a written and video essay arguing that people with 'software brain'—who view the world through automation—are becoming detached from the general public, which explains why AI remains unpopular despite surging usage numbers for ChatGPT. This analysis highlights a critical cultural and industry tension: the tech elite's enthusiasm for automation clashes with the public's desire for human-centered experiences, potentially shaping how AI products are designed and marketed in the future. Patel cites an NBC News poll showing AI has a lower favorability rating than ICE, and notes that Gen Z in particular seems to hate AI more as they encounter it. He contrasts the tech industry's 'software brain' mindset with the fact that regular people do not yearn for automation, using smart home technology as an example of a decade-long failure to engage the public.

rss · Simon Willison · Apr 24, 22:38

**Background**: The term 'software brain' describes a mindset that models everything in terms of information flows, data, and automation—a perspective that has dominated the business world for decades. Patel argues that while this mindset has driven innovation, it flattens the human experience and alienates people who do not see the world as something to be automated. The essay builds on a long-standing debate about the gap between tech enthusiasts and the general public, especially regarding AI adoption.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Apr/24/the-people-do-not-yearn-for-automation/">The people do not yearn for automation - simonwillison.net</a></li>
<li><a href="https://www.youtube.com/watch?v=1RKGWg2Ex2U">THE PEOPLE DO NOT YEARN FOR AUTOMATION | Decoder - YouTube The Verge argues many people dislike AI because it pushes ... THE PEOPLE DO NOT YEARN FOR AUTOMATION - Career Ahead Magazine Daring Fireball: Nilay Patel: 'Beware Software Brain' THE PEOPLE DO NOT YEARN FOR AUTOMATION - Nilay Patel | Aetos.AI</a></li>
<li><a href="https://careeraheadonline.com/the-people-do-not-yearn-for-automation/">THE PEOPLE DO NOT YEARN FOR AUTOMATION - Career Ahead Magazine</a></li>

</ul>
</details>

**Tags**: `#AI`, `#automation`, `#technology criticism`, `#software culture`, `#public perception`

---

<a id="item-5"></a>
## [Anthropic Postmortem Reveals Three Claude Code Bugs](https://simonwillison.net/2026/Apr/24/recent-claude-code-quality-reports/#atom-everything) ⭐️ 8.0/10

Anthropic published a postmortem confirming that three bugs in the Claude Code harness—not the underlying AI models—caused widespread reports of degraded quality over the past two months. This is significant because Claude Code is a widely used AI coding tool, and the bugs directly affected user experience by making the model appear forgetful and repetitive, eroding trust in the product. One critical bug, introduced on March 26, cleared Claude's older thinking every turn instead of only once after an idle session, causing the model to seem forgetful and repetitive.

rss · Simon Willison · Apr 24, 01:31

**Background**: Claude Code is an AI-powered coding assistant from Anthropic that helps developers write, debug, and refactor code. A "harness" is the software layer that manages how the AI model interacts with tools and maintains session state; bugs in this layer can degrade performance even if the model itself is fine.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents">Effective harnesses for long-running agents \ Anthropic</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion linked in the article likely expressed relief that the issues were confirmed and appreciated the transparency, while also noting the complexity of debugging agentic systems.

**Tags**: `#Claude Code`, `#Anthropic`, `#AI coding tools`, `#postmortem`, `#bug analysis`

---

<a id="item-6"></a>
## [Bluesky 'For You' Feed Runs on a Gaming PC with SQLite](https://simonwillison.net/2026/Apr/24/serving-the-for-you-feed/#atom-everything) ⭐️ 8.0/10

A guest post on the AT Protocol blog reveals that the Bluesky 'For You' custom feed, used by 72,000 users, is served by a single Go process using SQLite on a gaming PC in the developer's living room, with recommendations based on likes. This demonstrates that a decentralized social media feed can be operated at scale with surprisingly modest hardware and low cost ($30/month), challenging assumptions about infrastructure requirements for algorithmic recommendations. The Go server consumes the AT Protocol firehose, stores 90 days of data in SQLite (currently ~419GB), and uses a $7/month VPS on OVH for public internet traffic, connected to the living room server via Tailscale.

rss · Simon Willison · Apr 24, 01:08

**Background**: Bluesky is a decentralized social network built on the AT Protocol, which allows anyone to run custom feed algorithms. The firehose is a real-time stream of all events across the network, enabling third-party services to stay synchronized. SQLite is a lightweight, embedded database engine, typically not associated with large-scale production workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bskyinfo.com/glossary/firehose/">Firehose | AT Protocol Glossary</a></li>
<li><a href="https://docs.bsky.app/docs/starter-templates/custom-feeds">Custom Feeds | Bluesky</a></li>
<li><a href="https://bsky.social/about/blog/7-27-2023-custom-feeds">Algorithmic Choice with Custom Feeds - Bluesky</a></li>

</ul>
</details>

**Tags**: `#Bluesky`, `#AT Protocol`, `#Go`, `#SQLite`, `#decentralized social media`

---

<a id="item-7"></a>
## [Huawei unveils ADS 4, targeting L3 commercial use by 2025](https://t.me/zaihuapd/41039) ⭐️ 8.0/10

At the Huawei Qiankun Intelligent Technology Conference on April 22, Huawei announced the new ADS 4 autonomous driving system and introduced the industry's first highway L3 conditional autonomous driving commercial solution. Huawei predicts it will achieve L3 commercial capability by 2025. This marks a significant milestone in autonomous driving, as L3 allows drivers to disengage from driving under certain conditions, shifting responsibility to the vehicle. Huawei's move could accelerate industry-wide adoption of L3 technology and intensify competition among automakers and tech firms. ADS 4 adopts deep sensor fusion and a new world model architecture called WEWA, which reduces end-to-end latency. The system is designed to prioritize highway scenarios for L3 deployment, as noted by Huawei's BU CEO Jin Yuzhi.

telegram · zaihuapd · Apr 24, 01:40

**Background**: L3 autonomy, or conditional automation, allows the vehicle to handle all driving tasks in specific conditions (e.g., highways) while the driver must be ready to take over when requested. It is considered a critical step between driver-assistance L2 and full self-driving L4, requiring high-precision maps and robust sensor systems.

<details><summary>References</summary>
<ul>
<li><a href="https://auto.huawei.com/cn/news/2026/2026-04-23-jishu">2026 华为乾崑技术大会在京举行 - auto.huawei.com</a></li>
<li><a href="https://auto.news18a.com/news/storys_249621.html">auto.news18a.com/news/storys_249621.html</a></li>
<li><a href="https://www.zhihu.com/question/395047744">什么才是真正的L3自动驾驶？ - 知乎</a></li>

</ul>
</details>

**Tags**: `#autonomous driving`, `#Huawei`, `#L3 autonomy`, `#ADS 4`, `#smart vehicles`

---

<a id="item-8"></a>
## [Reverse Engineering Reveals Lifetime Subscription Flaw](https://github.com/Yu9191/flux) ⭐️ 8.0/10

A reverse engineering report published on GitHub reveals that a popular app's subscription validation relies on a developer-controlled server, with hardcoded logic to revoke local authorization after repeated server failures, potentially invalidating lifetime purchases. This finding raises critical questions about the definition of 'lifetime' in lifetime subscriptions and highlights a fundamental architectural flaw that could render paid users' purchases worthless if the developer's server goes down, affecting consumer rights and trust in subscription-based software. The app uses a hybrid validation mode where server-side status is primary and Apple's StoreKit 2 is secondary; the binary contains hardcoded logic that clears authorization caches after N consecutive verification failures, meaning a server outage can actively revoke local subscription status including lifetime purchases.

telegram · zaihuapd · Apr 24, 02:02

**Background**: In iOS apps, subscription validation can be done locally using StoreKit 2's signed transaction data from Apple, which provides a reliable way to verify purchases without relying on an external server. However, some developers choose to implement their own server-side validation for additional control, which introduces a dependency on server availability. The WCDB database mentioned in the report is a cross-platform database framework developed by WeChat, used here for local caching of subscription status.

<details><summary>References</summary>
<ul>
<li><a href="https://www.revenuecat.com/blog/engineering/ios-in-app-subscription-tutorial-with-storekit-2-and-swift/">iOS In-App Subscription Tutorial with StoreKit 2 and Swift</a></li>
<li><a href="https://developer.apple.com/videos/play/wwdc2021/10114/">Meet StoreKit 2 - WWDC21 - Videos - Apple Developer</a></li>
<li><a href="https://explore.market.dev/ecosystems/windows/projects/wcdb">WCDB is a cross-platform database framework developed by WeChat.</a></li>

</ul>
</details>

**Tags**: `#reverse engineering`, `#subscription validation`, `#software architecture`, `#consumer rights`, `#server dependency`

---

<a id="item-9"></a>
## [OpenAI Open-Sources Model Monitoring Evaluation Suite](https://github.com/openai/monitorability-evals) ⭐️ 8.0/10

OpenAI has open-sourced the evaluation suite accompanying its research paper "Monitoring Monitorability," providing standardized tools to assess and improve the monitorability of AI model behaviors. The suite includes 12 public datasets such as AIME, GPQA, and WMDP, along with evaluation logic and prompt templates. This release directly addresses the critical challenge of monitoring advanced AI systems, especially as models become more capable of complex reasoning and potentially deceptive behaviors. By providing open-source tools, OpenAI enables the broader research community to collaborate on developing robust AI safety monitoring standards. The suite covers three categories of evaluations: intervention, process, and outcome attributes, but excludes private datasets like FrontierMath due to copyright and privacy restrictions. OpenAI noted technical limitations in evaluations like Anti-Scheming and is iterating with feedback from the GPT 5.4 Thinking system.

telegram · zaihuapd · Apr 24, 05:51

**Background**: The suite is based on OpenAI's research paper "Monitoring Monitorability," which explores how to effectively monitor a model's chain-of-thought reasoning to detect unsafe behaviors. The paper found that monitoring internal reasoning is far more effective than monitoring outputs alone. The Weapons of Mass Destruction Proxy (WMDP) benchmark, included in the suite, is a dataset of multiple-choice questions measuring hazardous knowledge in biosecurity, cybersecurity, and chemical security.

<details><summary>References</summary>
<ul>
<li><a href="https://ninza7.medium.com/can-we-trust-ai-thinking-openais-verdict-on-monitoring-is-out-9f2fe709185d">Can We Trust AI “Thinking”? OpenAI ’s Verdict on Monitoring Is Out</a></li>
<li><a href="https://arxiv.org/html/2512.18311v1">Monitoring Monitorability</a></li>
<li><a href="https://openai.com/index/evaluating-chain-of-thought-monitorability/">Evaluating chain-of-thought monitorability | OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI安全`, `#开源`, `#模型评估`, `#监控`

---

<a id="item-10"></a>
## [AI Table Tennis Robot Defeats Elite Human Players](https://t.me/zaihuapd/41046) ⭐️ 8.0/10

Researchers have developed 'Ace', an autonomous table tennis robot that uses event-driven vision sensors and model-agnostic reinforcement learning to defeat elite human players in real-time matches. This marks a major breakthrough in physical AI, demonstrating that robots can handle high-speed, high-precision real-world interactions previously thought too challenging. The technology could eventually be applied to sports training, rehabilitation, and other domains requiring rapid physical response. Ace uses event-driven vision sensors that capture motion with extremely low latency, combined with a model-agnostic reinforcement learning algorithm to adapt strategies on the fly. In official matches, it consistently returned high-speed, high-spin balls and defeated professional players multiple times.

telegram · zaihuapd · Apr 24, 06:01

**Background**: Traditional AI has excelled in turn-based games like chess and Go, but real-time physical sports like table tennis require split-second perception and reaction. Event-driven vision sensors, unlike conventional frame-based cameras, only record changes in the scene, drastically reducing latency and data volume. Model-agnostic reinforcement learning allows the robot to learn and adapt without relying on a pre-defined model of the environment.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.csdn.net/weixin_41496173/article/details/141365402">深度解析DeepMind乒乓球AI：从AlphaGo到AlphaPingPong的进化之路_ai 乒乓球-CSDN博客</a></li>
<li><a href="https://www.prophesee.ai/wp-content/uploads/2021/10/Prophesee-Synsense-PR-CN.pdf">SynSense 时识科技与 Prophesee 普诺飞思达成战略合</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#AI`, `#reinforcement learning`, `#physical AI`, `#table tennis`

---

<a id="item-11"></a>
## [Samsung union strike vote threatens chip supply](https://t.me/zaihuapd/41053) ⭐️ 8.0/10

Samsung Electronics' labor union, representing about 90,000 members, is voting on a strike plan that, if approved, would begin on May 21 and last 18 days, potentially halving production at the Pyeongtaek semiconductor plant and disrupting global chip supply. This strike could significantly impact global semiconductor supply chains, as Samsung is a major memory chip manufacturer; any production disruption may exacerbate chip shortages and affect industries relying on memory components. The union demands a 7% base salary increase, removal of the performance bonus cap, and introduction of a profit-based bonus pool to close the pay gap with rival SK Hynix. Samsung has offered a 6.2% raise plus special bonuses for the memory chip division and expressed willingness to continue dialogue.

telegram · zaihuapd · Apr 24, 14:02

**Background**: Samsung Electronics is one of the world's largest semiconductor manufacturers, particularly in memory chips like DRAM and NAND flash. The Pyeongtaek plant is a key production facility. Since the AI boom in late 2022, SK Hynix has gained an edge in high-bandwidth memory (HBM) for AI chips, leading to better performance and higher bonuses for its workers, which has widened the pay gap between the two companies and fueled discontent among Samsung employees.

<details><summary>References</summary>
<ul>
<li><a href="https://hk.finance.yahoo.com/news/獎金僅sk海力士30-三星4萬員工氣炸喊罷工-產線恐停擺-004057735.html">獎金僅SK海力士30%！三星4萬員工氣炸喊罷工 產線恐停擺</a></li>
<li><a href="https://news.tvbs.com.tw/world/3186727">三星史上最大規模罷工！員工不滿待遇差距 破4萬人上街18天</a></li>
<li><a href="https://tech.ifeng.com/c/8sYl73iOPBJ">三星员工抗议与SK海力士存在巨大薪资差距，威胁将长期罢工</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#supply chain`, `#Samsung`, `#labor strike`, `#hardware`

---

<a id="item-12"></a>
## [Overthinking and scope creep sabotage projects](https://kevinlynagh.com/newsletter/2026_04_overthinking/) ⭐️ 7.0/10

Kevin Lynagh published an essay explaining how overthinking, scope creep, and structural diffing derail projects, using his own experience building kitchen bins as an example. This article resonates deeply with software engineers and researchers because it identifies a common, painful pattern that leads to wasted time and unfinished work, offering practical insights to avoid it. The author illustrates how the desire for a perfect design leads to endless iterations and scope creep, ultimately preventing project completion. He contrasts this with the concept of structural diffing, where comparing incremental changes can help maintain focus.

hackernews · alcazar · Apr 24, 14:28

**Background**: Scope creep refers to the uncontrolled expansion of a project's requirements beyond its original plan, often leading to delays and budget overruns. Structural diffing is a technique for comparing tree-shaped data structures, commonly used in version control to show meaningful changes in code rather than just line-by-line differences.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Diff">diff - Wikipedia</a></li>
<li><a href="https://tiniacoleyba.com/blog/scope-creep-in-software-3-concrete-examples/">Scope Creep in Software: 3 Concrete Examples - Tiniaco Leyba</a></li>
<li><a href="https://github.com/Wilfred/difftastic/wiki/Structural-Diffs">Structural Diffs · Wilfred/difftastic Wiki</a></li>

</ul>
</details>

**Discussion**: Commenters shared related experiences, with one noting that PhD research suffers from similar scope creep due to exhaustive literature review. Another quoted Obama's 'Better is good' to emphasize that small improvements compound over time, while a CEO remarked that teams rarely regret shipping early with a smaller scope.

**Tags**: `#software engineering`, `#project management`, `#productivity`, `#scope creep`, `#technical debt`

---

<a id="item-13"></a>
## [Honker Brings Postgres NOTIFY/LISTEN to SQLite](https://simonwillison.net/2026/Apr/24/honker/#atom-everything) ⭐️ 7.0/10

Honker is a new Rust-based SQLite extension that implements Postgres-style NOTIFY/LISTEN queue semantics, providing cross-process event notification and durable streaming with Python async bindings. This project fills a significant gap for SQLite-based applications that previously required external message brokers like Redis or Celery for background jobs and inter-process messaging, reducing operational complexity and eliminating dual-write bugs. The extension requires WAL mode and uses a stat call on the .db-wal file every 1ms for near-real-time polling without running a full SQL query. It also implements the transactional outbox pattern, ensuring items are only queued if the enclosing transaction commits successfully.

rss · Simon Willison · Apr 24, 01:50

**Background**: Postgres's NOTIFY and LISTEN commands allow database sessions to send and receive asynchronous notifications with optional payload strings, commonly used for building message queues and event-driven architectures. SQLite, while widely used for its simplicity and embedded nature, lacked this built-in publish-subscribe capability, forcing developers to rely on external services for similar functionality.

<details><summary>References</summary>
<ul>
<li><a href="https://byteiota.com/honker-postgres-notify-listen-for-sqlite/">Honker: Postgres NOTIFY/LISTEN for SQLite | byteiota</a></li>
<li><a href="https://news.ycombinator.com/item?id=47874647">Show HN: Honker – Postgres NOTIFY/LISTEN Semantics for SQLite ...</a></li>
<li><a href="https://thinhdanggroup.github.io/postgres-as-a-message-bus/">Postgres as a Message Bus: Implementing Durable Event Queues ...</a></li>

</ul>
</details>

**Discussion**: The creator noted on Hacker News that Honker delivers push-style event delivery with single-digit millisecond latency without requiring a separate daemon or broker, and that many high-traffic applications now run on a Framework+SQLite+Litestream stack, making this extension a natural fit.

**Tags**: `#SQLite`, `#Rust`, `#Python`, `#queues`, `#database`

---

<a id="item-14"></a>
## [Apple Requires USCI from App Store Developers in China](https://t.me/zaihuapd/41043) ⭐️ 7.0/10

Apple has begun requiring all App Store developers to provide their Unified Social Credit Code (USCI) for submission to Chinese tax authorities. This regulatory change directly affects all developers distributing apps on the China App Store, potentially impacting app availability and developer compliance costs. The Unified Social Credit Code is an 18-character alphanumeric identifier issued to registered organizations in China, used across tax, market regulation, and banking systems.

telegram · zaihuapd · Apr 24, 04:21

**Background**: The Unified Social Credit Code (USCC) is a mandatory identifier for all legal entities in China, combining business registration and tax identification into one code. Apple's move aligns with broader Chinese regulatory requirements for digital platforms to report developer tax information.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unified_Social_Credit_Identifier">Unified Social Credit Identifier - Wikipedia</a></li>
<li><a href="https://fdichina.com/blog/unified-social-credit-code-china/">Unified Social Credit Code : 5 Essential Facts and How to Verify It in...</a></li>
<li><a href="https://www.registrationchina.com/articles/unified-social-credit-code-uscc/">What is the Unified Social Credit Code in China</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#App Store`, `#China`, `#regulation`, `#developer`

---

<a id="item-15"></a>
## [US AI tool users show income stratification: Claude high, Meta AI low](https://epoch.ai/data-insights/service-by-income) ⭐️ 7.0/10

A combined analysis of three surveys conducted by Epoch AI and Ipsos from March to April 2026 reveals that weekly active users of major AI tools in the US are increasingly stratified by income: 79.8% of Claude users come from households earning over $100,000 per year, while only 36.5% of Meta AI users fall into that bracket. This income-based segmentation has significant implications for product positioning, accessibility, and market strategy, highlighting that different AI tools appeal to vastly different socioeconomic groups and potentially reinforcing digital inequality. Among Meta AI users, 32.1% come from households earning under $50,000 per year, compared to only 6.4% for Claude; ChatGPT, Gemini, Grok, and Copilot fall in between, with 55.9% to 63.7% of their users in the high-income bracket.

telegram · zaihuapd · Apr 24, 05:06

**Background**: The data comes from Epoch AI, a research organization tracking AI trends, and Ipsos, a global market research firm. The analysis is based on three surveys conducted in March-April 2026, covering weekly active users of major AI tools in the US. The overall US adult population has about 50% of individuals in households earning over $100,000 per year, serving as a baseline for comparison.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Epoch_AI">Epoch AI</a></li>
<li><a href="https://www.ipsos.com/en-us">Ipsos | Global Market Research and Public Opinion Specialist</a></li>

</ul>
</details>

**Tags**: `#AI tools`, `#user demographics`, `#income inequality`, `#market analysis`, `#Epoch AI`

---

<a id="item-16"></a>
## [Tesla Cybercab enters production in North America](https://weibo.com/3615027564/QCheybgVu) ⭐️ 7.0/10

Tesla has announced that its fully autonomous Cybercab, which lacks a steering wheel, pedals, and side mirrors, has started mass production in North America. The vehicle is designed exclusively for autonomous driving and robotaxi services, with onboard AI handling all driving tasks. This marks a significant milestone for autonomous driving and robotaxi services, as Cybercab represents a paradigm shift in vehicle design by removing traditional driver controls. It positions Tesla to advance its robotaxi network and could accelerate the commercialization of autonomous ride-hailing. The Cybercab is purpose-built for driverless operation, with a dedicated architecture and interaction system tailored for autonomous scenarios. Tesla first unveiled the Cybercab in October 2024, and Elon Musk had previously stated a goal of deploying 1 million autonomous taxis within a year.

telegram · zaihuapd · Apr 24, 08:26

**Background**: Robotaxis, or autonomous taxis, are self-driving vehicles that operate without a human driver, offering ride-hailing services through a network. Tesla has long pursued full self-driving (FSD) technology, and the Cybercab is its first production vehicle built specifically for this purpose, eliminating manual controls entirely.

<details><summary>References</summary>
<ul>
<li><a href="https://lifeofze.com/2024/10/16/tesla-introduce-robotaxi-cybercab/">完全 自 动 驾 驶 交通的时代来临， TESLA 揭开 ROBOTAXI CYBERCAB ...</a></li>
<li><a href="https://lovemandarinvoice.com/tesla-cybercab/">Tesla 发布完全 自 动 驾 驶 汽车 – Mandarin Voice</a></li>
<li><a href="https://auto123channel.com/2024/10/11/all-new-tesla-cybercab-official-debut/">售价 RM130,000！ 全新 Tesla Cybercab ...</a></li>

</ul>
</details>

**Tags**: `#autonomous driving`, `#Tesla`, `#robotaxi`, `#electric vehicles`, `#AI`

---

<a id="item-17"></a>
## [Android Verified Email Registration Eliminates OTPs](https://www.androidauthority.com/android-verified-email-no-magic-links-otps-3660150/) ⭐️ 7.0/10

Google has added a Verified Email feature to Android's Credential Manager API, enabling users to register for apps using cryptographically verified email credentials stored on their device, eliminating the need for OTPs or magic links. This streamlines the email-based registration and authentication process on Android, significantly improving user experience and security by removing the friction and phishing risks associated with OTPs and magic links. The feature currently supports only personal Gmail accounts; Workspace, managed accounts, and non-Gmail addresses may still require additional verification. It also supports account recovery and sensitive operation re-authentication, and requires Android 9+ with Google Play Services version 25.49.xx or higher.

telegram · zaihuapd · Apr 24, 12:33

**Background**: The Credential Manager API is Android's recommended Jetpack library for credential exchange, unifying support for passkeys, passwords, and federated sign-in. The Verified Email feature implements the W3C's Digital Credential API standard, issuing cryptographically verified email credentials directly to Android devices through this API.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.android.com/identity/credential-manager">About Credential Manager - Identity | Android Developers</a></li>
<li><a href="https://developers.google.com/identity/android-credential-manager">Android Credential Manager API - Google Developers</a></li>
<li><a href="https://android-developers.googleblog.com/2026/04/streamline-auth-credential-manager-verified-email.html">Streamline User Journeys with Verified Email via Credential ...</a></li>

</ul>
</details>

**Tags**: `#Android`, `#Authentication`, `#Credential Manager`, `#Google`, `#Security`

---