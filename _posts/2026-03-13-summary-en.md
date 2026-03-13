---
layout: default
title: "Horizon Summary: 2026-03-13 (EN)"
date: 2026-03-13
lang: en
---

> From 26 items, 9 important content pieces were selected

---

1. [ByteDance Plans Overseas Deployment of 36,000 Nvidia B200 Chips to Accelerate AI Research](#item-1) ⭐️ 9.0/10
2. [Investigation reveals $2B in grants and 45-state lobbying behind age-verification bills](#item-2) ⭐️ 8.0/10
3. [Shopify CEO uses AI autoresearch to make Liquid template engine 53% faster](#item-3) ⭐️ 8.0/10
4. [AI's Transformative Impact on Software Development Explored in Major NYT Feature](#item-4) ⭐️ 8.0/10
5. [Shanghai's First Brain-Computer Interface Surgery Enables Paralyzed Patient to Drink Water via Thought-Controlled Robotic Glove](#item-5) ⭐️ 8.0/10
6. [AWS S3 policy change eliminates bucketsquatting vulnerability](#item-6) ⭐️ 7.0/10
7. [AI-assisted coding reveals a pre-existing divide between craftsmanship-focused and outcome-focused developers.](#item-7) ⭐️ 7.0/10
8. [Apple May Globally Reduce App Store Commission from 30% to 20%](#item-8) ⭐️ 7.0/10
9. [Research: Alipay DeepLink with JSBridge could leak personal data via external pages](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [ByteDance Plans Overseas Deployment of 36,000 Nvidia B200 Chips to Accelerate AI Research](https://www.wsj.com/tech/chinas-bytedance-gets-access-to-top-nvidia-ai-chips-d68bce3a) ⭐️ 9.0/10

According to The Wall Street Journal, ByteDance is partnering with Southeast Asian cloud provider Aolani Cloud to deploy approximately 500 Nvidia Blackwell computing systems, totaling about 36,000 B200 chips, in Malaysia, with hardware investment potentially exceeding $2.5 billion. ByteDance plans to use this computing power for overseas AI research and to support its global AI service demands. This massive deployment represents a strategic move by a leading Chinese tech company to secure cutting-edge AI hardware outside of U.S. export restriction zones, directly fueling the global AI arms race. The scale of investment underscores the critical importance of advanced compute infrastructure for developing and deploying next-generation AI models and services at a global level. The deployment involves Nvidia's next-generation Blackwell platform, with the B200 chip reportedly consuming up to 1200W of power, significantly more than its predecessor, the H100. The partnership with Aolani Cloud, which specializes in AI-centric cloud infrastructure, facilitates this deployment in Malaysia, a location not subject to the same U.S. export controls as mainland China.

telegram · zaihuapd · Mar 13, 08:45

**Background**: Nvidia's Blackwell is a GPU microarchitecture and computing platform designed as the successor to the Hopper architecture, powering chips like the B200. It is engineered for massive-scale AI workloads, particularly for training and running trillion-parameter large language models (LLMs). U.S. export restrictions have limited the sale of Nvidia's most advanced AI chips, like the H100 and newer models, to companies in China, prompting firms to seek alternative deployment strategies overseas.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://www.tweaktown.com/news/97059/nvidias-full-spec-blackwell-b200-ai-gpu-uses-1200w-of-power-up-from-700w-on-hopper-h100/index.html">NVIDIA 's full- spec Blackwell B 200 AI GPU uses 1200W of power, up...</a></li>
<li><a href="https://www.aolanicloud.com/">AOLANI</a></li>

</ul>
</details>

**Tags**: `#AI Infrastructure`, `#NVIDIA`, `#ByteDance`, `#High-Performance Computing`, `#Geopolitics`

---

<a id="item-2"></a>
## [Investigation reveals $2B in grants and 45-state lobbying behind age-verification bills](https://old.reddit.com/r/linux/comments/1rshc1f/i_traced_2_billion_in_nonprofit_grants_and_45/) ⭐️ 8.0/10

An investigation traced over $2 billion in nonprofit grants and coordinated lobbying efforts across 45 U.S. states that are pushing for age-verification legislation. The analysis found that these bills, often based on copy-pasted templates, are being promoted to establish a broader digital surveillance infrastructure. This matters because these bills, framed as child protection measures, could mandate operating systems and app stores to create pervasive age-bracketing and identity verification systems. This establishes the technical and legal groundwork for mass surveillance, fundamentally reshaping online anonymity and privacy for all users. The investigation notes that the bill texts are often identical, sourced from just two primary templates, suggesting a highly coordinated push. One key template, the "App Store Accountability Act," specifically requires app stores to verify user ages and share that data with developers.

hackernews · shaicoleman · Mar 13, 10:15

**Background**: Age-verification laws require digital platforms to confirm a user's age, often through government ID or biometric data. Proponents argue they protect children online, but critics warn they create "digital public infrastructure" that can enable pervasive surveillance. Similar systems, like digital IDs linked to biometrics, have raised significant privacy and human rights concerns globally by enabling comprehensive tracking of populations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eff.org/deeplinks/2026/03/ab-1043s-internet-age-gates-hurt-everyone">A.B. 1043's Internet Age Gates Hurt Everyone - EFF.org</a></li>
<li><a href="https://en.wikipedia.org/wiki/Digital_public_infrastructure">Digital public infrastructure - Wikipedia</a></li>
<li><a href="https://www.accessnow.org/guide/digital-public-infrastructure/">Digital public infrastructure: policy recommendations</a></li>

</ul>
</details>

**Discussion**: Community comments express deep concern that age verification is a "trojan horse" for building a pervasive surveillance infrastructure, with one user noting it creates OS-level signals about identity. Others point to technical resistance projects and legal risks, such as potential CFAA liability for users who falsify age. There is also criticism of the lobbying process and advocacy for privacy-preserving alternatives like zero-knowledge proofs.

**Tags**: `#privacy`, `#policy`, `#surveillance`, `#lobbying`, `#digital-rights`

---

<a id="item-3"></a>
## [Shopify CEO uses AI autoresearch to make Liquid template engine 53% faster](https://simonwillison.net/2026/Mar/13/liquid/#atom-everything) ⭐️ 8.0/10

Shopify CEO Tobias Lütke submitted a pull request to the Liquid Ruby template engine repository, achieving a 53% faster parse and render time and 61% fewer memory allocations. He accomplished this by using a variant of Andrej Karpathy's 'autoresearch' AI system, which ran approximately 120 automated experiments over two days to identify dozens of micro-optimizations. This demonstrates a novel, practical application of AI-powered research agents for performance optimization in mature, widely-used open-source software. It highlights how AI can systematically uncover significant gains in codebases that have already been refined by human developers over many years, potentially setting a new standard for software optimization workflows. Key optimizations included replacing the StringScanner tokenizer with `String#byteindex` (reducing parse time by ~12%), implementing a pure-byte `parse_tag_token` to eliminate costly resets, and caching `to_s` results for small integers. The success of this effort was heavily dependent on Liquid's existing robust test suite of 974 unit tests, which provided a reliable benchmark for the AI agent.

rss · Simon Willison · Mar 13, 03:44

**Background**: Liquid is an open-source template engine written in Ruby, originally created by Tobias Lütke in 2005 and inspired by Django templates. It is widely used, most notably as the core templating language for Shopify themes. 'Autoresearch' is an open-source system recently released by AI researcher Andrej Karpathy; it enables AI coding agents to autonomously design and run hundreds of experiments to find effective techniques, originally conceived for optimizing AI model training.

<details><summary>References</summary>
<ul>
<li><a href="https://kenhuangus.substack.com/p/exploring-andrej-karpathys-autoresearch">Exploring Andrej Karpathy's Autoresearch: AI Agents Driving Autonomous ML Experimentation</a></li>
<li><a href="https://shopify.dev/docs/api/liquid">Liquid reference - Shopify Dev Docs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Program_optimization">Program optimization - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#performance`, `#ai-tools`, `#open-source`, `#ruby`, `#optimization`

---

<a id="item-4"></a>
## [AI's Transformative Impact on Software Development Explored in Major NYT Feature](https://simonwillison.net/2026/Mar/12/coding-after-coders/#atom-everything) ⭐️ 8.0/10

The New York Times Magazine published a major feature article titled 'Coding After Coders,' based on interviews with over 70 software developers from companies like Google, Amazon, Microsoft, and Apple. The article explores how AI tools like Claude and ChatGPT are fundamentally changing software development practices and the programming profession. This matters because it represents a mainstream examination of AI's profound impact on one of the core technology professions, signaling a potential industry-wide shift in how software is created. The perspectives from major tech companies and influential developers provide authoritative insight into whether AI will augment or replace human programmers, with implications for education, hiring, and the future of technical work. A key insight from the article is that programming may be uniquely resilient to AI 'hallucination' problems because code can be automatically tested for correctness, unlike outputs in fields like law. However, an anonymous Apple engineer expressed concern that AI automation strips away the 'fun and fulfilling' aspect of hand-crafting code, highlighting a potential cultural loss.

rss · Simon Willison · Mar 12, 19:23

**Background**: AI-assisted development tools, such as GitHub Copilot, Amazon CodeWhisperer, Cursor, and Claude Code, leverage large language models (LLMs) to help with code completion, debugging, and even generating entire applications from prompts. These tools are becoming integral to modern IDEs (Integrated Development Environments). A significant challenge with these AI coding assistants is 'hallucination,' where they generate plausible-sounding but incorrect or nonsensical code, which developers must vigilantly review and test.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/jamesmurdza/awesome-ai-devtools">Awesome AI-powered developer tools - GitHub 22 Best AI Coding Tools to Speed Up Development in 2026 Top Stories News about Oracle Corporation, New product development, SoundHound News about Tom Cruise, Tencent, Film industry Also in the news AI for Software Development: 27 Best Tools [2025] AI-assisted Software Development: Developer's Guide | Sonar 10 Best AI Tools for Developers 2026 (Compared) - Codeless Best AI -Powered IDEs and Coding Assistants in 2025 Awesome AI -powered developer tools - GitHub AI for Software Development : 27 Best Tools [2025] Best AI-Powered IDEs and Coding Assistants in 2025</a></li>
<li><a href="https://www.infoworld.com/article/3822251/how-to-keep-ai-hallucinations-out-of-your-code.html">How to keep AI hallucinations out of your code | InfoWorld</a></li>
<li><a href="https://playcode.io/blog/chatgpt-vs-claude-vs-gemini-coding-2026">ChatGPT vs Claude vs Gemini for Coding 2026 (Honest Comparison) | PlayCode Blog</a></li>

</ul>
</details>

**Tags**: `#AI-assisted-development`, `#software-engineering-future`, `#programming-tools`, `#industry-trends`

---

<a id="item-5"></a>
## [Shanghai's First Brain-Computer Interface Surgery Enables Paralyzed Patient to Drink Water via Thought-Controlled Robotic Glove](https://t.me/zaihuapd/40242) ⭐️ 8.0/10

At the World Brain-Computer Interface Joint Conference, Professor Mao Ying from Huashan Hospital disclosed that a patient paralyzed for four years after a car accident successfully drank water using a thought-controlled robotic glove. This was enabled by a coin-sized brain-computer interface (BCI) implant that captures neural signals from the sensorimotor cortex, with the surgery time significantly reduced through the use of intraoperative functional localization techniques. This represents a significant clinical milestone in translating BCI technology from the lab to real-world functional restoration for paralyzed individuals. The successful demonstration of performing an activity of daily living (drinking) highlights the potential of BCIs to dramatically improve independence and quality of life for people with severe motor disabilities. The BCI system consists of an internal implant and an external device, including the robotic glove. The intraoperative functional localization technique, which involves mapping critical brain areas during surgery, was key to reducing operative time and potentially improving surgical precision and safety.

telegram · zaihuapd · Mar 13, 09:30

**Background**: A brain-computer interface (BCI) is a system that creates a direct communication pathway between the brain and an external device, bypassing the body's normal neuromuscular output channels. For patients with spinal cord injuries or neurological disorders, BCIs aim to restore lost functions, such as movement, by interpreting neural signals to control assistive devices like robotic limbs or exoskeletons. Intraoperative functional localization is a neurosurgical technique used to identify and preserve eloquent brain areas (like those controlling movement or sensation) during operations, often using methods like electrocortical stimulation to map the cortex in real-time.

<details><summary>References</summary>
<ul>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC8275018/">New Techniques in Intraoperative Brain Mapping - PMC</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S2667325824001559">Signal acquisition of brain–computer interfaces: A medical ...</a></li>
<li><a href="https://link.springer.com/article/10.1007/s40747-023-01246-6">Assist -as-needed control with a soft robotic glove based on...</a></li>

</ul>
</details>

**Tags**: `#brain-computer interface`, `#medical robotics`, `#neurotechnology`, `#assistive technology`, `#neurosurgery`

---

<a id="item-6"></a>
## [AWS S3 policy change eliminates bucketsquatting vulnerability](https://onecloudplease.com/blog/bucketsquatting-is-finally-dead) ⭐️ 7.0/10

AWS recently changed its S3 bucket naming policies, effectively eliminating the practice of 'bucketsquatting' where attackers could claim bucket names that organizations might use in the future. This change makes S3 bucket names globally unique across all AWS accounts, preventing name collisions and squatting attacks. This is significant because bucketsquatting was a real cloud security threat where attackers could intercept traffic or deploy phishing sites by claiming bucket names that organizations might logically use. The resolution of this vulnerability improves the overall security posture of AWS S3 users and reduces a common attack vector in cloud infrastructure. The new policy ensures bucket name uniqueness across the entire AWS ecosystem, not just within individual accounts. While this solves the bucketsquatting problem for S3, similar naming vulnerabilities may still exist in other cloud services like Azure Storage Accounts, which also use globally unique names.

hackernews · boyter · Mar 13, 08:31

**Background**: Bucketsquatting is a cloud security attack where malicious actors register cloud resource names (like S3 bucket names) that legitimate organizations are likely to use in the future. AWS S3 buckets are object storage containers that require globally unique names across all AWS customers. Before this policy change, attackers could claim these names proactively, then potentially intercept traffic or conduct phishing when organizations eventually tried to use those logical names.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucketnamingrules.html">General purpose bucket naming rules - docs.aws.amazon.com</a></li>
<li><a href="https://cloud.google.com/transform/how-to-combat-bucket-squatting-in-five-steps">How to combat bucket squatting in five steps - Google Cloud</a></li>
<li><a href="https://gibraltarsolutions.com/blog/cloud-squatting/">Cloud Squatting: A Deep Dive into the Stealthy Cloud Threat</a></li>

</ul>
</details>

**Discussion**: The community discussion expanded beyond S3 to broader naming system issues across cloud platforms. Commenters noted similar problems with Azure Storage Account names and AWS account root user emails, which cannot be reused after deletion. Some suggested adopting Discord-like naming schemes with random suffixes to democratize namespace ownership and prevent squatting, while others welcomed the change as a good hygiene practice that infrastructure-as-code tools should adopt by default.

**Tags**: `#cloud-security`, `#aws-s3`, `#naming-systems`, `#infrastructure`, `#cybersecurity`

---

<a id="item-7"></a>
## [AI-assisted coding reveals a pre-existing divide between craftsmanship-focused and outcome-focused developers.](https://simonwillison.net/2026/Mar/12/les-orchard/#atom-everything) ⭐️ 7.0/10

Les Orchard, in a blog post titled "Grief and the AI Split," argues that AI-assisted coding tools are making a previously hidden divide among developers visible. The divide is between those who are motivated by the craft of hand-coding and those primarily focused on practical outcomes, a difference that was less apparent when all developers wrote code manually. This matters because it highlights a potential cultural and motivational schism in software engineering as AI tools become mainstream. Understanding this divide is crucial for teams, managers, and educators to navigate conflicts, structure workflows, and support developers with different values in an AI-augmented future. Orchard notes that before AI, both camps used the same tools and processes, making their differing motivations invisible. The key change is that AI presents a "fork in the road," forcing a visible choice between letting the machine generate code or insisting on hand-crafting it, thereby revealing underlying values.

rss · Simon Willison · Mar 12, 16:28

**Background**: AI-assisted coding refers to the use of generative AI models, often large language models (LLMs), to suggest, complete, or even generate entire blocks of code based on natural language prompts. Tools like GitHub Copilot and Amazon CodeWhisperer have popularized this approach. The debate touches on long-standing discussions in software engineering about the balance between art, craft, engineering discipline, and pragmatic delivery of working software.

**Tags**: `#AI-assisted-development`, `#software-engineering-culture`, `#developer-productivity`, `#programming-philosophy`

---

<a id="item-8"></a>
## [Apple May Globally Reduce App Store Commission from 30% to 20%](https://t.me/zaihuapd/40232) ⭐️ 7.0/10

Apple introduced complex new App Store terms in the EU last week, with details suggesting the company may reduce its standard commission rate from 30% to 20%. Analysts believe this change could potentially extend to the global market, marking Apple's first reduction of the standard 30% rate for all developers. This potential global commission reduction would significantly impact app developer economics by increasing their net revenue per transaction. It represents a major shift in Apple's long-standing App Store business model and could influence pricing strategies and profitability across the entire mobile app ecosystem. The new terms are described as extremely complex, with even Apple Design Award winner Ryan Jones stating that no developer friends could understand their specific meaning. Analysts argue that maintaining a 20% commission in the EU while keeping 30% elsewhere would be an unreasonable differential pricing strategy, suggesting a global adjustment is likely.

telegram · zaihuapd · Mar 13, 01:49

**Background**: Apple's App Store has historically charged developers a 30% commission on digital goods and services sold through the platform, with a reduced 15% rate for subscriptions after the first year. This commission structure has been a point of contention between Apple and developers, leading to regulatory scrutiny and legal challenges in multiple jurisdictions. The EU's Digital Markets Act has recently forced Apple to make changes to its App Store policies in Europe, creating pressure for broader reforms.

**Tags**: `#app-store`, `#apple`, `#mobile-development`, `#digital-marketplace`, `#developer-economics`

---

<a id="item-9"></a>
## [Research: Alipay DeepLink with JSBridge could leak personal data via external pages](https://innora.ai/zfb/) ⭐️ 7.0/10

Security researchers at Innora AI Security Research published a technical analysis showing that in Alipay versions com.eg.android.AlipayGphone v10.8.26.7000 and v10.8.30.8000, the combination of DeepLink and WebView JSBridge could form an attack chain. If a user clicks a link, an external page could call certain AlipayJSBridge APIs within the app, potentially accessing sensitive interfaces like tradePay and getLocation. This matters because Alipay is a widely used payment and lifestyle app in China, and a successful exploit could lead to the unauthorized access of sensitive user data like location and payment information. The vendor's dismissal of the issue as 'normal functionality' highlights the ongoing tension between app usability and robust security practices in mobile ecosystems. The researchers reported that iOS exposes 18 potentially accessible APIs, while Android exposes 13. They followed responsible disclosure procedures, but Ant Group responded on March 10, 2026, stating the reported behavior was 'normal functionality.' An editorial note cautions that the original article only clearly demonstrates location access and payment pop-up triggers, suggesting potential exaggeration.

telegram · zaihuapd · Mar 13, 11:43

**Background**: Deep Links are URLs that can open a specific page or trigger an action within a mobile app, bypassing the browser. However, insecure implementations can allow malicious apps or web pages to hijack these links. A WebView is an embedded browser component within an app, and a JSBridge is a mechanism that allows JavaScript code running in the WebView to call native app functions (Java/Kotlin on Android, Swift/Obj-C on iOS). If the JSBridge is improperly secured, external web content loaded via a Deep Link could potentially call sensitive native APIs.

<details><summary>References</summary>
<ul>
<li><a href="https://redfoxsec.com/blog/protect-your-android-app-preventing-exploitation-of-deep-links/">Preventing Exploitation of Deep Links - Redfox Security - Pen Testing Services</a></li>
<li><a href="https://medium.com/@youssefhussein212103168/exploiting-insecure-android-webview-with-javascript-interface-a4d3abf9ec09">Exploiting Insecure Android WebView with JavaScript Interface | by Youssefhussein</a></li>
<li><a href="https://opendocs.alipay.com/open/024kz4">Alipay JSAPI 使用说明 - 支付宝文档中心</a></li>

</ul>
</details>

**Tags**: `#mobile-security`, `#webview`, `#jsbridge`, `#alipay`, `#vulnerability`

---