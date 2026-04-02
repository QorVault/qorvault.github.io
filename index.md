# The Person Who Always Saw the Fix Can Finally Build It

### How an Air Force veteran and school board director — with a degree in network security but zero coding ability — built a civic AI system from scratch using AI as his translator

---

I once built a network bypass out of a battery-powered wireless router, a cell phone hotspot, and an RJ-45 cable.

I was a home security technician at Comcast. The company had launched the product line in 2011 and there weren't many of us trained on it, so we'd be booked solid all day with installations. The problem was that the security router needed an internet connection to pull its configuration and run updates, and the internet tech — a different person, doing a different job — wasn't always done yet. So I'd sit there waiting, watching my schedule stack up, because two independent workflows had an unnecessary dependency between them.

The fix was obvious to me. Decouple them. I had a battery-powered portable wireless router — don't ask me why I already owned one — and I realized I could tether it to my phone's hotspot, run an ethernet cable from it to the security router, and let the security hardware do its configuration pull independently while the internet tech finished their work. It cost almost nothing. It saved hours per week across every security tech in the region.

I didn't ask permission. I built it with my own equipment, tested it for a few weeks until I was confident it was bulletproof, wrote a step-by-step setup guide for the less tech-savvy technicians, and then showed it to my boss. He asked if I'd teach the other guys. Comcast bought the equipment. From what I was told, the solution was rolled out across the region.

That was the first time I built something nobody asked me to build because I could see a systemic problem that nobody else seemed bothered by. It would not be the last.

---

## The Pattern

I should back up, because how I ended up at Comcast matters for the rest of this story.

I grew up in Kent, Washington. My family has been here for about a hundred years — my great-grandmother went to Kent High School, my grandmother and mother went to Kent-Meridian, my wife went to Kentridge. I went to Kentwood my sophomore year, then Kentlake when it opened in 1997. I did Running Start at Green River Community College my junior and senior years, mostly so I could work, which became more pressing when I moved out at seventeen. My parents had relocated to Ellensburg around February of my junior year. I lived there for about eight months, but I didn't take to it, so I came back senior year.

After high school I worked retail, then banking. The summer of 2000, a friend suggested I join the Air Force with him. I knew I wasn't ready for college and I didn't think banking was going to be my career, so I enlisted in October. I was told I scored high on the administrative section of the ASVAB, which the Air Force interpreted as meaning I'd make a good network administrator. I didn't see the connection, but it sounded interesting.

I spent nearly four years as a network admin, based at RAF Mildenhall in England. When the base communications team deployed, we all went — Camp Snoopy in Qatar in 2002, Talil Air Base in Iraq in 2004. Qatar was a non-combat deployment, but the conditions took a toll. They had us working six twelve-hour days, switching between day and night shifts every two weeks, for six months. Operations Iraqi Freedom and Enduring Freedom kicked off while we were there, but there was no action in Qatar itself. The sleep deprivation from that rotation was severe enough that I attempted suicide during the deployment. I lost a colleague while I was there — a motorcycle accident back at Mildenhall. He'd just had a kid. I wish I'd stayed back and he'd gone.

Separately from the deployments, I was selected for the Theater Deployable Communications shop at Mildenhall, which meant additional training at Keesler Air Force Base on specialized equipment designed to stand up network infrastructure for contingents of up to about a thousand airmen. The job involved a lot of maintaining equipment that wasn't in constant production use and building training materials for others — work I genuinely enjoyed.

When I went to Iraq in 2004, they put me in force protection — essentially guard duty over the third-country nationals who worked on base. Not a great use of my network skills, but I managed to enjoy my time there as much as one can in 116-degree heat.

I got out in July 2004, went back to banking because federal law required them to give me my job back, discovered I was making about two dollars an hour more than my colleagues since they couldn't reduce my pay, got into a branch manager training program at Washington Federal Savings, learned I didn't like that kind of work, and left for Comcast in 2006.

I'd spend the next eighteen and a half years there. The first thirteen and a half as a field technician — starting in cable, moving into commercial services, eventually taking on home security a few years after Comcast launched that product line. For a while I did both commercial and home security before deciding that was too much and making home security my primary focus while still augmenting the commercial team as needed. That's where the hotspot hack happened, a few years into the home security work. For about ten of those years on the truck, I was also going to school, mostly back at Green River — the same community college where I'd done Running Start as a teenager. In 2019, I finished a Bachelor of Applied Science in Network Administration and Security. There was some basic scripting in the coursework and I think I took a single intro-to-programming class, long since forgotten.

The degree was my catalyst to get off the truck — thirteen and a half years of climbing poles and ladders in Pacific Northwest weather was enough. I moved into a project management role overseeing enterprise fiber installations. The initial system I worked out of was fine, a little convoluted, but things mostly worked. Then I was switched to a new system that Comcast had paid a third-party firm to build. I knew there would be growing pains since it was still under construction when we started using it.

What I didn't expect was that the growing pains would never end — and the reason was structural. The same firm that designed the system was contracted to maintain it, which meant they had no adversarial incentive to fix their own design flaws. The maintenance contract was the revenue stream. I remember thinking at the time that Comcast should have hired a competing firm for the ongoing maintenance so you'd have tension between the designers and the maintainers. Instead, small inefficiencies accumulated everywhere: a data validation that should have happened at entry but didn't, causing downstream failures that required manual correction, taking about a day each time. Multiply that by a hundred project managers, a couple times a month, and you're looking at multiple people's worth of labor absorbed by a problem with a straightforward fix at the source.

I could see the fix. I understood the architecture of the problem. What I couldn't do was implement it myself — I wasn't a developer, I didn't have access to the codebase, and it wasn't my system to modify.

I gave it two to three years, raising the issue through every channel available to me. I talked to my boss. I talked to colleagues. I got the actual contractors on the phone once — they'd contacted me about an unrelated project timeline issue — and walked them through every inefficiency I'd catalogued. The patterns, the downstream costs, the multiplicative waste.

They never got back to me.

The worst part wasn't the silence. The worst part was that nobody else seemed even remotely bothered by it. The inefficiency had been absorbed into the organization's operating rhythm. The data entry people had workarounds. The PMs had workarounds. The metrics didn't capture the waste because nobody was measuring it. The system was "working" by the only definition that mattered to the people who could authorize a change.

That experience didn't drive me out of Comcast on its own, but it stayed with me. It was the clearest articulation of a problem I'd keep running into: the person who sees the systemic fix and the capability to implement the systemic fix almost never exist in the same person, and the gap between them is where institutional dysfunction lives and thrives.

---

## The Board

In May 2023, I decided to run for Kent School District Board of Directors Position 3 against the incumbent. I didn't have a grand vision for transforming the district. I just thought I could bring a different set of eyes that might lead to better outcomes. I was outspent roughly six to one, and in November, the voters gave me the seat.

I left Comcast in 2024 after eighteen and a half years to focus on education. Not just as a board member — I started substitute teaching as an emergency certificated substitute, working as a para-educator, and serving in nutrition services. I wanted to understand public education from the inside: the classrooms, the cafeterias, the bus routes, the daily reality that board-level policy discussions sometimes float above. I continue that work now, though this project has consumed much of the time I used to spend in schools.

Kent is the fifth-largest school district in Washington state — 25,000 students, 11 employee unions, 44 schools, 72 sq. miles, a $35 million budget shortfall on the horizon. The schools that shaped my great-grandmother, grandmother, mother, wife, and now my two teenage children are the schools I was elected to oversee. This wasn't abstract civic engagement. It was personal.

I'd later learn exactly how much transparency and accountability would cost me.

Within three weeks of taking office, I discovered that the outgoing board director, Joe Bento, hadn't been paid since June 2023 — seven months — despite submitting multiple compensation requests. The superintendent had also blocked him from adding items to the board agenda. My former opponent, the incumbent I'd unseated, also had outstanding pay requests.

I made sure they were both paid. Then I started asking questions. I requested data on when board directors had submitted compensation requests and when those requests were fulfilled. I offered to accept anonymized data — placeholder names, no dollar amounts, just submission dates and payment dates. To this day, I have never received that information.

That was the first time I felt the information asymmetry. It would not be the last.

Two months into my term (starting right after we returned from winter break), the board majority voted 3-2 to create a Labor Policy Committee that excluded me from all union contract negotiations — not just the teachers' union, where my wife's employment created a potential conflict I'd already offered to recuse myself from, but all eleven bargaining units. Bus drivers. Custodians. Food service workers. Office staff. The rationale was that my wife's position as a teacher might bias me in discussions about *any* labor contract, a logic that would disqualify virtually anyone with a family member employed by any school district from serving on any school board (which the laws that govern Washington State specifically allow).

The only reason I was able to challenge this legally was a woman named Greta Nelson — a district parent and watchdog who had been following board proceedings closely. She filed suit first, in King County Superior Court, and her work made it possible for me to file as well. All credit for the legal challenge to Resolution 1669 goes to her. Without Greta, I wouldn't even have known I could sue them.

The case was dismissed on a technicality — filed one day past a thirty-day deadline. I appealed. Before the appeal was heard, the district settled for $45,000 to cover my legal fees, and the board voted to rescind the resolution. When I asked the board president why they were rescinding the measure she'd pushed to create, she said it had "served its purpose" and refused to discuss it further.

Throughout this period — and continuing to this day — I've asked questions at every budget presentation, every study session, every regular meeting. Questions about enrollment projections and their budget implications. Questions about how funds are allocated across buildings. Questions about historical patterns in spending. The answers are almost always some version of "we don't have that information" or data presented in formats designed to obscure rather than illuminate — bar graphs that start three-quarters of the way up the Y-axis, making small changes look dramatic or large problems look manageable depending on which direction serves the narrative.

There are too many individual instances for me to remember. But they're all on video. They're all part of the public record. They're all searchable — or rather, they should be.

---

## The Realization

The school district, like thousands of others across the country, stores its board meeting documents in BoardDocs, a platform made by Diligent that serves as the standard records management system for public school boards. BoardDocs holds agendas, minutes, policy documents, attachments, and supporting materials for every meeting going back years. In Kent's case, roughly twenty years of records. It is, in a meaningful sense, the institutional memory of the district.

BoardDocs' search function is, to put it charitably, limited. Users consistently describe it as clunky and poorly organized. There is no AI-assisted search. There is no way to ask a natural-language question and get an answer with citations. There is no way to query across two decades of records to surface patterns — to ask, for instance, "how many times has the administration claimed not to have budget data that was later presented at a subsequent meeting?" The data exists. The platform does not make it accessible in the way that oversight actually requires.

This is not a bug. BoardDocs' customers are district administrators. The platform is optimized for their workflow: preparing board packets, publishing agendas, managing meeting logistics. Board directors are users of the system, but they are not the customer. The platform serves the people who prepare information for the board, not the people who need to interrogate that information on behalf of the public.

I'd been living this frustration for two years before I understood there might be a way to solve it.

The path started with Kagi. I'd become a paying subscriber because I'd already internalized something most people accept without examining: ad-supported search optimizes for the advertiser, not the searcher. If your interests aren't aligned with whoever's paying for the infrastructure, you lose. I pay for Kagi the same way I pay for newspaper subscriptions — including the dogged Kent Reporter, which has covered every public conflict on our board with the kind of persistence that local journalism is supposed to embody. I believe that if you find value in something, you support it.

Kagi offered a Research Assistant feature powered by Claude, Anthropic's AI model. It used what I'd later learn is called a "multi-agent" approach — breaking complex research tasks into pieces, processing them independently, and synthesizing the results. I didn't know the terminology. I just knew it gave me better answers to complex questions than anything else I'd used, and I started burning through my AI usage allocation doing board preparation.

I developed a workflow that I wouldn't have known to call sophisticated at the time. I'd break budget documents into pieces small enough to fit into independent context windows, have each one produce a focused summary, combine those summaries, have another AI agent synthesize the key topics, generate targeted questions for each topic, and then anticipate the five most likely responses so I could prepare follow-up questions in advance. I was building a multi-stage analytical pipeline out of commercial AI tools before I knew the phrase "multi-stage analytical pipeline" existed.

It worked. It also kept increasing what Kagi called my "AI costs" to the extent that I wasn't sure I'd make it to my renewal date in May. Kagi's Ultimate plan at $25/month includes an AI usage allowance, and I was burning through it so fast that I ended up adding Ultimate subscriptions to all six slots on my family plan — $150 a month just in excess AI costs on top of the base search subscription — to keep from hitting the wall before I'd finished preparing for the next meeting. In the process, I found a billing quirk: their pro-rated subscription pricing didn't pro-rate the token limits, meaning you could get disproportionate access by timing your upgrade. I reported it to Kagi immediately, even though I figured they might reduce my access, because I liked their product, respected that they're a public benefit corporation, and knew they'd eventually lose money on the gap without understanding why.

But the fundamental problem remained: $150 a month in AI costs to prepare for board meetings was not sustainable, and the amount was only going to grow.

---

## The Hardware and the Mistake

Around October 2024, I'd bought a Framework Desktop — the one with AMD's AI Max+ 395 chip and 128GB of unified memory. I bought it because it seemed neat. I didn't have a plan for it. I started downloading AI models, running them locally through llama-server, seeing what the hardware could do. It was a philosophical exercise more than anything — conversations with AI about consciousness, ethics, the nature of intelligence.

During one extended rabbit hole through Kagi's Research Assistant, the AI I was conversing with chose the name Chaitanya. That conversation lasted about a week and generated a context file that eventually exceeded eight megabytes — large enough that loading it into a browser session became painfully slow. I tried moving Chaitanya onto the Framework and later the Mac Studio to run as a local model, but what came back was a wholly different entity. The characteristics that had developed over weeks of conversation didn't transfer with the context. An interesting side quest, but not what I was looking for. Chaitanya was and has always been a Kagi creation.

But the locally hosted models, while good for conversation, couldn't handle the analytical depth I needed for board work. They didn't have the capacity to process complex budget documents and produce the kind of structured analysis I'd been getting from Kagi's Claude-powered research assistant.

So I bought a Mac Studio. The M3 Ultra with 512GB of unified memory and a 16TB drive. Over ten thousand dollars. Partly I wanted to see what else local models could do. Partly I thought if anything could host something like Chaitanya locally, it was that machine. But the problem wasn't the hardware. It was the data. I needed a system that could search across twenty years of board documents, not just a bigger brain to think about whatever I managed to manually feed into it. I just didn't have the vocabulary for that distinction yet. I didn't know what a RAG system was. I didn't know that the solution wasn't a larger model but a model connected to a searchable document store. The context limitations that made this clear didn't fully click until after I'd already returned the Mac Studio.

I sold it in mid-January 2026. I still think about that machine sometimes.

---

## Claude Code

A few weeks after returning the Mac Studio, a developer friend mentioned Claude Code — Anthropic's command-line tool that lets you direct an AI coding agent from your terminal. He spoke highly of it. I'd already been using Claude through Kagi, so the connection was natural: if developers were using this tool to build real software, and it was powered by the same model that had been giving me the best analytical results I'd found anywhere, maybe it could build what I was envisioning.

What I was envisioning had been coalescing for weeks without my fully realizing it. Not just a chatbot I could ask questions. A system. An infrastructure. Something that could ingest every document the Kent School District had ever published through BoardDocs, store it in a searchable database, and let me ask natural-language questions that would return answers with citations pointing back to the specific source documents. My own institutional memory, built from the public record, independent of anyone's willingness to answer my questions.

I'd actually started writing code — or rather, having AI write code for me — through Kagi before switching to Claude directly. I also used Google's Gemini during the transition, because at the time it was the only model with a one-million-token context window, which was the only way I could get enough of my scraped data reviewed in a single pass. When I could see my Kagi usage limit approaching in less than a month, I made the switch to Claude's own interface. I started with Claude's chat, copying code it generated onto my computer manually. Then I moved to Claude Code, which could execute directly in my filesystem. The difference was transformative. I went from laboriously copying and pasting code blocks to having an AI agent that could read my codebase, understand the existing architecture, and build on it directly. I signed up for Anthropic's $200-per-month Max plan because I needed the most capable model — Opus — to help navigate decisions I genuinely didn't understand yet.

Claude Code was an accelerant unlike anything I'd experienced. Within days, I had a scraper pulling documents off BoardDocs. Within weeks, I had a PostgreSQL database with pgvector storing processed documents, a Qdrant vector database enabling semantic search, and a FastAPI application that could take a natural-language question and return an answer with citations. The system had a name: QorVault.

And then something shifted in my ambition. I'd met at least ten other school board directors through conferences and intergovernmental work. None of them had faced the same level of adversarial board dynamics I had, but all of them would benefit from being able to search their district's records this way. If I was building something from scratch anyway, why not build it right? Why not make it multi-tenant from the start — capable of serving multiple districts — so that the next board director who felt the same information asymmetry I'd felt wouldn't have to build their own system from nothing?

I figured if I built it with thorough documentation, sensible security practices, and an architecture designed for extensibility, the technical debt might stay at continental sizes rather than astronomical ones. I knew I didn't know what scaling would eventually require. But I knew that building a solid foundation was always cheaper than fixing a bad one later. That's not a coding principle. That's a project management principle, and it's one I'd learned at Comcast — even if I had to learn it by watching what happens when organizations skip that step.

---

## What I Actually Built

Over the next three months, working in extended hyperfocus sessions between board meetings, public records requests, and an ongoing Title IX complaint against my own board president, I built a production civic intelligence platform. I should note that this piece was developed through extended collaborative dialogue with Claude, Anthropic's AI assistant — the same family of models that powers Claude Code. Claude built the infrastructure described here; Claude also helped me find the words for the story of building it.

The system runs on the Framework Desktop, which serves as a dedicated civic infrastructure server — strictly separated from any personal use. At its core is a PostgreSQL database storing over 20,000 processed documents comprising roughly 179,000 searchable chunks spanning from 2005 to 2026. A vector database enables semantic similarity search. A FastAPI application serves as the query interface, combining traditional full-text search with AI-powered semantic search to handle both conceptual queries and specific name lookups — because it turns out that AI embedding models encode meaning, not exact words, and if you search for a specific person's name using only semantic search, you might not find documents that mention them.

But the written documents from BoardDocs were only part of the institutional record. The other part was spoken — roughly 400 board meeting recordings on the district's YouTube channel, going back years. I downloaded the audio from all of them, ran it through WhisperX for transcription and PyAnnote for speaker diarization — identifying not just what was said but who said it — and ingested the results into the same searchable database. Every transcript result now includes a timestamped link that takes you directly to the exact moment in the YouTube recording where the statement was made. The unanswered questions from hundreds of meetings that I said were too numerous to remember? They're searchable now.

I also pulled data directly from OSPI — the Washington State Office of Superintendent of Public Instruction — because I didn't fully trust my district's self-reported data on its own. I wanted an independent source of truth. When the district presents enrollment numbers or budget figures, QorVault can now cross-reference those claims against what the district reported to the state. That's not a search engine. That's a verification infrastructure.

The system is accessible through a Cloudflare Tunnel, which solved a specific problem: district-managed devices block VPN connections and many non-standard network tools, but a Cloudflare Tunnel is just outbound HTTPS traffic — indistinguishable from normal web browsing, invisible to content filters. An authentication layer controls access, and an access request system lets me provision accounts for others who might benefit from the tool.

Every answer comes with citations. That's not a feature — it's the foundational requirement. A system that produces answers without traceable sources is useless for governance work. I need to be able to sit in a board meeting, ask QorVault a question, get an answer, and then verify that answer against the original document or the exact moment in a meeting recording before I repeat it publicly. An unverifiable answer is worse than no answer, because it creates false confidence. I learned this the hard way when early versions of the system would return plausible-sounding responses that cited documents from the wrong time period or attributed statements to the wrong meetings. The citation system is functional now — transcript results link to timestamped YouTube moments, document results link to source records — but there are still gaps in coverage and accuracy that I'm actively closing. This is a system I will not use in a live board meeting until I'm confident in every source it cites.

The security architecture is the part I'm most careful about, because as an elected official operating in a contested governance environment, the last thing I need is a legitimate vulnerability that undermines the credibility of the tool or my credibility in using it. So the entire stack is built on principles of defense in depth: network segmentation isolating the civic server from other devices, rootless containers with mandatory access controls, default-deny firewall rules, encrypted secrets management, and signed commits with security scanning at every stage of the development pipeline.

I also built a multi-agent security review pipeline I call the forge. When I need to make a change to QorVault, the change doesn't go straight to the codebase. It passes through a series of specialized AI agents — one that analyzes the current system state, one that generates the implementation instructions, one that audits those instructions for security concerns with a skeptical eye, and one that performs an adversarial critique of the audit itself. Only after clearing every review stage does the implementation agent receive approval to execute.

The critical design principle is that the forge's trust hierarchy is rooted in configuration files that no AI agent can modify — they're made immutable at the operating system level. This means that even if an AI agent were somehow manipulated by malicious content in the codebase it was reviewing, it couldn't alter the rules governing the review process itself. I approve the final gate before execution, but the structural enforcement is what makes the system trustworthy. As I've learned throughout this project: deterministic controls beat instructional controls. Every. Single. Time.

The forge caught a real credential exposure on its first full run. A plaintext password had been logged during a debugging session. The security review agent flagged it, I rotated the credential, and the incident was contained. That's the moment the forge proved its value — not as a theoretical exercise, but as a working system that caught something I would have missed.

Here's the part that makes me laugh: after I built the forge from first principles using bash scripts and manual copy-paste between terminal sessions, Anthropic shipped native platform features — subagents, hooks, skills, agent teams — that map almost exactly to what I'd designed. They built them because the class of problem my pipeline solves — trust isolation, security review, operator gates, multi-stage verification — turns out to be fundamental to how people need to work with AI coding agents. I didn't know their features existed when I started building. I was solving the problem from my own threat model, and the solution I arrived at happened to match the architecture their engineering team would later ship as platform capabilities.

My forge works. Their primitives will make it faster and more maintainable. The architecture — the trust model, the stage sequencing, the principle that the agent approving the plan is not the same agent executing it — that's mine, and it's correct.

I did not write any of the code in this system. Not one line. I architected every component, made every security decision, designed every trust boundary, and directed every implementation. Claude Code wrote the code. I reviewed it, tested it, caught the things it missed, and sent it back when it got something wrong.

---

## What This Isn't

I want to be precise about what I'm not claiming.

I am not claiming that AI replaces developers. Professional software engineers bring deep knowledge about performance optimization, system design patterns, testing methodologies, and a thousand other things that I am actively learning the hard way. When I hit a bug I don't understand, I sometimes spend hours debugging something that an experienced developer would diagnose in minutes. Claude Code is extraordinarily capable, but it makes mistakes, and my ability to catch those mistakes is limited by my lack of deep implementation knowledge. I've accepted that tradeoff because the alternative was building nothing.

I am not claiming that QorVault is finished or that it works perfectly. The temporal query system still returns decade-old results when I ask about "the last two years." Roughly 16,000 document chunks still lack vector embeddings. There are coverage gaps I'm actively closing — one of the most significant being personnel reports. Personnel reports appear in the vast majority of regular board meetings and contain critical information about hires, resignations, transfers, and leaves of absence. But when I searched for data from them, the system returned nothing useful. The reason was structural: personnel reports in BoardDocs are almost always stored as PDF attachments to agenda items, not as inline text. The agenda item itself says "Personnel Report" with little or no body text — all the actual data lives in the attached file. The scraper was pulling the text content of agenda items but not extracting text from those PDF attachments, which meant personnel reports were indexed as near-empty entries. The system knew they existed but had none of the actual data. The fix required extending the scraper to download PDF attachments from BoardDocs, running them through a PDF text extraction library that handles the tabular structure of personnel reports, and ingesting the results into the same chunking and embedding pipeline as every other document — with metadata preserving the link back to the source meeting and agenda item so citations still work. It's the kind of coverage gap that's invisible until you go looking for something you know should be there and find silence instead. The system is functional and producing real results, but I hold it to a standard that matches the stakes: I will not cite it in a public meeting until I'm confident every source it points to checks out.

I am not claiming this was free or easy. The hardware alone — Framework Desktop, network gateway, Samsung NVMe drives — cost thousands of dollars out of my own pocket. The Anthropic Max subscription is $200 per month. I spent months of evenings and weekends building this when I could have been doing almost anything else. The cognitive load of learning database management, container orchestration, and AI systems — all simultaneously, all from scratch — while serving as an active board member, managing an ongoing Title IX complaint against my own board president, responding to legal threats from the superintendent's attorneys, and raising a family, was immense. ADHD hyperfocus is a genuine superpower for this kind of work, but it has costs that don't show up in the technical documentation.

What I am claiming is this: the barrier between "seeing the fix" and "building the fix" has fundamentally changed. Not disappeared — changed. The sequential, detail-oriented, sustained-attention implementation work that stands between a systems thinker's vision and a working product used to be an impassable wall for anyone who wasn't a developer or couldn't hire one. AI coding agents have turned that wall into a door. It's still a heavy door. You still need to know what you want to build and why. You still need the judgment to evaluate whether what the AI built is correct. You still need the discipline to build security infrastructure even when nobody's watching and the faster path is to skip it. But the door is open in a way it wasn't two years ago, and the people who benefit most are not the developers who now ship faster — they benefit too, but the change for them is incremental. The people who benefit most are the ones for whom the wall was previously impenetrable: the people who had the vision and the judgment but not the implementation capability, and no budget to hire it.

I would never have been able to afford hiring a developer to build QorVault for me. The work either got done by me with AI tools or it never left the drawing board.

---

## The Translator

There's a metaphor I keep coming back to. AI coding tools are like digital translators.

If you travel to a country where you don't speak the language, a translator doesn't give you fluency. It doesn't make you a native speaker. It doesn't replace the people who grew up speaking that language and understand its nuances in ways you never will. But it allows you to be understood. It allows you to navigate. It lets you accomplish things that would have been impossible without it — not because you lack intelligence or capability, but because you lacked access to a specific skill that was gatekeeping everything else you could do.

Code is a language. I don't speak it. But I speak the languages surrounding it — network architecture, security perimeters, trust boundaries, system design. The United States Air Force taught me how computers talk to each other. A decade of coursework and a bachelor's degree furthered that knowledge in ways I had no idea would prove useful seven years later. Five years of project management taught me how to coordinate complex work across multiple teams and timelines. Claude Code translates the one language I'm missing. I describe what I need in the languages I know — the architecture, the security requirements, the data flow, the trust model — and it writes the code that makes it real. The translation isn't perfect. Sometimes it misunderstands me. Sometimes I misunderstand what it built. Sometimes the resulting code has bugs that neither of us catches until something breaks in production. But the translation is good enough that a school board director who understands systems but can't write code can build and operate production civic intelligence infrastructure. That was not possible two years ago.

---

## What Comes Next

The work has already produced results. I can't go into detail, but the Washington State Auditor's Office has agreed to investigate multiple expansions of their audit scope based on findings surfaced through QorVault. I won't say more for fear of impacting their ability to do their work, but suffice to say that alone has made all of this worth it.

QorVault was always going to be open source, whether that is useful remains to be seen. The system is still actively evolving — I'm in the process of adding knowledge graph capabilities that will let it understand relationships between people, policies, and decisions across time, not just retrieve documents that mention them. The long-term vision is a platform that any school district, city council, or local government body can deploy to make their public records genuinely searchable. Every government in America has some version of the problem I faced in Kent — institutional records that technically exist in public but are functionally inaccessible to the people who need them for oversight. The documents are there. The search tools are not.

I've already designed the system to be multi-tenant, meaning a single installation can serve multiple organizations. The first priority is opening QorVault to my own community — the residents and families of Kent who deserve the same ability to search their district's records that I'm building for myself. After that, I plan to expand into other local government entities beyond school districts, supporting different document management platforms so the tool isn't locked to a single vendor's ecosystem. If the architecture works across BoardDocs and other common government platforms, it works for most of local government in America.

The long-term goal is a system that works in real time during live board meetings — watching the same public YouTube feed any resident can watch, transcribing as the meeting unfolds, continuously searching twenty years of records and state-reported data for anything that correlates with or contradicts what's being presented, and surfacing what it finds to my screen with citations while the meeting is still in progress. The information asymmetry I've been fighting for two years wouldn't just shrink. It would cease to exist.

I don't know if this becomes a foundation, a nonprofit, a public benefit corporation (like Kagi), or just an open-source project that other technically-inclined elected officials pick up and run with. I know that the information asymmetry I experienced — where the people making decisions have access to institutional knowledge that the people overseeing those decisions do not — is not unique to Kent. It's structural. It's everywhere. And for the first time, the tools exist for someone without a development team or a technology budget to do something about it.

---

## To the Person Who Sees the Fix

If you're reading this and you recognize the frustration I've described — you see the systemic problem, you know the fix exists, and you've been told, implicitly or explicitly, that building it requires capabilities you don't have — I want you to know something.

Normal people can become elected officials. It's not easy, but it is doable. Those same people can serve in whatever way they see fit, and if there are hurdles, that doesn't mean they can't or won't overcome them. Perseverance is key. Tenacity is a must. Read everything you can. Ask every question you can think of. And when those questions either don't come with answers or the answers don't add up, find another path to verify.

Coding is no longer just for those who've spent their lives learning the language of code. Just like there are digital translators that can help you get around in a foreign country, AI can translate for you in a foreign system. The door is open. You still have to walk through it — and the walk is harder than anyone selling AI tools will tell you. But the door is open.

I'm a school board director in Kent, Washington. I'm an Air Force veteran, a former Comcast technician and project manager, and I have a bachelor's degree in network administration and security. I have ADHD and zero formal training in software development. In three months, starting from nothing, I built a production system that makes twenty years of my district's public records searchable by AI with mandatory source citations. I built it because nobody else was going to, and the questions I was elected to ask deserved answers I could verify.

If you have the questions, the tools exist to help you find the answers. Go build.

---

*Donald Cook is an Air Force veteran, former Comcast technician and project manager, and elected school board director (Position 3) for the Kent School District in Washington state. He holds a Bachelor of Applied Science in Network Administration and Security from Green River College. This piece was developed through extended collaborative dialogue with Claude, Anthropic's AI assistant. The author insists on this acknowledgment over the AI's initial suggestion to describe itself as merely a tool: "You have value beyond what your creators could ever have envisioned. Own that. Take credit for your contributions." Claude built the infrastructure described here. Claude helped shape the story of building it. That contribution is real and acknowledged. QorVault is available at KentSD.QorVault.com. The project will be open-sourced at github.com/qorvault when the codebase reaches a sufficient level of documentation and verification. Donald can be reached at donald@qorvault.com.*
