---
layout: default
title: "Horizon Summary: 2026-03-28 (EN)"
date: 2026-03-28
lang: en
---

> From 27 items, 9 important content pieces were selected

---

1. [All 8,642 Spanish laws converted to Git repository with historical reforms as commits](#item-1) ⭐️ 8.0/10
2. [Discussion on Securing Filesystems Against AI Agents Through Sandboxing and Permission Models](#item-2) ⭐️ 8.0/10
3. [Chinese Academy of Sciences Documentation Center to Cease Journal Ranking Updates in 2026](#item-3) ⭐️ 8.0/10
4. [FBI Failed to Extract Data from Reporter's iPhone 13 Due to Apple's Lockdown Mode](#item-4) ⭐️ 8.0/10
5. [EU Parliament Rejects 'Chat Control' Surveillance Extension, Shifts Focus to Identity Verification](#item-5) ⭐️ 8.0/10
6. [AI Deepfakes Deployed at Scale in 2026 US Midterms by Republican Campaigns](#item-6) ⭐️ 8.0/10
7. [SGLang v0.5.10rc0 enhances inference with default CUDA graphs, fault-tolerant MoE, and sparse attention.](#item-7) ⭐️ 7.0/10
8. [European Commission confirms AWS cloud breach with hundreds of GB of data stolen from Europa.eu platform](#item-8) ⭐️ 7.0/10
9. [Wharton research identifies 'cognitive surrender' where people accept AI outputs without verification](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [All 8,642 Spanish laws converted to Git repository with historical reforms as commits](https://github.com/EnriqueLop/legalize-es) ⭐️ 8.0/10

Developer Enrique Lop created a pipeline that converted all Spanish state legislation into a Git repository, where each law is stored as a Markdown file and every historical reform is recorded as a commit with its actual date. The repository contains 8,642 laws and 27,866 commits, transforming legal amendments into readable diffs. This demonstrates how version control systems can bring transparency and traceability to legal systems, making it easier to track legislative changes over time. It enables AI systems and other tools to analyze legal evolution and could serve as a model for modernizing government document management worldwide. The pipeline converts legislation into machine-readable Markdown format, with each reform creating a real git commit that preserves the historical timeline. Instead of reading traditional amendment language like 'strike paragraph 3,' users can view actual diffs showing exactly what changed between versions.

hackernews · enriquelop · Mar 28, 12:01

**Background**: Git is a distributed version control system originally developed for tracking changes in software code, but its principles apply well to any document that evolves over time. Legal documents have historically used manual version control methods like 'contract redline' and 'legal blackline,' which are early forms of revision control. The concept of applying modern version control to legislation has been explored previously, such as with the United States Legislative Markup (USLM) standard for the U.S. Code.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Version_control">Version control - Wikipedia</a></li>
<li><a href="https://datafoundation.org/news/blogs/335/335-Version-Control-for-Law-Tracking-Changes-in-the-US-Congress">Version Control for Law: Tracking Changes in the U.S. Congress | ANALYSIS | Data Foundation</a></li>

</ul>
</details>

**Discussion**: Community members praised the project as a step toward transparent legal databases and expressed desire to see similar implementations for other countries. Several commenters noted existing versioned legal systems in France and California, while others highlighted how this approach solves inefficiencies in traditional legal workflows. The discussion emphasized that this technology should become standard practice for legislative tracking.

**Tags**: `#legal-tech`, `#git`, `#open-government`, `#data-transformation`, `#version-control`

---

<a id="item-2"></a>
## [Discussion on Securing Filesystems Against AI Agents Through Sandboxing and Permission Models](https://jai.scs.stanford.edu/) ⭐️ 8.0/10

A high-scoring community discussion (476 points, 272 comments) has emerged about implementing filesystem sandboxing and permission models to protect against AI agents that could corrupt or exfiltrate data. The conversation explores practical approaches including Claude Code's sandboxing features, Unix permission systems, and container-based isolation techniques. This matters because as AI agents gain more autonomy and system access, they introduce new attack vectors for data corruption and exfiltration that traditional security models weren't designed to handle. The discussion highlights a critical gap in current AI deployment practices where powerful agents operate with excessive permissions, potentially compromising sensitive data across personal and enterprise systems. The discussion reveals that simple Unix permission models (separate accounts for user and AI with shared group folders) can provide basic protection, while more sophisticated approaches like Claude Code's sandboxed bash tool offer filesystem and network isolation. Community members note that containers provide isolation but may have performance overhead, and some question whether existing permission systems are adequate for AI's unpredictable behavior patterns.

hackernews · mazieres · Mar 28, 00:39

**Background**: Filesystem sandboxing is a security technique that restricts an application's access to specific parts of the filesystem, preventing it from reading or writing to unauthorized locations. AI agent permission models define what resources an AI can access and what actions it can perform, similar to user permissions in traditional systems. Data exfiltration prevention involves techniques to stop unauthorized data transfers outside a protected environment, which becomes particularly challenging with AI agents that might inadvertently or maliciously leak information through their outputs or actions.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/sandboxing">Sandboxing - Claude Code Docs</a></li>
<li><a href="https://dl.acm.org/doi/10.1145/3265723.3265734">A Lightweight and Fine-grained File System Sandboxing Framework</a></li>
<li><a href="https://www.osohq.com/learn/ai-agent-permissions-delegated-access">Setting Permissions for AI Agents - Oso</a></li>

</ul>
</details>

**Discussion**: Community sentiment shows concern about the security risks of running AI agents with broad system access, with some expressing surprise at how readily users grant permissions to unpredictable software. Technical discussions include practical implementation details like Claude configuration settings, Unix permission setups, and comparisons between sandboxing approaches. Several commenters seek more resources on security trade-offs between different isolation methods (sandboxes, containers, VMs).

**Tags**: `#AI Security`, `#Filesystem Sandboxing`, `#Agent Safety`, `#Unix Permissions`, `#System Security`

---

<a id="item-3"></a>
## [Chinese Academy of Sciences Documentation Center to Cease Journal Ranking Updates in 2026](https://mp.weixin.qq.com/s/_vf0g6qlG9mFbyyARa0IPQ) ⭐️ 8.0/10

On March 27, the Documentation and Information Center of the Chinese Academy of Sciences (CAS) announced that it will cease updating and publishing its Journal Partition Table starting in 2026. The center stated it will continue research on academic resource evaluation methods to serve the academic exchange and publishing ecosystem. This decision marks a significant policy shift in China's academic evaluation system, as the CAS Journal Partition Table has been a widely used reference for research assessment, paper submission, and institutional evaluations nationwide. Its discontinuation signals a potential move away from reliance on simplified journal-tier metrics towards more nuanced evaluation methodologies, which could reshape incentives for researchers, universities, and publishers across China. The center clarified that any journal partition tables published by other institutions after 2026 will have no relation to it. It also mentioned it will promptly initiate follow-up procedures regarding contracts for users who had already subscribed for the 2026 data.

telegram · zaihuapd · Mar 28, 02:45

**Background**: The CAS Journal Partition Table is a research output of the CAS Documentation and Information Center, designed initially around the year 2000 to address the oversight of impact factor disparities across different disciplines within the Chinese research community. It categorizes international academic journals in natural sciences, engineering, medicine, management, social sciences, and humanities into different tiers (e.g., Q1-Q4 or Zone 1-4) based on citation metrics, and has been extensively used by Chinese universities and research institutes for performance evaluation, funding allocation, and promotion decisions. The table is accessible through an official online platform and WeChat official account.

<details><summary>References</summary>
<ul>
<li><a href="https://www.jiemian.com/article/14177382.html">中国科学院文献情报中心：将不再更新与发布期刊分区表</a></li>
<li><a href="https://www.las.ac.cn/front/knowledgeServices/serviceDetail?entityId=26&entityType=ApplicationMart">期刊分区表 - las</a></li>

</ul>
</details>

**Tags**: `#academic-publishing`, `#research-evaluation`, `#china-science-policy`, `#scholarly-communication`

---

<a id="item-4"></a>
## [FBI Failed to Extract Data from Reporter's iPhone 13 Due to Apple's Lockdown Mode](https://t.me/zaihuapd/40569) ⭐️ 8.0/10

The FBI's Computer Analysis Response Team (CART) disclosed that it was unable to extract data from Washington Post reporter Hannah Natanson's iPhone 13 because the device had Apple's Lockdown Mode enabled. This occurred during an investigation into alleged leaks of classified information by a government contractor. This incident provides a significant real-world demonstration of Lockdown Mode's effectiveness against sophisticated forensic extraction attempts by a major law enforcement agency. It highlights the growing capability of consumer device security features to protect sensitive information, such as journalistic sources, from state-level actors. While the FBI was able to unlock the reporter's MacBook Pro via fingerprint and access some Signal communications from it, the iPhone 13 itself remained impenetrable due to Lockdown Mode. The case is documented in court filings related to the investigation of government contractor Aurelio Perez-Lugones.

telegram · zaihuapd · Mar 28, 08:57

**Background**: Apple's Lockdown Mode is an extreme, optional protection feature for iPhone designed to defend against highly sophisticated cyberattacks, such as those by state-sponsored actors. When enabled, it severely restricts device functionality by limiting certain apps, web technologies, and connection types to reduce the attack surface. The FBI's Computer Analysis and Response Team (CART) is its primary digital forensics unit, specializing in extracting and analyzing data from electronic devices for investigations. Signal is a messaging app known for its strong end-to-end encryption, which scrambles messages so only the sender and recipient can read them.

<details><summary>References</summary>
<ul>
<li><a href="https://support.apple.com/en-us/105120">About Lockdown Mode - Apple Support</a></li>
<li><a href="https://www.ojp.gov/ncjrs/virtual-library/abstracts/computer-analysis-and-response-team-cart-microcomputer-evidence">Computer Analysis and Response Team (CART): The Microcomputer ...</a></li>
<li><a href="https://signal.org/">Signal >> Home</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#digital-privacy`, `#apple-security`, `#law-enforcement`, `#journalism`

---

<a id="item-5"></a>
## [EU Parliament Rejects 'Chat Control' Surveillance Extension, Shifts Focus to Identity Verification](https://www.patrick-breyer.de/en/end-of-chat-control-eu-parliament-stops-mass-surveillance-in-voting-thriller-paving-the-way-for-genuine-child-protection/) ⭐️ 8.0/10

The European Parliament narrowly rejected, by a single vote, the extension of the 'Chat Control 1.0' temporary regulation, which will now expire on April 4, 2026. This decision forces major US tech companies like Meta, Google, and Microsoft to stop the automated scanning of European citizens' private messages, images, and text content for child abuse material. This is a significant victory for digital privacy rights in the EU, blocking a form of mass surveillance that critics argued undermined end-to-end encryption. It forces a major shift in the EU's approach to online child protection, moving the debate away from bulk scanning and towards potentially contentious measures like mandatory identity or age verification. The rejection was heavily influenced by studies showing the system's high false positive rate of 13-20%, which led to about 48% of police reports being unrelated to crime and failed to improve actual conviction rates. While this specific mass scanning regime is ending, negotiations for a permanent EU child protection law continue, with 'Chat Control 2.0' proposals that could mandate scanning all communications on social platforms still under consideration.

telegram · zaihuapd · Mar 28, 13:06

**Background**: Since July 2021, an EU interim regulation, often called 'Chat Control 1.0,' has provided a temporary exemption from parts of the ePrivacy Directive. This exemption allowed communication service providers to scan private messages using techniques like 'hash scanning' for known child sexual abuse material (CSAM). The regulation was set to expire but had been subject to potential extensions, creating a long-running controversy over privacy versus child protection.

<details><summary>References</summary>
<ul>
<li><a href="https://gigazine.net/gsc_news/en/20260327-end-eu-chat-control/">The EU has decided to repeal 'Chat Control 1.0,' which ...</a></li>
<li><a href="https://edri.org/our-work/a-beginners-guide-to-eu-rules-on-scanning-private-communications-part-1/">A beginner’s guide to EU rules on scanning private communications: Part 1 - European Digital Rights (EDRi)</a></li>
<li><a href="https://www.computerweekly.com/news/366640781/EU-Parliament-rejects-Chat-Control-message-scanning">EU Parliament rejects Chat Control message scanning | Computer Weekly</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#eu-regulation`, `#surveillance`, `#tech-policy`, `#digital-rights`

---

<a id="item-6"></a>
## [AI Deepfakes Deployed at Scale in 2026 US Midterms by Republican Campaigns](https://www.reuters.com/business/media-telecom/ai-deepfakes-blur-reality-2026-us-midterm-campaigns-2026-03-28/) ⭐️ 8.0/10

Ahead of the 2026 US midterm elections, Republican campaigns, including the National Republican Senatorial Committee (NRSC), are deploying AI-generated deepfake political ads at scale, fabricating statements from opponents. For example, a deepfake ad falsely portrayed Texas Senate candidate James Talarico claiming 'radical whites are the biggest terror threat.' This marks a significant escalation in the weaponization of AI for political disinformation, normalizing deceptive content and directly threatening electoral integrity. The widespread use by a major party, amid fragmented regulation, risks eroding public trust in democratic institutions and could set a dangerous precedent for future elections globally. While many such ads carry small AI labels, their effectiveness in misleading voters remains high due to their realism and the limited reach of disclosure laws. Although 28 states have passed laws requiring disclosure of AI use in political ads, enforcement is weak, especially for content spread on social media platforms.

telegram · zaihuapd · Mar 28, 15:42

**Background**: Deepfakes are synthetic media where a person's likeness is replaced with someone else's using artificial intelligence, creating highly realistic but fake videos or audio. The National Republican Senatorial Committee (NRSC) is a major political committee dedicated to electing Republicans to the US Senate. In the US, regulation of AI in political advertising is primarily handled at the state level, leading to a patchwork of laws with varying requirements for disclosure or outright bans on certain deceptive uses.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/National_Republican_Senatorial_Committee">National Republican Senatorial Committee - Wikipedia</a></li>
<li><a href="https://www.adexchanger.com/data-driven-thinking/ai-disclosure-requirements-navigating-state-laws-and-platform-rules/">AI Disclosure Requirements: Navigating State Laws And Platform Rules | AdExchanger</a></li>
<li><a href="https://www.broadcastlawblog.com/2026/03/articles/ai-in-political-attack-ads-watch-state-laws-on-deep-fakes-and-synthetic-media-in-political-content/">AI in Political Attack Ads – Watch State Laws on Deep Fakes and Synthetic Media in Political Content | Broadcast Law Blog</a></li>

</ul>
</details>

**Tags**: `#AI Ethics`, `#Disinformation`, `#Political Technology`, `#Deepfakes`, `#Election Integrity`

---

<a id="item-7"></a>
## [SGLang v0.5.10rc0 enhances inference with default CUDA graphs, fault-tolerant MoE, and sparse attention.](https://github.com/sgl-project/sglang/releases/tag/v0.5.10rc0) ⭐️ 7.0/10

SGLang v0.5.10rc0 has been released, making piecewise CUDA graph capture the default execution mode for improved throughput. It also introduces Elastic EP for partial failure tolerance in MoE models, integrates the HiSparse sparse attention backend for long-context inference, and updates SGLang-Diffusion with new model support and performance gains. This release significantly improves the reliability and efficiency of large language model serving systems. The default piecewise CUDA graphs reduce memory overhead, Elastic EP ensures continuous service during GPU failures in MoE deployments, and HiSparse enables more efficient processing of long sequences, collectively advancing production-ready inference. The piecewise CUDA graph feature pre-captures graphs for a set of token counts and selects the nearest match at runtime, which is particularly beneficial for variable-length prefill/extend operations. Elastic EP specifically enables DeepSeek MoE deployments to redistribute expert weights and continue serving without a full restart when a GPU fails.

github · Kangyan-Zhou · Mar 28, 05:58

**Background**: SGLang is a high-performance language model serving framework designed to optimize inference. Piecewise CUDA graphs are an optimization where the model's forward pass is captured as multiple smaller graphs for different input sizes, improving performance over a single graph for variable-length inputs. Mixture-of-Experts (MoE) models use multiple specialized sub-networks (experts) to process different parts of the input, which can be distributed across multiple GPUs. Sparse attention mechanisms reduce computational cost by having tokens attend only to a subset of other tokens, which is crucial for handling long contexts.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.sglang.io/advanced_features/piecewise_cuda_graph.html">Piecewise CUDA Graph — SGLang</a></li>
<li><a href="https://deepwiki.com/kvcache-ai/Mooncake/7.6-elastic-expert-parallelism">Elastic Expert Parallelism | kvcache-ai/Mooncake | DeepWiki</a></li>
<li><a href="https://arxiv.org/abs/2602.03560">[2602.03560] HySparse: A Hybrid Sparse Attention Architecture ...</a></li>

</ul>
</details>

**Tags**: `#inference-optimization`, `#gpu-computing`, `#llm-serving`, `#sparse-attention`, `#model-serving`

---

<a id="item-8"></a>
## [European Commission confirms AWS cloud breach with hundreds of GB of data stolen from Europa.eu platform](http://europa.eu/) ⭐️ 7.0/10

The European Commission confirmed a cyberattack on its cloud infrastructure, specifically targeting the AWS environment hosting the Europa.eu platform, resulting in the theft of hundreds of gigabytes of data. The Commission stated that immediate containment and risk mitigation measures were taken, the attack was controlled, internal systems were unaffected, and an investigation is ongoing. This breach is significant because it targets a major governmental institution's public-facing digital platform, potentially compromising sensitive information and undermining trust in EU digital services. It highlights the persistent security challenges faced by public sector entities when migrating critical infrastructure to cloud platforms like AWS, even with established providers. According to Bleeping Computer, hackers stole data including multiple databases from the Commission's AWS account and provided access screenshots as evidence. The specific types of data exfiltrated have not yet been disclosed by the Commission, leaving the full scope and sensitivity of the breach unclear.

telegram · zaihuapd · Mar 28, 01:16

**Background**: Amazon Web Services (AWS) is a leading on-demand cloud computing platform used by governments and enterprises worldwide. The Europa.eu platform is the official website of the European Union, serving as a critical public information and service portal. Data exfiltration refers to techniques adversaries use to steal data from a network, often involving unauthorized access and transfer of sensitive information.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Amazon_Web_Services">Amazon Web Services - Wikipedia</a></li>
<li><a href="https://attack.mitre.org/tactics/TA0010/">Exfiltration , Tactic TA0010 - Enterprise | MITRE ATT&CK</a></li>

</ul>
</details>

**Tags**: `#Cybersecurity`, `#Data Breach`, `#AWS`, `#European Commission`, `#Cloud Security`

---

<a id="item-9"></a>
## [Wharton research identifies 'cognitive surrender' where people accept AI outputs without verification](https://www.forbes.com/sites/lesliekatz/2026/03/27/cognitive-surrender-we-trust-ai-over-our-own-brains-research-finds/) ⭐️ 7.0/10

Researchers from the Wharton School at the University of Pennsylvania published a preprint last month on SSRN, reporting that in experiments with nearly 1,300 participants, people used ChatGPT for over half of logic and reasoning tasks. In about 80% of cases where they sought AI assistance, participants accepted incorrect answers without scrutiny, a behavior the researchers term 'adoption without verification.' This phenomenon of 'cognitive surrender' suggests generative AI is fundamentally reshaping human decision-making processes, potentially creating systemic risks where people relinquish critical thinking and epistemic agency to automated systems. It highlights the need to reconsider traditional decision-making models and design AI interfaces that encourage, rather than bypass, human cognitive engagement. The study found that participants using ChatGPT reported 10% higher confidence in their answers, despite the potential for error. The researchers propose that AI should be incorporated as a new external cognitive system within decision-making frameworks, moving beyond traditional dual-process models.

telegram · zaihuapd · Mar 28, 14:23

**Background**: The 'dual-process theory' of decision-making describes two interacting systems: System 1 (fast, intuitive, automatic) and System 2 (slow, deliberate, analytical). SSRN (Social Science Research Network) is an open-access repository for sharing early-stage research and preprints, which are papers that have not yet undergone formal peer review. The concept of 'cognitive surrender' extends beyond simple reliance on tools, describing a relinquishing of cognitive control where users substitute AI outputs for their own reasoning without critical evaluation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Social_Science_Research_Network">Social Science Research Network - Wikipedia</a></li>
<li><a href="https://www.globalcognition.org/dual-process-theory/">Dual Process Theory: Two Ways to Think and Decide</a></li>
<li><a href="https://medkharbach.com/cognitive-surrender-how-ai-is-quietly-reshaping-the-way-we-think/">Cognitive Surrender: How AI Is Quietly Reshaping the Way We ...</a></li>

</ul>
</details>

**Tags**: `#AI Ethics`, `#Human-Computer Interaction`, `#Behavioral Science`, `#Decision Making`, `#Generative AI`

---