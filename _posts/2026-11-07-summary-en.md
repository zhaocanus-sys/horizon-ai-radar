---
layout: default
title: "Horizon Summary: 2026-11-07 (EN)"
date: 2026-11-07
lang: en
---

> From 35 items, 22 important content pieces were selected

---

1. [Libghostty 1.0: Stable C ABI for Terminal Emulation](#item-1) ⭐️ 8.0/10
2. [Asahi Linux 7.3 Report: Technical Gains and Shift to Copyleft](#item-2) ⭐️ 8.0/10
3. [PwnEscape Part 2: Practical Firecracker VM Escape Exploit Detailed](#item-3) ⭐️ 8.0/10
4. [Claude helps solve first 3D structure of mysterious vault particle](#item-4) ⭐️ 8.0/10
5. [Jev orchestrates Opus escalation for 4x cheaper identity resolution](#item-5) ⭐️ 7.0/10
6. [Tesla to wind down Cybertruck production after poor sales](#item-6) ⭐️ 7.0/10
7. [RealPage settles rent-pricing antitrust case for nearly $360M](#item-7) ⭐️ 7.0/10
8. [Essay argues AI is dramatically accelerating AI research, sparking debate](#item-8) ⭐️ 7.0/10
9. [GitHub unveils new horizontally and vertically scalable Git storage architecture](#item-9) ⭐️ 7.0/10
10. [Unitree Factory Tour Sparks Debate on Western Robotics Competitiveness](#item-10) ⭐️ 7.0/10
11. [Restaurant Delivery Scam Uses 404 Typosquatted Domains to Skim Payments](#item-11) ⭐️ 7.0/10
12. [Norvig's 2011 essay on Chomsky and statistical learning resurfaces in LLM era](#item-12) ⭐️ 7.0/10
13. [Sodium-ion batteries near cost parity with LFP, 70 GWh under supply deals](#item-13) ⭐️ 7.0/10
14. [FAA to retire floppy-disk air traffic control systems by 2028](#item-14) ⭐️ 6.0/10
15. [Beginner's Guide to Bare-Metal Programming with UEFI](#item-15) ⭐️ 6.0/10
16. [Google launches Gemini Omni 1.2 Flash video model with better character consistency](#item-16) ⭐️ 6.0/10
17. [Devvm.dev launches per-project VM isolation for development](#item-17) ⭐️ 6.0/10
18. [MIT Press Essay on Volunteer-Built Internet Sparks Hacker News Debate](#item-18) ⭐️ 6.0/10
19. [Nilay Patel: AI Products Don't Justify Their Environmental, Economic, and Social Costs](#item-19) ⭐️ 6.0/10
20. [Microsoft patents AI that alters live speech in broadcasts](#item-20) ⭐️ 6.0/10
21. [Android Remote Control MCP v1.13.0 adds free E2E encrypted tunnel](#item-21) ⭐️ 6.0/10
22. [Lawyer builds game to catch planted errors in AI legal summaries](#item-22) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Libghostty 1.0: Stable C ABI for Terminal Emulation](https://mitchellh.com/writing/libghostty-1-0) ⭐️ 8.0/10

Mitchell Hashimoto released libghostty-vt 1.0, a portable, high-performance C library for terminal emulation extracted from Ghostty, with both the library and its C ABI now stable. This stable C ABI enables a wave of new terminal emulators and agentic coding tools to embed correct, fast terminal emulation without writing their own, reducing fragmentation and speeding up innovation in the terminal ecosystem. libghostty-vt is a zero-dependency library (not even libc) that handles VT sequence parsing, terminal state management, and renderer state management; it uses opaque handles and enum-keyed getters/setters for ABI stability.

hackernews · mfiguiere · Nov 6, 23:30 · [Discussion](https://news.ycombinator.com/item?id=50399933)

**Background**: Ghostty is a fast, feature-rich, cross-platform terminal emulator written in Zig that uses platform-native UI and GPU acceleration. libghostty is an embeddable library extracted from Ghostty's core, exposing a C and Zig API so any application can embed terminal emulation. Zig is a systems programming language that natively supports exporting libraries with the C ABI for use by other languages.

<details><summary>References</summary>
<ul>
<li><a href="https://mitchellh.com/writing/libghostty-1-0">Libghostty 1.0 – Mitchell Hashimoto</a></li>
<li><a href="https://lib.ghostty.org/vt/">libghostty-vt: libghostty-vt</a></li>
<li><a href="https://github.com/ghostty-org/ghostling">GitHub - ghostty-org/ghostling: A minimum viable terminal ...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (536 points, 89 comments) is overwhelmingly positive, with developers praising Mitchell for not promoting his competing product Rex and sharing practical experiences like Android integration and improved TUI performance. Some commenters highlight design insights such as opaque handles and ABI stability, while others discuss specific features like Kitty graphics protocol and OSC-8 hyperlinks.

**Tags**: `#terminal-emulator`, `#zig`, `#c-abi`, `#open-source`, `#developer-tools`

---

<a id="item-2"></a>
## [Asahi Linux 7.3 Report: Technical Gains and Shift to Copyleft](https://asahilinux.org/2026/11/progress-report-7-3/) ⭐️ 8.0/10

Asahi Linux published its 7.3 progress report, detailing technical advancements and announcing a controversial license change from a permissive license to a copyleft license to prevent exploitation. Asahi Linux is a major open-source project bringing Linux to Apple Silicon Macs, so its licensing shift signals growing concern about commercial exploitation of community work and could influence how other hardware-enablement projects license their code. The report states that the project became aware of multiple attempts to exploit its permissive licensing to hijack its work, with the aim of replacing the project and aggressively monetizing Linux on Apple Silicon; the new copyleft terms are intended to keep derivative works open.

hackernews · ackyshake · Nov 7, 05:20 · [Discussion](https://news.ycombinator.com/item?id=50401867)

**Background**: Asahi Linux is a volunteer-driven project that reverse-engineers Apple Silicon system-on-chips to run Linux on M-series Macs, since Apple provides no public documentation. Permissive licenses like MIT allow code to be reused in proprietary products with few conditions, while copyleft licenses such as the GPL require derivative works to remain under the same free terms. The report compares the situation to WINE, which was originally MIT-licensed and suffered from proprietary forks before later changing its license.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asahi_Linux">Asahi Linux</a></li>
<li><a href="https://en.wikipedia.org/wiki/Copyleft_license">Copyleft license</a></li>
<li><a href="https://asahilinux.org/about/">About - Asahi Linux</a></li>

</ul>
</details>

**Discussion**: Commenters largely supported the move to copyleft, with some expressing relief that Asahi abandoned a permissive license, while others debated whether the exploitation referred to Omarchy and noted that Omarchy Mac is itself built on Asahi. One commenter also promoted a competing project, Gravity Linux, claiming Vulkan 1.4 support and suspend-to-RAM progress.

**Tags**: `#Linux`, `#Apple Silicon`, `#Open Source Licensing`, `#Asahi Linux`, `#Hardware Enablement`

---

<a id="item-3"></a>
## [PwnEscape Part 2: Practical Firecracker VM Escape Exploit Detailed](https://pwn.ai/blog/firecracker-escape) ⭐️ 8.0/10

A new blog post from PWN.AI provides a practical walkthrough of exploiting the previously disclosed PwnEscape vulnerability (CVE-2026-122192) to escape Firecracker microVMs and achieve root code execution on the host. The exploit chain targets Firecracker v1.16.1 and demonstrates how a malicious guest can cross the microVM boundary by resolving the live VMM process and taking control of a root-run host process. Firecracker underpins AWS Lambda and other multi-tenant serverless platforms, so a practical guest-to-host escape undermines the isolation guarantees these services rely on. The write-up highlights that production deployments using Firecracker's jailer, namespaces, and seccomp may still be exposed if those controls are not properly configured, prompting organizations to reassess their containment posture. The exploit was demonstrated on a Firecracker configuration without the jailer, meaning privileges were not dropped and the process was not restricted via namespaces or seccomp; the authors note that deployments using those controls require a separate assessment of post-compromise privileges and resources. The vulnerability itself affects Firecracker v0.23.0 through v1.16.1 and, under certain host memory conditions, allows a root user in a guest to read or modify memory of the Firecracker process.

hackernews · SerCe · Nov 6, 19:33 · [Discussion](https://news.ycombinator.com/item?id=50397219)

**Background**: Firecracker is an open-source virtualization technology that creates lightweight microVMs, each with its own kernel and a KVM-enforced boundary, designed for secure multi-tenant container and function-based services. A VM escape occurs when a program breaks out of the virtual machine it runs on and interacts with the host operating system, often by exploiting the hypervisor or virtual machine monitor (VMM). Firecracker's production containment typically includes a jailer that drops privileges and restricts the VMM process through namespaces and seccomp filters.

<details><summary>References</summary>
<ul>
<li><a href="https://pwn.ai/blog/firecracker-escape">Firecracker VM Escape: PwnEscape Part 2. | PWN.AI Security ...</a></li>
<li><a href="https://aws.amazon.com/security/security-bulletins/2026-169-aws/">Vulnerability in Amazon Firecracker</a></li>
<li><a href="https://firecracker-microvm.github.io/">Firecracker</a></li>

</ul>
</details>

**Discussion**: Commenters debated the exploit's practical impact: one noted that the absence of the jailer in the demo means properly jailed deployments need separate assessment, while another argued for formally verified microkernels like Nova to reduce hypervisor complexity. Others pointed out that this is not a new vulnerability but a practical exploitation of a previously disclosed flaw, and one offered a public service hosting hundreds of database engines as a potential testing ground.

**Tags**: `#security`, `#virtualization`, `#firecracker`, `#exploitation`, `#hypervisor`

---

<a id="item-4"></a>
## [Claude helps solve first 3D structure of mysterious vault particle](https://www.reddit.com/r/artificial/comments/1xprvev/claude_helped_solve_the_first_3d_structure_of_a/) ⭐️ 8.0/10

Anthropic reported on November 5 that its science-focused version of Claude scanned about 15 billion computer-predicted proteins to identify a vault-like structure, leading to the first 3D structure of a vault particle encoded by a bacteriophage. The work, completed in under four months, is posted as a preprint on bioRxiv and has not yet been peer-reviewed. This marks a shift from AI merely accelerating known pipelines to AI actively guiding target selection, which could reshape how structural biology research is prioritized. If validated, it demonstrates AI's potential to uncover novel biology in poorly understood systems like vault particles. The preprint comes directly from Anthropic, so independent replication is essential; the team experimentally determined the structure after Claude's computational screen. Vault particles are hollow protein shells whose biological function remains unknown, making this a case of AI-driven discovery in a poorly characterized area.

reddit · r/artificial · /u/winer666 · Nov 6, 23:48

**Background**: Vault particles are large, hollow, barrel-shaped protein complexes found across the tree of life, and their cellular role is still not fully understood. Protein structure prediction uses computational methods to infer 3D shapes from amino acid sequences, and bioRxiv is a preprint server where biologists share findings before peer review.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/investigating-vault-particles-with-claude">Investigating vault particles with Claude \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vault_(organelle)">Vault (organelle) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/BioRxiv:_The_Preprint_Server_for_Biology">BioRxiv: The Preprint Server for Biology</a></li>

</ul>
</details>

**Tags**: `#AI for science`, `#protein structure prediction`, `#Claude`, `#Anthropic`, `#structural biology`

---

<a id="item-5"></a>
## [Jev orchestrates Opus escalation for 4x cheaper identity resolution](https://hightouch.com/blog/llm-judges-identity-resolution) ⭐️ 7.0/10

Hightouch published a blog post showing that using a smaller model, Jev, to decide when to escalate to Claude Opus achieves comparable accuracy to Opus alone at over 4x lower cost for identity resolution tasks. The post also tested GPT-6 Luna as a judge, but the hybrid Jev + Opus approach matched frontier accuracy most cost-effectively. This demonstrates a practical model orchestration pattern where a cheap decision model routes hard cases to a frontier model, potentially making high-accuracy LLM pipelines affordable for large-scale identity resolution and similar tasks. It also highlights the growing ecosystem of specialized small models like Jev that are designed for decision-making rather than chat. The approach relies on Jev's ability to return a choice, score, or yes/no probability instead of chat output, and the escalation policy is task-specific to identity resolution, so results may not generalize to other domains. The blog post does not claim general coding agent improvements, and the cost savings depend on the escalation rate and the relative pricing of the models involved.

hackernews · theanomaly · Nov 6, 19:48 · [Discussion](https://news.ycombinator.com/item?id=50397429)

**Background**: Identity resolution is the process of matching a person's scattered records across systems into one accurate, unified profile, which is important for customer data platforms and LLM applications that need reliable user context. Model routing or cascades send easy queries to a small model and escalate hard ones to a larger model to reduce inference cost, but most deployed routers use uncalibrated confidence scores and require per-workload threshold tuning. Jev is a proprietary AI model developed by TypeSafe AI, released in limited early access in September 2026, designed to make decisions within software by returning a choice, score, or yes/no probability instead of chat.

<details><summary>References</summary>
<ul>
<li><a href="https://hightouch.com/blog/llm-judges-identity-resolution">LLM Judges for Identity Resolution at 4x Lower Cost | Hightouch</a></li>
<li><a href="https://en.wikipedia.org/wiki/Jev_(AI_model)">Jev (AI model) - Wikipedia</a></li>
<li><a href="https://www.onesourcecloud.net/cms/model-routing-reduce-llm-inference-cost.html">Model Routing to Reduce LLM Inference Cost at Scale-OneSource...</a></li>

</ul>
</details>

**Discussion**: HN commenters debated the approach: some shared similar experiences with Qwen orchestrating Claude models, noting that escalation decisions often work well when the smaller model understands the larger model's capabilities, while others cautioned that the economics are highly task-specific. A prominent concern was privacy and ethics, with one commenter criticizing the work as 'AI-assisted privacy violation, 4 times cheaper' and urging developers to consider what they are building. Others saw the pattern as a step toward decision-model-controlled context management beyond static AGENTS.md files.

**Tags**: `#llm-orchestration`, `#cost-optimization`, `#model-routing`, `#identity-resolution`, `#privacy`

---

<a id="item-6"></a>
## [Tesla to wind down Cybertruck production after poor sales](https://www.nbcnews.com/tech/tech-news/tesla-wind-cybertruck-production-years-poor-sales-markets-rcna607817) ⭐️ 7.0/10

Tesla CEO Elon Musk announced on Friday that the company plans to wind down Cybertruck production at its Texas gigafactory around mid-2027, following years of weak sales. Musk called the Cybertruck the 'best vehicle Tesla has ever made' but acknowledged the wind-down as the 'end of an era'. The discontinuation of Tesla's flagship electric pickup signals significant headwinds for the EV market, including the expiration of federal tax credits and declining US EV sales share. It also raises questions about Tesla's future strategy as it pivots toward robotics and AI amid intensifying competition from Chinese EV makers. The Cybertruck, once touted as a rival to legacy pickup trucks, struggled to win mass-market appeal, with only 20,237 units sold in the US in 2025. Its high price, unconventional design, and impracticality for traditional truck uses like towing and hauling contributed to its commercial failure.

hackernews · PLenz · Nov 6, 12:13 · [Discussion](https://news.ycombinator.com/item?id=50391456)

**Background**: The Cybertruck is Tesla's first electric pickup truck, unveiled in 2019 with a futuristic stainless steel exoskeleton design. It was intended to capture a share of the lucrative US pickup market but faced production delays and quality issues. The EV market has also seen policy shifts, such as the expiration of federal tax credits, which have slowed US EV sales growth.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/news/tesla-wind-down-cybertruck-production-094210977.html">Tesla to wind down Cybertruck production at Texas factory as it...</a></li>
<li><a href="https://www.channelnewsasia.com/business/tesla-wind-down-cybertruck-production-after-years-poor-sales-in-few-markets-6530476">Tesla to wind down Cybertruck production after years of poor sales...</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/06/tesla-to-wind-down-cybertruck-production-as-elon-musk-focuses-on-robotics-and-ai">Tesla to wind down Cybertruck production as Elon... | The Guardian</a></li>

</ul>
</details>

**Discussion**: HN commenters expressed mixed views: some praised the Cybertruck's battery capacity for emergency power (equivalent to ~9 Powerwalls), while others criticized its impracticality for truck duties like towing and its narrow appeal. Many discussed Tesla's broader challenges, including the end of federal EV tax credits, the death of the emissions credit market, and competition from Chinese EVs.

**Tags**: `#tesla`, `#electric-vehicles`, `#automotive-industry`, `#business`, `#ev-market`

---

<a id="item-7"></a>
## [RealPage settles rent-pricing antitrust case for nearly $360M](https://www.multifamilydive.com/news/realpage-rent-pricing-case-360m-renters/873553/) ⭐️ 7.0/10

RealPage has agreed to pay nearly $360 million to settle a class-action antitrust lawsuit alleging its algorithmic rent-pricing software facilitated price collusion among landlords, without admitting fault or liability. The settlement sets a significant precedent for how algorithmic pricing tools are scrutinized under antitrust law, potentially affecting landlords, property managers, and software vendors across the rental housing industry. As part of the settlement, RealPage agreed to stop providing nonpublic data to its revenue management system for price recommendations and to stop using competitors' nonpublic data to inform pricing, though the company continues to face separate lawsuits from the DOJ and states.

hackernews · raybb · Nov 6, 23:37 · [Discussion](https://news.ycombinator.com/item?id=50399991)

**Background**: RealPage is a property management software company whose revenue management system uses aggregated market data, including private rental transaction information, to recommend rental prices. The U.S. Department of Justice sued RealPage in 2024, alleging its software enabled landlords to collude and inflate rents. Algorithmic price collusion occurs when competitors use shared algorithms to coordinate pricing without explicit communication, raising novel questions under antitrust law.

<details><summary>References</summary>
<ul>
<li><a href="https://www.justice.gov/archives/opa/pr/justice-department-sues-realpage-algorithmic-pricing-scheme-harms-millions-american-renters">Office of Public Affairs | Justice Department Sues RealPage for...</a></li>
<li><a href="https://www.claimdepot.com/settlements/realpage-rental-settlement">RealPage $359.93M Renters Antitrust Class Action Settlement</a></li>
<li><a href="https://www.genspark.ai/spark/understanding-the-realpage-algorithm/ec4bebe5-a057-46fc-8e85-6bba1ef3c736">Understanding the RealPage Algorithm - Genspark</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism that the settlement will change RealPage's behavior, noting the company still has a decade of pricing data to draw on. Others called for a public rental registry to address information disparity, and some debated whether lack of competition is a root cause of high living costs.

**Tags**: `#antitrust`, `#algorithmic-pricing`, `#real-estate`, `#regulation`, `#competition-policy`

---

<a id="item-8"></a>
## [Essay argues AI is dramatically accelerating AI research, sparking debate](https://www.planned-obsolescence.org/p/ai-is-dramatically-accelerating-ai) ⭐️ 7.0/10

An essay on planned-obsolescence.org argues that AI, particularly large language models, is dramatically accelerating AI research itself, potentially by up to 10x in some areas. The piece sparked a Hacker News discussion with 219 comments debating the depth and real-world significance of this acceleration. If AI truly accelerates AI research, it could lead to faster innovation cycles and compounding progress in the field, but skeptics argue that much of the observed speedup is limited to local experimentation and may not translate to broader scientific or societal impact. The debate highlights growing concerns about benchmark overfitting, capital-driven scaling, and the distinction between narrow speedups and genuine breakthroughs. Commenters noted that LLMs speed up parts of ML research like model architecture experiments and training strategy, but this does not imply imminent superintelligence; others pointed out that benchmarks are curated and can be trained on, and that much of the progress may stem from capital-intensive scaling rather than fundamental model intelligence.

hackernews · yurivish · Nov 6, 20:27 · [Discussion](https://news.ycombinator.com/item?id=50397994)

**Background**: The debate touches on neural scaling laws, which describe how model performance improves predictably with increases in model size, data, and compute. It also involves the limitations of LLM benchmarks, which are standardized tests used to evaluate model capabilities but can be gamed through overfitting. The concept of 'meta-science'—the study of how research itself is conducted—is relevant as AI tools increasingly assist in scientific discovery.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Neural_scaling_law">Neural scaling law - Wikipedia</a></li>
<li><a href="https://www.citrusx.ai/posts/7-llm-benchmarks-for-performance-capabilities-and-limitations">7 LLM Benchmarks for Performance, Capabilities, and Limitations</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was skeptical overall. Practitioners argued that AI mainly accelerates local, compute-bound experimentation and does not necessarily lead to world-changing outcomes; others raised concerns about benchmark overfitting and the role of capital-driven scaling versus genuine model intelligence, with some recommending alternative analyses.

**Tags**: `#AI research`, `#LLMs`, `#benchmarking`, `#scaling`, `#meta-science`

---

<a id="item-9"></a>
## [GitHub unveils new horizontally and vertically scalable Git storage architecture](https://github.blog/engineering/architecture-optimization/inside-githubs-new-git-storage-architecture/) ⭐️ 7.0/10

GitHub detailed a new Git storage architecture designed to scale both horizontally (across machines) and vertically (within a single repository), with most requirements driven by the need to support more developers and AI agents working on the same repo. This architecture aims to handle the growing load from AI agents and larger, busier repositories, which could improve reliability and performance for GitHub's massive user base, though it may not immediately address recent outages. The design carries over horizontal scaling techniques from the existing architecture while introducing new vertical scaling capabilities for intra-repo scalability, but GitHub admits that the most active repositories today will receive the benefits first.

hackernews · DAlperin · Nov 6, 19:24 · [Discussion](https://news.ycombinator.com/item?id=50397099)

**Background**: GitHub stores millions of Git repositories, and as more developers and AI agents contribute code, individual repositories grow larger and busier. Horizontal scaling adds more machines to distribute load, while vertical scaling improves the capacity of a single repository. GitHub's new architecture is an evolution of its existing system to meet these demands.

<details><summary>References</summary>
<ul>
<li><a href="https://github.blog/engineering/architecture-optimization/inside-githubs-new-git-storage-architecture/">Inside GitHub's new Git storage architecture - The GitHub Blog</a></li>

</ul>
</details>

**Discussion**: Commenters questioned whether the new architecture addresses recent outages, noted similarities to prior art like enroute.sh, and debated source control design for AI agents. Some expressed hope that it improves reliability, while others suggested alternative approaches like banning abusive users.

**Tags**: `#git`, `#github`, `#distributed-systems`, `#storage-architecture`, `#scalability`

---

<a id="item-10"></a>
## [Unitree Factory Tour Sparks Debate on Western Robotics Competitiveness](https://josef.cn/blog/unitree) ⭐️ 7.0/10

A blog post recounting a firsthand tour of Unitree's factory argues that the West will ultimately win in robotics because higher labor costs will drive automation, but commenters widely criticize the conclusion as a logical non-sequitur. The debate highlights a key question in robotics economics: whether high labor costs are sufficient to drive automation leadership, or whether manufacturing know-how and supply chain advantages in China will prove more decisive. The author claims Unitree robots are largely hand-assembled and labor accounts for only about 8% of manufacturing cost, so there is little incentive to automate in China; commenters counter that the remaining 92% of costs and other factors are ignored.

hackernews · josefchen · Nov 7, 01:05 · [Discussion](https://news.ycombinator.com/item?id=50400597)

**Background**: Unitree Robotics is a Chinese company founded in 2016 that produces quadruped and humanoid robots, including a humanoid model priced around $16,000. The blog post uses the factory tour to speculate on the future of Western robotics competitiveness, drawing comparisons between Chinese manual assembly and Western automation incentives.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unitree_Robotics">Unitree Robotics</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1043951X25000318">Labor cost, robots, and product quality - ScienceDirect</a></li>

</ul>
</details>

**Discussion**: Commenters largely reject the article's conclusion, with several pointing out that the argument that higher labor costs lead to more automation does not logically imply that the West will win the robotics race. Others note that financial imbalances, such as lower wages and rent in China, and the West's rent-extraction sector, may be more relevant factors.

**Tags**: `#robotics`, `#manufacturing`, `#automation`, `#economics`, `#unitree`

---

<a id="item-11"></a>
## [Restaurant Delivery Scam Uses 404 Typosquatted Domains to Skim Payments](https://www.infohawk.com/news/2026-11-05-scamwich-restaurant-skimming) ⭐️ 7.0/10

An investigative report details a payment-skimming campaign that used 404 typosquatted domains impersonating a single restaurant brand to intercept delivery orders and steal payment data. The campaign exploited common misspellings of the brand's domain to redirect users to fake sites that harvested payment information. This incident highlights the growing scale and sophistication of typosquatting-based payment fraud, which can affect any online business and erode consumer trust in e-commerce. It also underscores the role of ad networks in enabling such scams and the challenges of mitigating abuse in centralized platforms. The attackers registered 404 fake domains covering various misspellings of the restaurant brand, ensuring that users never encountered a 404 error and always landed on a scam site. The campaign likely relied on malicious ads and may extend beyond food delivery to other e-commerce sectors and markets.

hackernews · fiej · Nov 6, 19:19 · [Discussion](https://news.ycombinator.com/item?id=50397017)

**Background**: Typosquatting, also known as URL hijacking, is a form of cybersquatting where attackers register domain names that are common misspellings of a legitimate site to trick users who mistype the address. Payment skimming campaigns involve injecting malicious code or creating fake checkout pages to steal credit card details during online transactions. Ad networks like Google Ads have policies against ad network abuse, but enforcement can be inconsistent, allowing scam ads to proliferate.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Typosquatting">Typosquatting</a></li>
<li><a href="https://support.microsoft.com/en-us/edge/security/what-is-typosquatting">What is typosquatting ? | Microsoft Support</a></li>
<li><a href="https://moofdigital.com/google-ads-ad-network-abuse-policy-splits-into-3/">Google Ad Network Abuse Policy Splits into 3 - MooF Digital...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration with ad networks like Google AdSense for allowing scam ads, with some calling for RICO-style accountability. Others marveled at the scale of 404 domains and noted the irony of never seeing a 404 error, while some discussed the difficulty of defense and the trade-offs of centralized platforms versus federated alternatives.

**Tags**: `#security`, `#fraud`, `#typosquatting`, `#advertising`, `#web-security`

---

<a id="item-12"></a>
## [Norvig's 2011 essay on Chomsky and statistical learning resurfaces in LLM era](https://www.norvig.com/chomsky.html) ⭐️ 7.0/10

Peter Norvig's 2011 essay 'On Chomsky and the Two Cultures of Statistical Learning' is being revisited on Hacker News, where commenters debate its relevance to modern large language models (LLMs). The essay responds to Noam Chomsky's criticism of purely statistical approaches in machine learning, arguing that statistical models can provide both engineering success and scientific insight into language. This debate is central to understanding the ongoing tension between rule-based linguistic theories and data-driven machine learning, especially as LLMs like GPT-4 achieve unprecedented language generation capabilities. It affects how researchers and engineers justify their approaches and what counts as scientific progress in AI and linguistics. Norvig's essay specifically addresses Chomsky's points that statistical language models have engineering success but are irrelevant to science, that they are incomprehensible, and that they fail to reflect human cognitive processes. Norvig counters by arguing that statistical models better represent linguistic reality than Chomsky's idealized Universal Grammar framework.

hackernews · andsoitis · Nov 6, 08:18 · [Discussion](https://news.ycombinator.com/item?id=50389570)

**Background**: Noam Chomsky's generative linguistics, introduced in the 1950s, posits that language is governed by innate rule-based structures, such as Universal Grammar. In contrast, statistical learning in NLP uses probabilistic models trained on large corpora to perform tasks like translation and text generation. The debate between these two cultures—symbolic rule-based versus statistical data-driven—has shaped the field of AI and linguistics for decades.

<details><summary>References</summary>
<ul>
<li><a href="https://www.norvig.com/chomsky.html">On Chomsky and the Two Cultures of Statistical Learning</a></li>
<li><a href="https://en.wikipedia.org/wiki/Syntactic_Structures">Syntactic Structures - Wikipedia</a></li>
<li><a href="https://link.springer.com/chapter/10.1007/978-3-658-12153-2_3">On Chomsky and the Two Cultures of Statistical Learning 2. On Chomsky and the Two Cultures of Statistical Learning1 On Chomsky and the Two Cultures of Statistical Learning On Chomsky and the Two Cultures of Statistical Learning Colorless Green Ideas Learn Furiously: Chomsky and the Two ... On Chomsky and the Two Cultures of Statistical Learning</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News debate whether Norvig confuses engineering with science, with some arguing that LLMs' success does not validate statistical models as scientific explanations of language. Others contend that LLMs' ability to generate novel sentences (creative aspects of language use) challenges Chomsky's stance and provides insights into linguistic phenomena.

**Tags**: `#nlp`, `#linguistics`, `#machine-learning`, `#llm`, `#chomsky`

---

<a id="item-13"></a>
## [Sodium-ion batteries near cost parity with LFP, 70 GWh under supply deals](https://www.pv-magazine.com/2026/11/06/sodium-ion-batteries-approach-cost-parity-with-lfp-with-70-gwh-covered-by-supply-agreements/) ⭐️ 7.0/10

Sodium-ion batteries are approaching cost parity with lithium iron phosphate (LFP) chemistry, with 70 GWh of capacity already covered by supply agreements, according to a pv-magazine report. This marks early validation of cost-curve predictions for the sodium-ion chemistry. If sodium-ion reaches cost parity with LFP, it could become a cheaper and more sustainable alternative for stationary energy storage, reducing reliance on lithium and easing supply-chain pressure. This would benefit grid-scale and home storage deployments, where energy density is less critical than cost and safety. Sodium-ion batteries typically have lower energy density than lithium-ion, but they offer advantages in safety and low-temperature operation, making them suitable for stationary storage. The 70 GWh of supply agreements indicates commercial traction, though production is still ramping up, as CATL is only now scaling its Naxtra sodium-ion line.

hackernews · doener · Nov 6, 23:00 · [Discussion](https://news.ycombinator.com/item?id=50399657)

**Background**: Sodium-ion batteries use sodium ions as charge carriers instead of lithium, which is abundant and cheap. LFP (lithium iron phosphate) batteries are a low-cost, safe lithium-ion variant widely used in energy storage and some EVs. Cost parity means sodium-ion can match LFP on price, a key milestone for adoption in grid and home storage.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sodium-ion_battery">Sodium-ion battery - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lithium_iron_phosphate_battery">Lithium iron phosphate battery - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed enthusiasm for sodium-ion in home storage due to safety and low-temperature operation, with some noting real-world use in 12V replacements. Others highlighted the rapid cost decline as validation of predictions, and discussed the broader implications for lithium demand and energy investment priorities.

**Tags**: `#batteries`, `#energy-storage`, `#sodium-ion`, `#clean-energy`, `#hardware`

---

<a id="item-14"></a>
## [FAA to retire floppy-disk air traffic control systems by 2028](https://www.reuters.com/world/us/us-faa-says-it-will-phase-out-floppy-disks-air-traffic-control-by-2028-2026-11-05/) ⭐️ 6.0/10

The US Federal Aviation Administration announced it will phase out floppy-disk-based air traffic control systems by 2028, replacing four 1980s-era display systems with a single modern platform called E-IDS. This modernization affects the safety and efficiency of US air traffic control, which handles up to 45,000 flights daily, and highlights the challenges of upgrading critical legacy infrastructure across government and industry. The legacy IDS-4 systems use MS-DOS and 1.44 MB 3.5-inch floppy disks, and the replacement E-IDS has been in development since at least 2020 with a planned rollout starting in 2025; the FAA's rigorous safety risk management process can slow such upgrades.

hackernews · ChrisArchitect · Nov 6, 04:00 · [Discussion](https://news.ycombinator.com/item?id=50388001)

**Background**: Air traffic controllers rely on numerous legacy systems to monitor weather, conduct surveillance, and manage communications. The FAA's aging technology has contributed to flight delays and incidents, prompting GAO reports urging urgent modernization. Floppy disks, once standard storage, are now obsolete but persist in safety-critical systems where stability and predictability are prioritized over novelty.

<details><summary>References</summary>
<ul>
<li><a href="https://www.engadget.com/2308330/the-faa-is-finally-phasing-out-floppy-disks-from-air-traffic-control/">The FAA Is Finally Phasing Out Floppy Disks From Air Traffic Control</a></li>
<li><a href="https://korben.info/en/faa-retiring-floppy-disks-us-air-traffic-control.html">The FAA is finally getting rid of its floppy disks in US air traffic control</a></li>
<li><a href="https://www.gao.gov/products/gao-26-107992">Air Traffic Control Systems: Ambitious New Modernization ...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters with FAA experience described a rigorous safety culture that slows progress, while others debated whether floppy emulators or SD cards could have extended the systems' life and criticized political grandstanding over the announcement. Some noted the IDS-4 was actually developed in the early 1990s, not the 1980s, and questioned the vague description of the replacement system.

**Tags**: `#legacy-systems`, `#aviation`, `#government-it`, `#modernization`, `#safety-critical`

---

<a id="item-15"></a>
## [Beginner's Guide to Bare-Metal Programming with UEFI](https://kevinboone.me/efitest_index.html) ⭐️ 6.0/10

Kevin Boone published a beginner's guide to bare-metal programming using UEFI, covering setup, pitfalls, and tooling. The guide is part of a series and has sparked community discussion with additional resources and insights. This guide lowers the entry barrier for systems programmers interested in UEFI development, which is crucial for bootloaders, firmware, and low-level system software. It helps demystify the complex UEFI environment and encourages more developers to explore bare-metal programming. The guide highlights the lack of a C standard library in UEFI and the Windows-like coding style of EFI, and suggests using nm -D --undefined-only to verify no external symbols remain after linkage. Community members also point to edk2-libc as a standard library alternative and to existing resources like Rod Smith's and OSDev Wiki's guides.

hackernews · LaSombra · Nov 6, 16:50 · [Discussion](https://news.ycombinator.com/item?id=50394855)

**Background**: UEFI (Unified Extensible Firmware Interface) is the modern firmware interface that replaces BIOS and initializes hardware before loading the operating system. Bare-metal programming means writing software that runs directly on hardware without an OS, often used for bootloaders and firmware. UEFI provides a runtime environment for such programs, but it differs significantly from typical OS environments, lacking standard libraries and using its own conventions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UEFI">UEFI - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters appreciated the guide and shared additional resources: edk2-libc for standard library support, OSDev Wiki and Rod Smith's guides for alternative tutorials, and FreeBSD/NetBSD base environments for EFI development. They also noted practical tips like using nm -D --undefined-only to check for undefined symbols and mentioned other projects like a UEFI IRC client.

**Tags**: `#UEFI`, `#bare-metal`, `#systems-programming`, `#tutorial`, `#firmware`

---

<a id="item-16"></a>
## [Google launches Gemini Omni 1.2 Flash video model with better character consistency](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemini-omni-1-2-flash/) ⭐️ 6.0/10

Google has introduced Gemini Omni 1.2 Flash, a new multimodal video generation model that improves character consistency and can generate 15-second clips in a single call. It is being rolled out through Google Flow, Google Vids, and other Google products, though availability varies across free and paid tiers. Character consistency is one of the hardest problems in AI video generation, so improvements here could make the model more useful for creators building multi-scene narratives. The release also shows Google pushing its Gemini models deeper into creative tools like Flow and Vids, competing with other AI video platforms. The model supports video generation, editing, extension, and upscaling, and its 15-second clip length removes the need to stitch together two 10-second generations as with earlier Gemini Omni models. However, access is fragmented: Google Vids offers 15-second clips for free, while the Gemini app provides it on paid plans with different video length limits and no clear rollout timeline.

hackernews · thisisauserid · Nov 6, 13:35 · [Discussion](https://news.ycombinator.com/item?id=50392118)

**Background**: Google Flow is a generative AI video and multimedia creation tool introduced in 2025 that lets users create videos, music, and images using natural language prompts, built on models like Veo and Imagen. Character consistency refers to the ability to keep a character's appearance, expressions, and wardrobe uniform across different scenes, a challenge because diffusion-based video models start each generation from random noise, leading to variations even with identical prompts.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/products-and-platforms/products/workspace/omni-1-2-flash-google-vids/">Create longer AI videos with Omni 1 . 2 in Google Vids</a></li>
<li><a href="https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/gemini/omni-1-2-flash">Gemini Omni 1 . 2 Flash | Gemini Enterprise Agent Platform</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_Flow">Google Flow - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration over Google's confusing rollout and access restrictions, with some saying they cannot try the model despite paying for Google AI Plus. Others clarified that this is a video model available in Google Flow, not a replacement for Gemini 4, and noted that the claimed character consistency improvement is hard to verify from limited use.

**Tags**: `#AI`, `#video generation`, `#Google`, `#Gemini`, `#model release`

---

<a id="item-17"></a>
## [Devvm.dev launches per-project VM isolation for development](https://devvm.dev/) ⭐️ 6.0/10

Devvm.dev has launched a tool that creates a dedicated virtual machine for each software project, providing an isolated sandbox with the project's toolchain that is ready for a developer or a coding agent to start working. The VM opens a shell whose prompt starts with (devvm), and each project's VM owns its own Docker engine, database, services, and ports to avoid collisions with the host or other project VMs. This tool addresses the growing need for strong isolation when running AI coding agents and complex development environments, where cross-project dependency conflicts and security risks are common. It enters a crowded space of virtualization alternatives, so its success will depend on how well it handles enterprise requirements like secure access to internal registries and infrastructure. The VM is designed to be used with coding agents such as Claude Code, and a companion Claude Code skill exists to integrate devvm into agent workflows. However, the documentation does not clearly state whether images are built per project or copy-on-write from shared toolchains, and community members note that it lacks features like memory ballooning, GPU acceleration, and credential-injecting proxies found in enterprise setups.

hackernews · luispa · Nov 6, 17:30 · [Discussion](https://news.ycombinator.com/item?id=50395450)

**Background**: Development environment isolation tools aim to prevent conflicts between projects by encapsulating dependencies, services, and configurations in separate environments. Virtual machines provide stronger isolation than containers because they include their own kernel, making them suitable for running untrusted code or AI agents. Existing solutions include libvirt with cloud-init, krunkit, smolvm, and container-based tools like ddev, each with different trade-offs in performance, manageability, and feature set.

<details><summary>References</summary>
<ul>
<li><a href="https://devvm.dev/">devvm</a></li>
<li><a href="https://github.com/diazhh/claude-devvm-skill">GitHub - diazhh/claude- devvm -skill: Claude Code / devvm skill — give...</a></li>

</ul>
</details>

**Discussion**: Commenters compared devvm to existing tools like krunkit, libvirt, and smolvm, with some dismissing it as a toy that lacks enterprise features such as secure access to internal registries, memory ballooning, and GPU acceleration. Others shared their own similar projects and noted interesting features like proxying, while one commenter highlighted a security concern about .git hooks in cloned repositories potentially enabling malicious code execution.

**Tags**: `#virtualization`, `#development-environment`, `#VMs`, `#isolation`, `#tooling`

---

<a id="item-18"></a>
## [MIT Press Essay on Volunteer-Built Internet Sparks Hacker News Debate](https://thereader.mitpress.mit.edu/from-linux-to-wikipedia-how-volunteers-build-the-internet/) ⭐️ 6.0/10

An essay published on The MIT Press Reader examines how volunteer efforts built foundational internet projects like Linux and Wikipedia, and the piece sparked a Hacker News discussion with 319 points and 124 comments. The discussion highlights growing concerns about the commercialization and centralization of technology, and how these trends may erode the passion, skills, and decentralized nature that made early internet projects successful. Commenters noted that while volunteerism was crucial, many key contributors to projects like Linux were actually paid by companies with commercial interests, complicating the romantic narrative of purely volunteer-driven development.

hackernews · jonbaer · Nov 6, 04:17 · [Discussion](https://news.ycombinator.com/item?id=50388122)

**Background**: The MIT Press Reader is an online publication that features essays, interviews, and excerpts from the MIT Press catalog, aimed at a general audience but grounded in academic rigor. Linux and Wikipedia are often cited as flagship examples of volunteer-driven, decentralized collaboration that produced widely used resources.

<details><summary>References</summary>
<ul>
<li><a href="https://thereader.mitpress.mit.edu/">The MIT Press Reader</a></li>
<li><a href="https://en.wikipedia.org/wiki/The_MIT_Press_Reader">The MIT Press Reader</a></li>
<li><a href="https://www.varsitytech.com/built-by-the-people-open-source-internet/">Built By The People: The Open Source Story Behind The Internet</a></li>

</ul>
</details>

**Discussion**: Commenters expressed nostalgia for early volunteer-driven tech culture, with some arguing that commercialization and cloud computing have eroded passion and skills, while others pointed out that paid contributions were always part of the picture. A few highlighted the hopeful lesson that people will voluntarily build thorough, free knowledge resources when given the chance.

**Tags**: `#open-source`, `#volunteerism`, `#internet-history`, `#tech-culture`, `#community`

---

<a id="item-19"></a>
## [Nilay Patel: AI Products Don't Justify Their Environmental, Economic, and Social Costs](https://simonwillison.net/2026/Nov/6/nilay-patel/) ⭐️ 6.0/10

In a quote surfaced by Simon Willison's blog from The Vergecast episode 'Big Tech lost big in the 2026 election,' Nilay Patel argues that AI products are not good enough to justify their costs, citing data center noise, deepfake slop, and companies spending more than they earn. He contends that agents 'aren't real' and that the industry will not recover until it makes genuinely better products. This critique from a prominent tech commentator highlights growing skepticism about the AI industry's economics and societal costs, resonating with broader concerns about an AI bubble and the environmental footprint of data centers. It could influence public discourse and investor sentiment as spending on AI infrastructure continues to outpace revenue. Patel specifically points to the environmental burden of data centers (the 'whine' in backyards), the poor quality of AI-generated content ('deep fake slop'), and the gap between industry spending and revenue. He also mentions hacked refrigerators holding blood storage in Europe as an example of real-world security costs, and ties the industry's political lobbying to 'crypto-corruption.'

rss · Simon Willison · Nov 6, 17:13

**Background**: AI agents are systems that use machine learning and natural language processing to autonomously perform tasks, but their practical reliability and adoption remain debated. Data centers powering AI have significant electricity, water, and carbon footprints, and recent analyses suggest the AI industry is spending hundreds of billions annually on infrastructure while revenue lags far behind, fueling bubble concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pbs.org/newshour/science/energy-water-use-and-pollution-of-ai-and-data-centers-rival-most-countries">Energy, water use and pollution of AI and data centers rival ...</a></li>
<li><a href="https://shattered.io/ai-boom-real-or-bubble-nikhil-kamath-700b-vs-100b-2026/">AI Boom or Bubble: $700B Spend vs $100B Revenue [2026]</a></li>
<li><a href="https://www.microsoft.com/en-us/copilot/ai-knowledge/ai-agents-faq">AI Agent FAQ: Definitions and Explanations | M365 Copilot</a></li>

</ul>
</details>

**Tags**: `#AI industry`, `#AI economics`, `#tech criticism`, `#commentary`, `#AI hype`

---

<a id="item-20"></a>
## [Microsoft patents AI that alters live speech in broadcasts](https://www.reddit.com/r/artificial/comments/1xp3pww/microsoft_files_patent_for_ai_that_can_alter_what/) ⭐️ 6.0/10

Microsoft has filed a patent for an AI system that can modify spoken words in real-time during live broadcasts, according to a Reddit post linking to the filing. The technology would allow words to be altered as they are spoken, raising concerns about potential media manipulation. This patent highlights the growing capability of AI to manipulate audio in real-time, which could have significant implications for media authenticity and public trust. If commercialized, such technology could be used to spread misinformation or alter live events, affecting broadcasters, audiences, and regulators. The patent application describes a system for real-time speech modification during live broadcasts, but it is unclear whether Microsoft intends to productize the technology. Similar real-time voice alteration tools already exist for entertainment and privacy, but this patent specifically targets broadcast speech.

reddit · r/artificial · /u/Resident-Fall4351 · Nov 6, 04:25

**Background**: Real-time speech modification uses AI to alter voice characteristics such as pitch, tone, or content as a person speaks. While such technology has been used in voice changers for gaming and anonymity, applying it to live broadcasts raises ethical questions about consent and authenticity. Microsoft has previously filed patents for controversial AI applications, including chatbots that simulate deceased individuals.

<details><summary>References</summary>
<ul>
<li><a href="https://www.altered.ai/real-time/">Real-Time Voice Changer | Altered</a></li>
<li><a href="https://www.cnet.com/science/microsoft-patent-details-tech-that-could-turn-dead-people-into-ai-chatbots/">Microsoft patent details tech that could turn dead people into... - CNET</a></li>
<li><a href="https://plato.stanford.edu/entries/ethics-ai/">Ethics of Artificial Intelligence and Robotics (Stanford Encyclopedia of...)</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion likely expresses concerns about the ethical implications, such as the potential for misuse in propaganda and the erosion of trust in live media. Some commenters may question Microsoft's motives and call for transparency and regulation.

**Tags**: `#AI ethics`, `#patent`, `#live broadcasting`, `#speech modification`, `#Microsoft`

---

<a id="item-21"></a>
## [Android Remote Control MCP v1.13.0 adds free E2E encrypted tunnel](https://www.reddit.com/r/artificial/comments/1xpf8k5/android_remote_control_mcp_v1130_is_out_free/) ⭐️ 6.0/10

Android Remote Control MCP v1.13.0 introduces a built-in, free end-to-end encrypted HTTPS tunnel that requires no account and uses Let's Encrypt, Google Trust Services, and ZeroSSL for certificates. The app also monitors Certificate Transparency logs to warn if a certificate for the user's name is issued to another key. This release makes it significantly easier and more private for AI agents to remotely control Android apps, as users can set up a secure tunnel in under a minute without creating accounts or relying on third-party services like Cloudflare or ngrok that can see traffic. It lowers the barrier for integrating Android automation into AI workflows via MCP. The encryption terminates on the phone, and the certificate key never leaves the device; the app also watches Certificate Transparency logs for unauthorized certificate issuance. The project is now licensed under GPL-3.0-or-later, and the tunnel source code is available in a separate repository.

reddit · r/artificial · /u/daniele_dll · Nov 6, 15:13

**Background**: MCP (Model Context Protocol) is an open standard developed by Anthropic that allows AI applications like Claude or ChatGPT to connect to external tools and data sources. Android Remote Control MCP is an MCP server that runs on an Android phone and uses the accessibility service to let AI agents control any app without needing adb, cables, or root. Certificate Transparency (CT) is a system for logging and monitoring TLS certificate issuance, allowing anyone to audit certificates.

<details><summary>References</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>
<li><a href="https://www.anthropic.com/news/model-context-protocol">Introducing the Model Context Protocol \ Anthropic</a></li>
<li><a href="https://certificate.transparency.dev/">Certificate Transparency : Certificate Transparency</a></li>

</ul>
</details>

**Tags**: `#MCP`, `#Android`, `#end-to-end-encryption`, `#AI-agents`, `#open-source`

---

<a id="item-22"></a>
## [Lawyer builds game to catch planted errors in AI legal summaries](https://www.reddit.com/r/artificial/comments/1xpgt8f/i_am_a_lawyer_and_made_a_small_game_an_ai_summary/) ⭐️ 6.0/10

A lawyer created "Catch the AI," a small game where players read an AI-generated summary of a real judgment containing four planted mistakes and must highlight the exact words in the judgment that disprove each error to score a catch. The game is part of "May or Shall," a legal AI tool built on the principle that human judgment comes first and AI drafting follows. This game highlights a real and underappreciated problem in legal AI: summaries that read fluently but subtly misstate the law, such as overbroad holdings or misreported rulings. By requiring players to cite the exact source text, it demonstrates a human-in-the-loop verification method that could influence how legal professionals evaluate AI outputs. The game uses a real judgment and an AI summary with four planted errors, and a catch only counts when the player highlights the specific words in the judgment that prove the summary wrong. It is available as a web app at app.mayorshall.com/play and is part of a Chrome extension and website called "May or Shall."

reddit · r/artificial · /u/siddiboyz · Nov 6, 16:16

**Background**: Large language models are prone to "hallucinate," generating plausible but false information, which is especially risky in high-stakes legal work. Studies and trackers have documented cases where AI-generated legal content led to sanctions, and researchers are exploring human-in-the-loop evaluation to combine human oversight with AI efficiency. "May or Shall" is a legal AI tool that emphasizes human judgment first, with AI assisting in drafting and summarization.

<details><summary>References</summary>
<ul>
<li><a href="https://www.damiencharlotin.com/hallucinations/">AI Hallucination Cases Database – Damien Charlotin</a></li>
<li><a href="https://dho.stanford.edu/wp-content/uploads/Legal_RAG_Hallucinations.pdf">Hallucination‐Free? Assessing the Reliability of Leading AI ...</a></li>
<li><a href="https://app.mayorshall.com/play">Play to Demo: test your legal reading | May or Shall</a></li>

</ul>
</details>

**Tags**: `#ai`, `#legal-tech`, `#hallucination`, `#evaluation`, `#human-in-the-loop`

---