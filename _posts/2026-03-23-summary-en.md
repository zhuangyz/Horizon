---
layout: default
title: "Horizon Summary: 2026-03-23 (EN)"
date: 2026-03-23
lang: en
---

> From 28 items, 6 important content pieces were selected

---

1. [Starlette 1.0 Released, Marking Stability for the ASGI Framework Powering FastAPI](#item-1) ⭐️ 8.0/10
2. [OpenAI urges UK to include AI chatbots in Google's search choice screen](#item-2) ⭐️ 8.0/10
3. [Guide to migrating digital services from US to EU providers for data sovereignty](#item-3) ⭐️ 7.0/10
4. [GitHub's reliability reportedly falls to 'three nines' availability amid outages and security concerns.](#item-4) ⭐️ 7.0/10
5. [Research compares JavaScript sandboxing techniques including isolated-vm, vm2, QuickJS, ShadowRealm, and Deno Workers](#item-5) ⭐️ 7.0/10
6. [Interactive Visualizer Created to Demonstrate Bram Cohen's CRDT-Based Version Control Concept](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Starlette 1.0 Released, Marking Stability for the ASGI Framework Powering FastAPI](https://simonwillison.net/2026/Mar/22/starlette/#atom-everything) ⭐️ 8.0/10

Starlette, the foundational Python ASGI framework, has released version 1.0 in March 2026, marking its first major stable release. The update introduces breaking changes, most notably replacing the `on_startup` and `on_shutdown` parameters with a new `lifespan` async context manager system. This release is significant because Starlette is the underlying engine for the highly popular FastAPI framework, meaning its stability directly impacts a vast ecosystem of modern Python web applications. The 1.0 milestone provides a stable API foundation for developers and projects, like Datasette, that previously hesitated to build on it due to version instability. The project's stewardship transferred to Marcelo Trylesinski in September 2025 to facilitate sponsorship. A key technical shift is the move to the `lifespan` pattern, which uses Python's `contextlib.asynccontextmanager` for cleaner management of startup and shutdown logic compared to the old callback parameters.

rss · Simon Willison · Mar 22, 23:57

**Background**: Starlette is a lightweight, asynchronous web framework built for the ASGI (Asynchronous Server Gateway Interface) specification, which is the modern successor to WSGI for Python. It provides the core request/response handling and routing that FastAPI builds upon, adding automatic data validation and OpenAPI documentation. ASGI enables Python frameworks to handle HTTP, WebSockets, and other protocols asynchronously, improving performance for I/O-bound operations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asynchronous_Server_Gateway_Interface">Asynchronous Server Gateway Interface - Wikipedia</a></li>
<li><a href="https://dev.to/ceb10n/understanding-fastapi-how-starlette-works-43i1">Understanding FastAPI: How Starlette works - DEV Community</a></li>
<li><a href="https://leapcell.medium.com/fastapi-is-overkill-starlette-and-pydantic-are-all-you-really-need-2b2d55c53de0">FastAPI is Overkill: Starlette and Pydantic Are All You Really Need | by Leapcell | Medium</a></li>

</ul>
</details>

**Tags**: `#python`, `#web-frameworks`, `#asgi`, `#backend-development`, `#fastapi`

---

<a id="item-2"></a>
## [OpenAI urges UK to include AI chatbots in Google's search choice screen](https://assets.publishing.service.gov.uk/media/69b970dcc06ba9576435ab5a/OpenAI.pdf) ⭐️ 8.0/10

On March 6, OpenAI formally submitted a recommendation to the UK's Competition and Markets Authority (CMA) that the eligibility criteria for Google's search choice screen should explicitly include AI chatbots with search capabilities. This would allow services like ChatGPT to be selectable as default search options on Android devices and Chrome browsers. This move is significant as it represents a strategic effort by a leading AI company to shape competition policy in its favor, potentially challenging Google's dominance in search. If adopted, it could accelerate the integration of conversational AI into mainstream search ecosystems and give users more choice beyond traditional search engines. OpenAI argues that services like ChatGPT, which offer conversational or multimodal information discovery, are functionally similar to Google's own AI Overviews and AI Mode features. It also recommends using transparent, dynamic popularity metrics to determine which services qualify and expanding the choice screen to include voice, visual, and AI-assisted search entry points.

telegram · zaihuapd · Mar 23, 14:50

**Background**: The UK's Competition and Markets Authority (CMA) is a regulatory body responsible for promoting competition and preventing anti-competitive practices. Google's search choice screen is a mechanism, mandated by regulators in some regions like the EU and UK, that appears on Android devices and Chrome to let users select a default search engine from a list of options, aiming to reduce Google's default advantage. AI Overviews and AI Mode are Google's own AI-powered search features that provide summarized answers and conversational interactions, respectively, moving beyond traditional link lists.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_Overviews">AI Overviews - Wikipedia</a></li>
<li><a href="https://frankknow.com/google-ai-mode/">AI Mode 是什麼？Google 搜尋進化！教你提升被 AI 引用的機會</a></li>

</ul>
</details>

**Tags**: `#AI Regulation`, `#Search Competition`, `#OpenAI`, `#UK CMA`, `#ChatGPT`

---

<a id="item-3"></a>
## [Guide to migrating digital services from US to EU providers for data sovereignty](https://rz01.org/eu-migration/) ⭐️ 7.0/10

A comprehensive guide and discussion has been published, detailing practical strategies for migrating digital services and infrastructure away from US-based corporations to EU-based alternatives. The conversation includes specific technical implementation details, legal considerations across different jurisdictions, and comparative analysis of service providers. This matters because it addresses growing concerns about privacy, data sovereignty, and reducing dependency on US tech giants, especially in light of EU regulations like GDPR. A successful migration can help individuals and organizations better control their data, comply with regional laws, and potentially mitigate risks associated with foreign surveillance or data access laws. The discussion acknowledges that migration is complex, often reaching about 90% completion with lingering small dependencies, and that some EU-based services may still have indirect ties to US companies. It also highlights practical challenges, such as configuring email sending from custom domains with certain providers.

hackernews · exitnode · Mar 23, 10:17

**Background**: Data sovereignty refers to the concept that data is subject to the laws and governance structures of the country where it is located. The EU has established a strong legal framework for data protection, notably the General Data Protection Regulation (GDPR), which aims to give individuals control over their personal data. Cloud migration strategies are systematic approaches for moving digital assets and infrastructure between environments, such as from on-premises or one cloud provider to another. EU-based cloud alternatives, such as OVHcloud and STACKIT, are often promoted for their compliance with EU data protection regulations.

<details><summary>References</summary>
<ul>
<li><a href="https://incountry.com/blog/the-eus-data-sovereignty-framework/">The EU’s data sovereignty framework - InCountry</a></li>
<li><a href="https://www.digitalocean.com/resources/articles/cloud-migration-strategy">Complete Cloud Migration Strategy Guide: Planning and ...</a></li>
<li><a href="https://www.softwareseni.com/comparing-european-cloud-providers-and-open-source-alternatives-to-us-platforms/">Comparing European Cloud Providers and Open Source ...</a></li>

</ul>
</details>

**Discussion**: Community sentiment is engaged and practical, with users sharing personal migration experiences and specific provider recommendations (e.g., mailbox.org). However, the discussion also includes critical viewpoints questioning whether EU jurisdictions offer substantially better privacy protections, citing concerns about local law enforcement powers and cross-border evidence orders. Some comments promote EU-based alternatives to specific US services.

**Tags**: `#privacy`, `#data-sovereignty`, `#digital-migration`, `#EU-regulation`, `#service-providers`

---

<a id="item-4"></a>
## [GitHub's reliability reportedly falls to 'three nines' availability amid outages and security concerns.](https://www.theregister.com/2026/02/10/github_outages/) ⭐️ 7.0/10

GitHub is reportedly experiencing significant availability issues, with its overall platform reliability potentially dropping to around 99.9% (three nines), which translates to over 8 hours of downtime per year. This comes alongside recent security vulnerabilities, such as the exploitation of mutable references in GitHub Actions that led to a breach at Aqua Security and potentially infected thousands of CI/CD runs. GitHub is foundational infrastructure for the global software development ecosystem, and its declining reliability directly impacts millions of developers and businesses that depend on it for code hosting, collaboration, and CI/CD. This situation raises critical questions about the trade-offs between rapid feature expansion (like AI tools) and maintaining core platform stability and security, especially during a major infrastructure migration to Azure. The 'three nines' (99.9%) availability metric is a significant drop from the 'five nines' (99.999%) standard often expected for critical services, allowing for over 8 hours of downtime annually. Critics point to the ongoing migration of GitHub's infrastructure to Microsoft Azure, announced in 2025 with promises of improved reliability, as a potential root cause of the instability.

hackernews · richtr · Mar 23, 10:39

**Background**: In system reliability engineering, availability is often measured in 'nines.' 'Three nines' means 99.9% uptime, equating to about 8.76 hours of permissible downtime per year. For context, 'five nines' (99.999%) allows only about 5.26 minutes of downtime annually. GitHub Actions is GitHub's CI/CD platform that automates software workflows, and 'mutable references' within it can be a security risk if not properly secured, as they allow artifacts to be changed after creation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_availability">High availability - Wikipedia</a></li>
<li><a href="https://docs.github.com/en/actions/concepts/metrics">About GitHub Actions metrics</a></li>

</ul>
</details>

**Discussion**: The community expresses strong frustration, highlighting a perceived focus on AI features like Copilot at the expense of core platform stability and security. Many link the reliability issues directly to the mandated migration to Azure, citing past assurances from GitHub leadership that the move would improve availability. There is also significant concern about long-standing, unaddressed security flaws in GitHub Actions being exploited in real attacks.

**Tags**: `#infrastructure`, `#reliability`, `#devops`, `#cloud-services`, `#security`

---

<a id="item-5"></a>
## [Research compares JavaScript sandboxing techniques including isolated-vm, vm2, QuickJS, ShadowRealm, and Deno Workers](https://simonwillison.net/2026/Mar/22/javascript-sandboxing-research/#atom-everything) ⭐️ 7.0/10

Simon Willison conducted research comparing multiple JavaScript sandboxing techniques after being inspired by Aaron Harper's article about Node.js worker threads. The research, assisted by Claude Code, systematically evaluated isolated-vm, vm2, quickjs-emscripten, QuickJS-NG, ShadowRealm, and Deno Workers for secure code execution. This research matters because secure JavaScript sandboxing is fundamental for applications that need to execute untrusted code, such as online code editors, plugin systems, and serverless platforms. The comparison provides practical guidance for developers choosing isolation solutions in Node.js and JavaScript runtime environments. The research specifically examined isolated-vm which provides access to V8's Isolate functionality, ShadowRealm which is a Stage 2.7 ECMAScript proposal for isolated execution environments, and QuickJS implementations including both the original and NG fork. The comparison was prompted by exploring whether Node.js worker threads could enhance sandboxing security.

rss · Simon Willison · Mar 22, 19:53

**Background**: JavaScript sandboxing refers to techniques that isolate and execute untrusted code within a controlled environment to prevent access to sensitive system resources. isolated-vm is a Node.js library that leverages V8's Isolate API to create secure execution contexts. ShadowRealm is a TC39 proposal that aims to provide standardized synchronous isolated environments within the JavaScript language itself. QuickJS is a small, embeddable JavaScript engine that can be compiled to WebAssembly via quickjs-emscripten for browser or Node.js use.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/laverdet/isolated-vm">GitHub - laverdet/isolated-vm: Secure & isolated JS environments for nodejs · GitHub</a></li>
<li><a href="https://github.com/tc39/proposal-shadowrealm">GitHub - tc39/proposal-shadowrealm: ECMAScript Proposal ...</a></li>
<li><a href="https://deepwiki.com/tc39/proposal-shadowrealm">tc39/proposal-shadowrealm | DeepWiki</a></li>

</ul>
</details>

**Tags**: `#javascript`, `#sandboxing`, `#security`, `#runtime-environments`, `#nodejs`

---

<a id="item-6"></a>
## [Interactive Visualizer Created to Demonstrate Bram Cohen's CRDT-Based Version Control Concept](https://simonwillison.net/2026/Mar/22/manyana/#atom-everything) ⭐️ 7.0/10

Simon Willison created an interactive web tool called the Merge State Visualizer using Claude AI and Pyodide to demonstrate Bram Cohen's Manyana project, a 470-line Python proof-of-concept for CRDT-based version control. The tool provides a visual interface to understand how the conflict-free merge algorithms work in practice. This matters because it makes an advanced distributed systems concept accessible to developers, potentially accelerating understanding and adoption of CRDT-based approaches in version control. As AI-assisted development grows, tools that visualize complex algorithms become increasingly valuable for education and prototyping. The visualizer was built by feeding Cohen's Python code (minus comments) into Claude AI to generate an explanation, then using Pyodide to create the browser-based interactive interface. Manyana itself is described as a demo rather than a complete version control system, with features like cherry-picking and local undo not yet implemented.

rss · Simon Willison · Mar 22, 18:57

**Background**: CRDTs (Conflict-free Replicated Data Types) are data structures that enable distributed systems to maintain consistency across multiple replicas without requiring conflict resolution. Bram Cohen, creator of the BitTorrent protocol, recently proposed Manyana as a vision for applying CRDT principles to version control systems. Pyodide is a technology that allows Python to run directly in web browsers through WebAssembly.

<details><summary>References</summary>
<ul>
<li><a href="https://bramcohen.com/p/manyana">Manyana - by Bram Cohen - Bram’s Thoughts</a></li>
<li><a href="https://crdt.tech/">About CRDTs • Conflict-free Replicated Data Types</a></li>
<li><a href="https://scribbler.live/2024/07/08/Python-in-Browser.html">Python in the Browser with Pyodide</a></li>

</ul>
</details>

**Tags**: `#version-control`, `#crdt`, `#visualization`, `#python`, `#ai-tools`

---