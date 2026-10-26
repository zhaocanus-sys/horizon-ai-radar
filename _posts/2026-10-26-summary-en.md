---
layout: default
title: "Horizon Summary: 2026-10-26 (EN)"
date: 2026-10-26
lang: en
---

> From 32 items, 17 important content pieces were selected

---

1. [OpenAI and Anthropic Slash LLM Prices Up to 80% in Months](#item-1) ⭐️ 8.0/10
2. [IBM CEO says open-weight models are now good and cheap on-prem](#item-2) ⭐️ 7.0/10
3. [F-Zero X Ported to Nintendo 3DS with AI-Assisted Development](#item-3) ⭐️ 7.0/10
4. [Surveying Context Engineering: Organization and Relevance Matter as Much as Length](#item-4) ⭐️ 7.0/10
5. [Dan Luu argues for more ambitious software, sparking HN debate](#item-5) ⭐️ 7.0/10
6. [10-Year-Old CNN Outperforms Frontier LLMs in Skin Cancer Diagnosis](#item-6) ⭐️ 7.0/10
7. [Open-source sky camera lets Claude Code autonomously detect and classify meteors](#item-7) ⭐️ 7.0/10
8. [Opus 5.5 writes sloppy code but still succeeds, study finds](#item-8) ⭐️ 7.0/10
9. [PaperPilot: Zero-Cloud, Pure-Rust PDF Engine with WASM and MCP](#item-9) ⭐️ 6.0/10
10. [Stanford archive shares behind-the-scenes photos of NeXT office](#item-10) ⭐️ 6.0/10
11. [Dolly Parton's Imagination Library Sparks HN Discussion on Local Funding](#item-11) ⭐️ 6.0/10
12. [Show HN: Modular Keyboard Reconfigurable into Any Shape](#item-12) ⭐️ 6.0/10
13. [arXiv Paper Argues Attention Is Not Necessary for Language Modeling](#item-13) ⭐️ 6.0/10
14. [Public PoC Released for Steal My Bitcoin CTF Exploit](#item-14) ⭐️ 6.0/10
15. [Disney Animation's Filmmaking Process Sparks Debate on Craft and AI](#item-15) ⭐️ 6.0/10
16. [DreamHost Forces Password Resets After Active Security Incident](#item-16) ⭐️ 6.0/10
17. [Opus planning with local Qwen coding cuts cloud cost 75% but doubles build time](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI and Anthropic Slash LLM Prices Up to 80% in Months](https://minimaxir.com/2026/10/cheap-llms/) ⭐️ 8.0/10

OpenAI and Anthropic have cut their large language model API prices by as much as 80% over the past few months, according to an analysis that has drawn 285 comments. The reductions reflect an intensifying price war between the two leading AI labs. The price cuts significantly lower the cost of building AI applications, benefiting enterprises and developers who rely on these APIs. They also signal that inference costs are falling fast, which could reshape competitive dynamics and pressure smaller providers. The analysis notes that exact cost structures remain opaque, but techniques such as quantization, KV cache compression, continuous batching, and speculative decoding are known to reduce inference costs substantially. DeepSeek's reported $38 revenue per GPU-hour for Flash V4 suggests significant margin room even at lower prices.

hackernews · minimaxir · Oct 25, 21:11 · [Discussion](https://news.ycombinator.com/item?id=50236102)

**Background**: LLM inference is the process of running a trained model to generate responses, and its cost depends on GPU hardware, model size, and optimization techniques. Over the past two years, OpenAI and Anthropic have engaged in a quiet price war, offering cheaper tiers, larger free contexts, and discounts on cached prompts. Falling hardware costs and software optimizations have made it feasible to serve models at much lower prices.

<details><summary>References</summary>
<ul>
<li><a href="https://specpicks.com/reviews/openai-anthropic-token-price-war-local-inference-2026">OpenAI vs Anthropic Token Price War : When a $300 | SpecPicks</a></li>
<li><a href="https://www.costmyai.com/blog/openai-anthropic-price-war-2026">The OpenAI - Anthropic Price War of 2026: What Is... | CostMyAI</a></li>
<li><a href="https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/">Mastering LLM Techniques : Inference Optimization</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some see competition driving down prices and cite cheaper alternatives like Kimi and GLM, while others warn of a race to the bottom and an unsustainable 'AI winter' scenario. A recurring theme is skepticism about regulation, with one commenter suggesting OpenAI and Anthropic may push for rules to disadvantage open models from China.

**Tags**: `#LLM pricing`, `#AI industry`, `#competition`, `#inference costs`, `#regulation`

---

<a id="item-2"></a>
## [IBM CEO says open-weight models are now good and cheap on-prem](https://www.theregister.com/systems/2026/10/22/ibm-ceo-says-open-weight-models-are-now-irresistibly-good-and-cheap-on-prem/5304640) ⭐️ 7.0/10

IBM's CEO stated that open-weight AI models have reached a level of quality and cost-efficiency that makes on-premises deployment attractive for enterprises. The remark, reported by The Register, sparked a Hacker News discussion with 217 points and 116 comments on privacy, cost, and vendor incentives. A major enterprise vendor publicly endorsing open-weight models as production-ready signals a shift away from exclusive reliance on closed API providers, potentially accelerating on-prem AI adoption among privacy-sensitive organizations. It also intensifies competition among infrastructure vendors and AI labs over where inference workloads run. The statement is a vendor claim rather than a technical benchmark, and critics note that IBM sells hardware and infrastructure that would benefit from on-prem AI adoption. Community members also point to practical trade-offs such as slightly lower output quality and higher token usage compared with paid frontier models.

hackernews · Betelbuddy · Oct 26, 01:47 · [Discussion](https://news.ycombinator.com/item?id=50238088)

**Background**: Open-weight models are AI models whose trained parameters are published for anyone to download, run, and modify, usually under licenses that may restrict commercial use. On-premises deployment means running these models on an organization's own infrastructure rather than through public cloud APIs, which can improve data control and privacy. IBM has invested in open models through its Granite family and the CNCF-governed llm-d inference project.

<details><summary>References</summary>
<ul>
<li><a href="https://getmorefromai.com/glossary/open-weights-model">Open - weights model : Definition , Examples, and... | GetMoreFromAI</a></li>
<li><a href="https://www.ibm.com/granite">Granite - IBM</a></li>
<li><a href="https://newsroom.ibm.com/2026-10-20-llm-d-1-0-advances-open,-cost-efficient-ai-inference-for-production-scale">llm-d 1.0 Advances Open, Cost-Efficient AI Inference for ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that open models are now viable for many workloads, with one practitioner reporting months of use without paid models and citing privacy as a key benefit. Others caution that IBM has a hardware-selling motive, while some see IBM's entry as a positive counterweight to AI labs and expect more companies to seriously consider self-hosting inference.

**Tags**: `#open-weight-models`, `#on-prem-ai`, `#IBM`, `#LLM-deployment`, `#industry-analysis`

---

<a id="item-3"></a>
## [F-Zero X Ported to Nintendo 3DS with AI-Assisted Development](https://hypnotize.works/gdx-3ds/postmortem/index.html) ⭐️ 7.0/10

A homebrew developer released a native port of F-Zero X for the Nintendo 3DS, built on the G-Diffuser PC port and the game's decompilation, achieving version 1.0.0 with support for both Old and New 3DS. The port includes full stereoscopic 3D, audio, and an optional Expansion Kit (64DD content) streamed from the SD card, and the author published a detailed postmortem on the technical challenges and use of AI (Claude) in development. This project demonstrates how AI-assisted coding can streamline the porting of complex games to constrained hardware like the 3DS, potentially lowering the barrier for homebrew developers. It also adds to a growing trend of 3DS ports (e.g., Melee) and sparks discussion about the practical costs and benefits of AI tools in game development. The port supports both Old and New 3DS models, with the New 3DS build enabling the 64DD Expansion Kit content via SD card streaming. The author notes that the project served as a learning experience for using Claude more efficiently, and an upcoming update will add 64DD support on original 3DS, local and online multiplayer, and QR code sharing for custom courses.

hackernews · bpierre · Oct 25, 23:27 · [Discussion](https://news.ycombinator.com/item?id=50237078)

**Background**: F-Zero X is a futuristic racing game originally released for the Nintendo 64 in 1998. The 3DS is a dual-screen handheld console with stereoscopic 3D capabilities, and homebrew development for it often uses devkitPro and devkitARM. Decompilation projects reverse-engineer game code into compilable source, enabling native ports to other platforms; the G-Diffuser project is a PC port of F-Zero X that serves as the base for this 3DS version.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/cruxxxxxx/gdx-3ds">GitHub - cruxxxxxx/gdx-3ds: Unofficial 3DS Port of F-Zero X ...</a></li>
<li><a href="https://recompsoftware.com/p/gdx-3ds/">G-Diffuser 3DS: F-Zero X PC port, download & source · Recomp</a></li>
<li><a href="https://digitechbytes.com/general/f-zero-x-on-nintendo-3ds/">F-Zero X On Nintendo 3DS - Digitech Bytes</a></li>

</ul>
</details>

**Discussion**: The discussion includes the author announcing an upcoming update with 64DD support, multiplayer, and QR code sharing, and a commenter questioning why the 3DS is a popular target for ports instead of the more powerful Switch. Another commenter raises doubts about the real-world cost of using Claude, noting that most users pay subscription pricing rather than API pricing, while a developer working on a Game Boy port of F-Zero shares their own project.

**Tags**: `#game-development`, `#homebrew`, `#nintendo-3ds`, `#porting`, `#ai-assisted-coding`

---

<a id="item-4"></a>
## [Surveying Context Engineering: Organization and Relevance Matter as Much as Length](https://www.dbreunig.com/2026/10/24/the-state-of-context-engineering.html) ⭐️ 7.0/10

An article on dbreunig.com surveys the state of context engineering for LLMs, arguing that how context is organized and how relevant it is matter as much as its length. The piece sparked a 39-comment discussion covering dependency length, tree-based context compression, and strategic forgetting. This analysis pushes LLM application developers past the simplistic 'context too long' diagnosis toward more nuanced memory and context management strategies. As agents and long-running workflows become common, techniques like hierarchical summarization and strategic forgetting could directly affect reliability and cost. The discussion highlights concrete approaches such as VictorTaelin's UniiChat, which summarizes each message into a single line and builds a binary tree of summaries that an agent can navigate with a zoom tool, plus an implementation in the pi-optchat repository. Commenters also note that LLMs' attention works best when related concepts are close together in the text, making dependency length a useful concept.

hackernews · pchristensen · Oct 25, 20:32 · [Discussion](https://news.ycombinator.com/item?id=50235780)

**Background**: Context engineering is the discipline of deciding what information to put into an LLM's context window, how to format it, and what to leave out, and it has largely superseded simple prompt engineering as agents and retrieval-augmented systems grow more complex. LLMs have a fixed context window, so long conversations and large documents must be selected, compressed, or summarized. Research directions include tree-based context compression, which organizes text into semantic trees, and strategic forgetting, which deliberately drops low-utility memories to keep agent memory compact.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2507.13334">[2507.13334] A Survey of Context Engineering for Large ... What is context engineering? - IBM What Is Context Engineering? A Guide for AI & LLMs [2510.04618] Agentic Context Engineering: Evolving Contexts ... Context Engineering - langchain.com Context Engineering Guide | Prompt Engineering Guide GitHub - ypollak2/context-engineering-handbook: The ...</a></li>
<li><a href="https://www.ibm.com/think/topics/context-engineering">What is context engineering? - IBM</a></li>
<li><a href="https://arxiv.org/abs/2607.22562">[2607.22562] SF-AMS: Strategic Forgetting for Structured ...</a></li>

</ul>
</details>

**Discussion**: Commenters broadly agreed that the article moves beyond the 'context too long' scapegoat, with one emphasizing that attention works by linking related concepts and that dependency length matters. Others praised UniiChat's tree-based summarization with a zoom tool, argued that strategic forgetting mirrors why human memory is imperfect and aids creativity, and questioned whether a task baked into model weights should really be called 'poisoned context'.

**Tags**: `#context-engineering`, `#LLM`, `#prompt-engineering`, `#AI-agents`, `#memory-management`

---

<a id="item-5"></a>
## [Dan Luu argues for more ambitious software, sparking HN debate](https://danluu.com/ambitious/) ⭐️ 7.0/10

Dan Luu published an essay arguing that developers should be more ambitious with the software they build, which sparked a Hacker News discussion with over 710 comments. The discussion highlights growing concerns about code quality, the impact of AI-generated code, and the gap between software inside and outside the tech bubble, affecting developers and users alike. Commenters noted that AI can speed up development but often produces overfit, unmaintainable code, and shared examples of poor software quality in consumer products like heat pumps.

hackernews · ltratt · Oct 24, 21:47 · [Discussion](https://news.ycombinator.com/item?id=50225695)

**Background**: Dan Luu is a well-known software engineer and blogger who writes about performance, systems, and industry myths. His essays often challenge conventional wisdom and spark substantive debates in the tech community.

<details><summary>References</summary>
<ul>
<li><a href="https://danluu.com/perf-opt/">There's no reason for software to be slow anymore - danluu.com</a></li>
<li><a href="https://danluu.com/">danluu.com</a></li>

</ul>
</details>

**Discussion**: Commenters expressed diverse views: some warned that AI-generated code can be messy and overfit, others shared ambitious personal projects enabled by AI, and some emphasized the need for ambition in code quality and diversity of software. A recurring theme was that software quality outside the tech bubble is often poor.

**Tags**: `#software-engineering`, `#ambition`, `#code-quality`, `#AI`, `#HN-discussion`

---

<a id="item-6"></a>
## [10-Year-Old CNN Outperforms Frontier LLMs in Skin Cancer Diagnosis](https://lynchlab.net/llm-skin-cancer) ⭐️ 7.0/10

A 10-year-old Inception v3 convolutional neural network, fine-tuned on 68,011 dermoscopic and clinical images from the ISIC Archive, outperformed two frontier large language models in diagnosing skin cancer on a test set of 200 lesions. This result challenges the assumption that general-purpose frontier LLMs are universally superior, highlighting that specialized models with the right architecture can still be far more accurate and cost-effective for specific medical imaging tasks. The CNN was trained on a single H100 GPU and tested on lesions excluded from training, but the small test set of 200 lesions and the use of a single benchmark raise questions about generalizability and potential overfitting to the benchmark.

hackernews · sungam · Oct 25, 17:15 · [Discussion](https://news.ycombinator.com/item?id=50233779)

**Background**: Convolutional neural networks (CNNs) are deep learning models designed to process image data by capturing spatial relationships, and they have been the foundation of computer vision for years. In medical imaging, CNNs have been widely used for skin lesion classification, often achieving dermatologist-level performance. Frontier LLMs, such as those from OpenAI and Google, are general-purpose models trained on vast text and multimodal data, but their effectiveness for specialized medical diagnosis remains an open question.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Convolutional_neural_network">Convolutional neural network - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC10572538/">Skin Lesion Classification and Detection Using Machine ...</a></li>
<li><a href="https://www.nature.com/articles/s41591-025-04151-2">Holistic evaluation of large language models for medical ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that a specialized model beating a general-purpose LLM is unsurprising, comparing it to a calculator outperforming LLMs at arithmetic. Some criticize the result as 'benchmaxxing' due to the small test set, while others argue that LLMs' real potential lies in integrating additional clinical data and generating patient questions.

**Tags**: `#machine-learning`, `#medical-imaging`, `#LLM`, `#benchmarking`, `#model-specialization`

---

<a id="item-7"></a>
## [Open-source sky camera lets Claude Code autonomously detect and classify meteors](https://www.reddit.com/r/ClaudeAI/comments/1xfqc9x/i_built_an_open_source_sky_camera_that_claude/) ⭐️ 7.0/10

A developer built openskycam, an open-source 4K sky camera system that uses an MCP server to let Claude Code autonomously run meteor detection workflows, review detections, and retrain the model. On a Saturday night it detected 17 meteors and sorted them before the user woke up, and after retraining on approved detections, star false alarms dropped from about 50% to 7% while still catching 90% of meteors. This is a concrete real-world demonstration of an AI agent autonomously building and improving a computer vision pipeline, including self-directed dataset creation and model retraining, which is a valuable case study for agentic AI and edge ML. It shows how MCP and API-driven design can let Claude Code operate complex scientific workflows with minimal human intervention. The system requires an RTSP camera, a Raspberry Pi, a machine with large disk (macOS or Linux, GPU optional), and a Cloudflare account with a domain; setup can run unattended with `npm run setup -- --yes`. Guardrails are enforced by the MCP server rather than prompts—no key can create keys, deletes require confirmation, and edits fail rather than overwrite newer versions—and the server ships its own guides and skills (build-a-workflow, find-detections, verify-changes) so Claude learns rules from the server.

reddit · r/ClaudeAI · /u/Terrible_Award_2124 · Oct 26, 07:38

**Background**: MCP (Model Context Protocol) is an open standard that lets AI apps like Claude connect to external tools and data through MCP servers. Claude Code is Anthropic's agentic CLI that can read a codebase, edit files, and run commands. The project uses these to automate meteor detection from sky camera footage, a task that traditionally involves manually scrubbing video, labeling frames, and retraining models.

<details><summary>References</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/examples">Example Servers - Model Context Protocol</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://github.com/topics/meteor-detection">meteor - detection · GitHub Topics · GitHub</a></li>

</ul>
</details>

**Tags**: `#agentic-ai`, `#computer-vision`, `#open-source`, `#MCP`, `#meteor-detection`

---

<a id="item-8"></a>
## [Opus 5.5 writes sloppy code but still succeeds, study finds](https://www.reddit.com/r/ClaudeAI/comments/1xfkhum/opus_55_writes_slop_code_but_succeeds_anyways_a/) ⭐️ 7.0/10

A researcher ran Claude Opus 5.5 through all 196 checkpoints of the SlopCodeBench benchmark at a cost of $266 and found that while code messiness (structural erosion and verbosity) increased in 22 of 35 problems, it did not predict failure on subsequent checkpoints. Only 0.3% of previously passing tests regressed, and across the leaderboard, cleaner code did not correlate with higher solve rates. This challenges the SlopCodeBench paper's assumption that sloppy code causes agent failure, suggesting that code quality metrics like erosion and verbosity may not be reliable predictors of agent performance. It has implications for how the AI-agent and software engineering research community evaluates coding agents and designs benchmarks. The study found that code size, not messiness, predicted cost: each doubling of codebase size increased the next checkpoint's cost by about 19%. The author also notes that the headline 17% strict solve rate undersells Opus 5.5, which passed 84–92% of tests for each new specification, and cautions that this is a single run of one model on small programs with observational comparisons.

reddit · r/ClaudeAI · /u/aj_marshall · Oct 26, 02:05

**Background**: SlopCodeBench is a benchmark that evaluates coding agents by giving them a problem split into checkpoints, where each checkpoint requires adding a new feature on top of the agent's own previous code without breaking existing functionality. It measures code degradation using two metrics: structural erosion (complexity piling up in a few large, branchy functions) and verbosity (redundant code). The original paper reported that agent code gets messier over time and that agents get worse at keeping tests passing, suggesting a causal link.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.24755">[2603.24755] SlopCodeBench: Benchmarking How Coding Agents ... GitHub - SprocketLab/slop-code-bench: SlopCodeBench ... SlopCodeBench: Benchmarking How Coding Agents Degrade Over ... SlopCode Pitch V Who Knows - gabeorlanski.github.io SlopCode Bench | Snorkel AI NeurIPS Poster SlopCodeBench: Benchmarking How Coding Agents ...</a></li>
<li><a href="https://www.scbench.ai/">SlopCodeBench</a></li>
<li><a href="https://platform.claude.com/docs/en/models/opus-5-5/overview">Claude Opus 5.5 - Claude Platform Docs</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#code-quality`, `#benchmarks`, `#llm-evaluation`, `#software-engineering`

---

<a id="item-9"></a>
## [PaperPilot: Zero-Cloud, Pure-Rust PDF Engine with WASM and MCP](https://github.com/KrushnaVardhanReddy/PaperPilot) ⭐️ 6.0/10

PaperPilot is a new open-source project that provides a zero-cloud, pure-Rust PDF engine with WebAssembly (WASM) and Model Context Protocol (MCP) support. It was presented on Hacker News, where it received 116 points and 29 comments, with discussions around licensing and feature requests. This project matters because it offers a privacy-focused, local-first alternative for PDF processing, eliminating cloud dependency and leveraging Rust's safety and performance. Its integration with WASM and MCP could enable seamless use in web and AI applications, appealing to developers concerned with data privacy and efficiency. The engine is written entirely in Rust and compiled to WASM for browser use, with MCP support for AI tool integration. However, community members raised concerns about potential derivation from MuPDF, suggesting the license should be AGPLv3 instead of Apache if so.

hackernews · vardhan1237 · Oct 26, 03:29 · [Discussion](https://news.ycombinator.com/item?id=50238739)

**Background**: WebAssembly (WASM) is a binary instruction format that allows high-performance code to run in web browsers and other environments. The Model Context Protocol (MCP) is an open standard developed by Anthropic to connect AI applications with external data sources and tools. Pure-Rust PDF engines are emerging as alternatives to traditional C-based libraries, offering memory safety and modern concurrency.

<details><summary>References</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>
<li><a href="https://www.anthropic.com/news/model-context-protocol">Introducing the Model Context Protocol \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed interest in the privacy-focused approach and suggested features like password removal and signature support. One commenter questioned whether the engine was derived from MuPDF and urged disclosure and a license change to AGPLv3, while others shared their use of Typst for PDF generation and building browser extensions for simpler hosting.

**Tags**: `#PDF`, `#Rust`, `#WASM`, `#MCP`, `#open-source`

---

<a id="item-10"></a>
## [Stanford archive shares behind-the-scenes photos of NeXT office](https://exhibits.stanford.edu/menuez/browse/next-computer-inc?per_page=96&sort=pub_year_isi+asc%2C+title_sort+asc&view=masonry) ⭐️ 6.0/10

Stanford's Menuez exhibit has published a collection of behind-the-scenes photographs from NeXT Computer's office, capturing the company's early culture and workspace. The archive, sorted by publication year, offers a visual record of the era when Steve Jobs was leading NeXT after his departure from Apple. These photos offer a rare glimpse into the formative years of NeXT, the company whose acquisition by Apple in 1997 brought Jobs back and whose NeXTSTEP operating system became the foundation for macOS and iOS. The archive also fuels nostalgia for in-person, high-intensity startup culture that many in tech feel has faded. The collection is hosted on Stanford's exhibits site and includes 96 items per page, sorted chronologically. The photos are part of the Menuez archive, which documents Silicon Valley history, and the discussion highlights that only about 50,000 NeXTcubes were sold by 1991, yet one was used by Tim Berners-Lee to create the first web browser and server.

hackernews · Austin_Conlon · Oct 26, 03:31 · [Discussion](https://news.ycombinator.com/item?id=50238763)

**Background**: NeXT Computer was founded by Steve Jobs in 1985 after he was forced out of Apple. The company produced high-end workstations like the NeXTcube, which were technologically advanced but commercially unsuccessful due to high prices. Despite this, NeXT's software, NeXTSTEP, was highly influential and became the basis for Apple's modern operating systems after Apple acquired NeXT in 1997.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Steve_Jobs">Steve Jobs - Wikipedia</a></li>
<li><a href="https://simson.net/ref/NeXT/">NeXT Computer Historical Site</a></li>

</ul>
</details>

**Discussion**: Commenters expressed surprise at how dysfunctional Steve Jobs was as CEO in NeXT's early days, yet marveled that the company still produced valuable technology. Others felt a sense of melancholy about missing the era of in-person tech innovation, and some recommended the book 'Steve Jobs in Exile' and praised NeXTSTEP's distinctive UI.

**Tags**: `#NeXT`, `#Steve Jobs`, `#tech history`, `#nostalgia`, `#office culture`

---

<a id="item-11"></a>
## [Dolly Parton's Imagination Library Sparks HN Discussion on Local Funding](https://imaginationlibrary.com/) ⭐️ 6.0/10

A Hacker News post about Dolly Parton's Imagination Library, a program that mails free books to children from birth to age five, generated 527 points and 90 comments. The discussion highlighted personal stories and revealed that while the central organization negotiates wholesale pricing and selects books, per-book funding comes entirely from local charities and partners. The Imagination Library has distributed millions of books worldwide, and its decentralized funding model allows it to scale but also creates dependency on local charitable support. The discussion underscores the program's emotional impact on families and its role in early childhood literacy. The program operates in five countries and mails age-appropriate books monthly until age five, with wholesale costs around $2.50 per book. Funding is raised locally, meaning some areas may lack coverage if charities cannot partner, but the model enables rapid expansion and community engagement.

hackernews · jumploops · Oct 25, 18:23 · [Discussion](https://news.ycombinator.com/item?id=50234474)

**Background**: Dolly Parton's Imagination Library was founded in 1995 in Sevier County, Tennessee, inspired by her father's inability to read. It began as a local program and expanded nationally in 2000, now reaching children in the US, UK, Canada, Australia, and Ireland. The program is operated by the Dollywood Foundation and provides free books regardless of family income.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dollywood_Foundation">Dollywood Foundation - Wikipedia</a></li>
<li><a href="https://imaginationlibrary.com/about-us/">About Dolly Parton's Imagination Library</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dolly_Parton">Dolly Parton - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters shared heartfelt stories, such as a parent whose child eagerly awaits books in the mail and another whose final book arrived with a letter from Dolly ending 'I will always love you.' Some discussed the funding structure, noting that local charities sustain the program, and one commenter expressed initial frustration at receiving books despite being well-off but later appreciated the joy it brought their child.

**Tags**: `#charity`, `#education`, `#books`, `#community`, `#Dolly Parton`

---

<a id="item-12"></a>
## [Show HN: Modular Keyboard Reconfigurable into Any Shape](https://github.com/notaroomba/keybytes) ⭐️ 6.0/10

A developer shared a Show HN post for a modular keyboard project called Keybytes that can be reconfigured into arbitrary shapes, currently an early prototype with only two keys and firmware still in development. This project explores a novel approach to keyboard design by allowing users to create custom shapes like triangles or circles, which could appeal to ergonomics enthusiasts and DIY hardware makers, though it remains far from a practical product. The prototype uses I2C for communication between modules, which limits the number of devices to 127 addresses and may suffer from bus hangs with many slaves; the developer is still working on firmware and adding more keys.

hackernews · NotARoomba · Oct 25, 03:47 · [Discussion](https://news.ycombinator.com/item?id=50228115)

**Background**: I2C is a synchronous serial communication bus invented by Philips in 1980, commonly used to connect low-speed peripherals to microcontrollers. Modular keyboards are a niche in the DIY mechanical keyboard community, where enthusiasts build custom layouts using firmware like QMK or ZMK. This project aims to go beyond fixed layouts by making each key or cluster independently addressable and physically reconfigurable.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/I2c">I2C - Wikipedia</a></li>
<li><a href="https://zmk.dev/">Hello from ZMK Firmware | Modern, open source keyboard firmware .</a></li>

</ul>
</details>

**Discussion**: Commenters liked the idea but raised concerns: one noted I2C's 127-address limit and potential bus hangs, suggesting CAN bus instead; another pointed out that ergonomic keyboards are rarely perfectly columnar; and several asked for a full-layout demo to assess communication snappiness and structural integrity.

**Tags**: `#keyboard`, `#hardware`, `#modular`, `#DIY`, `#I2C`

---

<a id="item-13"></a>
## [arXiv Paper Argues Attention Is Not Necessary for Language Modeling](https://arxiv.org/abs/2512.19428) ⭐️ 6.0/10

A new arXiv paper (2025) titled 'Attention Is Not What You Need' claims that attention mechanisms are not required for language modeling, proposing an alternative architecture. The paper demonstrates its approach on an 18M-parameter model trained on an older dataset. If validated, this could challenge the dominant Transformer paradigm and open new directions for efficient language model design. However, the small-scale demonstration leaves its practical significance uncertain. The model uses a pairing operation (zt, zt+Δ) with a positive offset Δ, which critics argue allows the model to see the next token when predicting it, potentially invalidating the results. The evaluation is at toy scale (18M parameters) on an ancient dataset, raising concerns about generalizability.

hackernews · westurner · Oct 25, 23:52 · [Discussion](https://news.ycombinator.com/item?id=50237224)

**Background**: Attention mechanisms, introduced in the 2017 paper 'Attention Is All You Need', allow models to weigh the importance of different tokens in a sequence and are the core of Transformer architectures like BERT and GPT. Next-token prediction is a standard training objective for language models, where the model learns to predict the next word given previous context. Toy-scale evaluations are common in machine learning research for quick proof-of-concept but often fail to scale to real-world performance.

<details><summary>References</summary>
<ul>
<li><a href="https://poloclub.github.io/transformer-explainer/">Transformer Explainer: LLM Transformer Model Visually Explained</a></li>
<li><a href="https://arxiv.org/abs/2412.18619">[2412.18619] Next Token Prediction Towards Multimodal ...</a></li>
<li><a href="https://tensorgym.com/blog/transformer-attention">Complete Guide to Transformer Architecture & Attention Mechanisms</a></li>

</ul>
</details>

**Discussion**: Commenters question the paper's validity: one points out that the pairing operation (zt, zt+Δ) with positive Δ means the model uses the next token to predict itself, which is cheating; another criticizes the toy-scale 18M parameter evaluation as proving nothing; and a third argues that scale is what matters, as seen in other attention-free LLMs, though architecture still matters under compute constraints.

**Tags**: `#transformers`, `#attention-mechanism`, `#language-models`, `#machine-learning`, `#arxiv`

---

<a id="item-14"></a>
## [Public PoC Released for Steal My Bitcoin CTF Exploit](https://github.com/KillaBoi/StealMyBitcoin-PoC) ⭐️ 6.0/10

A public proof-of-concept exploit for the Steal My Bitcoin CTF challenge has been released on GitHub, demonstrating a PHP vulnerability (php2shell) in a single Python file. This PoC provides technical insight into the real-world exploitability of the php2shell vulnerability, which affects PHP versions 5.4–8.5 and allows remote code execution, impacting unpatched servers. The PoC uses PHP's built-in development server proxied through nginx, rather than fpm or mod_php, which community members note is not representative of typical production setups.

hackernews · davikr · Oct 26, 00:15 · [Discussion](https://news.ycombinator.com/item?id=50237379)

**Background**: PHP2Shell refers to two critical vulnerabilities (CVE-2026-109618 and CVE-2026-109619) in PHP that enable remote code execution. Discovered with AI assistance in August 2026 and announced in October, they affect PHP versions 5.4 through 8.5. The Steal My Bitcoin CTF challenge was designed to simulate a real-world scenario exploiting these vulnerabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/KillaBoi/StealMyBitcoin-PoC">KillaBoi/StealMyBitcoin-PoC: A public release of the Steal My Bitcoin ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/PHP2Shell">PHP2Shell - Wikipedia</a></li>
<li><a href="https://securitylabs.datadoghq.com/articles/php2shell-critical-vulnerabilities-in-php/">PHP2Shell - Critical vulnerabilities in PHP (CVE-2026-109618 ...</a></li>

</ul>
</details>

**Discussion**: Community members debate the realism of the challenge setup, noting it used PHP's dev server rather than typical fpm/mod_php configurations. Some argue the difficulty of exploitation suggests many unpatched servers may not have been compromised, while others question whether the PoC works with PHP-FPM and nginx.

**Tags**: `#security`, `#CTF`, `#PHP`, `#vulnerability`, `#exploit`

---

<a id="item-15"></a>
## [Disney Animation's Filmmaking Process Sparks Debate on Craft and AI](https://www.disneyanimation.com/process/) ⭐️ 6.0/10

Disney Animation published an overview of its filmmaking process on its website, and the Hacker News community discussed the craftsmanship involved, the potential for AI automation, and the future of 2D animation. The discussion highlights how traditional animation craftsmanship is being reevaluated in light of AI tools that can automate parts of the pipeline, potentially reshaping roles and creative processes in the animation industry. Community members noted that AI tools like Unreal Engine and generative models are enabling individual artists to produce high-quality animation, while others expressed nostalgia for hand-drawn 2D classics and questioned how much of the process can be automated.

hackernews · embedding-shape · Oct 25, 20:27 · [Discussion](https://news.ycombinator.com/item?id=50235738)

**Background**: Disney Animation's pipeline typically includes storyboarding, layout, animation, and rendering, with specialized software for each stage. The discussion touches on the shift from 2D to 3D animation and the emerging role of AI in automating tasks like rigging and in-betweening.

<details><summary>References</summary>
<ul>
<li><a href="https://www.disneyanimation.com/">Walt Disney Animation Studios</a></li>
<li><a href="https://www.youtube.com/watch?v=0SJgY0pbUnk">ENCANTO | Film Making Process | Disney Animation - YouTube</a></li>

</ul>
</details>

**Discussion**: Commenters shared a mix of admiration for Disney's attention to detail, nostalgia for 2D animation, and curiosity about AI's impact. Some argued that AI could revive 2D animation, while others noted that AI-driven films involve different creative decisions.

**Tags**: `#animation`, `#disney`, `#ai`, `#craftsmanship`, `#film-production`

---

<a id="item-16"></a>
## [DreamHost Forces Password Resets After Active Security Incident](https://www.dreamhoststatus.com/) ⭐️ 6.0/10

DreamHost is forcing password resets for email and FTP/SFTP users following an active security incident that began with connectivity issues affecting its File Manager, which was an installation of Monsta FTP. The company has expired passwords for some users and notified them via email, though the reset process is now complete. This incident highlights the security risks faced by hosting providers, especially those using third-party web applications like Monsta FTP, and affects many customers who rely on DreamHost for email and file transfer services. It also raises questions about the speed and transparency of incident disclosure. The incident may have been caused by a recently published PHP vulnerability in Monsta FTP, potentially leading to exfiltration of FTP credentials. Some users reported receiving password reset emails over 48 hours after the incident started, and confusion arose because some passwords were not actually expired despite the notification.

hackernews · greenchair · Oct 25, 13:09 · [Discussion](https://news.ycombinator.com/item?id=50231166)

**Background**: DreamHost is a Los Angeles-based web hosting provider and domain registrar founded in 1997, hosting over 1.5 million websites. Monsta FTP is a commercial PHP-based web FTP client that allows file management through a browser. FTP (File Transfer Protocol) is an older protocol for transferring files, while SFTP (SSH File Transfer Protocol) is a more secure alternative; both are commonly used for website management.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dreamhoststatus.com/">DreamHost Status</a></li>
<li><a href="https://en.wikipedia.org/wiki/DreamHost">DreamHost - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community members speculate that the File Manager (Monsta FTP) was compromised via a PHP vulnerability, leading to credential theft. Some users express frustration with DreamHost's slow and confusing disclosure, while others share long-term loyalty or validation for having migrated away.

**Tags**: `#security`, `#incident-response`, `#hosting`, `#web-security`, `#dreamhost`

---

<a id="item-17"></a>
## [Opus planning with local Qwen coding cuts cloud cost 75% but doubles build time](https://www.reddit.com/r/ClaudeAI/comments/1xfgyl1/same_game_built_twice_opus_alone_vs_opus_planning/) ⭐️ 6.0/10

A Reddit user built the same 5-level pixel platformer twice on a MacBook Pro M5 Max using Atomic Agent: once with Opus 5.5 alone, and once in Fusion mode where Opus 5.5 planned and reviewed while a local Qwen 3.8 27B model wrote the code with 3 workers. The hybrid approach cut cloud cost from $2.52 to $0.62 (75% reduction) and Opus output tokens from 90.7k to 11.3k, but increased build time from 16 to 42 minutes. This experiment illustrates a practical hybrid local/cloud agent workflow that can dramatically reduce API costs for code generation, which is relevant as developers seek to optimize LLM spending. It highlights the tradeoff between cost and latency, showing that offloading output-heavy tasks to local models can be viable for non-urgent, parallelizable work. The hybrid run used 3 local workers sharing a single GPU, which caused the 2.5x slowdown; the local model produced a slightly less complete result (24/25 checklist items vs 25/25 for Opus alone), though both games were functional with 5 levels, a boss, and a win screen. The author notes this is a single run per mode and only cloud cost is compared, not local compute or electricity.

reddit · r/ClaudeAI · /u/GapNew4766 · Oct 25, 23:21

**Background**: Atomic Agent is a local AI agent tool that supports multiple run modes, including Fusion, where an orchestrator model (like Claude Opus) plans and reviews while a pool of worker models executes subtasks, potentially using local models via llama.cpp. Qwen 3.8 27B is a quantized open-weight model that can run on consumer hardware and is capable of coding tasks. Hybrid inference, combining cloud LLMs for high-level reasoning with local models for bulk generation, is an emerging pattern for cost optimization.

<details><summary>References</summary>
<ul>
<li><a href="https://atomicagent.io/docs/features/fusion/">Fusion run mode | Atomic Agent docs</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen / Qwen 3 . 8 - 27 B · Hugging Face</a></li>
<li><a href="https://www.datasumi.com/blog/hybrid-ai-cloud-local-llm">Hybrid AI Architecture: Cut LLM Costs 50% While Keeping ...</a></li>

</ul>
</details>

**Tags**: `#LLM-agents`, `#cost-optimization`, `#local-models`, `#hybrid-inference`, `#code-generation`

---