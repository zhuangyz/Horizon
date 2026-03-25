---
layout: default
title: "Horizon Summary: 2026-03-25 (EN)"
date: 2026-03-25
lang: en
---

> From 27 items, 12 important content pieces were selected

---

1. [Arm to sell its own designed chips for the first time, with Meta as first major customer and TSMC as manufacturer](#item-1) ⭐️ 9.0/10
2. [Swift 6.3 Released with Official Android SDK, Enabling Native Android App Development](#item-2) ⭐️ 9.0/10
3. [Apifox Desktop Client Compromised in Supply Chain Attack, Stealing SSH Keys and Git Credentials](#item-3) ⭐️ 9.0/10
4. [Google introduces TurboQuant for extreme KV cache compression in LLMs.](#item-4) ⭐️ 8.0/10
5. [OpenAI to Discontinue Sora AI Video Generator, Wind Down Disney Partnership](#item-5) ⭐️ 8.0/10
6. [Tencent Disbands AI Lab, Hires ByteDance Seed Team Leaders to Accelerate Hunyuan Model Upgrade](#item-6) ⭐️ 8.0/10
7. [NASA shifts from Lunar Gateway to focus on 2029 lunar base, accelerates nuclear propulsion](#item-7) ⭐️ 8.0/10
8. [China Computer Federation Opposes NeurIPS Sanctions Policy, Calls for Boycott](#item-8) ⭐️ 8.0/10
9. [OpenAI Shuts Down Sora AI Video Generation App](#item-9) ⭐️ 7.0/10
10. [Claude Code introduces auto mode as safer alternative to dangerous permission bypass](#item-10) ⭐️ 7.0/10
11. [Major package managers adopt dependency cooldown features to combat supply chain attacks.](#item-11) ⭐️ 7.0/10
12. [Claude Code Launches Auto Mode: AI Autonomous Decision-Making with Built-in Safety Review](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Arm to sell its own designed chips for the first time, with Meta as first major customer and TSMC as manufacturer](https://www.bloomberg.com/news/articles/2026-03-24/arm-to-sell-its-own-chips-for-first-time-in-bid-for-ai-revenue) ⭐️ 9.0/10

Arm Holdings announced it will for the first time sell its own designed chips, starting with a new high-core-count 'AGI CPU' targeting AI data center workloads. Meta Platforms is the first major customer for this chip, which features up to 136 cores, a 300-watt power envelope, and will be manufactured by TSMC. This marks a major strategic shift for Arm, moving from a pure intellectual property (IP) licensing model to directly competing in the chip sales market. It intensifies competition in the data center CPU space, particularly for AI workloads, and could reshape the dynamics between chip designers, foundries, and major cloud customers like Meta. The Arm AGI CPU is designed to work alongside accelerator chips from companies like Nvidia and claims superior energy efficiency compared to traditional CPU designs from Intel and AMD. Systems based on this chip are already available from OEMs like Quanta Computer and Supermicro, with volume availability expected to expand in the second half of 2026.

telegram · zaihuapd · Mar 25, 02:45

**Background**: Arm Holdings is a British company primarily known for designing the CPU architecture and licensing the intellectual property (IP) to other companies like Apple, Qualcomm, and Samsung, who then manufacture their own chips. The 'AGI CPU' is built on Arm's Neoverse V3 architecture, which is specifically designed for cloud and data center applications. TSMC (Taiwan Semiconductor Manufacturing Company) is the world's largest contract semiconductor manufacturer, producing chips for companies like Apple, Nvidia, and AMD.

<details><summary>References</summary>
<ul>
<li><a href="https://newsroom.arm.com/blog/introducing-arm-agi-cpu">Announcing Arm AGI CPU: The silicon foundation for the agentic AI cloud era - Arm Newsroom</a></li>
<li><a href="https://www.arm.com/products/cloud-datacenter/arm-agi-cpu">Arm AGI CPU – Arm®</a></li>
<li><a href="https://www.cnbc.com/2026/03/24/arm-launches-its-own-cpu-with-meta-as-first-customer.html">Arm launches its own CPU, with Meta as first customer</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#artificial-intelligence`, `#data-center`, `#hardware`, `#arm-architecture`

---

<a id="item-2"></a>
## [Swift 6.3 Released with Official Android SDK, Enabling Native Android App Development](https://swift.org/blog/swift-6.3-released/) ⭐️ 9.0/10

Swift 6.3 was officially released on March 25, 2026, and it includes the first official release of the Swift SDK for Android. This enables developers to write native Android applications using Swift or integrate Swift code into existing Kotlin/Java applications via the Swift Java interoperability plugin. This represents a major paradigm shift, significantly expanding Swift's ecosystem beyond Apple platforms and potentially reshaping cross-platform mobile development workflows. It allows iOS developers to leverage their Swift expertise for Android development, potentially increasing code reuse and reducing the barrier to entry for building apps on both major mobile platforms. The Swift Java plugin allows Swift programs to call Java libraries by wrapping Java classes in corresponding Swift types. Developers can start experimenting with the new capability by visiting the official 'Getting Started with the Swift SDK for Android' guide and exploring the swift-android-examples repository for sample projects.

telegram · zaihuapd · Mar 25, 03:45

**Background**: Swift is a general-purpose programming language developed by Apple, first released in 2014, and is the primary language for developing applications across Apple's platforms (iOS, macOS, watchOS, tvOS). Native Android development has traditionally been done using Java or Kotlin, with Kotlin being Google's preferred language since 2019. The concept of using Swift for Android has existed in community projects, but Swift 6.3 marks its first official, first-party support from the Swift project itself.

<details><summary>References</summary>
<ul>
<li><a href="https://www.swift.org/blog/swift-6.3-released/">Swift 6.3 Released | Swift .org</a></li>
<li><a href="https://github.com/swiftlang/swift-java">GitHub - swiftlang/swift-java: Java interopability support for Swift · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Swift_(programming_language)">Swift (programming language) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#swift`, `#android`, `#cross-platform`, `#mobile-development`, `#programming-languages`

---

<a id="item-3"></a>
## [Apifox Desktop Client Compromised in Supply Chain Attack, Stealing SSH Keys and Git Credentials](http://apifox.it.xn--comcdn-kr3e.openroute.xn--devupgrade-eh3i.feishu.it.com/) ⭐️ 9.0/10

The Apifox desktop client was compromised in a supply chain attack where attackers modified an event-tracking script on its CDN to inject malicious code. This code harvested sensitive data including SSH keys, Git credentials, shell history, and process lists from developers' machines, and could potentially deploy backdoors for lateral movement. This incident is significant because it directly targets developers using a popular API development tool, potentially compromising the security of countless software projects and their underlying infrastructure. It highlights the severe risks posed by supply chain attacks on developer tools, which can lead to widespread credential theft and unauthorized access to source code repositories and servers. The attack was active from March 4th and affected users on Windows, macOS, and Linux. Security researcher phith0n independently reverse-engineered the malicious payload and published analysis code. Users can check for compromise by looking for traces of the domain 'apifox.it.com' in specific local files, such as the 'Network Persistent State' file or LevelDB keys.

telegram · zaihuapd · Mar 25, 11:10

**Background**: A software supply chain attack involves injecting malicious code into a legitimate application or its update mechanism to infect all its users. SSH keys are cryptographic credentials used for secure remote access to servers and systems. Git credentials are used to authenticate with version control systems like GitHub or GitLab. LevelDB is a fast key-value storage library often used by applications to store local data, and the malicious script in this attack searched within its structure for sensitive information.

<details><summary>References</summary>
<ul>
<li><a href="https://www.crowdstrike.com/en-us/cybersecurity-101/cyberattacks/supply-chain-attack/">What Is a Supply Chain Attack? - CrowdStrike</a></li>
<li><a href="https://martin.kleppmann.com/2013/05/24/improving-security-of-ssh-private-keys.html">Improving the security of your SSH private key files — Martin Kleppmann’s blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/LevelDB">LevelDB - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#security`, `#supply-chain-attack`, `#api-tools`, `#developer-tools`, `#incident-response`

---

<a id="item-4"></a>
## [Google introduces TurboQuant for extreme KV cache compression in LLMs.](https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/) ⭐️ 8.0/10

Google Research has introduced TurboQuant, a new method that combines random rotation and quantization to compress the KV cache in Large Language Models (LLMs) down to 3 bits without retraining. The technique, along with related methods QJL and PolarQuant, was announced in a blog post and will be presented at ICLR 2026 and AISTATS 2026. This matters because the KV cache is a major memory bottleneck during LLM inference, especially for long-context tasks, limiting model deployment and efficiency. By drastically reducing KV cache memory usage (e.g., by 6x or more), TurboQuant can enable longer context windows, higher throughput, and lower-cost inference, making advanced LLMs more accessible. In tests, 4-bit TurboQuant achieved up to an 8x speedup in computing attention logits on H100 GPUs compared to 32-bit unquantized keys. The method also outperformed existing techniques like PQ and RabbiQ in high-dimensional vector search recall, and it maintained downstream task performance in long-context 'needle-in-a-haystack' evaluations.

hackernews · ray__ · Mar 25, 05:00

**Background**: During inference, LLMs store past Key (K) and Value (V) vectors from the attention mechanism in a 'KV cache' to avoid recomputation, but this cache consumes significant memory, scaling with context length. KV cache compression techniques aim to reduce this memory footprint to improve inference efficiency. Quantization is a common compression method that reduces the numerical precision (e.g., from 32 bits to 4 bits) of these stored vectors.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2508.06297v1">KV Cache Compression for Inference Efficiency in LLMs: A Review</a></li>
<li><a href="https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/">TurboQuant: Redefining AI efficiency with extreme compression</a></li>

</ul>
</details>

**Discussion**: The community shows active technical engagement, with one user noting a potential missing citation for a foundational rotation technique. Another user requests a simpler explanation of the random rotation concept, while others highlight rapid independent implementations in llama.cpp and PyTorch. A separate comment criticizes the blog post's explanation as unclear for a lay audience.

**Tags**: `#AI Efficiency`, `#Model Compression`, `#KV Cache`, `#LLM Inference`, `#Quantization`

---

<a id="item-5"></a>
## [OpenAI to Discontinue Sora AI Video Generator, Wind Down Disney Partnership](https://www.bloomberg.com/news/articles/2026-03-24/openai-plans-to-discontinue-support-for-sora-ai-video-generator?srnd=phx-technology) ⭐️ 8.0/10

OpenAI plans to discontinue its Sora AI video generator application and its developer API, roughly six months after the app's high-profile launch. The company is also winding down its partnership with Disney related to Sora, reallocating resources toward AI agents and a new model codenamed 'Spud'. This decision signals a significant strategic pivot for a leading AI company, moving away from a flagship generative video product to focus on autonomous AI agents and next-generation foundation models. It highlights the intense competition and rapid evolution in the AI industry, where even high-profile products can be short-lived as companies chase new technological frontiers. The discontinuation is part of a broader effort to streamline OpenAI's product lineup. Concurrently, the company is restructuring some safety and security teams to integrate their work more closely into the development process for its new priorities.

telegram · zaihuapd · Mar 25, 00:30

**Background**: Sora is a text-to-video model and app developed by OpenAI that generates short, realistic video clips from text prompts. AI agents, like OpenAI's Codex, are systems designed to autonomously accomplish complex tasks, such as software engineering. The new model 'Spud' represents OpenAI's next major AI initiative, with CEO Sam Altman suggesting it could have significant economic impact.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sora_(text-to-video_model)">Sora (text-to- video model) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://www.theinformation.com/articles/openai-ceo-shifts-responsibilities-preps-spud-ai-model">OpenAI CEO Shifts Responsibilities, Preps ‘Spud’ AI Model</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI-Strategy`, `#Video-Generation`, `#Product-Discontinuation`, `#Industry-News`

---

<a id="item-6"></a>
## [Tencent Disbands AI Lab, Hires ByteDance Seed Team Leaders to Accelerate Hunyuan Model Upgrade](https://mp.weixin.qq.com/s/24ZWs8JFP6seQSSIhU6mOw) ⭐️ 8.0/10

Tencent has officially disbanded its AI Lab and reorganized its large model R&D system, while simultaneously hiring multiple key technical leaders from ByteDance's Seed team. The company plans to release a new generation of its Hunyuan foundational model in April 2026. This move signals a major strategic pivot for Tencent, consolidating its AI research efforts towards a more product-oriented, large-model-centric approach to compete in China's intensifying generative AI race. The talent acquisition from a key competitor like ByteDance's advanced Seed team represents a direct effort to rapidly bolster its technical capabilities and infrastructure. Key hires include Xiao Xuefeng, former head of ByteDance Seed's visual AI platform team, who is now assistant head of Tencent's AI Infra department, and Huang Qi, who leads the training Infra group. The reorganization also involved transferring some former AI Lab personnel to the Large Language Model department.

telegram · zaihuapd · Mar 25, 03:00

**Background**: Tencent's Hunyuan is a proprietary, trillion-parameter large language model based on the Transformer architecture, first unveiled in September 2023. ByteDance's Seed team, established in 2023, is dedicated to pushing the boundaries of general AI, with research spanning LLMs, vision, speech, and AI infrastructure. An 'AI Infra' department typically focuses on the underlying computational systems, tools, and platforms needed to develop and deploy AI models at scale.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tencent.com/en-us/articles/2201685.html">Tencent Unveils Hunyuan, its Proprietary Large Foundation ...</a></li>
<li><a href="https://seed.bytedance.com/en/">ByteDance Seed</a></li>

</ul>
</details>

**Tags**: `#AI-Industry`, `#Organizational-Strategy`, `#Large-Language-Models`, `#Tencent`, `#Talent-Mobility`

---

<a id="item-7"></a>
## [NASA shifts from Lunar Gateway to focus on 2029 lunar base, accelerates nuclear propulsion](https://www.nasa.gov/news-release/nasa-unveils-initiatives-to-achieve-americas-national-space-policy/) ⭐️ 8.0/10

NASA has announced a strategic shift, pausing development of the Lunar Gateway orbital station to prioritize establishing a permanent lunar surface base by 2029. The agency also plans to launch its first nuclear-powered interplanetary spacecraft, Space Reactor-1 Freedom, to Mars by 2028 to demonstrate nuclear electric propulsion technology. This represents a major reallocation of resources within NASA's Artemis program, moving from an orbital staging post to direct, sustained surface operations, which could accelerate the timeline for establishing a long-term human presence on the Moon. The parallel push for nuclear propulsion is critical for enabling faster and more capable crewed missions to Mars, marking a significant technological leap for deep space exploration. The new plan aims for at least one lunar landing per year initially, with the goal of increasing to crewed missions every six months after the Artemis V mission, leveraging more commercial partnerships and reusable hardware. NASA also expects to conduct 30 robotic lunar landings starting in 2027 through its Commercial Lunar Payload Services program.

telegram · zaihuapd · Mar 25, 04:30

**Background**: The Lunar Gateway was a planned small space station in orbit around the Moon, intended to serve as a staging point for astronauts traveling to the lunar surface under the Artemis program. The Artemis program is NASA's flagship Moon exploration initiative, formally established in 2017, with the goal of returning humans to the Moon and eventually sending crewed missions to Mars. Nuclear Electric Propulsion (NEP) is a technology that uses a nuclear reactor to generate electricity, which then powers highly efficient electric thrusters, offering much greater efficiency and mission flexibility compared to traditional chemical rockets for deep space travel.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lunar_Gateway">Lunar Gateway - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artemis_program">Artemis program - Wikipedia</a></li>
<li><a href="https://www.insightsonindia.com/2026/03/25/space-reactor-1-sr-1-freedom-spacecraft/">NASA Space Reactor 1 Freedom : Nuclear Spacecraft & Mars Mission...</a></li>

</ul>
</details>

**Tags**: `#space-exploration`, `#nasa`, `#lunar-base`, `#nuclear-propulsion`, `#artemis-program`

---

<a id="item-8"></a>
## [China Computer Federation Opposes NeurIPS Sanctions Policy, Calls for Boycott](https://www.ccf.org.cn/Focus/2026-03-25/865918.shtml) ⭐️ 8.0/10

The China Computer Federation (CCF) issued a formal statement on March 25, 2026, strongly opposing NeurIPS 2026's policy of prohibiting submissions from institutions on US sanctions lists. The CCF called on Chinese researchers to boycott the conference by refusing to submit papers or provide academic services, and threatened to remove NeurIPS from its prestigious Recommended Conference List if the policy is not revoked. This represents a major escalation in the politicization of global AI research, as a leading national academic body directly challenges the policies of a top-tier conference. The CCF's recommended list significantly influences Chinese researchers' publication choices and career evaluations, so its potential delisting of NeurIPS could drastically reshape participation patterns and collaboration networks in one of the world's largest AI research communities. The controversy stems from NeurIPS 2026's explicit prohibition of submissions from "certain organizations on US sanctions lists" in its official submission guidelines. The CCF's threat to delist NeurIPS is particularly consequential because its Recommended Conference List is a widely recognized benchmark in China for evaluating research impact and academic reputation.

telegram · zaihuapd · Mar 25, 14:07

**Background**: NeurIPS (Conference on Neural Information Processing Systems) is one of the world's most prestigious annual conferences in artificial intelligence and machine learning. The CCF Recommended International Academic Conference and Journal Directory is a highly influential ranking system within China's computer science community, guiding researchers on where to publish and affecting institutional evaluations. US sanctions lists, such as the Department of Commerce's Entity List, include foreign universities and research institutions subject to export controls and restrictions, which are now being extended to academic conference participation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Neural_Information_Processing_Systems">Conference on Neural Information Processing Systems - Wikipedia</a></li>
<li><a href="https://www.iconf.com/news/820">CCF Recommended Conference List and How to Understand Computer Science Conference Rankings丨ICONF</a></li>
<li><a href="https://researchpolicy.caltech.edu/research-security/export-compliance/restricted-party-screening/foreign-universities-sanctioned-by-the-us-government">Foreign Universities Sanctioned by the U.S. Government</a></li>

</ul>
</details>

**Tags**: `#academic-policy`, `#ai-research`, `#geopolitics`, `#research-ethics`, `#conferences`

---

<a id="item-9"></a>
## [OpenAI Shuts Down Sora AI Video Generation App](https://twitter.com/soraofficialapp/status/2036532795984715896) ⭐️ 7.0/10

OpenAI is shutting down its Sora AI video generation app, which was launched to significant initial excitement. The decision comes after the app failed to retain users beyond a short period of novelty-driven engagement. This shutdown highlights the challenges even leading AI companies face in achieving product-market fit and sustaining user engagement beyond initial hype. It signals a potential shift in OpenAI's product strategy, moving away from standalone consumer apps that rely on novelty and towards more integrated or utility-focused offerings. The shutdown announcement came shortly after OpenAI published a primer on Sora safeguards, suggesting either a lack of internal communication or a sudden strategic pivot. The app reportedly struggled with user retention, as many users, after an initial burst of creative activity, found no compelling reason to return regularly.

hackernews · mikeocool · Mar 24, 20:01

**Background**: Sora was an AI model and app developed by OpenAI capable of generating short, realistic videos from text prompts. It was part of a wave of generative AI tools moving beyond static images into dynamic video content. The app allowed users to create and share these AI-generated videos, positioning itself as a platform for creative expression.

**Discussion**: Community sentiment is mixed, with users sharing personal experiences and strategic critiques. Some users, like meken, fondly recalled the initial creative joy but confirmed the novelty wore off quickly, leading to abandonment. Others, like johnfn, criticized Sora for lacking the utility and respect for user time found in OpenAI's other products like GPT. Commenters also noted the awkward timing of the shutdown relative to recent safety publications and questioned the app's core value proposition of a dedicated AI video feed.

**Tags**: `#AI`, `#OpenAI`, `#product-strategy`, `#video-generation`, `#startup-failure`

---

<a id="item-10"></a>
## [Claude Code introduces auto mode as safer alternative to dangerous permission bypass](https://simonwillison.net/2026/Mar/24/auto-mode-for-claude-code/#atom-everything) ⭐️ 7.0/10

Anthropic has introduced auto mode for Claude Code, a new permissions mode where Claude makes permission decisions on behalf of users with safeguards monitoring actions before execution. This mode uses Claude Sonnet 4.6 as a classifier model to review conversations and block potentially harmful actions that escalate beyond task scope, target untrusted infrastructure, or appear driven by hostile content. This development is significant because it provides a safer alternative to the --dangerously-skip-permissions flag, which allowed fully unattended execution without safeguards. Auto mode represents an important advancement in AI-assisted coding security by introducing automated permission decisions with built-in safety checks, potentially reducing risks of destructive actions, supply chain attacks, and unauthorized system modifications. The auto mode includes extensive default filters covering areas like test artifacts, local operations within project scope, read-only operations, and declared dependencies, while blocking actions like force pushing to Git, pushing directly to default branches, and executing code from external sources. Users can view the complete default rules by running 'claude auto-mode defaults' and can customize these filters with their own rules for specific security requirements.

rss · Simon Willison · Mar 24, 23:57

**Background**: Claude Code is an AI-assisted coding tool that previously included a --dangerously-skip-permissions flag enabling 'Safe YOLO mode' where the system bypassed all permission prompts for uninterrupted execution. Claude Sonnet 4.6 is Anthropic's latest Sonnet model with enhanced capabilities across coding, computer use, long-context reasoning, and agent planning, supporting a 1M token context window. AI-generated code security has become increasingly important as studies have shown vulnerabilities can emerge in both human-written and AI-generated code, necessitating better safeguards in development workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-sonnet-4-6">Introducing Claude Sonnet 4.6</a></li>
<li><a href="https://blog.promptlayer.com/claude-dangerously-skip-permissions/">claude -- dangerously - skip - permissions</a></li>
<li><a href="https://link.springer.com/article/10.1007/s10664-024-10590-1">How secure is AI-generated code: a large-scale comparison of ...</a></li>

</ul>
</details>

**Tags**: `#AI-assisted-coding`, `#developer-tools`, `#code-security`, `#claude-ai`, `#permissions`

---

<a id="item-11"></a>
## [Major package managers adopt dependency cooldown features to combat supply chain attacks.](https://simonwillison.net/2026/Mar/24/package-managers-need-to-cool-down/#atom-everything) ⭐️ 7.0/10

A recent analysis, prompted by the March 2026 LiteLLM supply chain attack, reveals that a majority of major package managers have now implemented dependency cooldown mechanisms. These include pnpm (10.16), Yarn (4.10.0), Bun (1.3), Deno (2.6), uv (0.9.17), pip (26.0), and npm (11.10.0), which all added features in late 2025 and early 2026 to delay the installation of newly published packages. This widespread adoption represents a significant shift in software supply chain security, moving from reactive detection to proactive delay as a defense. By giving the community time to scrutinize new releases, these cooldowns can block a high percentage of supply chain attacks, as evidenced by research suggesting a 7-day cooldown can prevent 80% of such incidents. Implementation details vary: most tools use settings like `minimumReleaseAge` or `--exclude-newer` to specify a delay period (e.g., 7 days), and many offer exemptions for trusted packages. A notable limitation is that pip 26.0 currently only supports absolute timestamps for its `--uploaded-prior-to` flag, requiring a workaround for relative durations.

rss · Simon Willison · Mar 24, 21:11

**Background**: A dependency cooldown is a security practice that intentionally delays the installation of a newly published software package version for a set period (e.g., 24 hours to 7 days). This creates a window where the package is public but not automatically adopted, allowing security researchers and automated tools time to detect if it contains malicious code introduced via a supply chain attack. Supply chain attacks target the software development and distribution process, often by compromising a legitimate package's publisher account or build system to inject malware that then spreads to all downstream users.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.yossarian.net/2025/11/21/We-should-all-be-using-dependency-cooldowns">We should all be using dependency cooldowns - blog.yossarian.net</a></li>
<li><a href="https://christian-schneider.net/blog/dependency-cooldowns-supply-chain-defense/">Dependency cooldowns: a simple supply chain fix</a></li>
<li><a href="https://securitylabs.datadoghq.com/articles/litellm-compromised-pypi-teampcp-supply-chain-campaign/">LiteLLM compromised on PyPI: Tracing the March 2026 TeamPCP...</a></li>

</ul>
</details>

**Tags**: `#package-management`, `#security`, `#supply-chain`, `#devops`, `#software-engineering`

---

<a id="item-12"></a>
## [Claude Code Launches Auto Mode: AI Autonomous Decision-Making with Built-in Safety Review](https://claude.com/blog/auto-mode) ⭐️ 7.0/10

Anthropic has introduced 'Auto Mode' for Claude Code, a feature that allows the AI to autonomously decide permissions during task execution. This mode uses safety classifiers to review each tool call before execution, automatically approving safe actions while blocking high-risk operations like mass file deletion or sensitive data exfiltration. This represents a significant advancement in AI-assisted coding by striking a balance between workflow efficiency and safety. It enables developers to run longer, more complex tasks with fewer manual interruptions, while mitigating the severe risks associated with completely disabling permission checks, which could lead to catastrophic errors. The feature is currently available in research preview for Team plan users and will roll out to Enterprise and API users in the coming days, supporting the Claude Sonnet 4.6 and Opus 4.6 models. While safer than the `--dangerously-skip-permissions` flag, Anthropic cautions that Auto Mode is not zero-risk, recommends use in isolated environments, and notes it may slightly increase token consumption and latency.

telegram · zaihuapd · Mar 25, 01:15

**Background**: Claude Code is an AI-powered coding assistant developed by Anthropic. Previously, users faced a trade-off: either approve every action manually, which interrupts workflow, or use the `--dangerously-skip-permissions` flag, which grants the AI unrestricted access to the file system, shell commands, and network operations, posing significant security risks. Auto Mode introduces an intermediate, classifier-driven layer to automate safe decisions while blocking dangerous ones.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/blog/auto-mode">Auto mode for Claude Code | Claude</a></li>
<li><a href="https://www.zdnet.com/article/claude-code-auto-mode/">How Claude Code's new auto mode prevents AI coding disasters - without slowing you down | ZDNET</a></li>
<li><a href="https://aiwiki.ai/wiki/Claude_--dangerously-skip-permissions">Claude --dangerously-skip-permissions - AI Wiki - Artificial Intelligence Wiki</a></li>

</ul>
</details>

**Tags**: `#AI-Assisted Coding`, `#Developer Tools`, `#AI Safety`, `#Claude`, `#Automation`

---