---
layout: default
title: "Horizon Summary: 2026-04-09 (EN)"
date: 2026-04-09
lang: en
---

> From 19 items, 5 important content pieces were selected

---

1. [Meta launches Muse Spark AI model with competitive benchmarks and new chat tools](#item-1) ⭐️ 8.0/10
2. [Meta Launches Muse Spark, First AI Model from Its Superintelligent Team](#item-2) ⭐️ 8.0/10
3. [ByteDance launches native full-duplex voice model Seeduplex, now live in Doubao app](#item-3) ⭐️ 8.0/10
4. [FBI Extracts Deleted Signal Messages from iPhone Notification Database](#item-4) ⭐️ 8.0/10
5. [macOS kernel bug causes network failure after 49.7 days, requires reboot](#item-5) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Meta launches Muse Spark AI model with competitive benchmarks and new chat tools](https://simonwillison.net/2026/Apr/8/muse-spark/#atom-everything) ⭐️ 8.0/10

Meta announced Muse Spark, its first major AI model release in a year, which is currently available as a hosted model through a private API preview and on meta.ai. The model features 'Instant' and 'Thinking' modes, with a future 'Contemplating' mode promised, and self-reported benchmarks show it competitive with models like GPT-5.4 and Gemini 3.1 Pro on selected tests. This marks Meta's re-entry into the competitive frontier model race after a year, signaling its continued investment in AI despite a shift from open weights to hosted services. The model's performance and planned 'Contemplating' mode position it to challenge established leaders like OpenAI and Google in complex reasoning tasks. The model has a 262k token context window and supports text, image, and speech input. Meta acknowledges performance gaps in areas like long-horizon agentic systems and coding, as evidenced by lower scores on the Terminal-Bench 2.0 benchmark which tests AI agents on complex terminal tasks. The meta.ai chat interface was found to have access to 16 tools, including web search and semantic search across Meta's social platforms.

rss · Simon Willison · Apr 8, 23:07

**Background**: Large Language Models (LLMs) like GPT and Gemini are AI systems trained on vast text data to generate human-like text, answer questions, and perform tasks. Benchmarks are standardized tests used to compare the performance of different AI models across various capabilities. Terminal-Bench 2.0 is a specific open-source benchmark that evaluates an AI agent's ability to complete long, multi-step tasks in a simulated command-line terminal environment, which is particularly relevant for coding and software engineering workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/muse-spark">Muse Spark - Intelligence, Performance & Price Analysis</a></li>
<li><a href="https://www.vals.ai/benchmarks/terminal-bench-2">Terminal - Bench 2 . 0</a></li>
<li><a href="https://www.ai21.com/glossary/ai-agent/what-are-long-horizon-tasks/">What are Long-Horizon Tasks? | AI21</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#meta`, `#llm`, `#ai-models`, `#tech-announcement`

---

<a id="item-2"></a>
## [Meta Launches Muse Spark, First AI Model from Its Superintelligent Team](https://ai.meta.com/blog/introducing-muse-spark-msl/) ⭐️ 8.0/10

Meta has launched Muse Spark, the first AI model from its Superintelligence Labs, featuring native multimodal reasoning, tool calling, and multi-agent collaboration. The model is now available on the Meta AI website and app, with plans to replace existing Llama models across WhatsApp, Instagram, Facebook, and Meta smart glasses in the coming weeks. This launch represents a major strategic shift for Meta, as Muse Spark is positioned to become the core AI across its massive consumer platforms, directly impacting billions of users. Its claimed performance gains over models like GPT-5.4 and Gemini 3.1 signal Meta's intensified competition in the frontier AI race. A key feature is 'Contemplating mode,' which orchestrates multiple reasoning agents in parallel, reportedly achieving scores of 58% on the Humanity's Last Exam benchmark and 38% on Frontier Science Research. Meta also disclosed it has rebuilt its pre-training stack over the past nine months and is investing heavily in infrastructure like the $27 billion Hyperion data center project.

telegram · zaihuapd · Apr 8, 16:42

**Background**: Meta's Superintelligence Labs is a team focused on developing advanced, frontier AI systems. Native multimodal reasoning means the model is inherently designed from the ground up to process and understand different types of data (like text, images, and audio) together, rather than stitching separate models together. Multi-agent collaboration involves orchestrating multiple specialized AI 'agents' to work in parallel on complex tasks, potentially improving reasoning and problem-solving.

<details><summary>References</summary>
<ul>
<li><a href="https://www.neowin.net/news/meta-launches-muse-spark-ai-with-reasoning-and-native-multimodal-capabilities/">Meta launches Muse Spark AI with reasoning and native ...</a></li>
<li><a href="https://news.aibase.com/news/26959">Meta Shocks the Scene! Muse Spark Personal Super Intelligent Model...</a></li>
<li><a href="https://fortune.com/2026/03/26/meta-ai-data-center-hyperion-louisiana/">Meta's $27 billion AI data center is causing chaos in small ...</a></li>

</ul>
</details>

**Tags**: `#AI Models`, `#Multimodal AI`, `#Meta`, `#Large Language Models`, `#Deployment`

---

<a id="item-3"></a>
## [ByteDance launches native full-duplex voice model Seeduplex, now live in Doubao app](https://seed.bytedance.com/seeduplex) ⭐️ 8.0/10

ByteDance has officially launched Seeduplex, a native full-duplex voice large model, which is now fully deployed in its Doubao app. This marks the first large-scale commercial application of full-duplex technology in the industry, moving it out of the lab to serve hundreds of millions of users. This deployment represents a significant step towards more natural and fluid human-computer voice interaction, as it allows for simultaneous listening and speaking, akin to a real human conversation. It could set a new standard for voice assistants and interactive AI applications, impacting a vast user base through ByteDance's popular platform. The model combines voice pre-training with reinforcement learning (RL) to achieve precise interference suppression and dynamic endpoint detection while maintaining extremely fast response times. This technical approach is designed to significantly improve the naturalness and fluency of conversations.

telegram · zaihuapd · Apr 9, 05:35

**Background**: Traditional voice interaction systems typically operate in a half-duplex mode, where the system and user take turns speaking and listening. Full-duplex models, in contrast, are engineered for real-time bidirectional exchange, allowing for overlapping speech, interruptions, and rapid back-and-forth like a natural conversation. Dynamic endpoint detection is a key challenge, as it involves the model intelligently determining when a user has finished speaking based on context, rather than relying on simple silence thresholds.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/full-duplex-spoken-dialogue-model">Full-Duplex Spoken Dialogue Model</a></li>
<li><a href="https://arxiv.org/abs/2210.14252">Dynamic Speech Endpoint Detection with Regression Targets - arXiv</a></li>

</ul>
</details>

**Tags**: `#speech-recognition`, `#generative-ai`, `#real-time-systems`, `#bytedance`, `#voice-interface`

---

<a id="item-4"></a>
## [FBI Extracts Deleted Signal Messages from iPhone Notification Database](https://www.404media.co/fbi-extracts-suspects-deleted-signal-messages-saved-in-iphone-notification-database-2/) ⭐️ 8.0/10

During a trial in Texas, the FBI forensically extracted incoming Signal messages from a suspect's iPhone, even after the app was deleted, by accessing copies stored in the device's push notification database. The technique, confirmed by testimony, only recovered incoming messages, not outgoing ones. This reveals a significant privacy vulnerability for users of encrypted messaging apps like Signal, as enabling lock screen previews can leave message content persistently stored by iOS in a forensically accessible location. It highlights a gap between app-level encryption and data retention by the operating system, with implications for digital privacy and legal evidence collection. The extraction was possible because the iPhone's notification system saved preview content to an internal database, likely the `KnowledgeC.db` file, when lock screen previews were enabled for Signal. Signal acknowledged a request for comment on March 12 but did not follow up, and Apple did not respond.

telegram · zaihuapd · Apr 9, 14:05

**Background**: Signal is a popular messaging app known for its end-to-end encryption, which is designed to prevent anyone except the sender and recipient from reading message content. iOS manages notifications through a system database (often referred to as `KnowledgeC.db`), which can store notification content, including message previews, for various apps. Digital forensics techniques can analyze this database to recover data that users may believe has been deleted from the app itself.

<details><summary>References</summary>
<ul>
<li><a href="https://www.404media.co/fbi-extracts-suspects-deleted-signal-messages-saved-in-iphone-notification-database-2/">FBI Extracts Suspect’s Deleted Signal Messages Saved in iPhone Notification Database</a></li>
<li><a href="https://dfir.pubpub.org/pub/g2v1z97i">iOS KnowledgeC.db Notifications - DFIR Review - PubPub</a></li>
<li><a href="https://support.signal.org/hc/en-us/articles/360007062172-Signal-Permissions-OS-Notification-Settings">Signal Permissions & OS Notification Settings</a></li>

</ul>
</details>

**Tags**: `#digital-forensics`, `#privacy`, `#encryption`, `#iOS`, `#signal`

---

<a id="item-5"></a>
## [macOS kernel bug causes network failure after 49.7 days, requires reboot](https://www.tomshardware.com/software/macos/macos-has-a-49-7-day-networking-time-bomb-built-in-that-only-a-reboot-fixes-comparison-operation-on-unreliable-time-value-stops-machines-dead-in-their-tracks) ⭐️ 7.0/10

Researchers from Photon discovered a kernel-level bug in macOS that causes network connections to fail after precisely 49 days, 17 hours, 2 minutes, and 47 seconds of continuous system uptime. The issue stems from a 32-bit unsigned integer overflow in the `tcp_now` timer within Apple's XNU kernel TCP stack, which disrupts the cleanup of closed TCP connections. This is a significant 'time bomb' style bug that can silently cripple network connectivity on macOS devices, including servers and workstations with long uptimes, potentially disrupting critical services. It highlights a fundamental flaw in a core networking component of a major operating system, affecting reliability and requiring user intervention (a reboot) to resolve. The bug specifically prevents the establishment of new network connections while existing ones may remain active, eventually exhausting available ephemeral ports. The current workaround is a full system reboot, and researchers note that Apple's implementation appears to mishandle the timer wrap-around as specified in RFC 7323.

telegram · zaihuapd · Apr 9, 12:16

**Background**: The `tcp_now` is a kernel-internal TCP clock that tracks elapsed milliseconds since boot using a 32-bit unsigned integer. Such integers have a maximum value of 4,294,967,295. After this many milliseconds (approximately 49.7 days), the counter overflows, or 'wraps around'. Proper handling of this wrap-around is crucial for TCP timestamp calculations used in algorithms like PAWS (Protection Against Wrapped Sequence numbers) to manage connections. RFC 7323 defines standards for TCP timestamps and their wrap-around behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://schwarztech.net/snippets/we-found-a-ticking-time-bomb-in-macos-tcp-networking-it-detonates-after-exactly-49-days">» We Found a Ticking Time Bomb in macOS TCP Networking – It ...</a></li>
<li><a href="https://www.techpowerup.com/348105/apple-macbooks-lose-network-connectivity-after-49-7-days-due-to-macos-time-bomb-bug">Apple MacBooks Lose Network Connectivity After 49.7 Days Due ...</a></li>
<li><a href="https://www.rfc-editor.org/info/rfc7323">Information on RFC 7323 - » RFC Editor</a></li>

</ul>
</details>

**Tags**: `#macOS`, `#Kernel`, `#Networking`, `#Security`, `#TCP/IP`

---