---
layout: default
title: "Horizon Summary: 2026-11-19 (EN)"
date: 2026-11-19
lang: en
---

> From 27 items, 23 important content pieces were selected

---

1. [Google Releases Gemini 4 Neon Frontier Model](#item-1) ⭐️ 9.0/10
2. [Critical unauthenticated RCE found in Nginx HTTP/2](#item-2) ⭐️ 9.0/10
3. [Anthropic Prices IPO at $1.5T Valuation, Raising $105B](#item-3) ⭐️ 9.0/10
4. [OpenAI Releases GPT-6.2 Astra and Sol with Lower API Prices](#item-4) ⭐️ 9.0/10
5. [Ruby Patches Seven Memory Corruption Vulnerabilities in Regexp and String Case Conversion](#item-5) ⭐️ 8.0/10
6. [Microsoft Unveils Seven New AI Models at Ignite 2026](#item-6) ⭐️ 8.0/10
7. [LLM-Assisted Reverse Engineering Sparks Debate on Process and Productivity](#item-7) ⭐️ 8.0/10
8. [Google DeepMind releases Genie 4 generative world model for AI Ultra subscribers](#item-8) ⭐️ 8.0/10
9. [Interactive site lets you explore Voyager 1 down to a single memory chip](#item-9) ⭐️ 8.0/10
10. [Datasette Lite rewritten with service workers and Pyodide to run full server-side app in browser](#item-10) ⭐️ 8.0/10
11. [Inside Deutsche Bank: 15 Million Leaked Files Expose Systemic Failures](#item-11) ⭐️ 7.0/10
12. [DaisyRose-27B: Post-Trained Qwen Variant Sparks Debate on Benchmarks](#item-12) ⭐️ 7.0/10
13. [Unreal Tournament 2004 Ported to Run in the Browser](#item-13) ⭐️ 7.0/10
14. [Blog Post Argues Companies Need Smart People Who Care, Sparking HN Debate](#item-14) ⭐️ 7.0/10
15. [OpenAI touts AI models for chip design, sparking debate](#item-15) ⭐️ 7.0/10
16. [Gemini 4 Neon emerges as a top-tier Opus 5.5 competitor](#item-16) ⭐️ 7.0/10
17. [KPMG trial finds AI agents ask better audit questions than accountants](#item-17) ⭐️ 7.0/10
18. [curl Maintainer Questions AI Rust Rewrites' Ability to Keep Up](#item-18) ⭐️ 7.0/10
19. [Simon Willison and Prime Radiant introduce external sandbox pattern for coding agents](#item-19) ⭐️ 7.0/10
20. [ExitPath: Open-Source Alternatives to Slack, Notion, and Microsoft 365](#item-20) ⭐️ 6.0/10
21. [US Air Force Seeks Next-Gen Data Cartridge for F-22](#item-21) ⭐️ 6.0/10
22. [llm-gemini 0.38 adds Gemini 4 Neon support amid pricing confusion](#item-22) ⭐️ 6.0/10
23. [datasette-arrows 0.1a0 Adds Apache Arrow Streaming Export to Datasette](#item-23) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Google Releases Gemini 4 Neon Frontier Model](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/) ⭐️ 9.0/10

Google announced Gemini 4 Neon, a new frontier model in its Gemini 4 family, designed for complex coding, analytical reasoning, and production-grade enterprise workflows. The release quickly became a top Hacker News discussion with 754 points and 630 comments. This release expands Google's frontier model lineup and intensifies competition with Anthropic's Opus and OpenAI's GPT models, giving developers more options for agentic enterprise tasks. It also highlights the trend of model families with specialized variants rather than a single flagship. Neon is positioned as a balanced model between Carbon (long-horizon tasks) and Hydrogen (fast everyday execution), and early users report it serving at 127 tokens per second on OpenRouter, much faster than Carbon's 46 tokens per second. Despite higher overall scores on some benchmarks, it scores lower on research-scale reasoning evaluations like CritPt compared to Carbon.

hackernews · yigitdemirag · Nov 18, 21:34 · [Discussion](https://news.ycombinator.com/item?id=50552424)

**Background**: Gemini is Google's family of large multimodal AI models, offered in different sizes and versions through the Gemini API, AI Studio, and Vertex AI. A frontier model refers to a model at or near the leading edge of capability at a given time, typically from a small number of AI labs. The Gemini 4 family includes multiple variants like Carbon, Neon, and Hydrogen, each optimized for different use cases.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-4-neon/">Gemini 4 Neon - Model Card — Google DeepMind</a></li>
<li><a href="https://aistudio.google.com/docs/models/gemini-4-neon">Gemini 4 Neon - Gemini API | Google AI Studio</a></li>
<li><a href="https://www.laurenceo.com/intelligence/glossary/frontier-ai-model">What Is Frontier AI model ? Definition and Why It Matters</a></li>

</ul>
</details>

**Discussion**: Commenters debated the model's positioning within the Gemini family, noting that Carbon remains the 'long-horizon' model despite Neon's higher overall scores. Some users questioned why Neon, supposedly the flagship, is served much faster than Carbon on OpenRouter, while others compared its real-world intelligence unfavorably to Anthropic's Opus 5.5.

**Tags**: `#AI/ML`, `#LLM`, `#Google Gemini`, `#model release`, `#benchmarks`

---

<a id="item-2"></a>
## [Critical unauthenticated RCE found in Nginx HTTP/2](https://www.wiz.io/blog/nginx-http2-rce-vulnerabilities) ⭐️ 9.0/10

On November 18, 2026, F5 disclosed two critical vulnerabilities, CVE-2026-123007 and CVE-2026-123633, in Nginx's HTTP/2 implementation that allow unauthenticated remote code execution. Both flaws carry a CVSS v4.0 score of 9.2 and affect Nginx Open Source and Nginx Plus. Nginx is one of the most widely deployed web servers, so a remotely exploitable flaw in its HTTP/2 stack poses a significant risk to internet-facing infrastructure. The disclosure has also reignited debate over responsible disclosure practices and the real-world exploitability of the bug. CVE-2026-123007 is an integer underflow in HTTP/2 flow-control accounting that lets an attacker read and overwrite memory in the Nginx worker process, potentially leading to code execution without credentials or user interaction. Exploitation may require large amounts of HTTP/2 traffic and specific CPU instructions, and HTTP/2 is not enabled by default in Nginx.

hackernews · speedping · Nov 18, 15:19 · [Discussion](https://news.ycombinator.com/item?id=50547374)

**Background**: HTTP/2 is a major revision of the HTTP protocol that improves performance through multiplexing and header compression, and it is supported by Nginx when explicitly configured. Remote code execution (RCE) is a class of vulnerability where an attacker can run arbitrary code on a target system, often with severe consequences. Responsible disclosure is the practice of privately reporting vulnerabilities to vendors to allow time for patches before public details are released.

<details><summary>References</summary>
<ul>
<li><a href="https://www.netspi.com/blog/executive-blog/critical-vulnerability/nginx-http-2-critical-remote-code-execution-vulnerability-cve-2026-123007/">NGINX ( HTTP/2 ) – Critical Remote Code Execution ...</a></li>
<li><a href="https://safe.security/resources/blog/cve-2026-123007-cve-2026-123633-nginx-http-2-rce-two-critical-flaws-turn-protocol-handling-into-remote-code-execution/">NGINX HTTP/2 RCE: CVE-2026-123007 & CVE-2026-123633 | SAFE</a></li>
<li><a href="https://www.paruluniversity.ac.in/blog/responsible-disclosure-and-vulnerability-reporting-why-finding-a-bug-is-only-half-the-job/">Responsible Disclosure and Vulnerability Reporting: Why Finding...</a></li>

</ul>
</details>

**Discussion**: Commenters are divided on severity: some argue the bug is a non-issue because it requires 128GB of HTTP/2 traffic and specific CPU instructions, while others criticize the week-long window where the fix was public before disclosure and call for a PSA. Others note that HTTP/2 is not enabled by default and only about 12% of servers use it, though that still represents a huge number at internet scale.

**Tags**: `#nginx`, `#security`, `#vulnerability`, `#http2`, `#rce`

---

<a id="item-3"></a>
## [Anthropic Prices IPO at $1.5T Valuation, Raising $105B](https://www.anthropic.com/news/anthropic-prices-initial-public-offering) ⭐️ 9.0/10

Anthropic has priced its initial public offering, offering 980 million shares of Class A common stock at $83 per share, raising approximately $105 billion in cash and achieving a $1.5 trillion market capitalization. The offering size was increased from a previously planned 825 million shares, and includes $26 billion from strategic investors such as Google and Nvidia, minus $1.9 billion from existing holders selling 23.6 million shares. This is a landmark event for the AI industry, as Anthropic becomes one of the most valuable public companies just five years after its founding, signaling a new era of public-market participation in AI. The IPO could reshape how AI companies access capital and set a benchmark for future AI IPOs, affecting investors, employees, and the broader tech ecosystem. The offering consists of 980 million Class A shares at $83 each, with employees allowed to sell immediately, which some view as a negative signal. The total cash raised includes $81.34 billion from the share sale and $26 billion from strategic investors, net of $1.9 billion from existing holders selling shares.

hackernews · surprisetalk · Nov 18, 23:30 · [Discussion](https://news.ycombinator.com/item?id=50553843)

**Background**: An initial public offering (IPO) is the process by which a private company sells shares to the public for the first time, transitioning to a publicly traded company. Market capitalization is calculated by multiplying the share price by the total number of outstanding shares, representing the total equity value of the company. Anthropic, founded in 2021 by former OpenAI researchers, is an AI safety and research company known for its Claude models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Initial_public_offering">Initial public offering - Wikipedia</a></li>
<li><a href="https://us.plus500.com/en/newsandmarketinsights/market-capitalization-explained-us">Market Capitalization Explained | Plus500</a></li>

</ul>
</details>

**Discussion**: Commenters expressed astonishment at the speed of Anthropic's rise, noting that a company founded in 2021 reached a $1.5T market cap, a valuation Apple didn't achieve until 2020. Some questioned the decision to let employees sell immediately, viewing it as a bad sign, while others highlighted the expanded offering size and the massive wealth creation implied.

**Tags**: `#AI`, `#IPO`, `#Anthropic`, `#finance`, `#industry-news`

---

<a id="item-4"></a>
## [OpenAI Releases GPT-6.2 Astra and Sol with Lower API Prices](https://simonwillison.net/2026/Nov/17/gpt62-astra-and-sol/) ⭐️ 9.0/10

OpenAI has released GPT-6.2 Astra, a new frontier model for complex tasks, and GPT-6.2 Sol, an efficient model for everyday work, both available via API as gpt-6.2-astra and gpt-6.2-sol. Simon Willison shipped LLM 0.38 with support for the new models and noted that Astra is priced at $8/$40 per million input/output tokens, 20% cheaper than its predecessor. The 20% price cut and a 60% reduction in cached input costs ($0.40 vs $1 per million tokens) significantly lower the expense of long-running agentic workflows that repeatedly process large contexts. The release also keeps OpenAI competitive with Anthropic's Claude Fable 5.2, which has identical pricing. GPT-6.2 Sol remains at $2/$10 per million tokens, unchanged from 6.1 Sol and 6 Sol, while Astra matches Claude Fable 5.2's $8/$40 pricing. In Simon Willison's pelican benchmark, Astra produced the most detailed drawing at max effort, but neither model performed as well as Claude Fable 5.2 on a complex Three.js animation task.

rss · Simon Willison · Nov 17, 22:38

**Background**: OpenAI periodically releases new model versions with tiered offerings: a frontier model for demanding tasks and an efficient model for routine use. API pricing is typically quoted per million tokens, and prompt caching allows repeated input content to be billed at a much lower rate, which is especially valuable for agentic applications that maintain long conversation histories. Simon Willison's LLM CLI tool is a popular open-source utility for interacting with language models from the command line, and it often adds support for new models shortly after release.

<details><summary>References</summary>
<ul>
<li><a href="https://llm.datasette.io/">LLM : A CLI utility and Python library for interacting with Large...</a></li>
<li><a href="https://simonwillison.net/2023/Jul/12/llm/">My LLM CLI tool now supports self-hosted language models via plugins</a></li>
<li><a href="https://tokenmix.ai/docs/prompt-caching">Prompt Caching API — Reduce LLM Cost and... | TokenMix Docs</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#LLM`, `#model release`, `#API pricing`, `#agentic AI`

---

<a id="item-5"></a>
## [Ruby Patches Seven Memory Corruption Vulnerabilities in Regexp and String Case Conversion](https://www.ruby-lang.org/en/news/2026/11/18/multiple-vulnerabilities-in-regexp-and-string/) ⭐️ 8.0/10

Ruby disclosed seven vulnerabilities in its regular expression engine and string case conversion, including heap overflows, a double free, and out-of-bounds reads, and released Ruby 4.0.10, 3.4.13, and 3.3.14 to fix them. Proof-of-concept exploits show that some of these flaws can trigger remote code execution. These are memory corruption bugs in core Ruby components, so any application that compiles attacker-controlled regular expressions or processes untrusted strings with case conversion could be exposed to remote code execution. The fact that some were found by autonomous AI models highlights the growing risk that memory-unsafe languages like C, on which Ruby depends, are broadly vulnerable to automated bug discovery. The flaws include a buffer overflow when upcasing the German sharp s (ß) in Windows-1252 encoding, where the character expands to "SS" and the code checks buffer headroom one character at a time, and a Shift_JIS downcase issue that can produce incorrect output or crashes. The advisories note that converting a crafted regular expression to a string may allow information disclosure or remote code execution.

hackernews · runesoerensen · Nov 18, 23:52 · [Discussion](https://news.ycombinator.com/item?id=50554038)

**Background**: Ruby's regular expression engine, Onigmo, is written in C and compiles patterns that can come from user input, such as CI configuration in GitLab. Memory-unsafe languages like C require manual bounds checking, and mistakes can lead to heap overflows, double frees, or out-of-bounds reads that attackers may exploit for code execution. AI models are increasingly being used to find such bugs in established software, as noted in the community discussion.

<details><summary>References</summary>
<ul>
<li><a href="https://www.openwall.com/lists/oss-security/2026/11/19/1">oss-security - Ruby: multiple vulnerabilities in Regexp and ...</a></li>
<li><a href="https://seclists.org/oss-sec/2026/q4/782">Ruby: multiple vulnerabilities in Regexp and String case ...</a></li>
<li><a href="https://www.ruby-lang.org/en/news/2026/10/23/regexp-fixes-for-gitlab-cves/">Regexp compilation fixes related to GitLab's CVE-2026-89078...</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted specific exploitation details, such as the Windows-1252 ß upcasing buffer overflow and a Shift_JIS downcase crash with a crafted string. One commenter argued that autonomous AI models finding these bugs shows memory-unsafe languages are "completely exposed," and warned about attackers using abliterated models at scale without disclosure.

**Tags**: `#security`, `#ruby`, `#memory-safety`, `#vulnerabilities`, `#ai-security`

---

<a id="item-6"></a>
## [Microsoft Unveils Seven New AI Models at Ignite 2026](https://microsoft.ai/news/microsoft-ignite-2026/) ⭐️ 8.0/10

At Ignite 2026, Microsoft announced a family of seven new AI models focused on scalable price-performance, including MAI Code 2, which reportedly reaches 98% of GPT-6.1 Sol's coding quality at about 40% of the price, and MAI Cyber 2 Flash, which beats GPT-6 Astra's quality at less than 2% of the cost per task on the CyberGym-E2E benchmark. This marks Microsoft's most aggressive push yet into first-party frontier models, directly challenging OpenAI and Anthropic on cost-efficiency rather than raw capability, and could pressure competitors to lower prices while giving enterprises a cheaper alternative for coding and security workloads. Microsoft also announced that its second-generation AI accelerator, Maia 200, is now in production running its largest models with 1.7x more tokens per watt, and the lineup includes models for coding, cyber, image, and audio, plus general availability of Microsoft-Decision-1.1.

hackernews · gmays · Nov 18, 16:08 · [Discussion](https://news.ycombinator.com/item?id=50548021)

**Background**: Microsoft has historically relied on OpenAI models for its AI products but has been building its own MAI (Microsoft AI) model family to reduce dependence and control costs. 'Scalable price-performance' refers to delivering competitive quality at much lower cost per task, a key concern as enterprises scale AI workloads. The Ignite conference is Microsoft's annual event for enterprise customers and developers.

<details><summary>References</summary>
<ul>
<li><a href="https://microsoft.ai/news/microsoft-ignite-2026/">Seven new world-class models at scalable price-performance ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neural_scaling_law">Neural scaling law - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were divided: some praised MAI Code 2 as genuinely competitive with Opus and Sol, while others argued Microsoft should open-source or open-weight its models to gain market share, comparing the situation to Windows Phone. A recurring theme was skepticism about Microsoft's innovation and leadership, with some saying they see no reason to use its tech stack.

**Tags**: `#AI/ML`, `#Microsoft`, `#LLM models`, `#model releases`, `#industry competition`

---

<a id="item-7"></a>
## [LLM-Assisted Reverse Engineering Sparks Debate on Process and Productivity](https://www.slowchronicle.com/posts/llm-assisted-reverse-engineering) ⭐️ 8.0/10

A Slow Chronicle article detailing practical methods for using large language models to assist reverse engineering was widely discussed on Hacker News, where commenters shared concrete successes such as reverse engineering a CCTV cloud plugin with Gemini in about two hours and unlocking premium features in Android apps with Codex. The discussion shows LLM-assisted reverse engineering is moving from research curiosity to a practical workflow that can dramatically shorten analysis time for security researchers, hobbyists, and developers, while also raising questions about skill development and over-reliance on AI. Commenters highlighted that LLMs are most effective when guided by a scientific-method approach with definitive experiments, since models like Claude tend to get stuck in guessing loops on harder targets; one noted that Android apps are relatively easy targets for subscription unlocking, while others emphasized that the process itself builds valuable skills.

hackernews · ioma8 · Nov 18, 22:29 · [Discussion](https://news.ycombinator.com/item?id=50553225)

**Background**: Reverse engineering is the process of analyzing compiled software to recover its design, functionality, or source code, and it is traditionally labor-intensive and requires deep expertise. Large language models are increasingly integrated with tools like Ghidra and Radare2 to assist with decompilation, deobfuscation, and binary analysis, as surveyed in recent academic work and curated tool lists.

<details><summary>References</summary>
<ul>
<li><a href="https://www.slowchronicle.com/posts/llm-assisted-reverse-engineering">LLM assisted reverse engineering · Slow Chronicle</a></li>
<li><a href="https://arxiv.org/html/2509.21821v2">Potential and Challenges of Large Language Models for Reverse ...</a></li>
<li><a href="https://github.com/ram-elgov/awesome-llm-reverse-engineering">ram-elgov/awesome- llm - reverse - engineering : A curated list of tools ...</a></li>

</ul>
</details>

**Discussion**: The community is split: some share impressive productivity gains and practical workflows, while others like therepanic argue that using AI removes the satisfaction and skill-building of manual reverse engineering, and Retr0id notes that LLMs still require constant supervision to avoid endless guessing on complex targets.

**Tags**: `#reverse-engineering`, `#LLM`, `#AI-assisted-development`, `#security`, `#tooling`

---

<a id="item-8"></a>
## [Google DeepMind releases Genie 4 generative world model for AI Ultra subscribers](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/genie-4-now-available-project-genie/) ⭐️ 8.0/10

Google DeepMind announced Genie 4, its most interactive generative world model to date, available to eligible Google AI Ultra subscribers. Genie 4 can generate photorealistic, explorable worlds from text and image prompts in real time, and is multimodal, adding synchronized audio such as music, ambient noise, and interactive dialogue. This release pushes generative world models from research demos toward consumer products, potentially transforming game development, simulation, and interactive media. It also intensifies competition among AI labs racing to build general-purpose world simulators, while raising questions about access and pricing. Genie 4 is a spatiotemporal transformer that models both frame content and scene dynamics, and its model card notes improved realism and real-time interactive simulation. Access is currently limited to eligible Google AI Ultra subscribers, with regional and account-type restrictions noted by users.

hackernews · leumon · Nov 18, 18:49 · [Discussion](https://news.ycombinator.com/item?id=50550415)

**Background**: World models are AI systems that learn an internal representation of an environment to predict what happens next, enabling simulation and planning. Google DeepMind's Genie series generates interactive virtual worlds from prompts, and Genie 4 is the latest iteration, building on prior versions that were initially US-only. Google AI Ultra is Google's premium subscription tier that bundles access to advanced AI models and features.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/genie/">Genie 4 — Google DeepMind</a></li>
<li><a href="https://deepmind.google/models/model-cards/genie-4/">Genie 4 - Model Card — Google DeepMind</a></li>
<li><a href="https://en.wikipedia.org/wiki/Genie_(world_model)">Genie (world model) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration over unclear pricing and regional availability, with one noting their UK account only shows Genie 3. Others debated the ethical implications, with one longtime user saying the focus on capability and profitability misses potentially devastating consequences, while another praised DeepMind for pursuing craft over profit.

**Tags**: `#AI`, `#generative models`, `#world models`, `#Google DeepMind`, `#product launch`

---

<a id="item-9"></a>
## [Interactive site lets you explore Voyager 1 down to a single memory chip](https://rshekhar.com/voyager/) ⭐️ 8.0/10

A new interactive website (rshekhar.com/voyager) allows users to explore the Voyager 1 spacecraft's systems in detail, from its nuclear battery to individual memory chips, and includes live tracking of both Voyagers and a 4-minute film. The site was posted on Hacker News as a Show HN and reached the front page with 188 points and 46 comments. This project makes the complex engineering of humanity's most distant spacecraft accessible to a broad audience, combining technical depth with engaging visualization. It highlights the ongoing relevance of Voyager 1 as it reaches the milestone of one light-day from Earth, and fosters public interest in space exploration and engineering heritage. The site includes direct links to specific components such as the radioisotope thermoelectric generator (RTG) with its 24 plutonium spheres, the data computer's memory chips, and a single bit of the command computer's memory. It also features a live map showing which Deep Space Network dish is currently communicating with the spacecraft.

hackernews · raj-shekhar · Nov 18, 16:18 · [Discussion](https://news.ycombinator.com/item?id=50548161)

**Background**: Voyager 1, launched in 1977, is the farthest human-made object from Earth and recently reached a distance of one light-day (about 25.9 billion kilometers). It is powered by three radioisotope thermoelectric generators (RTGs) that convert heat from decaying plutonium-238 into electricity, and it carries the Golden Record, a phonograph record containing sounds and images of Earth. Communication with Voyager is maintained through NASA's Deep Space Network, a global array of large radio antennas.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Radioisotope_thermoelectric_generator">Radioisotope thermoelectric generator - Wikipedia</a></li>
<li><a href="https://science.nasa.gov/mission/voyager/golden-record-cover/">Golden Record Cover - NASA Science</a></li>
<li><a href="https://eyes.nasa.gov/apps/dsn-now/">DSN Now - Deep Space Network Now</a></li>

</ul>
</details>

**Discussion**: The Hacker News community responded positively, with the author providing direct links to hard-to-find sections. Commenters expressed admiration for the engineering of the 1970s, discussed technical details like failure modes of CMOS memory, and raised questions about the project's development process, including whether AI was used.

**Tags**: `#Voyager`, `#interactive-visualization`, `#spacecraft-engineering`, `#hardware`, `#Hacker News`

---

<a id="item-10"></a>
## [Datasette Lite rewritten with service workers and Pyodide to run full server-side app in browser](https://simonwillison.net/2026/Nov/17/datasette-lite/) ⭐️ 8.0/10

Simon Willison released a complete rewrite of Datasette Lite that uses service workers and Pyodide to run the full server-side Datasette Python application directly in the browser. The new version supports selecting any released Datasette version from PyPI, loading specific commits, tags, or branches from GitHub, choosing from over 100 SQLite versions, and installing additional plugins from PyPI or wheel URLs. This makes it possible to link directly to reproducible demos of work-in-progress features or bug reproductions without spinning up a web server, significantly lowering the barrier to sharing and testing Datasette-based work. It also demonstrates a practical, high-fidelity use of WebAssembly-based Python deployment in the browser. The URL parameters allow multiple ?install= flags for plugins, &url= for loading SQLite, JSON, CSV, or SQL files, and &metadata= for metadata configuration. The example demonstrates loading the datasette-maplibre plugin with a GeoJSON database to render interactive maps, showing that even complex visualization plugins work in the browser.

rss · Simon Willison · Nov 17, 16:48

**Background**: Datasette is an open-source tool for exploring and publishing data, built on SQLite and typically run as a Python web server. Pyodide compiles CPython to WebAssembly, allowing Python code and packages to run in the browser, while service workers act as proxy servers between the web app and the network, enabling offline capabilities and request interception. Datasette Lite previously ran a limited version of Datasette in the browser; this rewrite uses service workers to intercept requests and route them to the Pyodide-based Python application, making it nearly indistinguishable from the server-side version.

<details><summary>References</summary>
<ul>
<li><a href="https://pyodide.com/">Home - Pyodide</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API">Service Worker API - Web APIs | MDN</a></li>
<li><a href="https://github.com/simonw/datasette">GitHub - simonw/datasette: An open source multi-tool for ... Getting started - Datasette documentation GitHub - simonw/datasette-lite: Datasette running in your ... Installation - Datasette documentation Datasette: An open source multi-tool for exploring and ... Datasette Tools</a></li>

</ul>
</details>

**Tags**: `#WebAssembly`, `#Pyodide`, `#Datasette`, `#service workers`, `#Python in the browser`

---

<a id="item-11"></a>
## [Inside Deutsche Bank: 15 Million Leaked Files Expose Systemic Failures](https://www.inside-db.com/) ⭐️ 7.0/10

An international consortium of over 200 investigative journalists published a trove of more than 15 million internal Deutsche Bank documents, exposing missed warning signs of money laundering, sanctions violations, and compliance failures. The project, called 'Inside Deutsche Bank,' was discussed on Hacker News, where a reporter involved shared technical details about the data processing pipeline. The leak reveals systemic failures at one of the world's largest banks and could lead to regulatory scrutiny, fines, and reputational damage. It also highlights the growing role of collaborative investigative journalism and data-driven tools in exposing corporate misconduct. The documents, mostly Outlook mailbox exports, were processed using OpenAleph, an ElasticSearch-based tool maintained by DARC, and FollowTheMoney, a data schema for financial crime investigations. The consortium has stated it will not publish the raw data online, citing journalistic evaluation and privacy concerns.

hackernews · gyre007 · Nov 18, 15:38 · [Discussion](https://news.ycombinator.com/item?id=50547620)

**Background**: Deutsche Bank has faced repeated scandals and fines in recent years over money laundering and compliance failures. Investigative journalism consortia like the International Consortium of Investigative Journalists (ICIJ) have previously used large leaks, such as the Panama Papers, to expose financial wrongdoing. OpenAleph and FollowTheMoney are open-source tools designed to help journalists search and analyze massive document sets.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ft.com/content/df518845-ed97-4a38-8a38-7fa9d4d24003?syn-25a6b1a6=1">Leak of 15mn Deutsche Bank files exposes systemic failures</a></li>
<li><a href="https://www.dw.com/en/deutsche-bank-under-fire-after-internal-documents-made-public/a-79974543">Deutsche Bank under fire after internal documents published</a></li>
<li><a href="https://www.himalmag.com/inside-deutsche-bank-leak-investigation/">Inside Deutsche Bank: Leak of 15 million files from Deutsche ...</a></li>

</ul>
</details>

**Discussion**: HN commenters discussed the tech stack, with one reporter detailing the use of OpenAleph and FollowTheMoney. Others criticized the website for lacking a high-level summary of the scandal, and debated the ethics of not publishing raw data, with some arguing that selective omission can mislead the public. A few comments also touched on tax avoidance and unverified conspiracy theories.

**Tags**: `#investigative-journalism`, `#data-processing`, `#ElasticSearch`, `#FollowTheMoney`, `#transparency`

---

<a id="item-12"></a>
## [DaisyRose-27B: Post-Trained Qwen Variant Sparks Debate on Benchmarks](https://www.radixark.com/blog/daisyrose-27b) ⭐️ 7.0/10

RadixArk released DaisyRose-27B, a post-trained variant of Alibaba's Qwen 27B open model, claiming benchmark gains. The model is available on Hugging Face and has drawn significant attention on Hacker News for its performance improvements and local-hardware viability. This demonstrates that smaller companies and independent researchers can meaningfully improve open models through post-training, potentially democratizing access to high-performance LLMs that run on consumer hardware like MacBooks. It also raises questions about whether base model creators like Alibaba are leaving performance on the table. DaisyRose-27B is a dense 27-billion-parameter model that fits on a Mac Mini or MacBook Pro, making it attractive for local deployment. However, the community has raised concerns about overfitting to evaluation benchmarks, as the model's gains may be specific to the eval datasets used during post-training.

hackernews · de_sty · Nov 18, 19:39 · [Discussion](https://news.ycombinator.com/item?id=50551046)

**Background**: Post-training refers to further training of a pre-trained LLM to improve specific capabilities, often using techniques like supervised fine-tuning or reinforcement learning. Qwen 27B is a mid-sized open-weight model from Alibaba's Qwen family, known for its strong performance relative to its size. Benchmark overfitting occurs when a model is optimized too heavily for specific evaluation metrics, leading to inflated scores that may not reflect real-world performance.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/qwen/qwen3.8-27b">Qwen 3.8 27 B - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://en.wikipedia.org/wiki/Post-training_of_large_language_models">Post-training of large language models</a></li>
<li><a href="https://ai-tldr.dev/learn/evaluation-safety/benchmarks-leaderboards/benchmark-overfitting/">What Is Benchmark Overfitting? When Scores Stop Meaning Anything</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement about more post-training efforts on open models, with some noting that Qwen 27B punches above its weight and fits on consumer hardware. However, others raised concerns about heavy reliance on eval datasets, questioning whether AI self-improvement is imminent, and wondered why Alibaba didn't achieve similar gains. Some also asked for before/after results on other benchmarks to assess trade-offs.

**Tags**: `#LLM`, `#post-training`, `#open-models`, `#Qwen`, `#benchmarks`

---

<a id="item-13"></a>
## [Unreal Tournament 2004 Ported to Run in the Browser](https://ut2004.dev/) ⭐️ 7.0/10

A browser-based port of Unreal Tournament 2004 has been released at ut2004.dev, allowing players to run the classic multiplayer first-person shooter directly in a web browser without installation. This project demonstrates the growing capability of WebAssembly and related web technologies to bring complex, resource-intensive PC games to the browser, potentially opening the door to more legacy game preservation and accessible retro gaming. The port runs entirely in the browser, likely leveraging WebAssembly and Emscripten to compile the original game code. While technical details are sparse, the community notes that Epic Games has allowed the OldUnreal project to continue developing a non-browser version, which runs well on Linux.

hackernews · TheAceOfHearts · Nov 19, 01:29 · [Discussion](https://news.ycombinator.com/item?id=50554935)

**Background**: Unreal Tournament 2004 is a classic multiplayer first-person shooter developed by Epic Games and released in 2004. It is built on the Unreal Engine and is renowned for its fast-paced gameplay, diverse game modes, and extensive modding community. WebAssembly is a binary instruction format that allows code written in languages like C and C++ to run in web browsers at near-native speed, enabling complex applications like games to be ported to the web.

<details><summary>References</summary>
<ul>
<li><a href="https://unreal.fandom.com/wiki/Unreal_Tournament_2004">Unreal Tournament 2004 | Unreal Wiki | Fandom</a></li>
<li><a href="https://robaboukhalil.medium.com/porting-games-to-the-web-with-webassembly-70d598e1a3ec">Porting Games to the Web with WebAssembly</a></li>
<li><a href="https://github.com/bitburner/Awesome-Browser-Game-Ports">Awesome Browser Game Ports - GitHub</a></li>

</ul>
</details>

**Discussion**: Commenters express strong nostalgia for the game, praising its creativity in maps, music, and modding culture, with one noting that such a game could never be made with AI. Others ask about the authenticity of the Onslaught server and express interest in seeing other classic games like Star Trek Voyager Elite Force ported to the browser.

**Tags**: `#browser-gaming`, `#webassembly`, `#game-development`, `#unreal-tournament`, `#nostalgia`

---

<a id="item-14"></a>
## [Blog Post Argues Companies Need Smart People Who Care, Sparking HN Debate](https://violetpixel.com/blog/2026-11-17-we-need-smart-people-who-give-a-shit/) ⭐️ 7.0/10

A blog post titled 'We need smart people who give a shit' argues that companies need employees who are both intelligent and genuinely care about their work, and it sparked a rich Hacker News discussion with 494 points and 257 comments. The discussion highlights growing concerns about workplace incentives, management practices, and how AI may be dehumanizing engineering work and eroding craftsmanship, affecting software engineers and organizations broadly. Commenters debated whether the framing is out of touch with industry reality, noted that low pay and politics drive away smart people, and argued that AI reduces the cost of building systems faster than it reduces the cost of understanding them, raising reliability concerns.

hackernews · ExMachina73 · Nov 18, 23:53 · [Discussion](https://news.ycombinator.com/item?id=50554045)

**Background**: The post is an opinion piece on workplace culture and the value of craftsmanship in software engineering. Hacker News discussions often surface tensions around incentives, management, and the impact of AI on engineering practices, making this a representative community conversation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thoughtworks.com/insights/blog/agile-engineering-practices/why-ai-raising-stakes-software-engineering-craft">Why AI is raising the stakes of the software engineering craft</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed that the post's framing is out of touch, arguing that smart people leave when underpaid or forced to play politics, and that telling engineers to babysit LLMs instead of using their own judgment is dehumanizing. Others noted that AI reduces building costs faster than understanding costs, and that maintenance capacity is a key test of societal vigor.

**Tags**: `#workplace-culture`, `#software-engineering`, `#management`, `#AI`, `#craftsmanship`

---

<a id="item-15"></a>
## [OpenAI touts AI models for chip design, sparking debate](https://openai.com/index/advancing-chip-design-with-our-models/) ⭐️ 7.0/10

OpenAI published a blog post describing how its models, including GPT-6 Astra, optimized circuits used in 'Jalapeño' silicon and improved RISC-V core designs, marking its entry into AI-assisted chip design. This signals OpenAI's expansion into semiconductor design, potentially disrupting the EDA industry and raising concerns about AI companies competing with their own customers while having inside knowledge of their work. The post compares successive model versions (GPT-5.5 through 6.2) but lacks a human baseline, and it is unclear whether the RISC-V designs are publicly shared.

hackernews · vighneshiyer · Nov 18, 17:45 · [Discussion](https://news.ycombinator.com/item?id=50549493)

**Background**: Electronic design automation (EDA) is the software used to design and verify integrated circuits. AI agents are increasingly being applied to chip design workflows, with startups like ChipAgents raising significant funding to build agentic AI platforms for chip design.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Electronic_design_automation">Electronic design automation - Wikipedia</a></li>
<li><a href="https://www.businesswire.com/news/home/20260217568914/en/ChipAgents-Raises-$74M-to-Scale-an-Agentic-AI-Platform-to-Accelerate-Chip-Design">ChipAgents Raises $74M to Scale an Agentic AI Platform to Accelerate...</a></li>
<li><a href="https://openai.com/index/advancing-chip-design-with-our-models/">Advancing chip design with OpenAI models | OpenAI</a></li>

</ul>
</details>

**Discussion**: Commenters debated OpenAI competing with its customers, criticized the lack of a human baseline for comparison, and shared practical experiences of using agents to automate EDA workflows and simulations. Some also noted the absence of shared RISC-V designs and appreciated the 'Jalapeño' chip name.

**Tags**: `#AI`, `#chip-design`, `#EDA`, `#OpenAI`, `#hardware`

---

<a id="item-16"></a>
## [Gemini 4 Neon emerges as a top-tier Opus 5.5 competitor](https://micjm.com/blog/gemini-4-neon-looks-like-a-top-model/) ⭐️ 7.0/10

A blog post argues that Google's newly released Gemini 4 Neon is a top-tier model competitive with Anthropic's Opus 5.5, sparking a 69-comment Hacker News discussion about model specialization, orchestration, and coding performance. This signals that Google's Gemini 4 family can now compete at the frontier for coding and enterprise workflows, giving developers a viable alternative to Anthropic's Opus line and intensifying competition in the AI coding tools market. According to Google's model card, Gemini 4 Neon is positioned between Carbon (hardest long-horizon projects) and Hydrogen (fast everyday execution), balancing depth and efficiency for complex coding and analytical reasoning; it offers configurable thinking levels (Low to Extra high) and regional endpoints.

hackernews · seizethecheese · Nov 19, 00:29 · [Discussion](https://news.ycombinator.com/item?id=50554374)

**Background**: Gemini 4 Neon is part of Google DeepMind's Gemini 4 model family, which segments models by workload: Carbon for the hardest long-horizon tasks, Neon for balanced production-grade work, and Hydrogen for fast everyday execution. Opus 5.5 is Anthropic's latest flagship Claude model, released in September 2026, which leads in agentic coding and costs 40% less to run than Opus 5 on typical workloads. Multi-model orchestration—using different LLMs for different roles—has become a common practice among developers building complex software workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-4-neon/">Gemini 4 Neon - Model Card — Google DeepMind</a></li>
<li><a href="https://www.anthropic.com/claude-opus-5-5">Introducing Claude Opus 5.5 \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/models/opus-5-5/overview">Claude Opus 5.5 - Claude Platform Docs</a></li>

</ul>
</details>

**Discussion**: Commenters were divided: one practitioner said other Gemini models looked good in benchmarks but fell short in long-running orchestration, preferring Fable 5.2 as orchestrator with Opus 5.5 as workers; another was impressed and called Neon the first Google model that feels good for coding, while others questioned using pricey models like Fable for routine work and noted that tooling (e.g., Copilot vs. Claude Code) can matter as much as the underlying model.

**Tags**: `#LLM`, `#Gemini`, `#AI coding`, `#model comparison`, `#Hacker News`

---

<a id="item-17"></a>
## [KPMG trial finds AI agents ask better audit questions than accountants](https://europeanbusinessmagazine.com/ai-agents-better-questions-kpmg/) ⭐️ 7.0/10

KPMG conducted an internal trial in which AI agents generated audit questions that were judged to be better than those produced by its own accountants, according to a report covered by European Business Magazine. The finding sparked debate on Hacker News about whether AI can handle complex professional judgment tasks like auditing. Auditing is a high-stakes, judgment-heavy profession, so evidence that AI agents can outperform humans at parts of the workflow signals potential disruption across accounting and professional services. It also raises questions about how firms should evaluate and deploy LLM-based agents in regulated work. The trial was self-conducted by KPMG and the coverage is somewhat promotional, so the results should be treated cautiously; the experiment focused on question generation rather than the full audit process. Commenters noted that auditing requires judging materiality—deciding which issues are significant enough to affect an outside reader's view—not merely finding issues.

hackernews · Betelbuddy · Nov 18, 15:49 · [Discussion](https://news.ycombinator.com/item?id=50547777)

**Background**: AI agents are LLM-based systems that can autonomously carry out multi-step workflows, such as generating and refining audit questions. Auditing traditionally relies on experienced professionals who know where to dig deeper and how to weigh the significance of findings against the overall financial picture. KPMG is one of the Big Four accounting firms, making its internal experiments closely watched as a signal of how LLMs may reshape professional services.

<details><summary>References</summary>
<ul>
<li><a href="https://www.researchgate.net/publication/383069359_Artificial_Intelligence_Agentic_Auditing">(PDF) Artificial Intelligence Agentic Auditing</a></li>
<li><a href="https://alignment.anthropic.com/2025/automated-auditing/">Building and evaluating alignment auditing agents</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were split: some saw auditing as a perfect use case because LLMs reliably remember tedious details, while domain experts pushed back that experienced auditors learn what not to dig into and that an audit is about judging materiality, not just finding issues. Others questioned the credibility of a self-run KPMG experiment and argued AI agents may still struggle with poorly defined tasks, though some predicted properly trained agents could outperform humans by lacking any tendency toward laziness.

**Tags**: `#AI agents`, `#auditing`, `#LLM applications`, `#professional services`, `#AI evaluation`

---

<a id="item-18"></a>
## [curl Maintainer Questions AI Rust Rewrites' Ability to Keep Up](https://simonwillison.net/2026/Nov/18/daniel-stenberg/) ⭐️ 7.0/10

Daniel Stenberg, lead developer of curl, reported that while AI agents converted 185,000 lines of curl's C code into 340,000 lines of Rust over about three weeks, the actual curl project merged over 300 commits and 200 bugfixes in the same period, plus several security fixes. He asks whether these AI-generated Rust clones can keep pace with ongoing maintenance. This highlights a key limitation of AI-driven code translation: generating a large codebase is not the same as maintaining it. For open-source projects and the broader industry evaluating C-to-Rust rewrites for memory safety, it underscores that ongoing bug fixes and security patches are the real measure of a project's health. Stenberg counted the AI-generated Rust code at 340,000 lines versus 185,000 lines of original C, and noted that the clones lack the 200+ bugfixes and vulnerability fixes merged into curl during the same period. He also projects that another month would bring roughly 200 more fixes, widening the maintenance gap.

rss · Simon Willison · Nov 18, 15:58

**Background**: curl is a widely used command-line tool and library (libcurl) for transferring data over network protocols like HTTP, and its codebase is written in C. Rust is a systems programming language known for memory safety, making C-to-Rust translation attractive for reducing security vulnerabilities. AI coding agents have recently been used to perform such large-scale translations, but the resulting code must still be maintained alongside the original project.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rust_(programming_language)">Rust ( programming language ) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#curl`, `#rust`, `#ai-code-generation`, `#open-source-maintenance`, `#security`

---

<a id="item-19"></a>
## [Simon Willison and Prime Radiant introduce external sandbox pattern for coding agents](https://simonwillison.net/2026/Nov/17/external-sandboxes-for-coding-agents/) ⭐️ 7.0/10

Simon Willison and Prime Radiant released three sandbox server implementations—external-sandbox-v86, external-sandbox-container, and external-sandbox-quicksand—that demonstrate an 'external sandbox' pattern where agent-executed code runs in a dedicated sandbox separate from the agent itself. Each implementation exposes the same localhost API, allowing tools like Pi, Claude Code, or Codex to send code execution requests to the sandbox. This pattern addresses a critical security gap in AI coding agents: by isolating code execution from the agent, it reduces the risk of prompt injection attacks or model mistakes causing damaging actions on the host machine. It makes it safer to experiment with local models and provides a reusable foundation for sandboxing untrusted agent-generated code. The three implementations use different isolation technologies: v86 runs Alpine Linux inside WebAssembly via a Node.js server, the container version uses Apple Containers, and the Quicksand version bundles QEMU and Alpine Linux in a Python package. All include an optional HTTP/HTTPS allow-list proxy for controlling network access and a credential replacement mechanism to make authenticated API calls without exposing secrets to the agent.

rss · Simon Willison · Nov 17, 22:52

**Background**: Prompt injection is a class of attack where malicious instructions are hidden in content an AI agent reads, causing the agent to follow the attacker's commands instead of the user's. For coding agents that can execute shell commands, write files, and make network calls, a successful injection can lead to arbitrary code execution or data exfiltration. Sandboxing—running untrusted code in an isolated environment—is a key defense, and the external sandbox pattern extends this by keeping the agent outside the sandbox so that even if the agent is compromised, the blast radius is limited.

<details><summary>References</summary>
<ul>
<li><a href="https://galileo.ai/blog/ai-prompt-injection-attacks-detection-and-prevention">Why Prompt Injection Attacks Are GenAI's #1 Vulnerability | Galileo</a></li>
<li><a href="https://aipatternbook.com/sandbox">Sandbox - Encyclopedia of Agentic Coding Patterns</a></li>
<li><a href="https://primeradiant.com/about/">About | Prime Radiant</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#sandboxing`, `#security`, `#prompt-injection`, `#local-models`

---

<a id="item-20"></a>
## [ExitPath: Open-Source Alternatives to Slack, Notion, and Microsoft 365](https://exitpath-ruddy.vercel.app/) ⭐️ 6.0/10

ExitPath is a new open-source directory that curates alternatives to popular proprietary productivity suites like Slack, Notion, and Microsoft 365. It was recently featured on Hacker News, sparking discussion about the practical challenges of migrating away from these tools. This resource is valuable for organizations considering de-Google or de-Microsoft migrations, as it provides a centralized list of open-source options. It also highlights real adoption blockers such as calendaring, SSO, and operational overhead, which are critical for enterprise adoption. The directory covers alternatives for communication, note-taking, and productivity suites, but community feedback points out missing categories like identity/SSO and calendaring. Self-hosting complexity and user experience are also noted as significant hurdles.

hackernews · zerocool0101 · Nov 18, 16:04 · [Discussion](https://news.ycombinator.com/item?id=50547980)

**Background**: Self-hosting refers to running software on servers you control, often using open-source projects as alternatives to cloud services. Single sign-on (SSO) is an authentication scheme that allows users to log in once to access multiple applications, typically via protocols like SAML or OpenID Connect. Calendaring, especially free/busy scheduling and resource booking, is a key feature of Microsoft Exchange that open-source alternatives often struggle to replicate.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Self-hosting_(network)">Self-hosting (network) - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/boshyan-narek_sso-single-sign-on-explained-sso-can-activity-7170030146475790336-g2p6">SSO ( Single Sign - On ) explained . SSO can be thought of as a master...</a></li>
<li><a href="https://slashdot.org/story/07/11/29/176253/quality-open-source-calendaring--scheduling">Quality Open Source Calendaring / Scheduling? - Slashdot</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted major blockers: difficulty getting open-source solutions running and poor user experience, making it hard to justify time away from revenue-generating work. Calendaring (especially free/busy and resource booking) was cited as a key reason people stick with Outlook/Exchange, and identity/SSO was noted as a critical missing piece for enterprises. Some also mentioned specific tools like Zulip and a new GitHub alternative, MoruForge.

**Tags**: `#open-source`, `#self-hosting`, `#productivity-tools`, `#enterprise-software`, `#migration`

---

<a id="item-21"></a>
## [US Air Force Seeks Next-Gen Data Cartridge for F-22](https://sam.gov/workspace/contract/opp/8948e8601e964c6aba9c801eee16b1be/view) ⭐️ 6.0/10

The US Air Force Materiel Command has posted a contract opportunity for a next-generation micro-Data Transfer Cartridge (mDTC) for the F-22 fighter jet, specifying at least 256 MB of storage and read/write compatibility. This contract highlights the military's ongoing reliance on legacy PCMCIA/CF storage for mission data transfer, affecting all US military aircraft up to the F-35 and platforms like LCACs, and shows how specialized suppliers must maintain outdated tech for critical operations. The mDTC must have at least 256 MB of storage and be readable and writable in a PCMCIA-compatible device; commenters note that these cards often use FPGA/microcontroller with microSD due to broken PCMCIA protocol implementations in aircraft.

hackernews · birdboat00 · Nov 18, 15:35 · [Discussion](https://news.ycombinator.com/item?id=50547583)

**Background**: PCMCIA (Personal Computer Memory Card International Association) cards were once standard for portable storage in laptops, and CompactFlash (CF) cards are electrically compatible with PCMCIA via adapters. Military aircraft use these cards to transfer mission planning data from ground systems to the aircraft before flight. The F-22, a fifth-generation stealth fighter, relies on such cartridges for loading GPS keys, sensor data, and weapons information.

**Discussion**: Commenters shared technical insights: one described building replacement PCMCIA cards with FPGA/microcontroller and microSD to work around broken protocol implementations; another noted that CF cards are still widely used across US military aircraft and LCACs; and a third recommended industrial flash suppliers like Delkin Devices.

**Tags**: `#military-tech`, `#storage`, `#PCMCIA`, `#hardware`, `#aviation`

---

<a id="item-22"></a>
## [llm-gemini 0.38 adds Gemini 4 Neon support amid pricing confusion](https://simonwillison.net/2026/Nov/18/llm-gemini/) ⭐️ 6.0/10

Simon Willison released llm-gemini 0.38, adding support for Google's newly announced Gemini 4 Neon model. The release coincides with Google's introduction of Neon, which joins Carbon and Hydrogen in the Gemini 4 lineup, while Argon is no longer mentioned. This update lets users of the LLM command-line tool immediately access Gemini 4 Neon, which Google positions for deep reasoning in software engineering and science. It also highlights growing concerns about the complexity of Google's Gemini 4 pricing tiers, which could confuse developers choosing models. Neon is priced at $3 per million input tokens and $15 per million output tokens, making it temporarily the most expensive option because Carbon is currently discounted to $2/$10 until December 1st. Neon supports thinking levels low, medium, high, and xhigh, and is available via the Gemini API in Google AI Studio (paid) and Google AI Pro/Ultra subscriptions.

rss · Simon Willison · Nov 18, 23:59

**Background**: llm-gemini is a plugin for Simon Willison's LLM command-line tool that allows users to interact with Google's Gemini models from the terminal. Google's Gemini 4 series includes multiple models with different price and performance trade-offs: Carbon for hardest long-horizon projects, Neon for deep reasoning, and Hydrogen for speed and efficiency. The lineup previously included Argon, but it has been omitted from the Neon announcement, and pricing has changed with promotional discounts.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-4-neon/">Gemini 4 Neon - Model Card — Google DeepMind</a></li>
<li><a href="https://aistudio.google.com/docs/models/gemini-4-neon">Gemini 4 Neon - Gemini API | Google AI Studio</a></li>
<li><a href="https://fourweekmba.com/ai-gemini-4-models-explained-carbon-argon-hydrogen-prices/">Gemini 4 Models Explained: Carbon, Argon, Hydrogen Prices</a></li>

</ul>
</details>

**Tags**: `#llm`, `#gemini`, `#google`, `#pricing`, `#tooling`

---

<a id="item-23"></a>
## [datasette-arrows 0.1a0 Adds Apache Arrow Streaming Export to Datasette](https://simonwillison.net/2026/Nov/18/datasette-arrows/) ⭐️ 6.0/10

Simon Willison released datasette-arrows 0.1a0, an alpha plugin that implements Apache Arrow IPC stream export for Datasette using the new streaming capability of the register_output_renderer() plugin hook introduced in Datasette 1.0a43. The plugin was built almost in a single shot by Claude Fable 5.2, which suggested the Arrow streaming format. This plugin demonstrates how third-party developers can extend Datasette's streaming export system beyond the built-in CSV and TSV formats, enabling typed columnar exports that integrate directly with tools like DuckDB, pandas, Polars, and PyArrow. It lowers the barrier for building high-performance data export plugins and signals a more extensible export architecture in Datasette 1.0. The Arrow export respects filters, sort order, and ?_col= options, and Datasette's allow_stream and max_stream_mb settings apply to these exports; adding ?_dl=1 downloads the response as a file. The screenshot shown comes from Datasette's main branch, where Arrow is grouped with TSV and CSV under "All rows in this table", but the most recent release does not yet group streaming formats this way—that grouping is coming in the next alpha release.

rss · Simon Willison · Nov 18, 17:09

**Background**: Datasette is an open-source tool for exploring and publishing data, and its plugin system lets developers add custom output formats through hooks like register_output_renderer(). Datasette core already supports streaming CSV and TSV exports, which can export millions of rows without loading everything into memory because those formats can be written in chunks. Apache Arrow is a columnar in-memory data format with an IPC streaming format that preserves typed columns and supports zero-copy reads, making it efficient for passing data to analytical tools such as pandas, Polars, and DuckDB.

<details><summary>References</summary>
<ul>
<li><a href="https://arrow.apache.org/">Apache Arrow | Apache Arrow</a></li>
<li><a href="https://github.com/datasette/datasette-arrows">GitHub - datasette/datasette-arrows: Streaming exports for ...</a></li>
<li><a href="https://simonwillison.net/2026/Nov/18/datasette-arrows/">Release: datasette-arrows 0.1a0 - simonwillison.net</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#apache-arrow`, `#plugins`, `#streaming`, `#data-export`

---