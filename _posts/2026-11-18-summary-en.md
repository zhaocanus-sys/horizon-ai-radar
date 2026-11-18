---
layout: default
title: "Horizon Summary: 2026-11-18 (EN)"
date: 2026-11-18
lang: en
---

> From 27 items, 22 important content pieces were selected

---

1. [Java4Shell: Critical RCE in OpenJDK's Base64 Decoder](#item-1) ⭐️ 9.0/10
2. [OpenAI releases GPT-6.2 Astra and Sol with major cost and speed gains](#item-2) ⭐️ 9.0/10
3. [Quad9 Exits France Over DNS Blocking Orders, Cloudflare Warns](#item-3) ⭐️ 8.0/10
4. [Google's AI answers reportedly cut search traffic by 40%](#item-4) ⭐️ 8.0/10
5. [Microsoft's ONNX Runtime GitHub Repository Goes Offline](#item-5) ⭐️ 8.0/10
6. [Microsoft launches MAI Code 2 and Code 2 Flash coding models](#item-6) ⭐️ 8.0/10
7. [SolidJS 2.0 Released with Server RPC and Agent-Friendly Diagnostics](#item-7) ⭐️ 8.0/10
8. [Simon Willison and Prime Radiant release external sandbox pattern for coding agents](#item-8) ⭐️ 8.0/10
9. [Datasette Lite rewritten with service workers and Pyodide to run full server app in browser](#item-9) ⭐️ 8.0/10
10. [AI Summaries Threaten Independent Site All About Berlin](#item-10) ⭐️ 7.0/10
11. [IRS sign-in requires ID.me, sparking privacy and accessibility concerns](#item-11) ⭐️ 7.0/10
12. [Nvidia stops disclosing Singapore sales as subsidiary revenue hits $104B](#item-12) ⭐️ 7.0/10
13. [Highly Classified US National Security Communications Network Goes Down](#item-13) ⭐️ 7.0/10
14. [Phrack Issue 73 Released with Docker Escape Exploit](#item-14) ⭐️ 7.0/10
15. [Harvard study finds AI coding agents shift bottleneck to code review](#item-15) ⭐️ 7.0/10
16. [Blog benchmarks agent harness and model combinations on terminal tasks](#item-16) ⭐️ 7.0/10
17. [Tencent Releases Hy4 Flash Open-Weights Model](#item-17) ⭐️ 7.0/10
18. [Web Browser Engineering: A Book on Building a Browser from Scratch](#item-18) ⭐️ 7.0/10
19. [Job candidate says YC startup used LinkedIn account without permission](#item-19) ⭐️ 6.0/10
20. [Archive Team races to preserve Apple Support Community before 2026 closure](#item-20) ⭐️ 6.0/10
21. [jQuery 4.1.0 Released, Sparking Nostalgia and Design Discussions](#item-21) ⭐️ 6.0/10
22. [Ole Rømer's 1676 Discovery of Light's Finite Speed Commemorated](#item-22) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Java4Shell: Critical RCE in OpenJDK's Base64 Decoder](https://calif.io/java4shell/) ⭐️ 9.0/10

Researchers disclosed a critical remote code execution vulnerability in OpenJDK, tracked as CVE-2026-114938 and dubbed Java4Shell, which is triggered when processing Base64-encoded data on CPUs supporting AVX-512. The flaw allows unauthenticated attackers to corrupt heap memory and potentially execute arbitrary code, with a CVSSv4.0 score of 9.2. This vulnerability affects a vast number of Java-based systems, including servers, cloud services, and enterprise applications, and can be exploited remotely without authentication. Given the widespread use of OpenJDK and the potential for remote code execution, it poses a significant risk to critical infrastructure and could lead to large-scale breaches. The vulnerability resides in the optimized assembly code for AVX-512 Base64 decoding, and exploitation requires network-based heap grooming (Remote Heap Feng Shui) that is sensitive to network conditions such as RTT and jitter. While denial of service is easier to achieve, reliable remote code execution demands additional tailoring to the application and JVM environment.

hackernews · werrett · Nov 17, 21:11 · [Discussion](https://news.ycombinator.com/item?id=50538240)

**Background**: OpenJDK is the open-source implementation of the Java Platform, Standard Edition, and its HotSpot JVM includes optimized assembly routines for common operations like Base64 encoding and decoding. AVX-512 is an advanced CPU instruction set that accelerates vectorized operations, and the vulnerable code path is only present in HotSpot-based JDKs (including Oracle JDK and GraalVM) when running on AVX-512-capable hardware. Heap grooming, also known as heap feng shui, is an exploitation technique that manipulates memory allocation patterns to place controlled data at predictable locations, increasing the reliability of memory corruption exploits.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wiz.io/blog/cve-2026-114938-rce-java4shell-openjdk">CVE-2026-114938 OpenJDK RCE (Java4Shell): Everything You Need ...</a></li>
<li><a href="https://securitylabs.datadoghq.com/articles/java4shell-remote-code-execution-in-openjdk-cve-2026-114938/">Java4Shell: Remote Code Execution in OpenJDK (CVE-2026-114938)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Heap_feng_shui">Heap feng shui - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community has reacted with a mix of awe and concern: some praised the sophistication of the remote heap grooming exploit, while others shared detection tools like Semgrep's scripts and noted that the attack is sensitive to network conditions. There is also speculation that the vulnerability may be related to the AVX-512 implementation and could be mitigated by disabling AVX-512 with the -XX:UseAVX=2 flag, though this remains unconfirmed.

**Tags**: `#security`, `#Java`, `#OpenJDK`, `#RCE`, `#exploit`

---

<a id="item-2"></a>
## [OpenAI releases GPT-6.2 Astra and Sol with major cost and speed gains](https://openai.com/index/introducing-gpt-6-2-astra-sol/) ⭐️ 9.0/10

OpenAI has released GPT-6.2 Astra, its new frontier model for demanding projects, and GPT-6.2 Sol, an efficient model for everyday work, both producing better results with fewer output tokens. The models are now available via API and GitHub Copilot, with early testers reporting top-tier performance and significant cost reductions. The release signals a shift toward more cost-efficient frontier AI, with community benchmarks showing comparable accuracy at a fraction of previous costs, which could make advanced AI more accessible for businesses and developers at scale. However, criticism of office-task quality highlights persistent gaps in document and presentation generation. In independent evaluations, GPT-6.2 Astra topped a parametric CAD harness and scored 92 on PacBench (6.6 min, $2.04), while GPT-6.2 Sol scored 87 (6.3 min); in data analytics, Astra's cost dropped from ~$20 to ~$4 and Sol's from $2.6 to $1.2 with similar accuracy, partly due to a 20% token reduction and fewer tool calls. Some users noted cases where the model 'finished early' and missed answers, and office document examples were criticized as poor.

hackernews · jasondavies · Nov 17, 17:46 · [Discussion](https://news.ycombinator.com/item?id=50535230)

**Background**: GPT-6.2 Astra and Sol are incremental updates to OpenAI's GPT-6 family, with Astra positioned as the high-end frontier model and Sol as the efficient, versatile variant. 'Frontier model' refers to the most advanced model a lab offers for complex tasks, while 'output tokens' are the units of text the model generates, directly affecting cost and speed. Benchmarks like PacBench and CAD harnesses are community-run tests that evaluate models on specific tasks such as game generation or 3D modeling.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-6-2-astra-sol/">Introducing GPT-6.2 Astra and Sol | OpenAI</a></li>
<li><a href="https://github.blog/changelog/2026-11-17-openais-gpt-6-2-astra-and-gpt-6-2-sol-now-available/">OpenAI’s GPT-6.2 Astra and GPT-6.2 Sol now available</a></li>
<li><a href="https://plotly.com/blog/gpt-6-2-sol-plotly-data-analytics-bench/">GPT-6.2 Sol Benchmark Results for Data Analysis - Plotly</a></li>

</ul>
</details>

**Discussion**: Community reaction is largely positive on performance and cost: testers report Astra and Sol as top models in CAD evals and data analytics, with dramatic cost reductions and fast speeds. However, some users criticize the quality of office/document outputs (slides, workbooks, memos) as notably poor, and note occasional premature completion that misses answers.

**Tags**: `#openai`, `#llm`, `#model-release`, `#benchmarks`, `#ai`

---

<a id="item-3"></a>
## [Quad9 Exits France Over DNS Blocking Orders, Cloudflare Warns](https://blog.cloudflare.com/quad9-withdrawal-from-france/) ⭐️ 8.0/10

Quad9, a public DNS resolver, has withdrawn its services from France in response to DNS blocking orders, as reported by Cloudflare's blog. The move was discussed on Hacker News with Quad9's CTO, who confirmed the withdrawal and highlighted broad support for their position at IETF 127. This event sets a precedent for how DNS resolvers respond to government blocking orders, potentially affecting internet freedom and the availability of public DNS services in Europe. It raises questions about corporate accountability and the future of privacy-focused DNS resolvers like Quad9, Cloudflare, and Google. Quad9's withdrawal means users in France may no longer access its security and privacy-focused DNS service, which blocks malicious domains. The orders target DNS blocking of pirate sites, and other providers like Cloudflare, Google, and OpenDNS are responding differently, with Cloudflare not committing to withdrawal.

hackernews · subset · Nov 17, 22:13 · [Discussion](https://news.ycombinator.com/item?id=50538994)

**Background**: DNS (Domain Name System) translates domain names into IP addresses, and public DNS resolvers like Quad9 provide alternative services with added security and privacy features. DNS blocking orders require resolvers to prevent access to certain domains, often for copyright enforcement, which can conflict with privacy and freedom of information. Quad9 is a non-profit resolver that emphasizes user privacy and security.

<details><summary>References</summary>
<ul>
<li><a href="https://codekhabar.com/post/france-orders-isps-to-ready-dns-blocks-for-major-social-platforms-on-oct-24">France DNS Block Order for Social Media on Oct 24... — CodeKhabar</a></li>
<li><a href="https://torrentfreak.com/dns-piracy-blocking-orders-google-cloudflare-and-opendns-respond-differently-250511/">DNS Piracy Blocking Orders : Google, Cloudflare, and... * TorrentFreak</a></li>
<li><a href="https://on.quad9.net/">A public and free DNS service for a better security and privacy</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion, with 160 comments, shows strong support for Quad9 and concern over internet overregulation. Quad9's CTO noted general dread at IETF about DNS blocking, while users criticized Cloudflare for not committing to similar action and lamented the decline of European internet freedoms.

**Tags**: `#DNS`, `#internet-regulation`, `#privacy`, `#France`, `#Cloudflare`

---

<a id="item-4"></a>
## [Google's AI answers reportedly cut search traffic by 40%](https://revscope.co/blog/search-seo-geo-2026/) ⭐️ 8.0/10

A report claims that Google's AI-generated search answers are reducing search traffic by 40%, sparking debate about the death of SEO and the future of web discovery. This shift could fundamentally change how websites attract visitors and monetize content, affecting publishers, SEO professionals, and the entire web ecosystem. The 40% figure is speculative and not officially confirmed by Google; the discussion also highlights concerns about AI-generated answers being gamed and the potential loss of diverse web content.

hackernews · slashdev · Nov 18, 00:17 · [Discussion](https://news.ycombinator.com/item?id=50540178)

**Background**: Google's AI-powered search features, such as AI Overviews, use generative AI to synthesize direct answers from multiple sources instead of just linking to websites. SEO (search engine optimization) is the practice of optimizing web content to rank higher in search results, and a decline in search traffic could disrupt the online publishing economy.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/products-and-platforms/products/search/generative-ai-search/">How Google is improving Search with Generative AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Search_engine_optimization">Search engine optimization - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters have mixed feelings: some welcome the end of clickbait and praise AI for directly answering queries, while others mourn the loss of web discovery and worry about ads in AI outputs and the gaming of AI answers. A few note that ChatGPT has already reduced their Google usage far more than 40%.

**Tags**: `#AI`, `#search`, `#SEO`, `#Google`, `#web`

---

<a id="item-5"></a>
## [Microsoft's ONNX Runtime GitHub Repository Goes Offline](https://github.com/microsoft/onnxruntime) ⭐️ 8.0/10

Microsoft's ONNX Runtime GitHub repository, which had approximately 22,000 stars, has unexpectedly gone offline, with no advance warning or official explanation from Microsoft. ONNX Runtime is a widely used cross-platform inference accelerator, and its sudden disappearance disrupts dependent machine learning pipelines and raises concerns about supply chain security in open-source AI infrastructure. The repository's disappearance coincides with reports of a compromised PyPI package for Microsoft's Agent Framework, leading to speculation that the takedown may be a security response; however, Microsoft has not confirmed the cause.

hackernews · nvader · Nov 17, 23:18 · [Discussion](https://news.ycombinator.com/item?id=50539610)

**Background**: ONNX Runtime is an open-source runtime for executing machine learning models in the Open Neural Network Exchange (ONNX) format, developed by Microsoft and used across many frameworks and platforms. GitHub repositories can be taken offline for various reasons, including security incidents, accidental deletion, or policy violations.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/microsoft/onnxruntime">GitHub - microsoft/onnxruntime: ONNX Runtime : cross-platform, high...</a></li>

</ul>
</details>

**Discussion**: Commenters speculate that the takedown may be linked to a compromised PyPI package for Microsoft's Agent Framework, with some noting that ONNX automatically exfiltrates telemetry data unless disabled. Others report pipeline failures and express concern about the lack of warning for a repository with 22k stars.

**Tags**: `#ONNX Runtime`, `#GitHub`, `#supply chain security`, `#Microsoft`, `#open source`

---

<a id="item-6"></a>
## [Microsoft launches MAI Code 2 and Code 2 Flash coding models](https://microsoft.ai/news/introducing-mai-code-2-and-mai-code-2-flash/) ⭐️ 8.0/10

Microsoft introduced MAI Code 2 and MAI Code 2 Flash, two coding-focused models that claim near-frontier performance at a fraction of the cost of competing models. MAI Code 2 is positioned for enterprise coding tasks and production code, while Code 2 Flash targets high-volume, routine development work. This release intensifies competition in the AI coding assistant market, where Microsoft can leverage its GitHub Copilot distribution to challenge OpenAI and Anthropic. The claimed cost-performance advantage could pressure rivals' pricing and accelerate adoption of specialized coding models in enterprise workflows. According to Microsoft, MAI Code 2 delivers 98% of GPT-6.1 Sol's performance at 40% of the cost and 96% of Claude Opus 5.5's at 5% of the cost. MAI Code 2 Flash is a lightweight, cost-efficient variant optimized for code explanations, targeted edits, and rapid iteration, and a further-optimized MAI Work Flash serves multiple Microsoft products across M365 and Fabric IQ.

hackernews · lemonish97 · Nov 17, 18:25 · [Discussion](https://news.ycombinator.com/item?id=50535885)

**Background**: MAI Code 2 and Code 2 Flash are Microsoft's latest entries in the competitive market for large language models specialized for software development. These models are designed to assist with tasks like code generation, debugging, and test creation, and they are being integrated into GitHub Copilot's model selector. The AI coding assistant space has seen rapid iteration, with models from OpenAI, Anthropic, and others vying for developer adoption based on benchmark performance and cost.

<details><summary>References</summary>
<ul>
<li><a href="https://microsoft.ai/news/introducing-mai-code-2-and-mai-code-2-flash/">MAI Code 2 and Code 2 Flash : Everyday coding at... | Microsoft AI</a></li>
<li><a href="https://microsoft.ai/models/mai-code-2/">MAI Code 2 | Microsoft AI</a></li>
<li><a href="https://github.blog/changelog/2026-11-17-mai-code-2-and-mai-code-2-flash-in-github-copilot/">MAI Code 2 and MAI Code 2 Flash in GitHub... - GitHub Changelog</a></li>

</ul>
</details>

**Discussion**: Commenters reported positive early experiences with MAI Code 2 in GitHub Copilot, with one user noting it resolved tricky Python build issues and Azure deployment problems comparably to Claude Opus. Others debated the sustainability of OpenAI and Anthropic's lead, speculated that MAI Code 2 might be a smaller specialized model, and questioned the benchmark cost comparisons. Some expressed frustration with GitHub Copilot's value, with one team canceling their subscription.

**Tags**: `#AI/ML`, `#coding-models`, `#Microsoft`, `#LLM-benchmarks`, `#developer-tools`

---

<a id="item-7"></a>
## [SolidJS 2.0 Released with Server RPC and Agent-Friendly Diagnostics](https://www.solidjs.com/blog/solid-2-0-the-long-hold/) ⭐️ 8.0/10

SolidJS has announced version 2.0, reaching stable after five years of development. The release introduces new server RPC, live, and broadcast primitives, first-class async support in the reactive graph, optimistic actions, draft-first stores, and diagnostics designed to be 'Built to Be Written by Agents'. This is a major release for a notable reactive UI framework, aiming to seamlessly bridge the client-server gap with primitives that feel more natural than alternatives like LiveView or htmx. The focus on agent-friendly developer experience also reflects a growing trend of optimizing frameworks for AI-assisted coding. The release includes server functions, async in the reactive graph, and a smaller API surface. Community members note that the 'Built to Be Written by Agents' features are essentially better debug diagnostics that also benefit human developers, and migration from 1.0 to 2.0 RC has been documented by early adopters.

hackernews · pier25 · Nov 17, 18:56 · [Discussion](https://news.ycombinator.com/item?id=50536387)

**Background**: SolidJS is a JavaScript UI library that uses fine-grained reactivity instead of a virtual DOM, meaning only specific computations re-execute when data changes, leading to efficient updates. Solid 2.0 builds on this foundation by adding server-side capabilities and async primitives to simplify full-stack development. The framework has gained attention for its performance and intuitive model, often compared to React.

<details><summary>References</summary>
<ul>
<li><a href="https://www.solidjs.com/blog/solid-2-0-the-long-hold/">Solid 2.0 - The Long Hold - solidjs.com</a></li>
<li><a href="https://github.com/solidjs-community/solid-primitives">GitHub - solidjs-community/solid-primitives: A library of ... Solid Primitives Overview - SolidJS Documentation @solid-primitives/broadcast-channel - npm Solid: Fine-grained reactive UI</a></li>
<li><a href="https://primitives.solidjs.community/">Solid Primitives</a></li>

</ul>
</details>

**Discussion**: HN commenters praised Solid's seamless server RPC, live, and broadcast primitives as more natural than LiveView or htmx, and one noted that the agent-friendly diagnostics also improve human developer experience. Others shared migration experiences from Solid 1.0 to 2.0 RC and expressed admiration for the team's passion, though some noted the still-limited component library ecosystem.

**Tags**: `#solidjs`, `#javascript`, `#frontend`, `#reactive-programming`, `#web-frameworks`

---

<a id="item-8"></a>
## [Simon Willison and Prime Radiant release external sandbox pattern for coding agents](https://simonwillison.net/2026/Nov/17/external-sandboxes-for-coding-agents/) ⭐️ 8.0/10

Simon Willison and Prime Radiant introduced the 'external sandbox' pattern, where agent-executed code runs in a dedicated sandbox while the agent itself stays outside, and released three sandbox server implementations (v86, container, quicksand) that expose the same localhost API for tools like Pi, Claude Code, and Codex. This addresses a pressing safety concern: prompt injection or agent mistakes could otherwise damage the host machine, and the pattern makes it safer to experiment with local models. The concrete, reusable implementations lower the barrier for developers to adopt sandboxing in agent workflows. The three implementations are external-sandbox-v86 (Node.js server running Alpine Linux in WebAssembly via v86), external-sandbox-container (Python server using Apple Containers), and external-sandbox-quicksand (Python server using Microsoft's Quicksand, which bundles QEMU and Alpine Linux). They also include an optional HTTP/HTTPS allow-list proxy and a credential replacement mechanism so the agent can make authenticated API calls without seeing secrets.

rss · Simon Willison · Nov 17, 22:52

**Background**: Coding agents like Claude Code and Codex can execute arbitrary code and shell commands, so a mistake or prompt injection attack—where hidden instructions in content trick the agent—could compromise the whole development environment. Sandboxing isolates that execution, and the external sandbox pattern keeps the agent outside the sandbox so it can still orchestrate work while the risky code runs in a contained environment. Prime Radiant is the AI research lab behind Superpowers, a composable skills framework for coding agents.

<details><summary>References</summary>
<ul>
<li><a href="https://primeradiant.com/superpowers/">Superpowers | Prime Radiant</a></li>
<li><a href="https://primeradiant.com/about/">About | Prime Radiant</a></li>
<li><a href="https://zybe.ai/blog/what-a-prompt-injection-looks-like-on-a-laptop">Prompt Injection Attacks on AI Agents : a Real Example · ZYBE</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#sandboxing`, `#security`, `#prompt-injection`, `#developer-tools`

---

<a id="item-9"></a>
## [Datasette Lite rewritten with service workers and Pyodide to run full server app in browser](https://simonwillison.net/2026/Nov/17/datasette-lite/) ⭐️ 8.0/10

Simon Willison released a complete rewrite of Datasette Lite that uses service workers and Pyodide to run the full Datasette Python application directly in the browser. The new version supports loading any released Datasette version from PyPI, specific GitHub commits/tags/branches, over 100 SQLite versions, and installing additional plugins from PyPI or wheel URLs. This demonstrates that a full server-side Python web application can run client-side with near-parity, enabling shareable URLs that reproduce demos or bugs without spinning up a server. It lowers the barrier for sharing interactive data explorations and plugin demos, and signals broader momentum for Python-in-the-browser via WebAssembly. URL parameters like ?install=datasette-maplibre and &url=... allow chaining plugin installs and loading SQLite databases, JSON, CSV, or SQL scripts; the example loads a GeoJSON country database with the datasette-maplibre plugin to render maps. Service workers act as a programmable proxy to intercept requests, which is how the Python app's HTTP handling is emulated in the browser.

rss · Simon Willison · Nov 17, 16:48

**Background**: Datasette is an open-source tool for exploring and publishing data as an interactive website and API, typically run as a Python server. Pyodide is a port of CPython to WebAssembly that lets Python code and packages run in the browser, while service workers are background scripts that can intercept and handle network requests. Datasette Lite combines these to run Datasette entirely client-side, and the rewrite makes it behave almost like the real server-side application.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/pyodide/pyodide">GitHub - pyodide/pyodide: Pyodide is a Python distribution ... Pyodide — Version 314.0.8 Pyodide — Version 314.1.0.dev0 Pyodide - GitHub Running Python in the Browser with Pyodide | Wasm Docs</a></li>
<li><a href="https://web.dev/learn/pwa/service-workers/">Service workers - web.dev Using Service Workers - Web APIs | MDN - MDN Web Docs Service Workers Deep Dive: What Actually Happens in the Browser Service worker overview | Workbox | Chrome for Developers Service Worker API - Web APIs | MDN - MDN Web Docs</a></li>
<li><a href="https://github.com/simonw/datasette">GitHub - simonw/datasette: An open source multi-tool for ... Datasette: An open source multi-tool for exploring and ... Getting started - Datasette documentation Installation - Datasette documentation datasette-python · PyPI Datasette</a></li>

</ul>
</details>

**Tags**: `#WebAssembly`, `#Pyodide`, `#Datasette`, `#Service Workers`, `#Python`

---

<a id="item-10"></a>
## [AI Summaries Threaten Independent Site All About Berlin](https://nicolasbouliane.com/blog/death-by-ai) ⭐️ 7.0/10

Nicolas Bouliane, owner of the Berlin-focused website All About Berlin, published a blog post describing how AI-generated summaries and chatbots are reducing traffic and revenue for his site. The post sparked a Hacker News discussion with 95 comments about the ethics and long-term viability of AI companies profiting from freely available human content. This highlights a growing economic threat to independent content creators, as AI search features like Google's AI Overviews and chatbots increasingly answer user queries directly, reducing the need to click through to source websites. If unchecked, this trend could undermine the open web's incentive structure, leaving less high-quality human-generated content available for AI training and for society. The article is a personal account from the site owner, and the Hacker News discussion includes comments from users like jeppester, adamddev1, and bodge5000 debating whether it is acceptable for large AI companies to take human work without payment and replace jobs with technology built on that work. Some commenters, like helsinkiandrew, argue that users prefer AI summaries over clicking through potentially outdated or affiliate-driven links.

hackernews · grey-area · Nov 18, 06:47 · [Discussion](https://news.ycombinator.com/item?id=50542705)

**Background**: AI-powered search summaries, such as Google's AI Overviews, and conversational chatbots are increasingly used to answer user queries directly on the search results page or in chat interfaces, which can reduce traffic to the original websites that provided the information. This has led to concerns among publishers and independent creators about revenue loss, as their content is used to train AI models and generate answers without compensation or attribution. The debate touches on issues of copyright, fair use, and the sustainability of the open web.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2602.18455">Impact of AI Search Summaries on Website Traffic: Evidence ... Google AI Overviews Impact on Traffic: 2026 Data Explained Impact of AI Search Summaries on Website Traffic: Evidence ... Google AI Search Summaries Slash Website Traffic – What ... AI Impact on Website Traffic: 2026 Report - First Page Sage Impact of AI Search Summaries on Website Traffic: Evidence ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49752056">Microsoft exec called AI scraping 'the largest theft of labor ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration with large AI companies profiting from freely available human content without compensation, with some questioning the long-term viability of an ecosystem where AI simultaneously relies on and discourages openly published human work. Others noted that users often prefer AI-generated summaries over clicking through links of unknown quality, highlighting a tension between convenience and supporting original content creators.

**Tags**: `#AI ethics`, `#content economics`, `#open web`, `#Hacker News discussion`, `#sustainability`

---

<a id="item-11"></a>
## [IRS sign-in requires ID.me, sparking privacy and accessibility concerns](https://consumerrights.wiki/w/ID.me_terms_required_for_IRS_sign-in) ⭐️ 7.0/10

A Hacker News discussion highlighted that the IRS requires ID.me for sign-in, with users sharing frustrations about accessibility and privacy and noting alternatives like login.gov. This matters because it affects many taxpayers who may face barriers to accessing government services, and it raises questions about the role of third-party identity providers in federal digital identity. Users noted that ID.me requires a smartphone for sign-up, which can exclude those without one, and that the federal government aims to offer login.gov as an alternative within two years.

hackernews · DeepLogin · Nov 18, 00:51 · [Discussion](https://news.ycombinator.com/item?id=50540437)

**Background**: ID.me is a digital identity verification service used by government agencies to confirm users' identities online. Login.gov is a single sign-on solution for U.S. federal government websites, allowing users to access multiple agencies with one account. The IRS has been using ID.me for identity verification, but some users have raised concerns about privacy and accessibility.

<details><summary>References</summary>
<ul>
<li><a href="https://www.id.me/individuals/government">Verify Your Identity to Access Government Services | ID.me</a></li>
<li><a href="https://en.wikipedia.org/wiki/Login.gov">Login.gov - Wikipedia</a></li>
<li><a href="https://www.login.gov/">The public’s one account for government. | Login.gov</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration that ID.me requires a smartphone, making it impossible for some to access services like TreasuryDirect, and some shared workarounds or noted that login.gov is now accepted for IRS sign-in. Others questioned why ID.me isn't available for non-government use, highlighting broader interest in verified digital identity.

**Tags**: `#digital identity`, `#privacy`, `#government services`, `#accessibility`, `#ID.me`

---

<a id="item-12"></a>
## [Nvidia stops disclosing Singapore sales as subsidiary revenue hits $104B](https://www.ft.com/content/dbde7a30-548c-4f9d-a4be-7898a0c24dcf) ⭐️ 7.0/10

Nvidia has stopped disclosing its Singapore sales figures after its Singaporean subsidiary's external revenue reached $104 billion in 2025, up 72% year over year, according to company accounts reviewed by the Financial Times. The change in disclosure comes amid geopolitical scrutiny over whether advanced AI chips are being routed to China through Singapore, and it could affect investor visibility into Nvidia's revenue sources and raise concerns about sanctions compliance. The $104 billion figure represents external revenue of Nvidia's Singaporean subsidiary, which includes orders routed through the entity, not necessarily end demand from Singapore; Nvidia also switched its quarterly revenue reporting in SEC filings after July 2025, making Singapore's contribution less visible.

hackernews · louiereederson · Nov 17, 17:12 · [Discussion](https://news.ycombinator.com/item?id=50534631)

**Background**: Nvidia designs GPUs that are crucial for AI development, and like many chip companies, it sells through a network of OEMs, ODMs, and resellers rather than directly to end customers. Singapore has become a major billing hub for Nvidia, accounting for nearly a fifth of its global revenue last year, but the country does not enforce other nations' unilateral export controls, leading to concerns that chips could be diverted to China.

<details><summary>References</summary>
<ul>
<li><a href="https://www.channelnewsasia.com/singapore/nvidia-ai-chips-us-export-controls-singapore-deepseek-china-4944231">Singapore does not condone businesses who use local ties to bypass...</a></li>
<li><a href="https://www.bbc.com/news/articles/ck1exevgql4qo">Nvidia : How the Jensen Huang scandal exposed a headache for...</a></li>
<li><a href="https://stockanalysis.com/stocks/nvda/">NVIDIA (NVDA) Stock Price & Overview</a></li>

</ul>
</details>

**Discussion**: Commenters debated the significance of the disclosure change, with some clarifying that the $104B is external revenue of the Singapore subsidiary and includes orders routed through it, while others speculated about sanctions evasion and noted the timing of Nvidia's reporting change in SEC filings.

**Tags**: `#Nvidia`, `#revenue-disclosure`, `#sanctions`, `#semiconductors`, `#geopolitics`

---

<a id="item-13"></a>
## [Highly Classified US National Security Communications Network Goes Down](https://www.cnn.com/2026/11/17/politics/highly-classified-national-security-communications-network-goes-down) ⭐️ 7.0/10

A highly classified US national security communications network, reportedly used by the National Security Agency (NSA), went down, prompting an investigation according to CNN and Reuters reports from November 17, 2026. The outage of a top-secret network highlights vulnerabilities in critical government infrastructure and raises concerns about IT competence and the growing threat of AI-assisted cyberattacks, affecting national security operations and public trust. The network is likely part of the NSA's classified intranet, possibly related to JWICS or SIPRNet, which handle top-secret and secret-level communications; the cause remains unclear, and public disclosure of such an outage is unusual.

hackernews · monkeydust · Nov 17, 15:38 · [Discussion](https://news.ycombinator.com/item?id=50532849)

**Background**: JWICS (Joint Worldwide Intelligence Communications System) is the most secure US government network for top-secret information, while SIPRNet handles secret-level communications. These networks are isolated from the public internet and are critical for military and intelligence operations. Outages are rare and typically not publicly announced due to security concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Joint_Worldwide_Intelligence_Communications_System">Joint Worldwide Intelligence Communications System - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/SIPRNet">SIPRNet - Wikipedia</a></li>
<li><a href="https://www.breitbart.com/tech/2026/11/17/report-outage-highly-classified-nsa-network-prompts-investigation/">Report: Outage of Highly Classified NSA Network Prompts...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters debated the causes, with some blaming corporate IT downsizing trends and others speculating about AI-assisted attacks; many expressed surprise at the public disclosure and called for competent, well-paid IT staff across sectors.

**Tags**: `#cybersecurity`, `#national-security`, `#infrastructure`, `#IT-operations`, `#hackernews`

---

<a id="item-14"></a>
## [Phrack Issue 73 Released with Docker Escape Exploit](https://phrack.org/issues/73/introduction_md) ⭐️ 7.0/10

Phrack issue 73 has been released, featuring technical security articles including a Docker escape exploit, and has sparked nostalgic and ethical discussion on Hacker News. Phrack remains a culturally significant hacker zine with substantive technical content, and its release prompts important discussions about vulnerability disclosure ethics and the evolution of computer security. The issue includes a Docker escape exploit, and community members question whether such exploits are responsibly disclosed with CVEs or dropped without warning.

hackernews · notmine1337 · Nov 17, 18:31 · [Discussion](https://news.ycombinator.com/item?id=50535992)

**Background**: Phrack is an e-zine written by and for hackers, first published in 1985, covering topics from phreaking to cybersecurity. It is widely read by both hackers and security professionals and is considered a cultural document of the hacker scene.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Phrack_Magazine">Phrack Magazine</a></li>
<li><a href="https://phrack.org/">Phrack Magazine</a></li>
<li><a href="https://www.paloaltonetworks.com/blog/cloud-security/leaky-vessels-vulnerabilities-container-escape/">Container Escape: New Vulnerabilities Affecting Docker and ... Docker Fixes CVE-2025-9074, Critical Container Escape ... Docker security announcements | Docker Docs Docker Escape: Breaking Out of Containers - by Ruben Santos Docker CopyEscape Vulnerability Lets Containers Write Outside ... Docker Container Escape Vulnerabilities Guide - safeguard.sh Escaping Docker Containers in 2026: Exploiting CVE-2026-31431 ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed nostalgia for earlier eras of Phrack and phreaking, questioned the disclosure ethics of the Docker escape exploit, and appreciated the unpolished, expressive nature of the zine compared to modern professional comments.

**Tags**: `#security`, `#hacking`, `#phrack`, `#exploit`, `#community`

---

<a id="item-15"></a>
## [Harvard study finds AI coding agents shift bottleneck to code review](https://complexdiscovery.com/harvard-researchers-find-ai-coding-agents-shifted-the-bottleneck-to-code-review/) ⭐️ 7.0/10

A Harvard working paper by economists Fiona Chen and James Stratton analyzed roughly 300 million work events across more than 700 software firms from 2021 through March 2026, finding that AI coding agents were associated with about 30% more lines of code, 20% more commits, and 23% more pull requests per worker, but no significant increase in completed issues. This research quantifies a major shift in software engineering workflows: AI agents accelerate code generation but push the bottleneck to human code review, potentially limiting overall productivity gains and raising questions about review practices, code ownership, and quality assurance. The study estimates each worker added about 1,500 extra lines of code per month after AI agent adoption, yet finished output remained flat, suggesting review capacity and process constraints absorb the extra volume; the findings are correlational and based on work-event telemetry rather than controlled experiments.

hackernews · judahmeek · Nov 17, 21:16 · [Discussion](https://news.ycombinator.com/item?id=50538303)

**Background**: AI coding agents are LLM-powered tools that can autonomously write, debug, test, and document code, and they are increasingly integrated into developer workflows via IDEs and CLIs. Code review—the process where peers inspect proposed changes before merging—has long been a quality gate, but it can become a bottleneck when the volume of changes outpaces reviewer capacity. The Harvard paper uses large-scale telemetry from software firms to measure how agent adoption affects code volume and shipped work.

<details><summary>References</summary>
<ul>
<li><a href="https://tech-insider.org/ai-coding-agents-30-percent-more-code-not-software-2026/">AI Coding Agents: 30% More Code, No More Finished Work</a></li>
<li><a href="https://letsdatascience.com/news/harvard-study-finds-ai-coding-agents-raise-code-volume-not-o-ea78729b">Harvard study finds AI coding agents add code while review ...</a></li>
<li><a href="https://aiweekly.co/alerts/harvard-study-ai-coding-agents-lift-code-30-shipped-output-flat">Harvard Study: AI Coding Agents Lift Code 30%, Shipped Output ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that code review has become the new bottleneck, with some noting the research feels dated relative to fast-moving industry practice. Others debate radical alternatives, such as dropping traditional PR reviews in favor of continuous system-level review, and question whether code ownership and reviewer expertise will erode as AI writes more code.

**Tags**: `#AI coding agents`, `#code review`, `#software engineering`, `#developer productivity`, `#research`

---

<a id="item-16"></a>
## [Blog benchmarks agent harness and model combinations on terminal tasks](https://runta.com/blog/introducing-frontierharness-eval-v1-1/) ⭐️ 7.0/10

A blog post on runta.com introduced FrontierHarness Eval v1.1, benchmarking various agent harness and model combinations on terminal tasks. The post sparked a Hacker News discussion with 366 points and 125 comments, where commenters questioned the headline framing and debated how much harness choice matters relative to model capability. As LLM-based coding agents become more widely used, understanding whether performance gains come from the model or the surrounding harness is critical for developers choosing tools and for benchmark designers. The discussion highlights that evaluation methodology and framing can significantly shape how results are interpreted by the community. Commenters noted that 64% of spending went to tasks that did not pass Terminal Bench verifiers, and the original headline was changed after criticism. One commenter argued that harnesses are fairly simple loops and that model choice dominates performance, while another contended that as models become more capable, the harness matters more than the model.

hackernews · Edward40 · Nov 17, 14:53 · [Discussion](https://news.ycombinator.com/item?id=50532191)

**Background**: An agent harness is the runtime around a language model that turns it into an agent, including the step loop, tool access, file and service permissions, and rules or checks. Terminal-Bench is an open-source benchmark that measures how well AI agents complete real, complex tasks in a command-line environment, such as compiling code, configuring servers, or debugging. The FrontierHarness Eval appears to compare different harness and model pairings on such terminal tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://handbook.modular.com/model-interaction/agent-harnesses/">Agent harnesses | LLM Inference Handbook</a></li>
<li><a href="https://www.tbench.ai/">TERMINAL - BENCH</a></li>
<li><a href="https://qaskills.sh/blog/terminal-bench-agent-benchmark-guide-2026">Terminal - Bench Guide: Benchmarking AI Agents (2026) | QASkills.sh</a></li>

</ul>
</details>

**Discussion**: Commenters criticized the original clickbait headline and unclear benchmark interpretation, with seizethecheese suspecting the framing was designed to pander to 'wasting money on AI' upvotes. xyzzy_plugh argued that the best harness depends on the problem and that as models become more capable, the harness appears to matter more than the model, while cpeth countered that harnesses are simple loops and barely matter for overall performance.

**Tags**: `#ai-agents`, `#llm-evaluation`, `#coding-agents`, `#benchmarking`, `#hacker-news`

---

<a id="item-17"></a>
## [Tencent Releases Hy4 Flash Open-Weights Model](https://hy.tencent.ai/research/hy4-flash) ⭐️ 7.0/10

Tencent released Hy4 Flash, an open-weights model with 224 billion total parameters (including 64 billion Engram parameters) and only 12 billion active parameters, supporting multimodal inputs and up to 1M tokens of context. It is available on Hugging Face, ModelScope, and GitCode, and scored well on Plotly's independent data analytics benchmarks, beating GPT-6 Luna on cost-efficiency. This model offers frontier-competitive performance at a very low cost, with Plotly's benchmark showing only $0.13 to answer 43 data analytics questions compared to ~$20 for expensive frontier models. It intensifies competition in the open-weights LLM space, potentially driving down prices and expanding access to high-quality AI for everyday workflows. Hy4 Flash has 224B total parameters with 64B Engram parameters and 12B active parameters, enabling efficient inference. It supports multimodal inputs and a 1M token context length, and is released alongside an FP8 version and a pre-trained base model.

hackernews · lyra1337 · Nov 17, 21:06 · [Discussion](https://news.ycombinator.com/item?id=50538184)

**Background**: Open-weights models are those whose trained parameters are publicly released, allowing anyone to download, run, and fine-tune them, in contrast to proprietary models accessible only via APIs. Tencent's Hy model family is a series of large language models, and Hy4 Flash is a cost-efficient variant of the flagship Hy4, designed for lower latency and cost. DeepSeek is another prominent Chinese AI company known for releasing open-weights models, and comparisons to DeepSeek highlight the competitive landscape.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/tencent/Hy4-flash">tencent / Hy 4 - flash · Hugging Face</a></li>
<li><a href="https://www.tencent.com/tencent-launches-hy4-flash-to-power-high-speed-cost-efficient-ai-deployment-for-everyday-workflows/">Tencent Launches Hy 4 flash to Power High-Speed... - Tencent</a></li>
<li><a href="https://openrouter.ai/tencent/hy4-flash">Hy 4 flash - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Discussion**: Community members praised Hy4 Flash for its strong performance on data analytics benchmarks and low cost, with some noting it beats DeepSeek Flash in their usage. Users expressed excitement about increased competition driving down prices and features, and curiosity about running the model locally on two 128GB machines.

**Tags**: `#llm`, `#open-weights`, `#model-release`, `#benchmarks`, `#ai-pricing`

---

<a id="item-18"></a>
## [Web Browser Engineering: A Book on Building a Browser from Scratch](https://browser.engineering/) ⭐️ 7.0/10

The book 'Web Browser Engineering' by Pavel Panchekha and Chris Harrelson, which teaches how to build a complete web browser from first principles in Python, was recently published by Oxford University Press in 2025. The online version has been available since 2021 and is now accompanied by author commentary and community discussion. This book fills a gap in systems and software engineering education by demystifying the inner workings of web browsers, which are ubiquitous but often opaque. It provides a hands-on, incremental approach that benefits students, developers, and anyone curious about browser internals. The book guides readers through building a basic but complete browser in a few thousand lines of Python, covering networking, parsing, layout, and JavaScript. The code for each chapter is available on GitHub, and the book requires Python 3.9+ and additional packages like dukpy and skia for later chapters.

hackernews · ibobev · Nov 17, 20:01 · [Discussion](https://news.ycombinator.com/item?id=50537290)

**Background**: Web browsers are complex software that transform HTML, CSS, and JavaScript into interactive visual representations. A browser engine (or layout engine) is the core component responsible for this transformation, and building one from scratch is a monumental challenge attempted by few projects like Ladybird and Lightpanda. This book systematically explains all major components of a browser, making the topic accessible to a wide audience.

<details><summary>References</summary>
<ul>
<li><a href="https://browser.engineering/">Web Browser Engineering</a></li>
<li><a href="https://github.com/browserengineering/book">GitHub - browserengineering/book: Web browser engineering (a ... Web Browser Engineering - Oxford Academic Web Browser Engineering - Paperback - Pavel Panchekha; Chris ... Web Browser Engineering Web Browser Engineering - Google Books</a></li>
<li><a href="https://www.amazon.com/Web-Browser-Engineering-Pavel-Panchekha/dp/0198913869">Web Browser Engineering: Panchekha, Pavel, Harrelson, Chris ...</a></li>

</ul>
</details>

**Discussion**: The discussion was positive, with the author clarifying that the book was written without AI assistance and sharing its timeline. Commenters expressed enthusiasm, with one noting they are building their own browser and finding the book a valuable resource, while another linked to previous discussions on Hacker News.

**Tags**: `#web browsers`, `#systems programming`, `#education`, `#book`, `#software engineering`

---

<a id="item-19"></a>
## [Job candidate says YC startup used LinkedIn account without permission](https://reddit.com/r/recruitinghell/comments/1xyr6ml/interviewed_at_a_yc_startup_spent_30_hours/) ⭐️ 6.0/10

A job candidate interviewing at a Y Combinator-backed startup was asked to connect their personal LinkedIn account to the company's platform as a prerequisite, and later discovered the account had been used without proper permission, according to a Reddit post that drew 62 comments. The incident highlights growing privacy and consent concerns around how early-stage startups handle candidates' personal data, and it raises questions about whether linking third-party accounts during interviews should be treated as an ethical and legal red line. Commenters debated whether the candidate handed over credentials or merely linked the account via OAuth, and some argued the company could face legal liability for unauthorized use of profile data; the original post is anecdotal and the startup was not named.

hackernews · throwawaysleep · Nov 18, 05:11 · [Discussion](https://news.ycombinator.com/item?id=50542135)

**Background**: Y Combinator is a well-known startup accelerator that has funded over 5,000 companies since 2005, so its alumni carry reputational weight. LinkedIn's OAuth flow lets third-party apps request scoped access to a member's profile data, but LinkedIn's user agreement prohibits scraping or using data without consent, and the platform has pursued legal action against unauthorized data collection.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Y_Combinator">Y Combinator - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/linkedin/shared/authentication/authorization-code-flow">LinkedIn 3-Legged OAuth Flow - LinkedIn | Microsoft Learn</a></li>
<li><a href="https://www.codewords.ai/blog/scraping-linkedin-profiles">Scraping LinkedIn profiles: methods, risks, and pipelines</a></li>

</ul>
</details>

**Discussion**: Commenters were largely critical, with several saying they would refuse to hand over account passwords and others calling the practice "basically illegal" and urging the candidate to sue; one commenter questioned whether the issue was credential sharing or API-based account linking, while another suggested the candidate should have been compensated for leads generated.

**Tags**: `#startups`, `#ethics`, `#privacy`, `#recruiting`, `#LinkedIn`

---

<a id="item-20"></a>
## [Archive Team races to preserve Apple Support Community before 2026 closure](https://wiki.archiveteam.org/index.php/Apple_Discussions) ⭐️ 6.0/10

Archive Team is actively archiving the Apple Support Community, which Apple has announced will permanently close on November 20, 2026. Volunteers can track progress via the Archive Team tracker and contribute by running the ArchiveTeam Warrior virtual appliance. This effort highlights the growing role of volunteer archivists in preserving online history when corporations decline to do so, and it raises questions about corporate responsibility for maintaining access to user-generated support content that many people rely on. The archive is being coordinated through Archive Team's wiki and tracker, with the ArchiveTeam Warrior allowing anyone to easily donate bandwidth and storage. The closure date of November 20, 2026, gives volunteers a window to capture the forum's content before it disappears.

hackernews · digitaldragon · Nov 17, 23:32 · [Discussion](https://news.ycombinator.com/item?id=50539747)

**Background**: Archive Team is a volunteer group known for rescuing dying websites and online communities from deletion, often using distributed tools like the ArchiveTeam Warrior. The Apple Support Community is a long-running forum where users help each other troubleshoot Apple products, but Apple has decided to shut it down, prompting concerns about the loss of valuable troubleshooting knowledge.

<details><summary>References</summary>
<ul>
<li><a href="https://tracker.archiveteam.org/">ArchiveTeam Warrior</a></li>
<li><a href="https://www.youtube.com/watch?v=_nzD-QpmePE">Save Internet History With ArchiveTeam Warrior - YouTube</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed views: some found the forum unhelpful and full of misinformation, even welcoming its removal, while others criticized Apple for not archiving it themselves, arguing that corporations should preserve years of human effort. The overall sentiment leaned toward disappointment with Apple's lack of action.

**Tags**: `#digital-preservation`, `#apple`, `#online-communities`, `#archiving`, `#corporate-responsibility`

---

<a id="item-21"></a>
## [jQuery 4.1.0 Released, Sparking Nostalgia and Design Discussions](https://github.com/jquery/jquery/releases/tag/4.1.0) ⭐️ 6.0/10

jQuery 4.1.0 has been released as a minor update to the classic JavaScript library, following the major 4.0.0 release. The release itself is incremental, but it has generated substantial community discussion about jQuery's legacy and enduring design patterns. Although jQuery is no longer essential for modern web development, its event model and chaining patterns continue to influence framework design. The release highlights the library's ongoing maintenance and its role in supporting a large portion of the web. jQuery 4.0.0 was a major release that dropped support for older browsers and removed deprecated APIs, and the 3.x branch now only receives critical updates. The 4.1.0 update is a minor release with no groundbreaking changes, but it ensures compatibility and bug fixes for current users.

hackernews · petecooper · Nov 17, 19:50 · [Discussion](https://news.ycombinator.com/item?id=50537156)

**Background**: jQuery is a JavaScript library created in 2006 to simplify DOM manipulation, event handling, and Ajax across different browsers. It became ubiquitous in the 2010s, but modern browser APIs like querySelector and classList, along with frameworks like React and Vue, have reduced its necessity for new projects. Nevertheless, jQuery remains widely used in legacy systems and simple websites.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/jquery/jquery">GitHub - jquery / jquery : jQuery JavaScript Library · GitHub</a></li>
<li><a href="https://jquery.com/download/">Download jQuery | jQuery : The Write Less, Do More, JavaScript Library</a></li>

</ul>
</details>

**Discussion**: Commenters expressed nostalgia and appreciation for jQuery's design, particularly its event model that allows events on any object and its elegant method chaining. Some noted that while jQuery's original use cases have diminished, it still offers value for minor enhancements and remains a historical achievement that shaped modern JavaScript development.

**Tags**: `#jQuery`, `#JavaScript`, `#library release`, `#web development`, `#community discussion`

---

<a id="item-22"></a>
## [Ole Rømer's 1676 Discovery of Light's Finite Speed Commemorated](https://www.sciencenorway.no/culture-history-history-of-science/350-years-ago-this-man-discovered-that-light-has-a-finite-speed/2737969) ⭐️ 6.0/10

A ScienceNorway article commemorates the 350th anniversary of Ole Rømer's 1676 demonstration that light travels at a finite speed, based on his observations of Jupiter's moon Io. The story sparked a lively Hacker News discussion with over 300 points and 90 comments. Rømer's work was the first clear demonstration that light has a measurable speed, overturning the prevailing belief that light travels instantaneously. It remains a foundational moment in the history of science and continues to inspire discussions about measurement and discovery. Rømer timed eclipses of Jupiter's moon Io and noticed discrepancies in their predicted times depending on Earth's distance from Jupiter, leading to an estimate of light's speed about one-quarter too low. His method was correct, and the discrepancy was later explained by the finite speed of light.

hackernews · dxs · Nov 17, 19:25 · [Discussion](https://news.ycombinator.com/item?id=50536813)

**Background**: In the 17th century, many scientists, including Descartes, believed that light traveled instantaneously. Ole Rømer, a Danish astronomer working at the Royal Observatory in Paris, used the timing of eclipses of Jupiter's moon Io to show that light has a finite speed. By comparing the observed times of the eclipses when Earth was at different points in its orbit, he estimated the speed of light, though his value was about 25% too low.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rømer's_determination_of_the_speed_of_light">Rømer 's determination of the speed of light - Wikipedia</a></li>
<li><a href="https://www.amnh.org/learn-teach/curriculum-collections/cosmic-horizons-book/ole-roemer-speed-of-light">Ole Roemer Profile: First to Measure the Speed of Light | AMNH</a></li>

</ul>
</details>

**Discussion**: Commenters shared enthusiasm for the history of science, recommending books like 'Lightspeed' by Ken Gormley and discussing the precision of 17th-century clocks. Some asked for resources on other historical measurements, such as Eratosthenes' calculation of Earth's circumference, and others linked to a web comic and a sci-fi trilogy inspired by the topic.

**Tags**: `#history-of-science`, `#physics`, `#speed-of-light`, `#astronomy`, `#hacker-news`

---